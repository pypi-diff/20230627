# Comparing `tmp/ocamlec_plt-0.0.4.tar.gz` & `tmp/ocamlec_plt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocamlec_plt-0.0.4.tar", last modified: Tue Jun 27 10:33:57 2023, max compression
+gzip compressed data, was "ocamlec_plt-0.0.5.tar", last modified: Tue Jun 27 10:44:17 2023, max compression
```

## Comparing `ocamlec_plt-0.0.4.tar` & `ocamlec_plt-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      579 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/PKG-INFO
-drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/coevolution/
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      192 2023-06-27 09:30:09.000000 ocamlec_plt-0.0.4/coevolution/__init__.py
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)     6655 2023-06-27 09:28:38.000000 ocamlec_plt-0.0.4/coevolution/champions.py
-drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      579 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/PKG-INFO
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      231 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/SOURCES.txt
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)        1 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/dependency_links.txt
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       48 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/requires.txt
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       12 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/top_level.txt
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       38 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/setup.cfg
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)     1291 2023-06-27 10:33:48.000000 ocamlec_plt-0.0.4/setup.py
+drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:44:17.837170 ocamlec_plt-0.0.5/
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      579 2023-06-27 10:44:17.837170 ocamlec_plt-0.0.5/PKG-INFO
+drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:44:17.837170 ocamlec_plt-0.0.5/ocamlec_plt/
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      264 2023-06-27 09:31:49.000000 ocamlec_plt-0.0.5/ocamlec_plt/__init__.py
+drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:44:17.837170 ocamlec_plt-0.0.5/ocamlec_plt/coevolution/
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      192 2023-06-27 09:30:09.000000 ocamlec_plt-0.0.5/ocamlec_plt/coevolution/__init__.py
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)     6655 2023-06-27 09:28:38.000000 ocamlec_plt-0.0.5/ocamlec_plt/coevolution/champions.py
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)    37612 2023-06-27 08:41:36.000000 ocamlec_plt-0.0.5/ocamlec_plt/utils.py
+drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:44:17.837170 ocamlec_plt-0.0.5/ocamlec_plt.egg-info/
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      579 2023-06-27 10:44:17.000000 ocamlec_plt-0.0.5/ocamlec_plt.egg-info/PKG-INFO
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      300 2023-06-27 10:44:17.000000 ocamlec_plt-0.0.5/ocamlec_plt.egg-info/SOURCES.txt
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)        1 2023-06-27 10:44:17.000000 ocamlec_plt-0.0.5/ocamlec_plt.egg-info/dependency_links.txt
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       48 2023-06-27 10:44:17.000000 ocamlec_plt-0.0.5/ocamlec_plt.egg-info/requires.txt
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       12 2023-06-27 10:44:17.000000 ocamlec_plt-0.0.5/ocamlec_plt.egg-info/top_level.txt
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       38 2023-06-27 10:44:17.837170 ocamlec_plt-0.0.5/setup.cfg
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)     1286 2023-06-27 10:42:19.000000 ocamlec_plt-0.0.5/setup.py
```

### Comparing `ocamlec_plt-0.0.4/PKG-INFO` & `ocamlec_plt-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocamlec_plt
-Version: 0.0.4
+Version: 0.0.5
 Summary: OcamlEC plots
 Author: Mario Hevia Fajardo
 Author-email: <m.heviafajardo@bham.ac.uk>
 Keywords: python,ocamlec
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
```

### Comparing `ocamlec_plt-0.0.4/coevolution/champions.py` & `ocamlec_plt-0.0.5/ocamlec_plt/coevolution/champions.py`

 * *Files identical despite different names*

### Comparing `ocamlec_plt-0.0.4/ocamlec_plt.egg-info/PKG-INFO` & `ocamlec_plt-0.0.5/ocamlec_plt.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocamlec-plt
-Version: 0.0.4
+Version: 0.0.5
 Summary: OcamlEC plots
 Author: Mario Hevia Fajardo
 Author-email: <m.heviafajardo@bham.ac.uk>
 Keywords: python,ocamlec
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
```

### Comparing `ocamlec_plt-0.0.4/setup.py` & `ocamlec_plt-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 Created on Tue Jun 27 10:32:16 2023
 
 @author: mariohevia
 """
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'OcamlEC plots'
 LONG_DESCRIPTION = 'Package to plot and get statistics from OcamlEC files'
 
 # Setting up
 setup(
-       # the name must match the folder name 'verysimplemodule'
+       # the name must match the folder name 'ocamlec_plt'
         name="ocamlec_plt", 
         version=VERSION,
         author="Mario Hevia Fajardo",
         author_email="<m.heviafajardo@bham.ac.uk>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
```

