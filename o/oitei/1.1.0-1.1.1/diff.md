# Comparing `tmp/oitei-1.1.0.tar.gz` & `tmp/oitei-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oitei-1.1.0.tar", last modified: Wed Jun 14 15:38:13 2023, max compression
+gzip compressed data, was "oitei-1.1.1.tar", last modified: Tue Jun 27 18:46:20 2023, max compression
```

## Comparing `oitei-1.1.0.tar` & `oitei-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-14 15:38:13.265866 oitei-1.1.0/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1443 2023-06-14 15:38:13.265866 oitei-1.1.0/PKG-INFO
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1153 2023-06-14 14:55:56.000000 oitei-1.1.0/README.md
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-14 15:38:13.265866 oitei-1.1.0/oitei/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      280 2023-06-14 15:36:18.000000 oitei-1.1.0/oitei/__init__.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)    18676 2023-06-14 14:55:56.000000 oitei-1.1.0/oitei/converter.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      327 2023-06-14 14:55:56.000000 oitei-1.1.0/oitei/namespaces.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1156 2023-06-14 14:55:56.000000 oitei-1.1.0/oitei/tei_template.py
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-14 15:38:13.265866 oitei-1.1.0/oitei.egg-info/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1443 2023-06-14 15:38:13.000000 oitei-1.1.0/oitei.egg-info/PKG-INFO
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      241 2023-06-14 15:38:13.000000 oitei-1.1.0/oitei.egg-info/SOURCES.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        1 2023-06-14 15:38:13.000000 oitei-1.1.0/oitei.egg-info/dependency_links.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)       11 2023-06-14 15:38:13.000000 oitei-1.1.0/oitei.egg-info/requires.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        6 2023-06-14 15:38:13.000000 oitei-1.1.0/oitei.egg-info/top_level.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)       38 2023-06-14 15:38:13.265866 oitei-1.1.0/setup.cfg
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      551 2023-06-14 15:36:42.000000 oitei-1.1.0/setup.py
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-27 18:46:20.129896 oitei-1.1.1/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1443 2023-06-27 18:46:20.129896 oitei-1.1.1/PKG-INFO
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1153 2023-06-14 14:55:56.000000 oitei-1.1.1/README.md
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-27 18:46:20.125896 oitei-1.1.1/oitei/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      280 2023-06-27 18:45:44.000000 oitei-1.1.1/oitei/__init__.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)    18676 2023-06-14 14:55:56.000000 oitei-1.1.1/oitei/converter.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      327 2023-06-14 14:55:56.000000 oitei-1.1.1/oitei/namespaces.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1156 2023-06-14 14:55:56.000000 oitei-1.1.1/oitei/tei_template.py
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2023-06-27 18:46:20.129896 oitei-1.1.1/oitei.egg-info/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1443 2023-06-27 18:46:20.000000 oitei-1.1.1/oitei.egg-info/PKG-INFO
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      241 2023-06-27 18:46:20.000000 oitei-1.1.1/oitei.egg-info/SOURCES.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        1 2023-06-27 18:46:20.000000 oitei-1.1.1/oitei.egg-info/dependency_links.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)       11 2023-06-27 18:46:20.000000 oitei-1.1.1/oitei.egg-info/requires.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        6 2023-06-27 18:46:20.000000 oitei-1.1.1/oitei.egg-info/top_level.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)       38 2023-06-27 18:46:20.129896 oitei-1.1.1/setup.cfg
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      551 2023-06-27 18:45:53.000000 oitei-1.1.1/setup.py
```

### Comparing `oitei-1.1.0/PKG-INFO` & `oitei-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oitei
-Version: 1.1.0
+Version: 1.1.1
 Summary: OpenITI mARkdown to TEI converter
 Home-page: http://github.com/OpenITI/oitei
 Author: Raff Viglianti
 Author-email: rviglian@umd.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `oitei-1.1.0/README.md` & `oitei-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oitei-1.1.0/oitei/converter.py` & `oitei-1.1.1/oitei/converter.py`

 * *Files identical despite different names*

### Comparing `oitei-1.1.0/oitei/tei_template.py` & `oitei-1.1.1/oitei/tei_template.py`

 * *Files identical despite different names*

### Comparing `oitei-1.1.0/oitei.egg-info/PKG-INFO` & `oitei-1.1.1/oitei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oitei
-Version: 1.1.0
+Version: 1.1.1
 Summary: OpenITI mARkdown to TEI converter
 Home-page: http://github.com/OpenITI/oitei
 Author: Raff Viglianti
 Author-email: rviglian@umd.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `oitei-1.1.0/setup.py` & `oitei-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "1.1.0"
+version = "1.1.1"
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="oitei",
     version=version,
```

