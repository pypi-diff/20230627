# Comparing `tmp/drf_misc-0.0.4.tar.gz` & `tmp/drf_misc-0.0.5.tar.gz`

## Comparing `drf_misc-0.0.4.tar` & `drf_misc-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.isort.cfg
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.pylintrc
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.0.4/ignore-spelling-words.txt
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.0.4/mypy.ini
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.4/setup.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/admin.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/apps.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/settings.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/api_exceptions.py
--rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/api_views.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/audit_service.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/cache.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/filter_backend.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/middlewares.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/models.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/paginations.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/parsers.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/permissions.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/serializers.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/services.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/throttling.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/decorators.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/epoch_util.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/misc.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/validator.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.0.4/LICENSE
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 drf_misc-0.0.4/README.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 drf_misc-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 drf_misc-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.0.5/.isort.cfg
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 drf_misc-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.0.5/.pylintrc
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.0.5/ignore-spelling-words.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.0.5/mypy.ini
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.5/setup.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 drf_misc-0.0.5/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 drf_misc-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/admin.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/apps.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/settings.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/api_exceptions.py
+-rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/api_views.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/audit_service.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/cache.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/fields.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/filter_backend.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/middlewares.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/models.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/paginations.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/parsers.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/permissions.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/serializers.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/services.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/core/throttling.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/utility/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/utility/decorators.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/utility/epoch_util.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/utility/misc.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 drf_misc-0.0.5/drf_misc/utility/validator.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 drf_misc-0.0.5/README.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 drf_misc-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 drf_misc-0.0.5/PKG-INFO
```

### Comparing `drf_misc-0.0.4/.pre-commit-config.yaml` & `drf_misc-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/.pylintrc` & `drf_misc-0.0.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/.github/workflows/publish.yaml` & `drf_misc-0.0.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/admin.py` & `drf_misc-0.0.5/drf_misc/admin.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/settings.py` & `drf_misc-0.0.5/drf_misc/settings.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/api_exceptions.py` & `drf_misc-0.0.5/drf_misc/core/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/api_views.py` & `drf_misc-0.0.5/drf_misc/core/api_views.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/audit_service.py` & `drf_misc-0.0.5/drf_misc/core/audit_service.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/filter_backend.py` & `drf_misc-0.0.5/drf_misc/core/filter_backend.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/middlewares.py` & `drf_misc-0.0.5/drf_misc/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/models.py` & `drf_misc-0.0.5/drf_misc/core/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 from __future__ import absolute_import, unicode_literals
 
 import time
 import uuid
 
 from django.db import models
 
+from drf_misc.core.fields import EpochField
+
 # pylint: disable=no-member,access-member-before-definition,invalid-name
 
 
 class _DateTimeStampingModel(models.Model):
-    created_at = models.CharField(max_length=32, null=True, default=None)
-    updated_at = models.CharField(max_length=32, null=True, default=None)
+    created_at = EpochField(default_current_time=True, milliseconds=True)
+    updated_at = EpochField(nullable=True, update_now=True, milliseconds=True)
 
     class Meta:
         abstract = True
 
     def save(self, *args, **kwargs):
         if not self.id:
             self.id = str(uuid.uuid4())
-            self.created_at = int(time.time())
         self.updated_at = int(time.time())
         super().save(*args, **kwargs)
 
 
 class AllInstanceManager(models.Manager):
     def get_queryset(self):
         return super(AllInstanceManager, self).get_queryset().filter()
```

### Comparing `drf_misc-0.0.4/drf_misc/core/paginations.py` & `drf_misc-0.0.5/drf_misc/core/paginations.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/serializers.py` & `drf_misc-0.0.5/drf_misc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/services.py` & `drf_misc-0.0.5/drf_misc/core/services.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/core/throttling.py` & `drf_misc-0.0.5/drf_misc/core/throttling.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/utility/misc.py` & `drf_misc-0.0.5/drf_misc/utility/misc.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/drf_misc/utility/validator.py` & `drf_misc-0.0.5/drf_misc/utility/validator.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/.gitignore` & `drf_misc-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/LICENSE` & `drf_misc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/README.md` & `drf_misc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.4/pyproject.toml` & `drf_misc-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "drf-misc"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Abhishek Sharma", email="abhishm20@gmail.com" },
 ]
 description = "A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -38,8 +38,8 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 line_length = 88
 default_section = "THIRDPARTY"
 known_first_party = []
-known_third_party = ["boto3", "django", "django_filters", "jwt", "moment", "rest_framework", "rest_framework_extensions", "unidecode"]
+known_third_party = ["boto3", "django", "django_filters", "jwt", "rest_framework", "rest_framework_extensions", "unidecode"]
```

### Comparing `drf_misc-0.0.4/PKG-INFO` & `drf_misc-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-misc
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services.
 Project-URL: Homepage, https://github.com/abhishm20/drf-misc
 Project-URL: Bug Tracker, https://github.com/abhishm20/drf-misc/issues
 Author-email: Abhishek Sharma <abhishm20@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

