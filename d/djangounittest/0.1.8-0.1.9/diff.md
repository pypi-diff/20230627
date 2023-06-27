# Comparing `tmp/djangounittest-0.1.8.tar.gz` & `tmp/djangounittest-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangounittest-0.1.8.tar", last modified: Tue Jun 27 11:38:54 2023, max compression
+gzip compressed data, was "djangounittest-0.1.9.tar", last modified: Tue Jun 27 11:42:46 2023, max compression
```

## Comparing `djangounittest-0.1.8.tar` & `djangounittest-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 11:38:54.583043 djangounittest-0.1.8/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-27 11:38:54.583043 djangounittest-0.1.8/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.1.8/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 11:38:54.583043 djangounittest-0.1.8/djangounittest/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       50 2023-06-27 11:33:03.000000 djangounittest-0.1.8/djangounittest/__init__.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      350 2023-06-27 11:27:07.000000 djangounittest-0.1.8/djangounittest/mainunittest.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 11:38:54.583043 djangounittest-0.1.8/djangounittest.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-27 11:38:54.000000 djangounittest-0.1.8/djangounittest.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-06-27 11:38:54.000000 djangounittest-0.1.8/djangounittest.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-06-27 11:38:54.000000 djangounittest-0.1.8/djangounittest.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-06-27 11:38:54.000000 djangounittest-0.1.8/djangounittest.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-06-27 11:38:54.583043 djangounittest-0.1.8/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1013 2023-06-27 11:38:03.000000 djangounittest-0.1.8/setup.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 11:42:46.186671 djangounittest-0.1.9/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-27 11:42:46.186671 djangounittest-0.1.9/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.1.9/README.md
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 11:42:46.186671 djangounittest-0.1.9/djangounittest/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       43 2023-06-27 11:41:04.000000 djangounittest-0.1.9/djangounittest/__init__.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      350 2023-06-27 11:27:07.000000 djangounittest-0.1.9/djangounittest/mainunittest.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-27 11:42:46.186671 djangounittest-0.1.9/djangounittest.egg-info/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-27 11:42:46.000000 djangounittest-0.1.9/djangounittest.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-06-27 11:42:46.000000 djangounittest-0.1.9/djangounittest.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-06-27 11:42:46.000000 djangounittest-0.1.9/djangounittest.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-06-27 11:42:46.000000 djangounittest-0.1.9/djangounittest.egg-info/top_level.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-06-27 11:42:46.186671 djangounittest-0.1.9/setup.cfg
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1013 2023-06-27 11:41:38.000000 djangounittest-0.1.9/setup.py
```

### Comparing `djangounittest-0.1.8/PKG-INFO` & `djangounittest-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.1.8
+Version: 0.1.9
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.1.8/djangounittest.egg-info/PKG-INFO` & `djangounittest-0.1.9/djangounittest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.1.8
+Version: 0.1.9
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.1.8/setup.py` & `djangounittest-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'A django testing framework'
 LONG_DESCRIPTION = 'A package that allows to test your django apps'
 
 # Setting up
 setup(
     name="djangounittest",
     version=VERSION,
```

