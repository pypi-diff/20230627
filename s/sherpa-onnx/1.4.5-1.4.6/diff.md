# Comparing `tmp/sherpa-onnx-1.4.5.tar.gz` & `tmp/sherpa-onnx-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.4.5.tar", last modified: Fri Jun 23 17:48:29 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.4.6.tar", last modified: Tue Jun 27 10:32:03 2023, max compression
```

## Comparing `sherpa-onnx-1.4.5.tar` & `sherpa-onnx-1.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:48:29.247019 sherpa-onnx-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-23 17:37:18.000000 sherpa-onnx-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 17:48:29.247019 sherpa-onnx-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 17:37:18.000000 sherpa-onnx-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 17:48:29.247019 sherpa-onnx-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-23 17:37:18.000000 sherpa-onnx-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:48:29.243020 sherpa-onnx-1.4.5/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:48:29.243020 sherpa-onnx-1.4.5/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:48:29.247019 sherpa-onnx-1.4.5/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-23 17:48:29.000000 sherpa-onnx-1.4.5/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-23 17:37:18.000000 sherpa-onnx-1.4.5/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-23 17:37:18.000000 sherpa-onnx-1.4.5/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-23 17:37:18.000000 sherpa-onnx-1.4.5/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:48:29.247019 sherpa-onnx-1.4.5/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 17:48:29.000000 sherpa-onnx-1.4.5/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-23 17:48:29.000000 sherpa-onnx-1.4.5/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:48:29.000000 sherpa-onnx-1.4.5/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:48:29.000000 sherpa-onnx-1.4.5/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 17:48:29.000000 sherpa-onnx-1.4.5/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 17:48:29.000000 sherpa-onnx-1.4.5/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.244605 sherpa-onnx-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 10:32:03.244605 sherpa-onnx-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:32:03.244605 sherpa-onnx-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.240605 sherpa-onnx-1.4.6/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.240605 sherpa-onnx-1.4.6/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.240605 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.244605 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.4.5/LICENSE` & `sherpa-onnx-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.5/PKG-INFO` & `sherpa-onnx-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.5
+Version: 1.4.6
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.4.5/setup.py` & `sherpa-onnx-1.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.5/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.5/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.5/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.5/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.4.6/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.5
+Version: 1.4.6
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

