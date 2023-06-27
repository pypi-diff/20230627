# Comparing `tmp/kk-plugins-0.1.0.tar.gz` & `tmp/kk-plugins-0.1.230627.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kk-plugins-0.1.0.tar", last modified: Sun Apr 30 03:03:20 2023, max compression
+gzip compressed data, was "kk-plugins-0.1.230627.tar", last modified: Tue Jun 27 13:58:54 2023, max compression
```

## Comparing `kk-plugins-0.1.0.tar` & `kk-plugins-0.1.230627.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 03:03:07.000000 kk-plugins-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-30 03:03:07.000000 kk-plugins-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:03:20.806913 kk-plugins-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/src/kk_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-30 03:03:07.000000 kk-plugins-0.1.0/src/kk_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-30 03:03:07.000000 kk-plugins-0.1.0/src/kk_plugins/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/src/kk_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:54.972088 kk-plugins-0.1.230627/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-27 13:58:54.972088 kk-plugins-0.1.230627/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 13:58:39.000000 kk-plugins-0.1.230627/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:58:54.972088 kk-plugins-0.1.230627/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-27 13:58:39.000000 kk-plugins-0.1.230627/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:54.972088 kk-plugins-0.1.230627/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:54.972088 kk-plugins-0.1.230627/src/kk_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 13:58:39.000000 kk-plugins-0.1.230627/src/kk_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-27 13:58:39.000000 kk-plugins-0.1.230627/src/kk_plugins/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-27 13:58:39.000000 kk-plugins-0.1.230627/src/kk_plugins/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:54.972088 kk-plugins-0.1.230627/src/kk_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-27 13:58:54.000000 kk-plugins-0.1.230627/src/kk_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-27 13:58:54.000000 kk-plugins-0.1.230627/src/kk_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:58:54.000000 kk-plugins-0.1.230627/src/kk_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 13:58:54.000000 kk-plugins-0.1.230627/src/kk_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 13:58:54.000000 kk-plugins-0.1.230627/src/kk_plugins.egg-info/top_level.txt
```

### Comparing `kk-plugins-0.1.0/PKG-INFO` & `kk-plugins-0.1.230627/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.1.0
+Version: 0.1.230627
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kk-plugins-0.1.0/setup.py` & `kk-plugins-0.1.230627/setup.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.0/src/kk_plugins/project.py` & `kk-plugins-0.1.230627/src/kk_plugins/project.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.0/src/kk_plugins.egg-info/PKG-INFO` & `kk-plugins-0.1.230627/src/kk_plugins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.1.0
+Version: 0.1.230627
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

