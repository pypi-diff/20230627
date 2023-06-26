# Comparing `tmp/trimnet-1.0.3.tar.gz` & `tmp/trimnet-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimnet-1.0.3.tar", last modified: Mon Jun 26 22:05:48 2023, max compression
+gzip compressed data, was "trimnet-1.0.4.tar", last modified: Mon Jun 26 22:27:42 2023, max compression
```

## Comparing `trimnet-1.0.3.tar` & `trimnet-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:05:48.672497 trimnet-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-26 22:05:20.000000 trimnet-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 22:05:48.672497 trimnet-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-26 22:05:20.000000 trimnet-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:05:48.672497 trimnet-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 22:05:20.000000 trimnet-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:05:48.672497 trimnet-1.0.3/trimnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 22:05:48.000000 trimnet-1.0.3/trimnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 22:05:48.000000 trimnet-1.0.3/trimnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:05:48.000000 trimnet-1.0.3/trimnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 22:05:48.000000 trimnet-1.0.3/trimnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 22:05:48.000000 trimnet-1.0.3/trimnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:05:48.672497 trimnet-1.0.3/trimnet_drug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:05:20.000000 trimnet-1.0.3/trimnet_drug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:27:42.419426 trimnet-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-26 22:27:12.000000 trimnet-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 22:27:42.419426 trimnet-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-26 22:27:12.000000 trimnet-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:27:42.419426 trimnet-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 22:27:12.000000 trimnet-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:27:42.419426 trimnet-1.0.4/trimnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 22:27:42.000000 trimnet-1.0.4/trimnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 22:27:42.000000 trimnet-1.0.4/trimnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:27:42.000000 trimnet-1.0.4/trimnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 22:27:42.000000 trimnet-1.0.4/trimnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 22:27:42.000000 trimnet-1.0.4/trimnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:27:42.419426 trimnet-1.0.4/trimnet_drug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:27:12.000000 trimnet-1.0.4/trimnet_drug/__init__.py
```

### Comparing `trimnet-1.0.3/LICENSE` & `trimnet-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trimnet-1.0.3/README.md` & `trimnet-1.0.4/README.md`

 * *Files identical despite different names*

