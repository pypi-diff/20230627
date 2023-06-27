# Comparing `tmp/setuptools_dso-2.9.tar.gz` & `tmp/setuptools_dso-2.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setuptools_dso-2.9.tar", last modified: Tue Jun 27 00:33:35 2023, max compression
+gzip compressed data, was "dist/setuptools_dso-2.9a1.tar", last modified: Wed Jun 21 18:43:40 2023, max compression
```

## Comparing `setuptools_dso-2.9.tar` & `setuptools_dso-2.9a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:33:35.000000 setuptools_dso-2.9/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 00:33:16.000000 setuptools_dso-2.9/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-27 00:33:16.000000 setuptools_dso-2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 00:33:16.000000 setuptools_dso-2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-27 00:33:35.000000 setuptools_dso-2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-27 00:33:16.000000 setuptools_dso-2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 00:33:16.000000 setuptools_dso-2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 00:33:35.000000 setuptools_dso-2.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1355 2023-06-27 00:33:16.000000 setuptools_dso-2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/setuptools_dso/
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-27 00:33:16.000000 setuptools_dso-2.9/src/setuptools_dso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-27 00:33:16.000000 setuptools_dso-2.9/src/setuptools_dso/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-06-27 00:33:16.000000 setuptools_dso-2.9/src/setuptools_dso/dsocmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-06-27 00:33:16.000000 setuptools_dso-2.9/src/setuptools_dso/probe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-27 00:33:16.000000 setuptools_dso-2.9/src/setuptools_dso/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/setuptools_dso/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 00:33:16.000000 setuptools_dso-2.9/src/setuptools_dso/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-27 00:33:16.000000 setuptools_dso-2.9/src/setuptools_dso/test/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-27 00:33:16.000000 setuptools_dso-2.9/src/setuptools_dso/test/test_probe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/setuptools_dso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/setuptools_dso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/setuptools_dso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/setuptools_dso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/setuptools_dso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 00:33:35.000000 setuptools_dso-2.9/src/setuptools_dso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/src/setuptools_dso/
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/dsocmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/src/setuptools_dso/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/test/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/test/test_probe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/top_level.txt
```

### Comparing `setuptools_dso-2.9/LICENSE` & `setuptools_dso-2.9a1/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.9/PKG-INFO` & `setuptools_dso-2.9a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools_dso
-Version: 2.9
+Version: 2.9a1
 Summary: setuptools extension to build non-python shared libraries
 Home-page: https://github.com/mdavidsaver/setuptools_dso
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Project-URL: Documentation, https://mdavidsaver.github.io/setuptools_dso
 Project-URL: Release Notes, https://mdavidsaver.github.io/setuptools_dso/releasenotes.html
```

### Comparing `setuptools_dso-2.9/README.md` & `setuptools_dso-2.9a1/README.md`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.9/setup.py` & `setuptools_dso-2.9a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as F:
     long_description = F.read()
 
 setup(
     name='setuptools_dso',
-    version="2.9",
+    version="2.9a1",
     description="setuptools extension to build non-python shared libraries",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mdavidsaver/setuptools_dso',
     project_urls={
         'Documentation':'https://mdavidsaver.github.io/setuptools_dso',
         'Release Notes':'https://mdavidsaver.github.io/setuptools_dso/releasenotes.html',
```

### Comparing `setuptools_dso-2.9/src/setuptools_dso/__init__.py` & `setuptools_dso-2.9a1/src/setuptools_dso/__init__.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.9/src/setuptools_dso/compiler.py` & `setuptools_dso-2.9a1/src/setuptools_dso/compiler.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.9/src/setuptools_dso/dsocmd.py` & `setuptools_dso-2.9a1/src/setuptools_dso/dsocmd.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.9/src/setuptools_dso/probe.py` & `setuptools_dso-2.9a1/src/setuptools_dso/probe.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.9/src/setuptools_dso/runtime.py` & `setuptools_dso-2.9a1/src/setuptools_dso/runtime.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.9/src/setuptools_dso/test/test_probe.py` & `setuptools_dso-2.9a1/src/setuptools_dso/test/test_probe.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.9/src/setuptools_dso.egg-info/PKG-INFO` & `setuptools_dso-2.9a1/src/setuptools_dso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-dso
-Version: 2.9
+Version: 2.9a1
 Summary: setuptools extension to build non-python shared libraries
 Home-page: https://github.com/mdavidsaver/setuptools_dso
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Project-URL: Documentation, https://mdavidsaver.github.io/setuptools_dso
 Project-URL: Release Notes, https://mdavidsaver.github.io/setuptools_dso/releasenotes.html
```

### Comparing `setuptools_dso-2.9/src/setuptools_dso.egg-info/SOURCES.txt` & `setuptools_dso-2.9a1/src/setuptools_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

