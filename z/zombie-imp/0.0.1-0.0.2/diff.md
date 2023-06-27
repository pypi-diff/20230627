# Comparing `tmp/zombie-imp-0.0.1.tar.gz` & `tmp/zombie-imp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zombie-imp-0.0.1.tar", last modified: Mon Jun 26 09:44:20 2023, max compression
+gzip compressed data, was "zombie-imp-0.0.2.tar", last modified: Tue Jun 27 09:57:00 2023, max compression
```

## Comparing `zombie-imp-0.0.1.tar` & `zombie-imp-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-06-26 09:44:20.201321 zombie-imp-0.0.1/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    13936 2023-06-26 08:32:31.000000 zombie-imp-0.0.1/LICENSE
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1369 2023-06-26 09:44:20.200322 zombie-imp-0.0.1/PKG-INFO
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      808 2023-06-26 09:40:39.000000 zombie-imp-0.0.1/README.md
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      272 2023-06-26 07:57:31.000000 zombie-imp-0.0.1/imp.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      701 2023-06-26 09:44:09.000000 zombie-imp-0.0.1/pyproject.toml
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)       38 2023-06-26 09:44:20.201321 zombie-imp-0.0.1/setup.cfg
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-06-26 09:44:20.198321 zombie-imp-0.0.1/zombie_imp/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      241 2023-06-26 07:34:34.000000 zombie-imp-0.0.1/zombie_imp/__init__.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    10554 2023-06-26 08:57:53.000000 zombie-imp-0.0.1/zombie_imp/imp_3_11.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     6429 2023-06-26 08:02:36.000000 zombie-imp-0.0.1/zombie_imp/pkgutil.py
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-06-26 09:44:20.200322 zombie-imp-0.0.1/zombie_imp.egg-info/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1369 2023-06-26 09:44:20.000000 zombie-imp-0.0.1/zombie_imp.egg-info/PKG-INFO
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      243 2023-06-26 09:44:20.000000 zombie-imp-0.0.1/zombie_imp.egg-info/SOURCES.txt
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)        1 2023-06-26 09:44:20.000000 zombie-imp-0.0.1/zombie_imp.egg-info/dependency_links.txt
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)       15 2023-06-26 09:44:20.000000 zombie-imp-0.0.1/zombie_imp.egg-info/top_level.txt
+drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-06-27 09:57:00.716718 zombie-imp-0.0.2/
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)    13936 2023-06-26 08:32:31.000000 zombie-imp-0.0.2/LICENSE
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)       55 2023-06-27 09:56:06.000000 zombie-imp-0.0.2/MANIFEST.in
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1369 2023-06-27 09:57:00.716718 zombie-imp-0.0.2/PKG-INFO
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      808 2023-06-26 09:40:39.000000 zombie-imp-0.0.2/README.md
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      341 2023-06-27 09:28:27.000000 zombie-imp-0.0.2/imp.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      701 2023-06-27 09:56:06.000000 zombie-imp-0.0.2/pyproject.toml
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)       38 2023-06-27 09:57:00.717718 zombie-imp-0.0.2/setup.cfg
+drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-06-27 09:57:00.713718 zombie-imp-0.0.2/test_zombie_imp/
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)    21129 2023-06-27 09:28:27.000000 zombie-imp-0.0.2/test_zombie_imp/test_imp.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1046 2023-06-27 09:28:27.000000 zombie-imp-0.0.2/test_zombie_imp/test_pkgutil_reanimations.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      879 2023-06-27 09:28:27.000000 zombie-imp-0.0.2/test_zombie_imp/test_same_files.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)    21142 2023-06-27 09:28:27.000000 zombie-imp-0.0.2/test_zombie_imp/test_zombie_imp.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      162 2023-06-27 09:37:59.000000 zombie-imp-0.0.2/tox.ini
+drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-06-27 09:57:00.715718 zombie-imp-0.0.2/zombie_imp/
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      300 2023-06-27 09:28:27.000000 zombie-imp-0.0.2/zombie_imp/__init__.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)    10608 2023-06-27 09:28:27.000000 zombie-imp-0.0.2/zombie_imp/imp_3_11.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     6429 2023-06-26 08:02:36.000000 zombie-imp-0.0.2/zombie_imp/pkgutil.py
+drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-06-27 09:57:00.715718 zombie-imp-0.0.2/zombie_imp.egg-info/
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1369 2023-06-27 09:57:00.000000 zombie-imp-0.0.2/zombie_imp.egg-info/PKG-INFO
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      406 2023-06-27 09:57:00.000000 zombie-imp-0.0.2/zombie_imp.egg-info/SOURCES.txt
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)        1 2023-06-27 09:57:00.000000 zombie-imp-0.0.2/zombie_imp.egg-info/dependency_links.txt
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)       15 2023-06-27 09:57:00.000000 zombie-imp-0.0.2/zombie_imp.egg-info/top_level.txt
```

### Comparing `zombie-imp-0.0.1/LICENSE` & `zombie-imp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zombie-imp-0.0.1/PKG-INFO` & `zombie-imp-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zombie-imp
-Version: 0.0.1
+Version: 0.0.2
 Summary: A copy of the `imp` module that was removed in Python 3.12
 Maintainer-email: Petr Viktorin <encukou@gmail.com>
 Project-URL: Homepage, https://github.com/encukou/zombie-imp
 Project-URL: Bug Tracker, https://github.com/encukou/zombie-imp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Operating System :: OS Independent
```

### Comparing `zombie-imp-0.0.1/README.md` & `zombie-imp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zombie-imp-0.0.1/pyproject.toml` & `zombie-imp-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zombie-imp"
-version = "0.0.1"
+version = "0.0.2"
 maintainers = [
   { name="Petr Viktorin", email="encukou@gmail.com" },
 ]
 description = "A copy of the `imp` module that was removed in Python 3.12"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zombie-imp-0.0.1/zombie_imp/imp_3_11.py` & `zombie-imp-0.0.2/zombie_imp/imp_3_11.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 functionality over this module.
 
 """
 # (Probably) need to stay in _imp
 from _imp import (lock_held, acquire_lock, release_lock,
                   get_frozen_object, is_frozen_package,
                   init_frozen, is_builtin, is_frozen,
-                  _fix_co_filename, _frozen_module_names)
+                  _fix_co_filename)
+try:
+    from _imp import _frozen_module_names
+except ImportError:
+    pass
 try:
     from _imp import create_dynamic
 except ImportError:
     # Platform doesn't support dynamic loading.
     create_dynamic = None
 
 from importlib._bootstrap import _ERR_MSG, _exec, _load, _builtin_from_name
```

### Comparing `zombie-imp-0.0.1/zombie_imp/pkgutil.py` & `zombie-imp-0.0.2/zombie_imp/pkgutil.py`

 * *Files identical despite different names*

### Comparing `zombie-imp-0.0.1/zombie_imp.egg-info/PKG-INFO` & `zombie-imp-0.0.2/zombie_imp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zombie-imp
-Version: 0.0.1
+Version: 0.0.2
 Summary: A copy of the `imp` module that was removed in Python 3.12
 Maintainer-email: Petr Viktorin <encukou@gmail.com>
 Project-URL: Homepage, https://github.com/encukou/zombie-imp
 Project-URL: Bug Tracker, https://github.com/encukou/zombie-imp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Operating System :: OS Independent
```

