# Comparing `tmp/miao-make-20230626.tar.gz` & `tmp/miao-make-20230627.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miao-make-20230626.tar", last modified: Sun Jun 25 16:37:52 2023, max compression
+gzip compressed data, was "miao-make-20230627.tar", last modified: Tue Jun 27 08:05:48 2023, max compression
```

## Comparing `miao-make-20230626.tar` & `miao-make-20230627.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-25 16:37:52.659414 miao-make-20230626/
--rw-r--r--   0 4nji       (501) staff       (20)     5532 2023-06-25 16:37:52.658750 miao-make-20230626/PKG-INFO
--rw-r--r--   0 4nji       (501) staff       (20)     5092 2023-06-25 16:35:46.000000 miao-make-20230626/README.md
--rw-r--r--   0 4nji       (501) staff       (20)      665 2023-06-25 03:28:05.000000 miao-make-20230626/pyproject.toml
--rw-r--r--   0 4nji       (501) staff       (20)       38 2023-06-25 16:37:52.659602 miao-make-20230626/setup.cfg
-drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-25 16:37:52.651539 miao-make-20230626/src/
--rwxr-xr-x   0 4nji       (501) staff       (20)    16901 2023-06-25 16:29:28.000000 miao-make-20230626/src/miao.py
-drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-25 16:37:52.657908 miao-make-20230626/src/miao_make.egg-info/
--rw-r--r--   0 4nji       (501) staff       (20)     5532 2023-06-25 16:37:52.000000 miao-make-20230626/src/miao_make.egg-info/PKG-INFO
--rw-r--r--   0 4nji       (501) staff       (20)      260 2023-06-25 16:37:52.000000 miao-make-20230626/src/miao_make.egg-info/SOURCES.txt
--rw-r--r--   0 4nji       (501) staff       (20)        1 2023-06-25 16:37:52.000000 miao-make-20230626/src/miao_make.egg-info/dependency_links.txt
--rw-r--r--   0 4nji       (501) staff       (20)       35 2023-06-25 16:37:52.000000 miao-make-20230626/src/miao_make.egg-info/entry_points.txt
--rw-r--r--   0 4nji       (501) staff       (20)       21 2023-06-25 16:37:52.000000 miao-make-20230626/src/miao_make.egg-info/requires.txt
--rw-r--r--   0 4nji       (501) staff       (20)        5 2023-06-25 16:37:52.000000 miao-make-20230626/src/miao_make.egg-info/top_level.txt
+drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-27 08:05:48.073601 miao-make-20230627/
+-rw-r--r--   0 4nji       (501) staff       (20)     5532 2023-06-27 08:05:48.072903 miao-make-20230627/PKG-INFO
+-rw-r--r--   0 4nji       (501) staff       (20)     5092 2023-06-25 16:35:46.000000 miao-make-20230627/README.md
+-rw-r--r--   0 4nji       (501) staff       (20)      665 2023-06-25 03:28:05.000000 miao-make-20230627/pyproject.toml
+-rw-r--r--   0 4nji       (501) staff       (20)       38 2023-06-27 08:05:48.073805 miao-make-20230627/setup.cfg
+drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-27 08:05:48.068518 miao-make-20230627/src/
+-rwxr-xr-x   0 4nji       (501) staff       (20)    16901 2023-06-27 08:05:27.000000 miao-make-20230627/src/miao.py
+drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-27 08:05:48.072096 miao-make-20230627/src/miao_make.egg-info/
+-rw-r--r--   0 4nji       (501) staff       (20)     5532 2023-06-27 08:05:48.000000 miao-make-20230627/src/miao_make.egg-info/PKG-INFO
+-rw-r--r--   0 4nji       (501) staff       (20)      260 2023-06-27 08:05:48.000000 miao-make-20230627/src/miao_make.egg-info/SOURCES.txt
+-rw-r--r--   0 4nji       (501) staff       (20)        1 2023-06-27 08:05:48.000000 miao-make-20230627/src/miao_make.egg-info/dependency_links.txt
+-rw-r--r--   0 4nji       (501) staff       (20)       35 2023-06-27 08:05:48.000000 miao-make-20230627/src/miao_make.egg-info/entry_points.txt
+-rw-r--r--   0 4nji       (501) staff       (20)       21 2023-06-27 08:05:48.000000 miao-make-20230627/src/miao_make.egg-info/requires.txt
+-rw-r--r--   0 4nji       (501) staff       (20)        5 2023-06-27 08:05:48.000000 miao-make-20230627/src/miao_make.egg-info/top_level.txt
```

### Comparing `miao-make-20230626/PKG-INFO` & `miao-make-20230627/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miao-make
-Version: 20230626
+Version: 20230627
 Summary: Cargo-like project management tool for working with CMake
 Author-email: Anji Wong <anzhi0708@gmail.com>
 Project-URL: Homepage, https://github.com/anzhi0708/miao
 Keywords: cmake,cmakelists
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miao-make-20230626/README.md` & `miao-make-20230627/README.md`

 * *Files identical despite different names*

### Comparing `miao-make-20230626/pyproject.toml` & `miao-make-20230627/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miao-make-20230626/src/miao.py` & `miao-make-20230627/src/miao.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import inspect
 import datetime
 import colorama
 import subprocess
 from typing import Union, Callable
 
 
-__VERSION__: str = "20230626"
+__VERSION__: str = "20230627"
 
 
 class Miao:
     """
     Project manager for generating CMake file
     """
```

### Comparing `miao-make-20230626/src/miao_make.egg-info/PKG-INFO` & `miao-make-20230627/src/miao_make.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miao-make
-Version: 20230626
+Version: 20230627
 Summary: Cargo-like project management tool for working with CMake
 Author-email: Anji Wong <anzhi0708@gmail.com>
 Project-URL: Homepage, https://github.com/anzhi0708/miao
 Keywords: cmake,cmakelists
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

