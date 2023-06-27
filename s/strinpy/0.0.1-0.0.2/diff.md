# Comparing `tmp/strinpy-0.0.1.tar.gz` & `tmp/strinpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strinpy-0.0.1.tar", last modified: Tue Jun 27 11:03:20 2023, max compression
+gzip compressed data, was "strinpy-0.0.2.tar", last modified: Tue Jun 27 11:07:42 2023, max compression
```

## Comparing `strinpy-0.0.1.tar` & `strinpy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:03:20.314155 strinpy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-27 11:03:11.000000 strinpy-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-27 11:03:20.314155 strinpy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-27 11:03:11.000000 strinpy-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:03:20.314155 strinpy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-27 11:03:11.000000 strinpy-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:03:20.310155 strinpy-0.0.1/strinpy/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 11:03:11.000000 strinpy-0.0.1/strinpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-27 11:03:11.000000 strinpy-0.0.1/strinpy/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:03:20.314155 strinpy-0.0.1/strinpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-27 11:03:20.000000 strinpy-0.0.1/strinpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 11:03:20.000000 strinpy-0.0.1/strinpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:03:20.000000 strinpy-0.0.1/strinpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 11:03:20.000000 strinpy-0.0.1/strinpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:42.402502 strinpy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-27 11:07:29.000000 strinpy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-27 11:07:42.402502 strinpy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-27 11:07:29.000000 strinpy-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:07:42.402502 strinpy-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-27 11:07:29.000000 strinpy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:42.398502 strinpy-0.0.2/strinpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 11:07:29.000000 strinpy-0.0.2/strinpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-27 11:07:29.000000 strinpy-0.0.2/strinpy/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:42.402502 strinpy-0.0.2/strinpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-27 11:07:42.000000 strinpy-0.0.2/strinpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 11:07:42.000000 strinpy-0.0.2/strinpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:07:42.000000 strinpy-0.0.2/strinpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 11:07:42.000000 strinpy-0.0.2/strinpy.egg-info/top_level.txt
```

### Comparing `strinpy-0.0.1/LICENSE` & `strinpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strinpy-0.0.1/PKG-INFO` & `strinpy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: strinpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: React like string builder
 Home-page: https://github.com/am230/strinpy
 Author: am230
 License: MIT Licence
 Keywords: string
 Platform: any
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 React like string builder
-===============================
+=========================
 
 .. image:: https://img.shields.io/github/license/mashape/apistatus.svg
    :target: http://opensource.org/licenses/MIT
 .. image:: https://badge.fury.io/py/strinpy.svg
     :target: https://badge.fury.io/py/strinpy
 
 Usage
```

### Comparing `strinpy-0.0.1/README.rst` & `strinpy-0.0.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 React like string builder
-===============================
+=========================
 
 .. image:: https://img.shields.io/github/license/mashape/apistatus.svg
    :target: http://opensource.org/licenses/MIT
 .. image:: https://badge.fury.io/py/strinpy.svg
     :target: https://badge.fury.io/py/strinpy
 
 Usage
```

### Comparing `strinpy-0.0.1/setup.py` & `strinpy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 author = 'am230'
 name = 'strinpy'
 py_modules = [name]
 
 setup(
     name=name,
-    version="0.0.1",
+    version="0.0.2",
     keywords=["string"],
     description="React like string builder",
     long_description=long_description,
     license="MIT Licence",
     long_description_content_type='text/x-rst',
     packages=find_packages(),
     url=f"https://github.com/{author}/{name}",
```

### Comparing `strinpy-0.0.1/strinpy/builder.py` & `strinpy-0.0.2/strinpy/builder.py`

 * *Files identical despite different names*

### Comparing `strinpy-0.0.1/strinpy.egg-info/PKG-INFO` & `strinpy-0.0.2/strinpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: strinpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: React like string builder
 Home-page: https://github.com/am230/strinpy
 Author: am230
 License: MIT Licence
 Keywords: string
 Platform: any
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 React like string builder
-===============================
+=========================
 
 .. image:: https://img.shields.io/github/license/mashape/apistatus.svg
    :target: http://opensource.org/licenses/MIT
 .. image:: https://badge.fury.io/py/strinpy.svg
     :target: https://badge.fury.io/py/strinpy
 
 Usage
```

