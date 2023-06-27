# Comparing `tmp/SpecLab-4.0.7.tar.gz` & `tmp/SpecLab-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpecLab-4.0.7.tar", last modified: Tue Jun 27 18:07:16 2023, max compression
+gzip compressed data, was "dist/SpecLab-4.0.8.tar", last modified: Tue Jun 27 18:37:10 2023, max compression
```

## Comparing `SpecLab-4.0.7.tar` & `SpecLab-4.0.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.0.7/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48678 2023-06-27 18:04:41.000000 SpecLab-4.0.7/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.0.7/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.0.7/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53071 2023-06-14 20:52:49.000000 SpecLab-4.0.7/SpecLab/gen/SpecLabFunctions.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.0.7/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.0.7/SpecLab/gen/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.0.7/SpecLab/gen/myfunc.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.0.7/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/aux/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/aux/param_files/
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-06-26 18:07:15.000000 SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param.default.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.0.7/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-06-26 18:06:59.000000 SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-06-26 18:06:44.000000 SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.0.7/SpecLab/aux/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   625389 2023-05-30 23:11:52.000000 SpecLab-4.0.7/SpecLab/aux/pyqtgraph10_speclab.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.0.7/SpecLab/doc/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      420 2023-06-26 17:45:13.000000 SpecLab-4.0.7/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1072 2023-06-26 17:41:16.000000 SpecLab-4.0.7/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.0.7/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     6325 2023-06-27 18:07:16.000000 SpecLab-4.0.7/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1424 2023-06-27 18:06:04.000000 SpecLab-4.0.7/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:37:10.000000 SpecLab-4.0.8/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:37:10.000000 SpecLab-4.0.8/SpecLab/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:37:10.000000 SpecLab-4.0.8/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.0.8/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48678 2023-06-27 18:35:53.000000 SpecLab-4.0.8/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:37:10.000000 SpecLab-4.0.8/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.0.8/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.0.8/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:37:10.000000 SpecLab-4.0.8/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53071 2023-06-14 20:52:49.000000 SpecLab-4.0.8/SpecLab/gen/SpecLabFunctions.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.0.8/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.0.8/SpecLab/gen/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.0.8/SpecLab/gen/myfunc.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.0.8/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:37:10.000000 SpecLab-4.0.8/SpecLab/aux/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:37:10.000000 SpecLab-4.0.8/SpecLab/aux/param_files/
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-06-26 18:07:15.000000 SpecLab-4.0.8/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.0.8/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-06-26 18:06:59.000000 SpecLab-4.0.8/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-06-26 18:06:44.000000 SpecLab-4.0.8/SpecLab/aux/param_files/imXam_param.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.0.8/SpecLab/aux/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   625389 2023-05-30 23:11:52.000000 SpecLab-4.0.8/SpecLab/aux/pyqtgraph10_speclab.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:37:10.000000 SpecLab-4.0.8/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.0.8/SpecLab/doc/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      470 2023-06-27 18:36:40.000000 SpecLab-4.0.8/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4595 2023-06-27 18:36:10.000000 SpecLab-4.0.8/SpecLab/doc/README.md
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1072 2023-06-26 17:41:16.000000 SpecLab-4.0.8/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.0.8/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     6354 2023-06-27 18:37:10.000000 SpecLab-4.0.8/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1389 2023-06-27 18:35:09.000000 SpecLab-4.0.8/setup.py
```

### Comparing `SpecLab-4.0.7/SpecLab/imXam/imXam.py` & `SpecLab-4.0.8/SpecLab/imXam/imXam.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: adam f kowalski, v4.0.7: June 27, 2023')
+print('imXam: adam f kowalski, v4.0.8: June 27, 2023')
 print(' To shut down gui, type q into terminal, type h for interactive commands, use middle mouse wheel to zoom in and out')
 print(' You may have to click on gui with left mouse button in order to use interactive commands')
 print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
```

### Comparing `SpecLab-4.0.7/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.0.8/SpecLab/cfg/SpecLab_config.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.0.8/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/gen/globals.py` & `SpecLab-4.0.8/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/gen/myfunc.py` & `SpecLab-4.0.8/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.0.8/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.0.8/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.0.8/SpecLab/aux/param_files/imXam_param.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/aux/pyqtgraph10_speclab.tar.gz` & `SpecLab-4.0.8/SpecLab/aux/pyqtgraph10_speclab.tar.gz`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/doc/KNOWN_ISSUES.txt` & `SpecLab-4.0.8/SpecLab/doc/KNOWN_ISSUES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/SpecLab/doc/LICENSE.txt` & `SpecLab-4.0.8/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.7/PKG-INFO` & `SpecLab-4.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.0
 Name: SpecLab
-Version: 4.0.7
+Version: 4.0.8
 Summary: IRAF imexam+DS9 replacement for Python
-Home-page: UNKNOWN
+Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 License: UNKNOWN
-Description: imXam: v4.0.7 (Latest)
+Description: imXam: v4.0.8 (Latest)
         ======================
         
         **imXam** is the first interactive program finished for the **SpecLab**
         python-only data reduction package. More (identify, standard, sensfunc,
         apall) will be added with the same GUI design (pyqtgraph10 + Plotly) in
         the future as these get finished.
```

