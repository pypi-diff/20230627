# Comparing `tmp/TheHive5py-0.0.1.tar.gz` & `tmp/TheHive5py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheHive5py-0.0.1.tar", last modified: Tue Jun 27 12:46:44 2023, max compression
+gzip compressed data, was "TheHive5py-0.0.2.tar", last modified: Tue Jun 27 12:50:23 2023, max compression
```

## Comparing `TheHive5py-0.0.1.tar` & `TheHive5py-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:46:44.549179 TheHive5py-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 12:46:29.000000 TheHive5py-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-27 12:46:44.549179 TheHive5py-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 12:46:29.000000 TheHive5py-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 12:46:29.000000 TheHive5py-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:46:44.549179 TheHive5py-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-27 12:46:29.000000 TheHive5py-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:46:44.549179 TheHive5py-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:46:44.549179 TheHive5py-0.0.1/src/TheHive5py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-27 12:46:44.000000 TheHive5py-0.0.1/src/TheHive5py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-27 12:46:44.000000 TheHive5py-0.0.1/src/TheHive5py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:46:44.000000 TheHive5py-0.0.1/src/TheHive5py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 12:46:44.000000 TheHive5py-0.0.1/src/TheHive5py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:46:44.549179 TheHive5py-0.0.1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:46:29.000000 TheHive5py-0.0.1/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 12:46:29.000000 TheHive5py-0.0.1/src/tests/showHelloWorld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:23.519655 TheHive5py-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 12:50:06.000000 TheHive5py-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-27 12:50:23.519655 TheHive5py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 12:50:06.000000 TheHive5py-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 12:50:06.000000 TheHive5py-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:50:23.519655 TheHive5py-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-27 12:50:06.000000 TheHive5py-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:23.515655 TheHive5py-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:23.519655 TheHive5py-0.0.2/src/TheHive5py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-27 12:50:23.000000 TheHive5py-0.0.2/src/TheHive5py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-27 12:50:23.000000 TheHive5py-0.0.2/src/TheHive5py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:50:23.000000 TheHive5py-0.0.2/src/TheHive5py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 12:50:23.000000 TheHive5py-0.0.2/src/TheHive5py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:23.519655 TheHive5py-0.0.2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:06.000000 TheHive5py-0.0.2/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 12:50:06.000000 TheHive5py-0.0.2/src/tests/showHelloWorld.py
```

### Comparing `TheHive5py-0.0.1/LICENSE` & `TheHive5py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TheHive5py-0.0.1/PKG-INFO` & `TheHive5py-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheHive5py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python client for TheHive5
 Author: Sn0wAlice
 Author-email: snow.alice@pm.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
```

### Comparing `TheHive5py-0.0.1/setup.py` & `TheHive5py-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "TheHive5py",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Sn0wAlice",
     author_email = "snow.alice@pm.me",
     description = "Python client for TheHive5",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
         "Development Status :: 4 - Beta",
```

### Comparing `TheHive5py-0.0.1/src/TheHive5py.egg-info/PKG-INFO` & `TheHive5py-0.0.2/src/TheHive5py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheHive5py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python client for TheHive5
 Author: Sn0wAlice
 Author-email: snow.alice@pm.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
```

