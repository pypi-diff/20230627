# Comparing `tmp/ipos-0.0.2.tar.gz` & `tmp/ipos-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipos-0.0.2.tar", last modified: Tue Jun 27 14:33:26 2023, max compression
+gzip compressed data, was "ipos-0.0.4.tar", last modified: Tue Jun 27 14:45:58 2023, max compression
```

## Comparing `ipos-0.0.2.tar` & `ipos-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:33:26.321557 ipos-0.0.2/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.2/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.2/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 14:33:26.321434 ipos-0.0.2/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.2/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:33:26.320361 ipos-0.0.2/ipos/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 14:33:21.000000 ipos-0.0.2/ipos/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     4629 2023-06-27 14:33:21.000000 ipos-0.0.2/ipos/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.2/ipos/core.py
--rw-r--r--   0 solst      (501) staff       (20)    18036 2023-06-27 14:33:21.000000 ipos-0.0.2/ipos/imp.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:33:26.321236 ipos-0.0.2/ipos.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.2/ipos.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 14:33:21.000000 ipos-0.0.2/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 14:33:26.321598 ipos-0.0.2/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.2/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:45:58.221802 ipos-0.0.4/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.4/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.4/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 14:45:58.221678 ipos-0.0.4/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.4/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:45:58.220299 ipos-0.0.4/ipos/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 14:45:51.000000 ipos-0.0.4/ipos/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     4629 2023-06-27 14:45:51.000000 ipos-0.0.4/ipos/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.4/ipos/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    18036 2023-06-27 14:45:51.000000 ipos-0.0.4/ipos/imp.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:45:58.221478 ipos-0.0.4/ipos.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 14:45:58.000000 ipos-0.0.4/ipos.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 14:45:58.000000 ipos-0.0.4/ipos.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:45:58.000000 ipos-0.0.4/ipos.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 14:45:58.000000 ipos-0.0.4/ipos.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.4/ipos.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 14:45:58.000000 ipos-0.0.4/ipos.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 14:45:58.000000 ipos-0.0.4/ipos.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 14:45:20.000000 ipos-0.0.4/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 14:45:58.221843 ipos-0.0.4/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.4/setup.py
```

### Comparing `ipos-0.0.2/LICENSE` & `ipos-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipos-0.0.2/PKG-INFO` & `ipos-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.2
+Version: 0.0.4
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.2/README.md` & `ipos-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ipos-0.0.2/ipos/_modidx.py` & `ipos-0.0.4/ipos/_modidx.py`

 * *Files identical despite different names*

### Comparing `ipos-0.0.2/ipos/imp.py` & `ipos-0.0.4/ipos/imp.py`

 * *Files identical despite different names*

### Comparing `ipos-0.0.2/ipos.egg-info/PKG-INFO` & `ipos-0.0.4/ipos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.2
+Version: 0.0.4
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.2/settings.ini` & `ipos-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ipos
 lib_name = ipos
-version = 0.0.2
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ipos
 nbs_path = nbs
 recursive = True
```

### Comparing `ipos-0.0.2/setup.py` & `ipos-0.0.4/setup.py`

 * *Files identical despite different names*

