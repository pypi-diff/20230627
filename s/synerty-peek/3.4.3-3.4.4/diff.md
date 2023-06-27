# Comparing `tmp/synerty-peek-3.4.3.tar.gz` & `tmp/synerty-peek-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synerty-peek-3.4.3.tar", last modified: Mon Jun 19 04:45:23 2023, max compression
+gzip compressed data, was "synerty-peek-3.4.4.tar", last modified: Tue Jun 27 02:03:08 2023, max compression
```

## Comparing `synerty-peek-3.4.3.tar` & `synerty-peek-3.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 04:45:23.666061 synerty-peek-3.4.3/
--rw-r--r--   0 root         (0) root         (0)      462 2023-06-19 04:45:23.666061 synerty-peek-3.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2984 2023-06-19 04:43:14.000000 synerty-peek-3.4.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 04:45:23.665061 synerty-peek-3.4.3/peek/
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-19 04:43:14.000000 synerty-peek-3.4.3/peek/__init__.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-19 04:45:23.675061 synerty-peek-3.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2051 2023-06-19 04:45:23.000000 synerty-peek-3.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 04:45:23.666061 synerty-peek-3.4.3/synerty_peek.egg-info/
--rw-r--r--   0 root         (0) root         (0)      462 2023-06-19 04:45:23.000000 synerty-peek-3.4.3/synerty_peek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-19 04:45:23.000000 synerty-peek-3.4.3/synerty_peek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 04:45:23.000000 synerty-peek-3.4.3/synerty_peek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 04:45:23.000000 synerty-peek-3.4.3/synerty_peek.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      802 2023-06-19 04:45:23.000000 synerty-peek-3.4.3/synerty_peek.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-19 04:45:23.000000 synerty-peek-3.4.3/synerty_peek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:03:08.423547 synerty-peek-3.4.4/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-06-27 02:03:08.423547 synerty-peek-3.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-06-27 02:01:00.000000 synerty-peek-3.4.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:03:08.422547 synerty-peek-3.4.4/peek/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-27 02:01:00.000000 synerty-peek-3.4.4/peek/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-27 02:03:08.423547 synerty-peek-3.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-06-27 02:03:08.000000 synerty-peek-3.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:03:08.423547 synerty-peek-3.4.4/synerty_peek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-06-27 02:03:08.000000 synerty-peek-3.4.4/synerty_peek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-27 02:03:08.000000 synerty-peek-3.4.4/synerty_peek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 02:03:08.000000 synerty-peek-3.4.4/synerty_peek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 02:03:08.000000 synerty-peek-3.4.4/synerty_peek.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-27 02:03:08.000000 synerty-peek-3.4.4/synerty_peek.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-27 02:03:08.000000 synerty-peek-3.4.4/synerty_peek.egg-info/top_level.txt
```

### Comparing `synerty-peek-3.4.3/README.rst` & `synerty-peek-3.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `synerty-peek-3.4.3/setup.py` & `synerty-peek-3.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 
 from setuptools import find_packages, setup
 
 pip_package_name = "synerty-peek"
-package_version = "3.4.3"
+package_version = "3.4.4"
 
 egg_info = "%s.egg-info" % pip_package_name
 if os.path.isdir(egg_info):
     shutil.rmtree(egg_info)
 
 if os.path.isfile("MANIFEST"):
     os.remove("MANIFEST")
```

### Comparing `synerty-peek-3.4.3/synerty_peek.egg-info/requires.txt` & `synerty-peek-3.4.4/synerty_peek.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-peek-admin-doc==3.4.*,>=3.4.3
-peek-admin-app==3.4.*,>=3.4.3
-peek-agent-service==3.4.*,>=3.4.3
-peek-core-device==3.4.*,>=3.4.3
-peek-core-docdb==3.4.*,>=3.4.3
-peek-core-email==3.4.*,>=3.4.3
-peek-core-search==3.4.*,>=3.4.3
-peek-core-user==3.4.*,>=3.4.3
-peek-core-screen==3.4.*,>=3.4.3
-peek-field-doc==3.4.*,>=3.4.3
-peek-field-app==3.4.*,>=3.4.3
-peek-field-service==3.4.*,>=3.4.3
-peek-logic-service==3.4.*,>=3.4.3
-peek-office-doc==3.4.*,>=3.4.3
-peek-office-app==3.4.*,>=3.4.3
-peek-office-service==3.4.*,>=3.4.3
-peek-platform==3.4.*,>=3.4.3
-peek-plugin-base==3.4.*,>=3.4.3
-peek-storage-service==3.4.*,>=3.4.3
-peek-worker-service==3.4.*,>=3.4.3
-peek-abstract-chunked-index==3.4.*,>=3.4.3
-peek-abstract-chunked-data-loader==3.4.*,>=3.4.3
+peek-admin-doc==3.4.*,>=3.4.4
+peek-admin-app==3.4.*,>=3.4.4
+peek-agent-service==3.4.*,>=3.4.4
+peek-core-device==3.4.*,>=3.4.4
+peek-core-docdb==3.4.*,>=3.4.4
+peek-core-email==3.4.*,>=3.4.4
+peek-core-search==3.4.*,>=3.4.4
+peek-core-user==3.4.*,>=3.4.4
+peek-core-screen==3.4.*,>=3.4.4
+peek-field-doc==3.4.*,>=3.4.4
+peek-field-app==3.4.*,>=3.4.4
+peek-field-service==3.4.*,>=3.4.4
+peek-logic-service==3.4.*,>=3.4.4
+peek-office-doc==3.4.*,>=3.4.4
+peek-office-app==3.4.*,>=3.4.4
+peek-office-service==3.4.*,>=3.4.4
+peek-platform==3.4.*,>=3.4.4
+peek-plugin-base==3.4.*,>=3.4.4
+peek-storage-service==3.4.*,>=3.4.4
+peek-worker-service==3.4.*,>=3.4.4
+peek-abstract-chunked-index==3.4.*,>=3.4.4
+peek-abstract-chunked-data-loader==3.4.*,>=3.4.4
 sphinx
 sphinx-rtd-theme
 sphinx-autobuild
 pytmpdir<1.1.0,>=1.0.2
 py-spy
```

