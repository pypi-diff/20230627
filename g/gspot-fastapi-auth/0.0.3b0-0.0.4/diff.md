# Comparing `tmp/gspot_fastapi_auth-0.0.3b0.tar.gz` & `tmp/gspot_fastapi_auth-0.0.4.tar.gz`

## Comparing `gspot_fastapi_auth-0.0.3b0.tar` & `gspot_fastapi_auth-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/requirements.in
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/requirements.txt
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/example/main.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/example/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/__init__.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/auth.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/base.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/models.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/permissions.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/providers.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/services.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/settings.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/test_factory.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/tests/tests.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/LICENSE
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/pyproject.toml
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/PKG-INFO
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/requirements.in
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/example/main.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/example/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/__init__.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/auth.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/base.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/models.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/permissions.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/providers.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/services.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/settings.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/test_factory.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/tests/tests.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/LICENSE
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.4/PKG-INFO
```

### Comparing `gspot_fastapi_auth-0.0.3b0/.pre-commit-config.yaml` & `gspot_fastapi_auth-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/requirements.txt` & `gspot_fastapi_auth-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/example/main.py` & `gspot_fastapi_auth-0.0.4/example/main.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/example/tests.py` & `gspot_fastapi_auth-0.0.4/example/tests.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/auth.py` & `gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/auth.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/models.py` & `gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/models.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/permissions.py` & `gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/providers.py` & `gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/providers.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/test_factory.py` & `gspot_fastapi_auth-0.0.4/src/gspot_fastapi_auth/test_factory.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/tests/tests.py` & `gspot_fastapi_auth-0.0.4/tests/tests.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/.gitignore` & `gspot_fastapi_auth-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/LICENSE` & `gspot_fastapi_auth-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3b0/pyproject.toml` & `gspot_fastapi_auth-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_fastapi_auth"
-version = "0.0.3b"
+version = "0.0.4"
 authors = [
     { name = "gravity48", email = "gravity4849@gmail.com" },
 ]
 description = "GSpot authentication package for FastApi"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_fastapi_auth-0.0.3b0/PKG-INFO` & `gspot_fastapi_auth-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_fastapi_auth
-Version: 0.0.3b0
+Version: 0.0.4
 Summary: GSpot authentication package for FastApi
 Project-URL: Homepage, https://github.com/gravity48/gspot_fastapi_auth
 Project-URL: Bug Tracker, https://github.com/gravity48/gspot_fastapi_auth/issues
 Author-email: gravity48 <gravity4849@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

