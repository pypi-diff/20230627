# Comparing `tmp/qqwry-linux-python3-0.0.5.tar.gz` & `tmp/qqwry-linux-python3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qqwry-linux-python3-0.0.5.tar", last modified: Tue Jun 27 07:54:52 2023, max compression
+gzip compressed data, was "dist/qqwry-linux-python3-0.0.6.tar", last modified: Tue Jun 27 08:04:11 2023, max compression
```

## Comparing `qqwry-linux-python3-0.0.5.tar` & `qqwry-linux-python3-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/
--rw-r--r--   0 root         (0) root         (0)    11558 2023-03-22 07:03:34.000000 qqwry-linux-python3-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-27 04:20:12.000000 qqwry-linux-python3-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry/
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-27 07:54:28.000000 qqwry-linux-python3-0.0.5/qqwry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry/shell/
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.5/qqwry/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.5/qqwry/shell/usage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry/src/
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-27 07:01:25.000000 qqwry-linux-python3-0.0.5/qqwry/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-06-27 06:07:50.000000 qqwry-linux-python3-0.0.5/qqwry/src/qqwry.py
--rw-r--r--   0 root         (0) root         (0)     7643 2023-06-27 07:54:13.000000 qqwry-linux-python3-0.0.5/qqwry/src/update_qqwry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 06:54:25.000000 qqwry-linux-python3-0.0.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-27 06:48:57.000000 qqwry-linux-python3-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-03-22 07:03:34.000000 qqwry-linux-python3-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-06-27 08:03:05.000000 qqwry-linux-python3-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-27 08:04:03.000000 qqwry-linux-python3-0.0.6/qqwry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry/shell/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.6/qqwry/shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.6/qqwry/shell/usage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry/src/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-27 07:01:25.000000 qqwry-linux-python3-0.0.6/qqwry/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-27 06:07:50.000000 qqwry-linux-python3-0.0.6/qqwry/src/qqwry.py
+-rw-r--r--   0 root         (0) root         (0)     7643 2023-06-27 07:54:13.000000 qqwry-linux-python3-0.0.6/qqwry/src/update_qqwry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry_linux_python3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry_linux_python3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry_linux_python3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry_linux_python3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry_linux_python3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry_linux_python3.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/qqwry_linux_python3.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 06:54:25.000000 qqwry-linux-python3-0.0.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 08:04:11.000000 qqwry-linux-python3-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-27 06:48:57.000000 qqwry-linux-python3-0.0.6/setup.py
```

### Comparing `qqwry-linux-python3-0.0.5/LICENSE` & `qqwry-linux-python3-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qqwry-linux-python3-0.0.5/qqwry/src/qqwry.py` & `qqwry-linux-python3-0.0.6/qqwry/src/qqwry.py`

 * *Files identical despite different names*

### Comparing `qqwry-linux-python3-0.0.5/qqwry/src/update_qqwry.py` & `qqwry-linux-python3-0.0.6/qqwry/src/update_qqwry.py`

 * *Files identical despite different names*

### Comparing `qqwry-linux-python3-0.0.5/setup.py` & `qqwry-linux-python3-0.0.6/setup.py`

 * *Files identical despite different names*

