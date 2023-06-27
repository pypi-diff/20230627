# Comparing `tmp/vsiew-2.3.6.tar.gz` & `tmp/vsiew-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.3.6.tar", last modified: Fri Jun 23 22:50:03 2023, max compression
+gzip compressed data, was "vsiew-2.3.7.tar", last modified: Tue Jun 27 17:16:31 2023, max compression
```

## Comparing `vsiew-2.3.6.tar` & `vsiew-2.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:50:03.338345 vsiew-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 22:49:38.000000 vsiew-2.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-23 22:50:03.338345 vsiew-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-23 22:49:38.000000 vsiew-2.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:50:03.338345 vsiew-2.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-23 22:49:38.000000 vsiew-2.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:50:03.334345 vsiew-2.3.6/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-23 22:49:38.000000 vsiew-2.3.6/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 22:49:38.000000 vsiew-2.3.6/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-23 22:49:38.000000 vsiew-2.3.6/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-23 22:49:38.000000 vsiew-2.3.6/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:50:03.338345 vsiew-2.3.6/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:31.038188 vsiew-2.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-27 17:16:09.000000 vsiew-2.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 17:16:31.038188 vsiew-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 17:16:09.000000 vsiew-2.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:16:31.038188 vsiew-2.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 17:16:09.000000 vsiew-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:31.038188 vsiew-2.3.7/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-27 17:16:09.000000 vsiew-2.3.7/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 17:16:09.000000 vsiew-2.3.7/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-27 17:16:09.000000 vsiew-2.3.7/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-27 17:16:09.000000 vsiew-2.3.7/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:31.038188 vsiew-2.3.7/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.3.6/LICENSE` & `vsiew-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.6/PKG-INFO` & `vsiew-2.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.6
+Version: 2.3.7
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.3.6/setup.py` & `vsiew-2.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.6/vsiew/__init__.py` & `vsiew-2.3.7/vsiew/__init__.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.6/vsiew/init.py` & `vsiew-2.3.7/vsiew/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             return 1
 
     def _get_uninstall_call(package: str) -> int:
         from subprocess import check_call
 
         try:
             return check_call([
-                sys.executable, '-m', 'pip', 'uninstall', package
+                sys.executable, '-m', 'pip', 'uninstall', package, '-y'
             ])
         except Exception:
             return 1
 
     def _get_iew_packages() -> Iterator[tuple[str, str]]:
         from http.client import HTTPSConnection
```

### Comparing `vsiew-2.3.6/vsiew.egg-info/PKG-INFO` & `vsiew-2.3.7/vsiew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.6
+Version: 2.3.7
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

