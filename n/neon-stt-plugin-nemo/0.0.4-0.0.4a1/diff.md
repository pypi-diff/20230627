# Comparing `tmp/neon-stt-plugin-nemo-0.0.4.tar.gz` & `tmp/neon-stt-plugin-nemo-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-stt-plugin-nemo-0.0.4.tar", last modified: Tue Jun 27 01:15:36 2023, max compression
+gzip compressed data, was "neon-stt-plugin-nemo-0.0.4a1.tar", last modified: Mon Jun 26 22:36:51 2023, max compression
```

## Comparing `neon-stt-plugin-nemo-0.0.4.tar` & `neon-stt-plugin-nemo-0.0.4a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:15:36.603062 neon-stt-plugin-nemo-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-27 01:15:32.000000 neon-stt-plugin-nemo-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-27 01:15:36.599063 neon-stt-plugin-nemo-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-27 01:15:32.000000 neon-stt-plugin-nemo-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:15:36.599063 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo/
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-27 01:15:32.000000 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:15:36.599063 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-27 01:15:36.000000 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 01:15:36.000000 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 01:15:36.000000 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-27 01:15:36.000000 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-27 01:15:36.000000 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 01:15:36.000000 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 01:15:36.000000 neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 01:15:36.603062 neon-stt-plugin-nemo-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-27 01:15:32.000000 neon-stt-plugin-nemo-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:36:51.726382 neon-stt-plugin-nemo-0.0.4a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-26 22:36:46.000000 neon-stt-plugin-nemo-0.0.4a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-26 22:36:51.726382 neon-stt-plugin-nemo-0.0.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-26 22:36:46.000000 neon-stt-plugin-nemo-0.0.4a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:36:51.722382 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-26 22:36:46.000000 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:36:51.726382 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-26 22:36:51.000000 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 22:36:51.000000 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:36:51.000000 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 22:36:51.000000 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-26 22:36:51.000000 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 22:36:51.000000 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:36:51.000000 neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:36:51.726382 neon-stt-plugin-nemo-0.0.4a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-26 22:36:46.000000 neon-stt-plugin-nemo-0.0.4a1/setup.py
```

### Comparing `neon-stt-plugin-nemo-0.0.4/LICENSE.md` & `neon-stt-plugin-nemo-0.0.4a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-stt-plugin-nemo-0.0.4/PKG-INFO` & `neon-stt-plugin-nemo-0.0.4a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-stt-plugin-nemo
-Version: 0.0.4
+Version: 0.0.4a1
 Summary: Nemo STT plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-stt-plugin-nemo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin stt
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-stt-plugin-nemo-0.0.4/README.md` & `neon-stt-plugin-nemo-0.0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo/__init__.py` & `neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-stt-plugin-nemo-0.0.4/neon_stt_plugin_nemo.egg-info/PKG-INFO` & `neon-stt-plugin-nemo-0.0.4a1/neon_stt_plugin_nemo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-stt-plugin-nemo
-Version: 0.0.4
+Version: 0.0.4a1
 Summary: Nemo STT plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-stt-plugin-nemo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin stt
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-stt-plugin-nemo-0.0.4/setup.py` & `neon-stt-plugin-nemo-0.0.4a1/setup.py`

 * *Files identical despite different names*

