# Comparing `tmp/norton_beer-1.0.0.tar.gz` & `tmp/norton_beer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "norton_beer-1.0.0.tar", last modified: Tue Jun 20 15:16:49 2023, max compression
+gzip compressed data, was "norton_beer-1.0.1.tar", last modified: Tue Jun 27 09:14:02 2023, max compression
```

## Comparing `norton_beer-1.0.0.tar` & `norton_beer-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-20 15:16:49.312372 norton_beer-1.0.0/
--rw-rw-r--   0 icg154    (7154) icg154    (7154)      122 2023-04-19 10:31:09.000000 norton_beer-1.0.0/AUTHORS
--rw-rw-r--   0 icg154    (7154) icg154    (7154)    34523 2023-04-19 10:31:09.000000 norton_beer-1.0.0/LICENSE
--rw-rw-r--   0 icg154    (7154) icg154    (7154)    41476 2023-06-20 15:16:49.312372 norton_beer-1.0.0/PKG-INFO
--rw-rw-r--   0 icg154    (7154) icg154    (7154)     1135 2023-06-20 12:43:46.000000 norton_beer-1.0.0/README.md
--rw-rw-r--   0 icg154    (7154) icg154    (7154)      680 2023-06-20 15:16:37.000000 norton_beer-1.0.0/pyproject.toml
--rw-rw-r--   0 icg154    (7154) icg154    (7154)       38 2023-06-20 15:16:49.312372 norton_beer-1.0.0/setup.cfg
-drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-20 15:16:49.308372 norton_beer-1.0.0/src/
-drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-20 15:16:49.312372 norton_beer-1.0.0/src/norton_beer/
--rw-rw-r--   0 icg154    (7154) icg154    (7154)     2229 2023-04-19 10:31:09.000000 norton_beer-1.0.0/src/norton_beer/__init__.py
--rw-rw-r--   0 icg154    (7154) icg154    (7154)     3816 2023-04-19 14:01:51.000000 norton_beer-1.0.0/src/norton_beer/apodization.py
--rw-rw-r--   0 icg154    (7154) icg154    (7154)     9522 2023-04-19 14:04:35.000000 norton_beer-1.0.0/src/norton_beer/ils.py
--rw-rw-r--   0 icg154    (7154) icg154    (7154)     5009 2023-04-19 14:02:19.000000 norton_beer-1.0.0/src/norton_beer/optimize.py
-drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-20 15:16:49.312372 norton_beer-1.0.0/src/norton_beer.egg-info/
--rw-rw-r--   0 icg154    (7154) icg154    (7154)    41476 2023-06-20 15:16:49.000000 norton_beer-1.0.0/src/norton_beer.egg-info/PKG-INFO
--rw-rw-r--   0 icg154    (7154) icg154    (7154)      411 2023-06-20 15:16:49.000000 norton_beer-1.0.0/src/norton_beer.egg-info/SOURCES.txt
--rw-rw-r--   0 icg154    (7154) icg154    (7154)        1 2023-06-20 15:16:49.000000 norton_beer-1.0.0/src/norton_beer.egg-info/dependency_links.txt
--rw-rw-r--   0 icg154    (7154) icg154    (7154)       27 2023-06-20 15:16:49.000000 norton_beer-1.0.0/src/norton_beer.egg-info/requires.txt
--rw-rw-r--   0 icg154    (7154) icg154    (7154)       12 2023-06-20 15:16:49.000000 norton_beer-1.0.0/src/norton_beer.egg-info/top_level.txt
-drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-20 15:16:49.312372 norton_beer-1.0.0/tests/
--rw-rw-r--   0 icg154    (7154) icg154    (7154)      699 2023-04-19 10:31:09.000000 norton_beer-1.0.0/tests/test_apodization.py
--rw-rw-r--   0 icg154    (7154) icg154    (7154)     1807 2023-04-19 10:31:09.000000 norton_beer-1.0.0/tests/test_ils.py
--rw-rw-r--   0 icg154    (7154) icg154    (7154)     1117 2023-04-19 16:19:25.000000 norton_beer-1.0.0/tests/test_optimize.py
+drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-27 09:14:02.151851 norton_beer-1.0.1/
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)      122 2023-04-19 10:31:09.000000 norton_beer-1.0.1/AUTHORS
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)    34523 2023-04-19 10:31:09.000000 norton_beer-1.0.1/LICENSE
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)    41809 2023-06-27 09:14:02.151851 norton_beer-1.0.1/PKG-INFO
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)     1468 2023-06-22 13:59:16.000000 norton_beer-1.0.1/README.md
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)      680 2023-06-27 09:12:40.000000 norton_beer-1.0.1/pyproject.toml
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)       38 2023-06-27 09:14:02.151851 norton_beer-1.0.1/setup.cfg
+drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-27 09:14:02.143851 norton_beer-1.0.1/src/
+drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-27 09:14:02.147851 norton_beer-1.0.1/src/norton_beer/
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)     2132 2023-06-22 13:59:31.000000 norton_beer-1.0.1/src/norton_beer/__init__.py
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)     3816 2023-04-19 14:01:51.000000 norton_beer-1.0.1/src/norton_beer/apodization.py
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)     9522 2023-04-19 14:04:35.000000 norton_beer-1.0.1/src/norton_beer/ils.py
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)     5009 2023-04-19 14:02:19.000000 norton_beer-1.0.1/src/norton_beer/optimize.py
+drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-27 09:14:02.151851 norton_beer-1.0.1/src/norton_beer.egg-info/
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)    41809 2023-06-27 09:14:02.000000 norton_beer-1.0.1/src/norton_beer.egg-info/PKG-INFO
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)      411 2023-06-27 09:14:02.000000 norton_beer-1.0.1/src/norton_beer.egg-info/SOURCES.txt
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)        1 2023-06-27 09:14:02.000000 norton_beer-1.0.1/src/norton_beer.egg-info/dependency_links.txt
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)       27 2023-06-27 09:14:02.000000 norton_beer-1.0.1/src/norton_beer.egg-info/requires.txt
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)       12 2023-06-27 09:14:02.000000 norton_beer-1.0.1/src/norton_beer.egg-info/top_level.txt
+drwxrwxr-x   0 icg154    (7154) icg154    (7154)        0 2023-06-27 09:14:02.151851 norton_beer-1.0.1/tests/
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)      699 2023-04-19 10:31:09.000000 norton_beer-1.0.1/tests/test_apodization.py
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)     1807 2023-04-19 10:31:09.000000 norton_beer-1.0.1/tests/test_ils.py
+-rw-rw-r--   0 icg154    (7154) icg154    (7154)     1117 2023-04-19 16:19:25.000000 norton_beer-1.0.1/tests/test_optimize.py
```

### Comparing `norton_beer-1.0.0/LICENSE` & `norton_beer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `norton_beer-1.0.0/PKG-INFO` & `norton_beer-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: norton_beer
-Version: 1.0.0
-Summary: norton_beer 1.0.0
+Version: 1.0.1
+Summary: norton_beer 1.0.1
 Author-email: Konstantin Ntokas <k.ntokas@fz-juelich.de>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -671,16 +671,20 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
+
+[![PyPI](https://img.shields.io/badge/PyPI-v1.0.0-blue)](https://pypi.org/project/norton-beer/1.0.0/)
 [![CI pipeline](https://github.com/konstntokas/norton_beer/actions/workflows/python-package.yml/badge.svg)](https://github.com/konstntokas/norton_beer/actions/workflows/python-package.yml)
 [![Coverage Status](https://coveralls.io/repos/github/konstntokas/norton_beer/badge.svg?branch=coverall_coverage)](https://coveralls.io/github/konstntokas/norton_beer?branch=coverall_coverage)
+[![DOCS](https://img.shields.io/badge/%F0%9F%95%AE-docs-green.svg)](https://norton-beer.readthedocs.io/en/latest/index.html)
+[![DOI](https://zenodo.org/badge/610608772.svg)](https://zenodo.org/badge/latestdoi/610608772)
 
 # norton_beer
 
 The 'norton_beer' library is a python tool box for the Norton-Beer apodization functions.
 
 
 ## Main features
@@ -689,22 +693,21 @@
 - the analytical Fourier transform of the apodization window also known as instrument line shape (ILS)
 - generation of new apodization window for a fixed spatial resolution of the ILS so that the sides lobes are minimized
 
 ## Installation
 
 To use norton_beer, first install it using pip:
 
-```pip install norton_beer```
+```pip install norton-beer```
 
 ## Testing
 
 To test the `norton_beer` package, clone the repository and run:
 
 ```pytest```
 
 Note that pytest needs to be installed on the local machine. 
 
 ## Documentation
 
-- add paper when published
-- add webpage of sphinx built documentation
+- [Documentation](https://norton-beer.readthedocs.io/en/latest/norton_beer.html)
```

### Comparing `norton_beer-1.0.0/README.md` & `norton_beer-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+
+[![PyPI](https://img.shields.io/badge/PyPI-v1.0.0-blue)](https://pypi.org/project/norton-beer/1.0.0/)
 [![CI pipeline](https://github.com/konstntokas/norton_beer/actions/workflows/python-package.yml/badge.svg)](https://github.com/konstntokas/norton_beer/actions/workflows/python-package.yml)
 [![Coverage Status](https://coveralls.io/repos/github/konstntokas/norton_beer/badge.svg?branch=coverall_coverage)](https://coveralls.io/github/konstntokas/norton_beer?branch=coverall_coverage)
+[![DOCS](https://img.shields.io/badge/%F0%9F%95%AE-docs-green.svg)](https://norton-beer.readthedocs.io/en/latest/index.html)
+[![DOI](https://zenodo.org/badge/610608772.svg)](https://zenodo.org/badge/latestdoi/610608772)
 
 # norton_beer
 
 The 'norton_beer' library is a python tool box for the Norton-Beer apodization functions.
 
 
 ## Main features
@@ -12,22 +16,21 @@
 - the analytical Fourier transform of the apodization window also known as instrument line shape (ILS)
 - generation of new apodization window for a fixed spatial resolution of the ILS so that the sides lobes are minimized
 
 ## Installation
 
 To use norton_beer, first install it using pip:
 
-```pip install norton_beer```
+```pip install norton-beer```
 
 ## Testing
 
 To test the `norton_beer` package, clone the repository and run:
 
 ```pytest```
 
 Note that pytest needs to be installed on the local machine. 
 
 ## Documentation
 
-- add paper when published
-- add webpage of sphinx built documentation
+- [Documentation](https://norton-beer.readthedocs.io/en/latest/norton_beer.html)
```

### Comparing `norton_beer-1.0.0/pyproject.toml` & `norton_beer-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "norton_beer"
-version = "1.0.0"
-description= "norton_beer 1.0.0"
+version = "1.0.1"
+description= "norton_beer 1.0.1"
 readme = "README.md"
 authors = [
     {name = "Konstantin Ntokas", email="k.ntokas@fz-juelich.de"},
 ]
 requires-python = ">=3.8" 
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `norton_beer-1.0.0/src/norton_beer/__init__.py` & `norton_beer-1.0.1/src/norton_beer/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,26 +7,22 @@
 Provides:
     1. Norton-Beer apodization window generation in spatial domain
     2. the analytical Fourier transform of the apodization window
        also known as instrument line shape (ILS)
     3. generation of new apodization window for a fixed spatial
        resolution of the ILS so that the sides lobes are minimized
 
-Documentation:
-    1. add paper when published
-    2. add webpage of sphinx built documentation
-
 Installation
 ------------
 
 To use norton_beer, first install it using pip:
 
 .. code-block:: console
 
-   pip install norton_beer
+   pip install norton-beer
 
 Testing
 -------
 
 To test the `norton_beer` package, clone the repository from github
 (https://github.com/konstntokas/norton_beer) and run:
```

### Comparing `norton_beer-1.0.0/src/norton_beer/apodization.py` & `norton_beer-1.0.1/src/norton_beer/apodization.py`

 * *Files identical despite different names*

### Comparing `norton_beer-1.0.0/src/norton_beer/ils.py` & `norton_beer-1.0.1/src/norton_beer/ils.py`

 * *Files identical despite different names*

### Comparing `norton_beer-1.0.0/src/norton_beer/optimize.py` & `norton_beer-1.0.1/src/norton_beer/optimize.py`

 * *Files identical despite different names*

### Comparing `norton_beer-1.0.0/src/norton_beer.egg-info/PKG-INFO` & `norton_beer-1.0.1/src/norton_beer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: norton-beer
-Version: 1.0.0
-Summary: norton_beer 1.0.0
+Version: 1.0.1
+Summary: norton_beer 1.0.1
 Author-email: Konstantin Ntokas <k.ntokas@fz-juelich.de>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -671,16 +671,20 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
+
+[![PyPI](https://img.shields.io/badge/PyPI-v1.0.0-blue)](https://pypi.org/project/norton-beer/1.0.0/)
 [![CI pipeline](https://github.com/konstntokas/norton_beer/actions/workflows/python-package.yml/badge.svg)](https://github.com/konstntokas/norton_beer/actions/workflows/python-package.yml)
 [![Coverage Status](https://coveralls.io/repos/github/konstntokas/norton_beer/badge.svg?branch=coverall_coverage)](https://coveralls.io/github/konstntokas/norton_beer?branch=coverall_coverage)
+[![DOCS](https://img.shields.io/badge/%F0%9F%95%AE-docs-green.svg)](https://norton-beer.readthedocs.io/en/latest/index.html)
+[![DOI](https://zenodo.org/badge/610608772.svg)](https://zenodo.org/badge/latestdoi/610608772)
 
 # norton_beer
 
 The 'norton_beer' library is a python tool box for the Norton-Beer apodization functions.
 
 
 ## Main features
@@ -689,22 +693,21 @@
 - the analytical Fourier transform of the apodization window also known as instrument line shape (ILS)
 - generation of new apodization window for a fixed spatial resolution of the ILS so that the sides lobes are minimized
 
 ## Installation
 
 To use norton_beer, first install it using pip:
 
-```pip install norton_beer```
+```pip install norton-beer```
 
 ## Testing
 
 To test the `norton_beer` package, clone the repository and run:
 
 ```pytest```
 
 Note that pytest needs to be installed on the local machine. 
 
 ## Documentation
 
-- add paper when published
-- add webpage of sphinx built documentation
+- [Documentation](https://norton-beer.readthedocs.io/en/latest/norton_beer.html)
```

### Comparing `norton_beer-1.0.0/tests/test_apodization.py` & `norton_beer-1.0.1/tests/test_apodization.py`

 * *Files identical despite different names*

### Comparing `norton_beer-1.0.0/tests/test_ils.py` & `norton_beer-1.0.1/tests/test_ils.py`

 * *Files identical despite different names*

### Comparing `norton_beer-1.0.0/tests/test_optimize.py` & `norton_beer-1.0.1/tests/test_optimize.py`

 * *Files identical despite different names*

