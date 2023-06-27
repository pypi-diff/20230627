# Comparing `tmp/api_linter_101-0.0.1.tar.gz` & `tmp/api_linter_101-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_linter_101-0.0.1.tar", last modified: Tue Jun 27 13:52:17 2023, max compression
+gzip compressed data, was "api_linter_101-0.0.2.tar", last modified: Tue Jun 27 13:59:55 2023, max compression
```

## Comparing `api_linter_101-0.0.1.tar` & `api_linter_101-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kattels    (502) staff       (20)        0 2023-06-27 13:52:17.393762 api_linter_101-0.0.1/
--rw-r--r--   0 kattels    (502) staff       (20)      468 2023-06-27 13:52:17.393633 api_linter_101-0.0.1/PKG-INFO
--rw-r--r--   0 kattels    (502) staff       (20)     1445 2023-06-26 10:29:28.000000 api_linter_101-0.0.1/README.md
-drwxr-xr-x   0 kattels    (502) staff       (20)        0 2023-06-27 13:52:17.392403 api_linter_101-0.0.1/api_linter_101/
--rw-r--r--   0 kattels    (502) staff       (20)       82 2023-06-27 10:47:40.000000 api_linter_101-0.0.1/api_linter_101/__init__.py
--rw-r--r--   0 kattels    (502) staff       (20)     5543 2023-06-27 13:50:20.000000 api_linter_101-0.0.1/api_linter_101/linter.py
--rw-r--r--   0 kattels    (502) staff       (20)     4153 2023-06-27 08:32:59.000000 api_linter_101-0.0.1/api_linter_101/logger.py
--rw-r--r--   0 kattels    (502) staff       (20)    15133 2023-06-27 10:54:36.000000 api_linter_101-0.0.1/api_linter_101/utils.py
-drwxr-xr-x   0 kattels    (502) staff       (20)        0 2023-06-27 13:52:17.393277 api_linter_101-0.0.1/api_linter_101.egg-info/
--rw-r--r--   0 kattels    (502) staff       (20)      468 2023-06-27 13:52:17.000000 api_linter_101-0.0.1/api_linter_101.egg-info/PKG-INFO
--rw-r--r--   0 kattels    (502) staff       (20)      320 2023-06-27 13:52:17.000000 api_linter_101-0.0.1/api_linter_101.egg-info/SOURCES.txt
--rw-r--r--   0 kattels    (502) staff       (20)        1 2023-06-27 13:52:17.000000 api_linter_101-0.0.1/api_linter_101.egg-info/dependency_links.txt
--rw-r--r--   0 kattels    (502) staff       (20)       21 2023-06-27 13:52:17.000000 api_linter_101-0.0.1/api_linter_101.egg-info/requires.txt
--rw-r--r--   0 kattels    (502) staff       (20)       15 2023-06-27 13:52:17.000000 api_linter_101-0.0.1/api_linter_101.egg-info/top_level.txt
-drwxr-xr-x   0 kattels    (502) staff       (20)        0 2023-06-27 13:52:17.393439 api_linter_101-0.0.1/bin/
--rw-r--r--   0 kattels    (502) staff       (20)      515 2023-06-27 13:50:46.000000 api_linter_101-0.0.1/bin/linting
--rw-r--r--   0 kattels    (502) staff       (20)       38 2023-06-27 13:52:17.393807 api_linter_101-0.0.1/setup.cfg
--rw-r--r--   0 kattels    (502) staff       (20)      794 2023-06-27 13:51:30.000000 api_linter_101-0.0.1/setup.py
+drwxr-xr-x   0 kattels    (502) staff       (20)        0 2023-06-27 13:59:55.944006 api_linter_101-0.0.2/
+-rw-r--r--   0 kattels    (502) staff       (20)      468 2023-06-27 13:59:55.943884 api_linter_101-0.0.2/PKG-INFO
+-rw-r--r--   0 kattels    (502) staff       (20)     1445 2023-06-26 10:29:28.000000 api_linter_101-0.0.2/README.md
+drwxr-xr-x   0 kattels    (502) staff       (20)        0 2023-06-27 13:59:55.942740 api_linter_101-0.0.2/api_linter_101/
+-rw-r--r--   0 kattels    (502) staff       (20)       82 2023-06-27 10:47:40.000000 api_linter_101-0.0.2/api_linter_101/__init__.py
+-rw-r--r--   0 kattels    (502) staff       (20)     5543 2023-06-27 13:50:20.000000 api_linter_101-0.0.2/api_linter_101/linter.py
+-rw-r--r--   0 kattels    (502) staff       (20)     4153 2023-06-27 08:32:59.000000 api_linter_101-0.0.2/api_linter_101/logger.py
+-rw-r--r--   0 kattels    (502) staff       (20)    15133 2023-06-27 10:54:36.000000 api_linter_101-0.0.2/api_linter_101/utils.py
+drwxr-xr-x   0 kattels    (502) staff       (20)        0 2023-06-27 13:59:55.943519 api_linter_101-0.0.2/api_linter_101.egg-info/
+-rw-r--r--   0 kattels    (502) staff       (20)      468 2023-06-27 13:59:55.000000 api_linter_101-0.0.2/api_linter_101.egg-info/PKG-INFO
+-rw-r--r--   0 kattels    (502) staff       (20)      320 2023-06-27 13:59:55.000000 api_linter_101-0.0.2/api_linter_101.egg-info/SOURCES.txt
+-rw-r--r--   0 kattels    (502) staff       (20)        1 2023-06-27 13:59:55.000000 api_linter_101-0.0.2/api_linter_101.egg-info/dependency_links.txt
+-rw-r--r--   0 kattels    (502) staff       (20)       21 2023-06-27 13:59:55.000000 api_linter_101-0.0.2/api_linter_101.egg-info/requires.txt
+-rw-r--r--   0 kattels    (502) staff       (20)       15 2023-06-27 13:59:55.000000 api_linter_101-0.0.2/api_linter_101.egg-info/top_level.txt
+drwxr-xr-x   0 kattels    (502) staff       (20)        0 2023-06-27 13:59:55.943684 api_linter_101-0.0.2/bin/
+-rw-r--r--   0 kattels    (502) staff       (20)      534 2023-06-27 13:56:57.000000 api_linter_101-0.0.2/bin/linting
+-rw-r--r--   0 kattels    (502) staff       (20)       38 2023-06-27 13:59:55.944049 api_linter_101-0.0.2/setup.cfg
+-rw-r--r--   0 kattels    (502) staff       (20)      794 2023-06-27 13:58:01.000000 api_linter_101-0.0.2/setup.py
```

### Comparing `api_linter_101-0.0.1/README.md` & `api_linter_101-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `api_linter_101-0.0.1/api_linter_101/linter.py` & `api_linter_101-0.0.2/api_linter_101/linter.py`

 * *Files identical despite different names*

### Comparing `api_linter_101-0.0.1/api_linter_101/logger.py` & `api_linter_101-0.0.2/api_linter_101/logger.py`

 * *Files identical despite different names*

### Comparing `api_linter_101-0.0.1/api_linter_101/utils.py` & `api_linter_101-0.0.2/api_linter_101/utils.py`

 * *Files identical despite different names*

### Comparing `api_linter_101-0.0.1/bin/linting` & `api_linter_101-0.0.2/bin/linting`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/python3
 import argparse
 from api_linter_101 import run_script
 
 parser = argparse.ArgumentParser()
 parser.add_argument("-s", "--spec", type=str, help="Path to the yaml specification file")
 parser.add_argument("-r", "--rule", type=str, help="Path to the rules that specification file must follow")
 parser.add_argument("-o", "--output", type=str, help="Output the linting errors possible options, json | yaml")
```

### Comparing `api_linter_101-0.0.1/setup.py` & `api_linter_101-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Linter for Open API specification documents'
 LONG_DESCRIPTION = 'A yaml linter for opeanpi documents. '
 
 # Setting up
 setup(
     name="api_linter_101",
     version=VERSION,
```

