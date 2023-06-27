# Comparing `tmp/SpoutGL-0.0.4.tar.gz` & `tmp/SpoutGL-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpoutGL-0.0.4.tar", last modified: Wed Aug  3 03:53:34 2022, max compression
+gzip compressed data, was "SpoutGL-0.0.5.tar", last modified: Tue Jun 27 08:32:48 2023, max compression
```

## Comparing `SpoutGL-0.0.4.tar` & `SpoutGL-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:53:34.656945 SpoutGL-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-08-03 03:53:27.000000 SpoutGL-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-08-03 03:53:34.656945 SpoutGL-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-08-03 03:53:27.000000 SpoutGL-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-08-03 03:53:27.000000 SpoutGL-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-03 03:53:34.656945 SpoutGL-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-08-03 03:53:27.000000 SpoutGL-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:53:34.656945 SpoutGL-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (121)    12120 2022-08-03 03:53:27.000000 SpoutGL-0.0.4/src/PySpoutGL.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:53:34.656945 SpoutGL-0.0.4/src/SpoutGL/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-03 03:53:27.000000 SpoutGL-0.0.4/src/SpoutGL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-03 03:53:27.000000 SpoutGL-0.0.4/src/SpoutGL/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-03 03:53:27.000000 SpoutGL-0.0.4/src/SpoutGL/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:53:34.656945 SpoutGL-0.0.4/src/SpoutGL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-08-03 03:53:34.000000 SpoutGL-0.0.4/src/SpoutGL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-08-03 03:53:34.000000 SpoutGL-0.0.4/src/SpoutGL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 03:53:34.000000 SpoutGL-0.0.4/src/SpoutGL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 03:53:34.000000 SpoutGL-0.0.4/src/SpoutGL.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:53:34.000000 SpoutGL-0.0.4/src/SpoutGL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:53:34.000000 SpoutGL-0.0.4/src/SpoutGL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:32:48.775334 SpoutGL-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-27 08:32:48.775334 SpoutGL-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:32:48.775334 SpoutGL-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:32:48.775334 SpoutGL-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/src/PySpoutGL.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:32:48.775334 SpoutGL-0.0.5/src/SpoutGL/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/src/SpoutGL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/src/SpoutGL/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/src/SpoutGL/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:32:48.775334 SpoutGL-0.0.5/src/SpoutGL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-27 08:32:48.000000 SpoutGL-0.0.5/src/SpoutGL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 08:32:48.000000 SpoutGL-0.0.5/src/SpoutGL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:32:48.000000 SpoutGL-0.0.5/src/SpoutGL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:32:48.000000 SpoutGL-0.0.5/src/SpoutGL.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 08:32:48.000000 SpoutGL-0.0.5/src/SpoutGL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 08:32:48.000000 SpoutGL-0.0.5/src/SpoutGL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:32:48.775334 SpoutGL-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-27 08:32:37.000000 SpoutGL-0.0.5/tests/test.py
```

### Comparing `SpoutGL-0.0.4/LICENSE` & `SpoutGL-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SpoutGL-0.0.4/PKG-INFO` & `SpoutGL-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpoutGL
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper around Spout frame streaming library for Windows
 Home-page: https://github.com/jlai/Python-SpoutGL
 Author: Jason Lai
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `SpoutGL-0.0.4/README.md` & `SpoutGL-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SpoutGL-0.0.4/setup.py` & `SpoutGL-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pybind11 import get_cmake_dir
 import pathlib
 import shutil
 import os.path
 
 import sys
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 is_64bits = sys.maxsize > 2**32
 
 spout_lib_base_dir = "vendor/SpoutGL/Binaries"
 spout_lib_dir = os.path.join(
     spout_lib_base_dir, "x64" if is_64bits else "Win32")
```

### Comparing `SpoutGL-0.0.4/src/PySpoutGL.cpp` & `SpoutGL-0.0.5/src/PySpoutGL.cpp`

 * *Files identical despite different names*

### Comparing `SpoutGL-0.0.4/src/SpoutGL.egg-info/PKG-INFO` & `SpoutGL-0.0.5/src/SpoutGL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpoutGL
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper around Spout frame streaming library for Windows
 Home-page: https://github.com/jlai/Python-SpoutGL
 Author: Jason Lai
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: BSD License
```

