# Comparing `tmp/ocamlec_plt-0.0.3.tar.gz` & `tmp/ocamlec_plt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocamlec_plt-0.0.3.tar", last modified: Tue Jun 27 10:02:58 2023, max compression
+gzip compressed data, was "ocamlec_plt-0.0.4.tar", last modified: Tue Jun 27 10:33:57 2023, max compression
```

## Comparing `ocamlec_plt-0.0.3.tar` & `ocamlec_plt-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:02:58.986934 ocamlec_plt-0.0.3/
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      529 2023-06-27 10:02:58.986934 ocamlec_plt-0.0.3/PKG-INFO
-drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:02:58.986934 ocamlec_plt-0.0.3/coevolution/
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      192 2023-06-27 09:30:09.000000 ocamlec_plt-0.0.3/coevolution/__init__.py
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)     6655 2023-06-27 09:28:38.000000 ocamlec_plt-0.0.3/coevolution/champions.py
-drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:02:58.986934 ocamlec_plt-0.0.3/ocamlec_plt.egg-info/
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      529 2023-06-27 10:02:58.000000 ocamlec_plt-0.0.3/ocamlec_plt.egg-info/PKG-INFO
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      231 2023-06-27 10:02:58.000000 ocamlec_plt-0.0.3/ocamlec_plt.egg-info/SOURCES.txt
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)        1 2023-06-27 10:02:58.000000 ocamlec_plt-0.0.3/ocamlec_plt.egg-info/dependency_links.txt
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       48 2023-06-27 10:02:58.000000 ocamlec_plt-0.0.3/ocamlec_plt.egg-info/requires.txt
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       12 2023-06-27 10:02:58.000000 ocamlec_plt-0.0.3/ocamlec_plt.egg-info/top_level.txt
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       38 2023-06-27 10:02:58.986934 ocamlec_plt-0.0.3/setup.cfg
--rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)     1238 2023-06-27 10:02:43.000000 ocamlec_plt-0.0.3/setup.py
+drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      579 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/PKG-INFO
+drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/coevolution/
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      192 2023-06-27 09:30:09.000000 ocamlec_plt-0.0.4/coevolution/__init__.py
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)     6655 2023-06-27 09:28:38.000000 ocamlec_plt-0.0.4/coevolution/champions.py
+drwxr-xr-x   0 mariohevia  (1000) mariohevia  (1000)        0 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      579 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/PKG-INFO
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)      231 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/SOURCES.txt
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)        1 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/dependency_links.txt
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       48 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/requires.txt
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       12 2023-06-27 10:33:57.000000 ocamlec_plt-0.0.4/ocamlec_plt.egg-info/top_level.txt
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)       38 2023-06-27 10:33:57.851174 ocamlec_plt-0.0.4/setup.cfg
+-rw-r--r--   0 mariohevia  (1000) mariohevia  (1000)     1291 2023-06-27 10:33:48.000000 ocamlec_plt-0.0.4/setup.py
```

### Comparing `ocamlec_plt-0.0.3/PKG-INFO` & `ocamlec_plt-0.0.4/ocamlec_plt.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: ocamlec_plt
-Version: 0.0.3
+Name: ocamlec-plt
+Version: 0.0.4
 Summary: OcamlEC plots
 Author: Mario Hevia Fajardo
 Author-email: <m.heviafajardo@bham.ac.uk>
 Keywords: python,ocamlec
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Visualization
 
 Package to plot and get statistics from OcamlEC files
```

### Comparing `ocamlec_plt-0.0.3/coevolution/champions.py` & `ocamlec_plt-0.0.4/coevolution/champions.py`

 * *Files identical despite different names*

### Comparing `ocamlec_plt-0.0.3/ocamlec_plt.egg-info/PKG-INFO` & `ocamlec_plt-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: ocamlec-plt
-Version: 0.0.3
+Name: ocamlec_plt
+Version: 0.0.4
 Summary: OcamlEC plots
 Author: Mario Hevia Fajardo
 Author-email: <m.heviafajardo@bham.ac.uk>
 Keywords: python,ocamlec
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Visualization
 
 Package to plot and get statistics from OcamlEC files
```

### Comparing `ocamlec_plt-0.0.3/setup.py` & `ocamlec_plt-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on Tue Jun 27 10:32:16 2023
 
 @author: mariohevia
 """
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'OcamlEC plots'
 LONG_DESCRIPTION = 'Package to plot and get statistics from OcamlEC files'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ocamlec_plt", 
@@ -30,10 +30,11 @@
         keywords=['python', 'ocamlec'],
         classifiers= [
             "Development Status :: 2 - Pre-Alpha",
             "Intended Audience :: Science/Research",
             "Intended Audience :: Education",
             "License :: Free for non-commercial use",
             "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.9",
             "Topic :: Scientific/Engineering :: Visualization"
         ]
 )
```

