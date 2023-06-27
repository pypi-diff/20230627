# Comparing `tmp/django_bg_task-0.0.3.tar.gz` & `tmp/django_bg_task-0.0.4.tar.gz`

## Comparing `django_bg_task-0.0.3.tar` & `django_bg_task-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.isort.cfg
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20827 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.pylintrc
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/ignore-spelling-words.txt
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/manage.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/mypy.ini
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/requirements.txt
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/apps.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/common.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/constants.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/handler.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/models.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/serializers.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/services.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/settings.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/urls.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/views.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/migrations/__init__.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/LICENSE
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/README.md
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/.isort.cfg
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20827 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/.pylintrc
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/ignore-spelling-words.txt
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/manage.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/mypy.ini
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/apps.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/common.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/constants.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/handler.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/models.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/serializers.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/services.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/settings.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/urls.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/views.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/django_task/migrations/__init__.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/README.md
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 django_bg_task-0.0.4/PKG-INFO
```

### Comparing `django_bg_task-0.0.3/.pre-commit-config.yaml` & `django_bg_task-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/.pylintrc` & `django_bg_task-0.0.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/manage.py` & `django_bg_task-0.0.4/manage.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/.github/workflows/publish.yaml` & `django_bg_task-0.0.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/django_task/common.py` & `django_bg_task-0.0.4/django_task/common.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/django_task/handler.py` & `django_bg_task-0.0.4/django_task/handler.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/django_task/models.py` & `django_bg_task-0.0.4/django_task/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,10 +14,7 @@
         max_length=20, default=TaskStatus.PENDING, choices=TaskStatus.choices
     )
     args = JSONField(blank=True, null=True)
     kwargs = JSONField(blank=True, null=True)
     return_value = JSONField(blank=True, null=True)
     failed_reason = JSONField(blank=True, null=True)
     counter = models.IntegerField(default=1)
-
-    created_at = models.CharField(max_length=32, blank=True, default=None)
-    updated_at = models.CharField(max_length=32, blank=True, default=None)
```

### Comparing `django_bg_task-0.0.3/django_task/services.py` & `django_bg_task-0.0.4/django_task/services.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/django_task/settings.py` & `django_bg_task-0.0.4/django_task/settings.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/django_task/views.py` & `django_bg_task-0.0.4/django_task/views.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/django_task/migrations/0001_initial.py` & `django_bg_task-0.0.4/django_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/.gitignore` & `django_bg_task-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/LICENSE` & `django_bg_task-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/README.md` & `django_bg_task-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.3/pyproject.toml` & `django_bg_task-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "django-bg-task"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Abhishek Sharma", email="abhishm20@gmail.com" },
 ]
 description = "A small Django DRF extension for managing background task with celery"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_bg_task-0.0.3/PKG-INFO` & `django_bg_task-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bg-task
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small Django DRF extension for managing background task with celery
 Project-URL: Homepage, https://github.com/abhishm20/django-task
 Project-URL: Bug Tracker, https://github.com/abhishm20/django-task/issues
 Author-email: Abhishek Sharma <abhishm20@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

