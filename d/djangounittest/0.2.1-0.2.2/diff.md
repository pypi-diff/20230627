# Comparing `tmp/djangounittest-0.2.1.tar.gz` & `tmp/djangounittest-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangounittest-0.2.1.tar", last modified: Tue Jun 27 12:04:17 2023, max compression
+gzip compressed data, was "djangounittest-0.2.2.tar", last modified: Tue Jun 27 12:08:12 2023, max compression
```

## Comparing `djangounittest-0.2.1.tar` & `djangounittest-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 12:04:17.734392 djangounittest-0.2.1/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-27 12:04:17.734392 djangounittest-0.2.1/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.1/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 12:04:17.734392 djangounittest-0.2.1/djangounittest/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       50 2023-06-27 11:52:52.000000 djangounittest-0.2.1/djangounittest/__init__.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      143 2023-06-27 12:03:22.000000 djangounittest-0.2.1/djangounittest/mainunittest.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 12:04:17.734392 djangounittest-0.2.1/djangounittest.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-27 12:04:17.000000 djangounittest-0.2.1/djangounittest.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-06-27 12:04:17.000000 djangounittest-0.2.1/djangounittest.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-06-27 12:04:17.000000 djangounittest-0.2.1/djangounittest.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-06-27 12:04:17.000000 djangounittest-0.2.1/djangounittest.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-06-27 12:04:17.734392 djangounittest-0.2.1/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1013 2023-06-27 12:04:04.000000 djangounittest-0.2.1/setup.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 12:08:12.521988 djangounittest-0.2.2/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-27 12:08:12.521988 djangounittest-0.2.2/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.2/README.md
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 12:08:12.521988 djangounittest-0.2.2/djangounittest/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       50 2023-06-27 12:07:17.000000 djangounittest-0.2.2/djangounittest/__init__.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      120 2023-06-27 12:07:33.000000 djangounittest-0.2.2/djangounittest/mainunittest.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 12:08:12.521988 djangounittest-0.2.2/djangounittest.egg-info/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-27 12:08:12.000000 djangounittest-0.2.2/djangounittest.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-06-27 12:08:12.000000 djangounittest-0.2.2/djangounittest.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-06-27 12:08:12.000000 djangounittest-0.2.2/djangounittest.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-06-27 12:08:12.000000 djangounittest-0.2.2/djangounittest.egg-info/top_level.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-06-27 12:08:12.521988 djangounittest-0.2.2/setup.cfg
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1013 2023-06-27 12:07:49.000000 djangounittest-0.2.2/setup.py
```

### Comparing `djangounittest-0.2.1/PKG-INFO` & `djangounittest-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.1
+Version: 0.2.2
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.1/djangounittest.egg-info/PKG-INFO` & `djangounittest-0.2.2/djangounittest.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.1
+Version: 0.2.2
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.1/setup.py` & `djangounittest-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'A django testing framework'
 LONG_DESCRIPTION = 'A package that allows to test your django apps'
 
 # Setting up
 setup(
     name="djangounittest",
     version=VERSION,
```

