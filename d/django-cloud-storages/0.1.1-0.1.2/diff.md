# Comparing `tmp/django_cloud_storages-0.1.1.tar.gz` & `tmp/django_cloud_storages-0.1.2.tar.gz`

## Comparing `django_cloud_storages-0.1.1.tar` & `django_cloud_storages-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/cloud_storages/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/cloud_storages/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0     7771 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.2/PKG-INFO
```

### Comparing `django_cloud_storages-0.1.1/requirements.txt` & `django_cloud_storages-0.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-0.1.1/cloud_storages/backends/appwrite.py` & `django_cloud_storages-0.1.2/cloud_storages/backends/appwrite.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import secrets
 import string
 import traceback
+import re
 
 from django.core.files.storage import Storage
 from django.core.files import File
 from django.utils.deconstruct import deconstructible
 from django.utils.deconstruct import deconstructible
 
 from appwrite.client import Client
@@ -15,14 +16,15 @@
 
 from cloud_storages.utils import *
 
 
 @deconstructible
 class AppWriteStorage(Storage):
     CHUNK_SIZE = 4 * 1024 * 1024
+    MAX_FILE_NAME_LENGTH = 30
     def __init__(self):
         self.APPWRITE_API_KEY = setting('APPWRITE_API_KEY')
         self.APPWRITE_PROJECT_ID = setting('APPWRITE_PROJECT_ID')
         self.APPWRITE_BUCKET_ID = setting('APPWRITE_BUCKET_ID')
         self.APPWRITE_API_ENDPOINT = setting('APPWRITE_API_ENDPOINT', "https://cloud.appwrite.io/v1")
         self.MEDIA_URL = setting('MEDIA_URL')
         
@@ -64,18 +66,21 @@
         return name
     
     def get_available_name(self, name, max_length=None):
         """
         Return a filename that's free on the target storage system and
         available for new content to be written to.
         """
-        new_name = self.get_valid_name(name)
+        formatted_name = self.get_valid_name(name)
+        new_name = formatted_name
+        index = 0
         while(1):
+            index += 1
             if self.exists(new_name['file_id']):
-                new_name = self.get_valid_name(name)
+                new_name = self.get_alternative_name(formatted_name, index=index)
                 continue
             break
         return new_name
     
     def generate_filename(self, filename):
         """
         Validate the filename by calling get_valid_name() and return a filename
@@ -85,27 +90,35 @@
         return name
 
     def get_valid_name(self, name):
         """
         Return a filename, based on the provided filename, that's suitable for
         use in the target storage system.
         """
+        res = name.rsplit('.', 1)  # Split on last occurrence of delimiter
+        if len(res[0])>self.MAX_FILE_NAME_LENGTH:
+            raise Exception(f"The entire file path length must be less than or equal to {self.MAX_FILE_NAME_LENGTH}")
         name = str(name).replace("\\", "/")
-        alphaNumeric = string.ascii_uppercase + string.digits
-        file_id = ''.join([secrets.choice(alphaNumeric) for i in range(36)])
-        return {'file_id': file_id, 'file_name': name}
+        name = re.sub(r"^\W+", "", name) # Remove special characters at beginning
+        # name = name.rsplit('.', 1)
+        # file_name = name[0] if len(name[0])<=self.MAX_FILE_NAME_LENGTH else name[0][0:30]
+        # name = f"{file_name}.{name[1]}"
+        # alphaNumeric = string.ascii_uppercase + string.digits
+        # file_id = ''.join([secrets.choice(alphaNumeric) for i in range(36)])
+        return {'file_id': name, 'file_name': name}
 
-    def get_alternative_name(self, file_root, file_ext):
+    def get_alternative_name(self, file_root, file_ext=None, index=0):
         """
         Return an alternative filename if one exists to the filename.
         """
-        name = str(name).replace("\\", "/")
-        alphaNumeric = string.ascii_uppercase + string.digits
-        file_id = ''.join([secrets.choice(alphaNumeric) for i in range(36)])
-        return {'file_id': file_id, 'file_name': name}
+        res = file_root['file_name'].rsplit('.', 1)  # Split on last occurrence of delimiter
+        file_name = f"{res[0]}({index})"
+        file_ext = res[1]
+        updated_name =  f"{file_name}.{file_ext}"
+        return {'file_id': updated_name, 'file_name': updated_name}
 
     def delete(self, name):
         """
         Delete the specified file from the storage system.
         """
         result = self.storage.delete_file(self.APPWRITE_BUCKET_ID, name)
```

### Comparing `django_cloud_storages-0.1.1/cloud_storages/backends/dropbox.py` & `django_cloud_storages-0.1.2/cloud_storages/backends/dropbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,16 @@
     def get_alternative_name(self, file_root, file_ext=None, index=0):
         """
         Return an alternative filename if one exists to the filename.
         """
         res = file_root.rsplit('.', 1)  # Split on last occurrence of delimiter
         file_name = f"{res[0]}({index})"
         file_ext = res[1]
-        return f"{file_name}.{file_ext}"
+        updated_name =  f"{file_name}.{file_ext}"
+        return updated_name
 
     def delete(self, name):
         """
         Delete the specified file from the storage system.
         """
         self.dbx.files_delete_v2(name)
```

### Comparing `django_cloud_storages-0.1.1/.gitignore` & `django_cloud_storages-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-0.1.1/LICENSE` & `django_cloud_storages-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-0.1.1/pyproject.toml` & `django_cloud_storages-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "django", "requests", "dropbox", "appwrite"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-cloud-storages"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
 ]
 description = "Cloud file storages for django."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_cloud_storages-0.1.1/PKG-INFO` & `django_cloud_storages-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloud-storages
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cloud file storages for django.
 Project-URL: Homepage, https://github.com/Samiddha99/django-cloud-storages
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-cloud-storages/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

