# Comparing `tmp/lazyforecast-0.0.0.tar.gz` & `tmp/lazyforecast-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyforecast-0.0.0.tar", last modified: Fri May 26 17:55:01 2023, max compression
+gzip compressed data, was "lazyforecast-0.0.1.tar", last modified: Tue Jun 27 10:10:23 2023, max compression
```

## Comparing `lazyforecast-0.0.0.tar` & `lazyforecast-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:01.720626 lazyforecast-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 17:54:52.000000 lazyforecast-0.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:01.720626 lazyforecast-0.0.0/LazyForecast/
--rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-05-26 17:54:52.000000 lazyforecast-0.0.0/LazyForecast/LazyForecast.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 17:54:52.000000 lazyforecast-0.0.0/LazyForecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-26 17:55:01.720626 lazyforecast-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-26 17:54:52.000000 lazyforecast-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:01.720626 lazyforecast-0.0.0/lazyforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-26 17:55:01.000000 lazyforecast-0.0.0/lazyforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 17:55:01.000000 lazyforecast-0.0.0/lazyforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:55:01.000000 lazyforecast-0.0.0/lazyforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 17:55:01.000000 lazyforecast-0.0.0/lazyforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 17:55:01.000000 lazyforecast-0.0.0/lazyforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 17:55:01.720626 lazyforecast-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-26 17:54:52.000000 lazyforecast-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:10:23.236893 lazyforecast-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 10:10:14.000000 lazyforecast-0.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:10:23.236893 lazyforecast-0.0.1/LazyForecast/
+-rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-06-27 10:10:14.000000 lazyforecast-0.0.1/LazyForecast/LazyForecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:10:14.000000 lazyforecast-0.0.1/LazyForecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-27 10:10:23.236893 lazyforecast-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-27 10:10:14.000000 lazyforecast-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:10:23.236893 lazyforecast-0.0.1/lazyforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-27 10:10:23.000000 lazyforecast-0.0.1/lazyforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 10:10:23.000000 lazyforecast-0.0.1/lazyforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:10:23.000000 lazyforecast-0.0.1/lazyforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 10:10:23.000000 lazyforecast-0.0.1/lazyforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 10:10:23.000000 lazyforecast-0.0.1/lazyforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:10:23.236893 lazyforecast-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-27 10:10:14.000000 lazyforecast-0.0.1/setup.py
```

### Comparing `lazyforecast-0.0.0/LICENSE` & `lazyforecast-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyforecast-0.0.0/LazyForecast/LazyForecast.py` & `lazyforecast-0.0.1/LazyForecast/LazyForecast.py`

 * *Files identical despite different names*

### Comparing `lazyforecast-0.0.0/setup.py` & `lazyforecast-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.0.0'
+VERSION = '0.0.1'
 
 # Short description
 DESCRIPTION = "LazyForecast is a Python library for performing univariate time series analysis using a lazy forecasting approach. This approach is designed to provide quick and simple forecasting models without requiring extensive configuration or parameter tuning."
 
 # Required packages
 INSTALL_PACKAGES = ["ipython", "matplotlib", "numpy", "pandas", "pmdarima", "scikit-learn", "tensorflow", "tqdm"]
 
@@ -33,8 +33,8 @@
     ],
     install_requires= INSTALL_PACKAGES,
     keywords= TAGS,
     extras_require={
         "dev": ["twine>=4.0.2"],
     },
     python_requires=">=3.9",
-)
+)
```

