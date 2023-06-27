# Comparing `tmp/oimdp-1.2.1.tar.gz` & `tmp/oimdp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oimdp-1.2.1.tar", last modified: Wed Jun 14 15:31:00 2023, max compression
+gzip compressed data, was "oimdp-1.3.0.tar", last modified: Tue Jun 27 18:16:27 2023, max compression
```

## Comparing `oimdp-1.2.1.tar` & `oimdp-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-14 15:31:00.232441 oimdp-1.2.1/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1082 2022-02-22 16:34:17.000000 oimdp-1.2.1/LICENSE
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1510 2023-06-14 15:31:00.232441 oimdp-1.2.1/PKG-INFO
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1208 2022-02-22 16:34:17.000000 oimdp-1.2.1/README.md
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-14 15:31:00.232441 oimdp-1.2.1/oimdp/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      143 2023-06-14 14:39:51.000000 oimdp-1.2.1/oimdp/__init__.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)    13117 2022-06-07 19:35:03.000000 oimdp-1.2.1/oimdp/parser.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     7112 2022-06-07 15:57:26.000000 oimdp-1.2.1/oimdp/structures.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1655 2022-06-07 16:06:14.000000 oimdp-1.2.1/oimdp/tags.py
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-14 15:31:00.232441 oimdp-1.2.1/oimdp.egg-info/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1510 2023-06-14 15:31:00.000000 oimdp-1.2.1/oimdp.egg-info/PKG-INFO
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      210 2023-06-14 15:31:00.000000 oimdp-1.2.1/oimdp.egg-info/SOURCES.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        1 2023-06-14 15:31:00.000000 oimdp-1.2.1/oimdp.egg-info/dependency_links.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        6 2023-06-14 15:31:00.000000 oimdp-1.2.1/oimdp.egg-info/top_level.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)       38 2023-06-14 15:31:00.232441 oimdp-1.2.1/setup.cfg
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      478 2023-06-14 14:43:00.000000 oimdp-1.2.1/setup.py
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-27 18:16:27.322096 oimdp-1.3.0/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1082 2022-02-22 16:34:17.000000 oimdp-1.3.0/LICENSE
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1510 2023-06-27 18:16:27.322096 oimdp-1.3.0/PKG-INFO
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1208 2022-02-22 16:34:17.000000 oimdp-1.3.0/README.md
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-27 18:16:27.322096 oimdp-1.3.0/oimdp/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      143 2023-06-27 18:14:43.000000 oimdp-1.3.0/oimdp/__init__.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)    13159 2023-06-27 15:05:07.000000 oimdp-1.3.0/oimdp/parser.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     7112 2022-06-07 15:57:26.000000 oimdp-1.3.0/oimdp/structures.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1655 2022-06-07 16:06:14.000000 oimdp-1.3.0/oimdp/tags.py
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-27 18:16:27.322096 oimdp-1.3.0/oimdp.egg-info/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1510 2023-06-27 18:16:27.000000 oimdp-1.3.0/oimdp.egg-info/PKG-INFO
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      210 2023-06-27 18:16:27.000000 oimdp-1.3.0/oimdp.egg-info/SOURCES.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        1 2023-06-27 18:16:27.000000 oimdp-1.3.0/oimdp.egg-info/dependency_links.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        6 2023-06-27 18:16:27.000000 oimdp-1.3.0/oimdp.egg-info/top_level.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)       38 2023-06-27 18:16:27.322096 oimdp-1.3.0/setup.cfg
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      478 2023-06-27 18:15:01.000000 oimdp-1.3.0/setup.py
```

### Comparing `oimdp-1.2.1/LICENSE` & `oimdp-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oimdp-1.2.1/PKG-INFO` & `oimdp-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oimdp
-Version: 1.2.1
+Version: 1.3.0
 Summary: OpenITI mARkdown Parser
 Home-page: http://github.com/OpenITI/oimdp
 Author: Raff Viglianti
 Author-email: rviglian@umd.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `oimdp-1.2.1/README.md` & `oimdp-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `oimdp-1.2.1/oimdp/parser.py` & `oimdp-1.3.0/oimdp/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     # Magic value
     magic_value = ilines[0]
     
     if strict and magic_value.strip() != "######OpenITI#":
         raise Exception(
             "This does not appear to be an OpenITI mARkdown document (strict mode)")
         sys.exit(1)
-    elif not magic_value.strip().startswith("######OpenITI#"):
+    elif not magic_value.strip().encode('ascii', 'ignore').decode('ascii').startswith("######OpenITI#"):
         raise Exception(
             "This does not appear to be an OpenITI mARkdown document")
         sys.exit(1)
 
     document.set_magic_value(magic_value)
 
     # RE patterns
```

### Comparing `oimdp-1.2.1/oimdp/structures.py` & `oimdp-1.3.0/oimdp/structures.py`

 * *Files identical despite different names*

### Comparing `oimdp-1.2.1/oimdp/tags.py` & `oimdp-1.3.0/oimdp/tags.py`

 * *Files identical despite different names*

### Comparing `oimdp-1.2.1/oimdp.egg-info/PKG-INFO` & `oimdp-1.3.0/oimdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oimdp
-Version: 1.2.1
+Version: 1.3.0
 Summary: OpenITI mARkdown Parser
 Home-page: http://github.com/OpenITI/oimdp
 Author: Raff Viglianti
 Author-email: rviglian@umd.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

