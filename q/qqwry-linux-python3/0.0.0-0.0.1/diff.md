# Comparing `tmp/qqwry-linux-python3-0.0.0.tar.gz` & `tmp/qqwry-linux-python3-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qqwry-linux-python3-0.0.0.tar", last modified: Tue Jun 27 06:47:04 2023, max compression
+gzip compressed data, was "dist/qqwry-linux-python3-0.0.1.tar", last modified: Tue Jun 27 06:48:59 2023, max compression
```

## Comparing `qqwry-linux-python3-0.0.0.tar` & `qqwry-linux-python3-0.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/
--rw-r--r--   0 root         (0) root         (0)    11558 2023-03-22 07:03:34.000000 qqwry-linux-python3-0.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-27 04:20:12.000000 qqwry-linux-python3-0.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry/
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.0/qqwry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry/shell/
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.0/qqwry/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.0/qqwry/shell/usage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry/src/
--rw-r--r--   0 root         (0) root         (0)      299 2023-06-27 06:35:06.000000 qqwry-linux-python3-0.0.0/qqwry/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-06-27 06:07:50.000000 qqwry-linux-python3-0.0.0/qqwry/src/qqwry.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-06-27 06:19:48.000000 qqwry-linux-python3-0.0.0/qqwry/src/update_qqwry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      483 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-27 06:42:02.000000 qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-27 06:42:52.000000 qqwry-linux-python3-0.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 06:47:04.000000 qqwry-linux-python3-0.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-27 06:40:02.000000 qqwry-linux-python3-0.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-03-22 07:03:34.000000 qqwry-linux-python3-0.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-27 04:20:12.000000 qqwry-linux-python3-0.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.1/qqwry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry/shell/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.1/qqwry/shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.1/qqwry/shell/usage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry/src/
+-rw-r--r--   0 root         (0) root         (0)      299 2023-06-27 06:35:06.000000 qqwry-linux-python3-0.0.1/qqwry/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-27 06:07:50.000000 qqwry-linux-python3-0.0.1/qqwry/src/qqwry.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-06-27 06:19:48.000000 qqwry-linux-python3-0.0.1/qqwry/src/update_qqwry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      483 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-27 06:42:02.000000 qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-27 06:42:52.000000 qqwry-linux-python3-0.0.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 06:48:59.000000 qqwry-linux-python3-0.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-27 06:48:57.000000 qqwry-linux-python3-0.0.1/setup.py
```

### Comparing `qqwry-linux-python3-0.0.0/LICENSE` & `qqwry-linux-python3-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qqwry-linux-python3-0.0.0/PKG-INFO` & `qqwry-linux-python3-0.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qqwry-linux-python3
-Version: 0.0.0
+Version: 0.0.1
 Summary: Using and downloading qqwry.dat, for Python 3.6+
 Home-page: https://github.com/lqshome/qqwry-linux-python3
 Author: unclear
 Author-email: qsykgg@gmail.com
 License: MIT License
 Description: # qqwry-linux-python3
         Linux下自动更新qqwry的工具
```

### Comparing `qqwry-linux-python3-0.0.0/qqwry/src/qqwry.py` & `qqwry-linux-python3-0.0.1/qqwry/src/qqwry.py`

 * *Files identical despite different names*

### Comparing `qqwry-linux-python3-0.0.0/qqwry/src/update_qqwry.py` & `qqwry-linux-python3-0.0.1/qqwry/src/update_qqwry.py`

 * *Files identical despite different names*

### Comparing `qqwry-linux-python3-0.0.0/qqwry_linux_python3.egg-info/PKG-INFO` & `qqwry-linux-python3-0.0.1/qqwry_linux_python3.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qqwry-linux-python3
-Version: 0.0.0
+Version: 0.0.1
 Summary: Using and downloading qqwry.dat, for Python 3.6+
 Home-page: https://github.com/lqshome/qqwry-linux-python3
 Author: unclear
 Author-email: qsykgg@gmail.com
 License: MIT License
 Description: # qqwry-linux-python3
         Linux下自动更新qqwry的工具
```

### Comparing `qqwry-linux-python3-0.0.0/setup.py` & `qqwry-linux-python3-0.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @Author  : unclear
 # @File    : setup.py
 # @Software: PyCharm
 import os
 import sys
 from setuptools import setup, find_packages
 
-NAME = "qqwry-linux-python3"
+NAME = "qqwry"
 AUTHOR = "unclear"
 EMAIL = "qsykgg@gmail.com"
 URL = "https://github.com/lqshome/qqwry-linux-python3"
 LICENSE = "MIT License"
 DESCRIPTION = "Using and downloading qqwry.dat, for Python 3.6+"
 
 if sys.version_info < (3, 6, 0):
@@ -34,15 +34,15 @@
     with open("README.md", encoding="utf8") as f_r:
         _long_description = f_r.read()
 except FileNotFoundError:
     _long_description = ""
 
 if __name__ == "__main__":
     setup(
-        name=NAME,
+        name='qqwry-linux-python3',
         version=__version__,
         author=AUTHOR,
         author_email=EMAIL,
         url=URL,
         license=LICENSE,
         description=DESCRIPTION,
         packages=find_packages(),
@@ -59,8 +59,8 @@
         zip_safe=True,
         classifiers=[
             "Programming Language :: Python :: 3",
             f"License :: OSI Approved :: {LICENSE}",
             "Operating System :: OS Independent",
         ],
         python_requires=">=3.6"
-    )
+    )
```

