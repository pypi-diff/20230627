# Comparing `tmp/pybarb-0.3.6.tar.gz` & `tmp/pybarb-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.6.tar", last modified: Fri Jun 23 14:03:27 2023, max compression
+gzip compressed data, was "pybarb-0.3.7.tar", last modified: Tue Jun 27 08:18:39 2023, max compression
```

## Comparing `pybarb-0.3.6.tar` & `pybarb-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:03:27.654268 pybarb-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 14:03:27.654268 pybarb-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-23 14:03:13.000000 pybarb-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:03:27.654268 pybarb-0.3.6/pybarb/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 14:03:13.000000 pybarb-0.3.6/pybarb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32202 2023-06-23 14:03:13.000000 pybarb-0.3.6/pybarb/pybarb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:03:27.654268 pybarb-0.3.6/pybarb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:03:27.654268 pybarb-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 14:03:13.000000 pybarb-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:18:39.527027 pybarb-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 08:18:39.527027 pybarb-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-27 08:18:28.000000 pybarb-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:18:39.527027 pybarb-0.3.7/pybarb/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 08:18:28.000000 pybarb-0.3.7/pybarb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32202 2023-06-27 08:18:28.000000 pybarb-0.3.7/pybarb/pybarb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:18:39.527027 pybarb-0.3.7/pybarb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:18:39.527027 pybarb-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 08:18:28.000000 pybarb-0.3.7/setup.py
```

### Comparing `pybarb-0.3.6/README.md` & `pybarb-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pybarb-0.3.6/pybarb/pybarb.py` & `pybarb-0.3.7/pybarb/pybarb.py`

 * *Files identical despite different names*

