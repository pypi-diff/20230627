# Comparing `tmp/django_restful_translator-0.1.3.tar.gz` & `tmp/django_restful_translator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restful_translator-0.1.3.tar", last modified: Fri Jun 23 10:28:48 2023, max compression
+gzip compressed data, was "django_restful_translator-0.1.4.tar", last modified: Tue Jun 27 12:22:46 2023, max compression
```

## Comparing `django_restful_translator-0.1.3.tar` & `django_restful_translator-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:28:48.154433 django_restful_translator-0.1.3/
--rw-r--r--   0 alex       (501) staff       (20)     1075 2023-06-23 08:32:22.000000 django_restful_translator-0.1.3/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     5030 2023-06-23 10:28:48.154306 django_restful_translator-0.1.3/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     4396 2023-06-23 09:55:35.000000 django_restful_translator-0.1.3/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:28:48.151830 django_restful_translator-0.1.3/django_restful_translator/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.3/django_restful_translator/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2139 2023-06-23 10:19:38.000000 django_restful_translator-0.1.3/django_restful_translator/admin.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:28:48.153062 django_restful_translator-0.1.3/django_restful_translator/drf/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.3/django_restful_translator/drf/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      432 2023-06-23 10:19:38.000000 django_restful_translator-0.1.3/django_restful_translator/drf/fields.py
--rw-r--r--   0 alex       (501) staff       (20)     2296 2023-06-23 10:19:38.000000 django_restful_translator-0.1.3/django_restful_translator/drf/serializers.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:28:48.153267 django_restful_translator-0.1.3/django_restful_translator/management/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 09:56:08.000000 django_restful_translator-0.1.3/django_restful_translator/management/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:28:48.153741 django_restful_translator-0.1.3/django_restful_translator/management/commands/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 09:56:15.000000 django_restful_translator-0.1.3/django_restful_translator/management/commands/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2663 2023-06-23 08:31:59.000000 django_restful_translator-0.1.3/django_restful_translator/management/commands/generatelocales.py
--rw-r--r--   0 alex       (501) staff       (20)     2685 2023-06-23 08:31:59.000000 django_restful_translator-0.1.3/django_restful_translator/management/commands/update_database_translations.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:28:48.154143 django_restful_translator-0.1.3/django_restful_translator/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     1218 2023-06-23 08:31:59.000000 django_restful_translator-0.1.3/django_restful_translator/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.3/django_restful_translator/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1041 2023-06-23 10:19:38.000000 django_restful_translator-0.1.3/django_restful_translator/models.py
--rw-r--r--   0 alex       (501) staff       (20)      641 2023-06-23 08:31:59.000000 django_restful_translator-0.1.3/django_restful_translator/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:28:48.152601 django_restful_translator-0.1.3/django_restful_translator.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     5030 2023-06-23 10:28:47.000000 django_restful_translator-0.1.3/django_restful_translator.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      893 2023-06-23 10:28:48.000000 django_restful_translator-0.1.3/django_restful_translator.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-23 10:28:47.000000 django_restful_translator-0.1.3/django_restful_translator.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       49 2023-06-23 10:28:48.000000 django_restful_translator-0.1.3/django_restful_translator.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       26 2023-06-23 10:28:48.000000 django_restful_translator-0.1.3/django_restful_translator.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-23 10:28:48.154481 django_restful_translator-0.1.3/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      916 2023-06-23 10:17:17.000000 django_restful_translator-0.1.3/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-27 12:22:46.555854 django_restful_translator-0.1.4/
+-rw-r--r--   0 alex       (501) staff       (20)     1075 2023-06-23 08:32:22.000000 django_restful_translator-0.1.4/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     5030 2023-06-27 12:22:46.555737 django_restful_translator-0.1.4/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     4396 2023-06-23 09:55:35.000000 django_restful_translator-0.1.4/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-27 12:22:46.553125 django_restful_translator-0.1.4/django_restful_translator/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.4/django_restful_translator/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2139 2023-06-23 10:19:38.000000 django_restful_translator-0.1.4/django_restful_translator/admin.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-27 12:22:46.554364 django_restful_translator-0.1.4/django_restful_translator/drf/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.4/django_restful_translator/drf/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      432 2023-06-23 10:19:38.000000 django_restful_translator-0.1.4/django_restful_translator/drf/fields.py
+-rw-r--r--   0 alex       (501) staff       (20)     2296 2023-06-23 10:19:38.000000 django_restful_translator-0.1.4/django_restful_translator/drf/serializers.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-27 12:22:46.554595 django_restful_translator-0.1.4/django_restful_translator/management/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 09:56:08.000000 django_restful_translator-0.1.4/django_restful_translator/management/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-27 12:22:46.555091 django_restful_translator-0.1.4/django_restful_translator/management/commands/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 09:56:15.000000 django_restful_translator-0.1.4/django_restful_translator/management/commands/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3024 2023-06-27 12:02:47.000000 django_restful_translator-0.1.4/django_restful_translator/management/commands/generatelocales.py
+-rw-r--r--   0 alex       (501) staff       (20)     2794 2023-06-27 12:02:47.000000 django_restful_translator-0.1.4/django_restful_translator/management/commands/update_database_translations.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-27 12:22:46.555560 django_restful_translator-0.1.4/django_restful_translator/migrations/
+-rw-r--r--   0 alex       (501) staff       (20)     1218 2023-06-23 08:31:59.000000 django_restful_translator-0.1.4/django_restful_translator/migrations/0001_initial.py
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.4/django_restful_translator/migrations/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1041 2023-06-23 10:19:38.000000 django_restful_translator-0.1.4/django_restful_translator/models.py
+-rw-r--r--   0 alex       (501) staff       (20)      641 2023-06-26 08:27:21.000000 django_restful_translator-0.1.4/django_restful_translator/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-27 12:22:46.553870 django_restful_translator-0.1.4/django_restful_translator.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     5030 2023-06-27 12:22:46.000000 django_restful_translator-0.1.4/django_restful_translator.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      893 2023-06-27 12:22:46.000000 django_restful_translator-0.1.4/django_restful_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-27 12:22:46.000000 django_restful_translator-0.1.4/django_restful_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       49 2023-06-27 12:22:46.000000 django_restful_translator-0.1.4/django_restful_translator.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       26 2023-06-27 12:22:46.000000 django_restful_translator-0.1.4/django_restful_translator.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-27 12:22:46.555901 django_restful_translator-0.1.4/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      916 2023-06-27 12:02:47.000000 django_restful_translator-0.1.4/setup.py
```

### Comparing `django_restful_translator-0.1.3/LICENSE` & `django_restful_translator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.3/PKG-INFO` & `django_restful_translator-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_restful_translator
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Django application providing translation functionalities for Django Rest Framework
 Home-page: https://github.com/AlexIvanchyk/django_restful_translator
 Author: Alex Ivanchyk
 Author-email: alexander.ivanchik@gmail.com
 License: MIT
 Keywords: django rest-framework translation i18n
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django_restful_translator-0.1.3/README.md` & `django_restful_translator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.3/django_restful_translator/admin.py` & `django_restful_translator-0.1.4/django_restful_translator/admin.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.3/django_restful_translator/drf/serializers.py` & `django_restful_translator-0.1.4/django_restful_translator/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.3/django_restful_translator/management/commands/generatelocales.py` & `django_restful_translator-0.1.4/django_restful_translator/management/commands/generatelocales.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,24 +30,28 @@
                 po = polib.POFile()
             # Iterate over each translatable model
             for model in translatable_models:
                 # Fetch objects with prefetched translations
                 objects = model.objects.all().prefetch_related('translations')
                 for obj in objects:
                     for field_name in model.translatable_fields:
+                        original_field_value = getattr(obj, field_name)
+                        if original_field_value is None or original_field_value == '':
+                            self.stdout.write(
+                                f'Skipping {model._meta.model_name} id {obj.id} due to None value for field {field_name}')
+                            continue
                         trans = next((t for t in obj.translations.all() if
                                       t.field_name == field_name and t.language == language), None)
                         if not trans:
                             # If translation doesn't exist, create a blank one for the .po file
-
                             trans = Translation(
                                 content_object=obj,
                                 field_name=field_name,
                                 language=language,
-                                field_value=getattr(obj, field_name) if language == settings.LANGUAGE_CODE else ""
+                                field_value=original_field_value if language == settings.LANGUAGE_CODE else ""
                             )
                         self.write_to_po_file(po, trans)
             # Save and close the .po file for this language
             po.save(po_file_path)
 
     def write_to_po_file(self, po, trans):
         entry = polib.POEntry(
```

### Comparing `django_restful_translator-0.1.3/django_restful_translator/management/commands/update_database_translations.py` & `django_restful_translator-0.1.4/django_restful_translator/management/commands/update_database_translations.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,19 +46,22 @@
             po = polib.pofile(po_file_path)
             # Iterate over each entry in the .po file
             for entry in po:
                 model_name, field_name, object_id = entry.tcomment.split("__")
                 model = next((m for m in translatable_models if m._meta.model_name == model_name), None)
                 if not model:
                     continue
+                field_value = entry.msgstr
+                if field_value == "":
+                    continue
                 # Fetch or create the Translation object
                 trans, created = Translation.objects.get_or_create(
                     content_type=ContentType.objects.get_for_model(model),
                     object_id=object_id,
                     field_name=field_name,
                     language=language,
-                    defaults={"field_value": entry.msgstr}
+                    defaults={"field_value": field_value}
                 )
                 # If the Translation object already existed, update it
                 if not created:
                     trans.field_value = entry.msgstr
                     trans.save()
```

### Comparing `django_restful_translator-0.1.3/django_restful_translator/migrations/0001_initial.py` & `django_restful_translator-0.1.4/django_restful_translator/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.3/django_restful_translator/models.py` & `django_restful_translator-0.1.4/django_restful_translator/models.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.3/django_restful_translator/utils.py` & `django_restful_translator-0.1.4/django_restful_translator/utils.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.3/django_restful_translator.egg-info/PKG-INFO` & `django_restful_translator-0.1.4/django_restful_translator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restful-translator
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Django application providing translation functionalities for Django Rest Framework
 Home-page: https://github.com/AlexIvanchyk/django_restful_translator
 Author: Alex Ivanchyk
 Author-email: alexander.ivanchik@gmail.com
 License: MIT
 Keywords: django rest-framework translation i18n
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django_restful_translator-0.1.3/django_restful_translator.egg-info/SOURCES.txt` & `django_restful_translator-0.1.4/django_restful_translator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.3/setup.py` & `django_restful_translator-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django_restful_translator',
-    version='0.1.3',
+    version='0.1.4',
     author='Alex Ivanchyk',
     author_email='alexander.ivanchik@gmail.com',
     description='A Django application providing translation functionalities for Django Rest Framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AlexIvanchyk/django_restful_translator',
     packages=find_packages(),
```

