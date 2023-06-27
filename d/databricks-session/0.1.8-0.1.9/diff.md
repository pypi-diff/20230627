# Comparing `tmp/databricks_session-0.1.8.tar.gz` & `tmp/databricks_session-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_session-0.1.8.tar", last modified: Tue Jun 27 03:08:02 2023, max compression
+gzip compressed data, was "databricks_session-0.1.9.tar", last modified: Tue Jun 27 05:10:54 2023, max compression
```

## Comparing `databricks_session-0.1.8.tar` & `databricks_session-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:08:02.505553 databricks_session-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 03:07:46.000000 databricks_session-0.1.8/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-27 03:07:46.000000 databricks_session-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-27 03:07:46.000000 databricks_session-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-27 03:07:46.000000 databricks_session-0.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-27 03:07:46.000000 databricks_session-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 03:07:46.000000 databricks_session-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 03:07:46.000000 databricks_session-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 03:07:46.000000 databricks_session-0.1.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-27 03:08:02.505553 databricks_session-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-27 03:07:46.000000 databricks_session-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-27 03:07:46.000000 databricks_session-0.1.8/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:08:02.505553 databricks_session-0.1.8/databricks_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-27 03:07:46.000000 databricks_session-0.1.8/databricks_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 03:07:46.000000 databricks_session-0.1.8/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 03:07:46.000000 databricks_session-0.1.8/package.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:07:46.000000 databricks_session-0.1.8/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 03:07:46.000000 databricks_session-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-27 03:07:46.000000 databricks_session-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 03:08:02.505553 databricks_session-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-27 03:07:46.000000 databricks_session-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 03:07:46.000000 databricks_session-0.1.8/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:10:54.410919 databricks_session-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 05:10:39.000000 databricks_session-0.1.9/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-27 05:10:39.000000 databricks_session-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-27 05:10:39.000000 databricks_session-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-27 05:10:39.000000 databricks_session-0.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-27 05:10:39.000000 databricks_session-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 05:10:39.000000 databricks_session-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 05:10:39.000000 databricks_session-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 05:10:39.000000 databricks_session-0.1.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-27 05:10:54.410919 databricks_session-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-27 05:10:39.000000 databricks_session-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-27 05:10:39.000000 databricks_session-0.1.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:10:54.410919 databricks_session-0.1.9/databricks_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-27 05:10:54.000000 databricks_session-0.1.9/databricks_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 05:10:54.000000 databricks_session-0.1.9/databricks_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:10:54.000000 databricks_session-0.1.9/databricks_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 05:10:54.000000 databricks_session-0.1.9/databricks_session.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:10:54.000000 databricks_session-0.1.9/databricks_session.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-27 05:10:54.000000 databricks_session-0.1.9/databricks_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 05:10:54.000000 databricks_session-0.1.9/databricks_session.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-27 05:10:39.000000 databricks_session-0.1.9/databricks_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 05:10:39.000000 databricks_session-0.1.9/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 05:10:39.000000 databricks_session-0.1.9/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:10:39.000000 databricks_session-0.1.9/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 05:10:39.000000 databricks_session-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-27 05:10:39.000000 databricks_session-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 05:10:54.414920 databricks_session-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-27 05:10:39.000000 databricks_session-0.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 05:10:39.000000 databricks_session-0.1.9/version.py
```

### Comparing `databricks_session-0.1.8/.gitignore` & `databricks_session-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_session-0.1.8/CHANGELOG.md` & `databricks_session-0.1.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.1.9](https://github.com/Broomva/databricks_session/compare/v0.1.8...v0.1.9) (2023-06-27)
+
+
+### Bug Fixes
+
+* **requirements:** add missing requirements ([09b9a4f](https://github.com/Broomva/databricks_session/commit/09b9a4fda460bed158378e588b3b497b30bfc2ff))
+
 ## [0.1.8](https://github.com/Broomva/databricks_session/compare/v0.1.7...v0.1.8) (2023-06-27)
 
 
 ### Bug Fixes
 
 * **ci:** add git pull to ci workflow ([#2](https://github.com/Broomva/databricks_session/issues/2)) ([3e3db17](https://github.com/Broomva/databricks_session/commit/3e3db17778e47a009b635ebc91d9904374819287))
```

### Comparing `databricks_session-0.1.8/CODE_OF_CONDUCT.md` & `databricks_session-0.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `databricks_session-0.1.8/CONTRIBUTING.rst` & `databricks_session-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `databricks_session-0.1.8/LICENSE` & `databricks_session-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_session-0.1.8/PKG-INFO` & `databricks_session-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks_session
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple util to get a spark and mlflow session objects from an .env file
 Home-page: https://github.com/Broomva/databricks_session
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `databricks_session-0.1.8/README.md` & `databricks_session-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `databricks_session-0.1.8/SECURITY.md` & `databricks_session-0.1.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `databricks_session-0.1.8/databricks_session.egg-info/PKG-INFO` & `databricks_session-0.1.9/databricks_session.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-session
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple util to get a spark and mlflow session objects from an .env file
 Home-page: https://github.com/Broomva/databricks_session
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `databricks_session-0.1.8/databricks_session.egg-info/SOURCES.txt` & `databricks_session-0.1.9/databricks_session.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks_session-0.1.8/databricks_session.py` & `databricks_session-0.1.9/databricks_session.py`

 * *Files identical despite different names*

### Comparing `databricks_session-0.1.8/setup.py` & `databricks_session-0.1.9/setup.py`

 * *Files identical despite different names*

