# Comparing `tmp/ieseg_credscore-0.23.5.tar.gz` & `tmp/ieseg_credscore-0.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieseg_credscore-0.23.5.tar", last modified: Tue Jun 27 12:46:49 2023, max compression
+gzip compressed data, was "ieseg_credscore-0.23.6.tar", last modified: Tue Jun 27 12:51:22 2023, max compression
```

## Comparing `ieseg_credscore-0.23.5.tar` & `ieseg_credscore-0.23.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:46:49.345426 ieseg_credscore-0.23.5/
--rw-rw-rw-   0        0        0     1092 2023-06-26 15:40:57.000000 ieseg_credscore-0.23.5/LICENSE.rst
--rw-rw-rw-   0        0        0     2942 2023-06-27 12:46:49.345426 ieseg_credscore-0.23.5/PKG-INFO
--rw-rw-rw-   0        0        0     2606 2023-06-26 16:44:47.000000 ieseg_credscore-0.23.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 12:46:49.270677 ieseg_credscore-0.23.5/ieseg_credscore/
--rw-rw-rw-   0        0        0     4597 2022-02-04 14:15:05.000000 ieseg_credscore-0.23.5/ieseg_credscore/OBG.py
--rw-rw-rw-   0        0        0    46370 2023-06-27 12:44:58.000000 ieseg_credscore-0.23.5/ieseg_credscore/WOE.py
--rw-rw-rw-   0        0        0       58 2023-06-27 12:18:23.000000 ieseg_credscore-0.23.5/ieseg_credscore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:46:49.334464 ieseg_credscore-0.23.5/ieseg_credscore.egg-info/
--rw-rw-rw-   0        0        0     2942 2023-06-27 12:46:48.000000 ieseg_credscore-0.23.5/ieseg_credscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-06-27 12:46:49.000000 ieseg_credscore-0.23.5/ieseg_credscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:46:48.000000 ieseg_credscore-0.23.5/ieseg_credscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 12:46:48.000000 ieseg_credscore-0.23.5/ieseg_credscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 12:46:48.000000 ieseg_credscore-0.23.5/ieseg_credscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-27 12:46:49.355395 ieseg_credscore-0.23.5/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-06-27 12:46:08.000000 ieseg_credscore-0.23.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:51:22.934836 ieseg_credscore-0.23.6/
+-rw-rw-rw-   0        0        0     1092 2023-06-26 15:40:57.000000 ieseg_credscore-0.23.6/LICENSE.rst
+-rw-rw-rw-   0        0        0     2942 2023-06-27 12:51:22.935833 ieseg_credscore-0.23.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-26 16:44:47.000000 ieseg_credscore-0.23.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 12:51:22.831183 ieseg_credscore-0.23.6/ieseg_credscore/
+-rw-rw-rw-   0        0        0     4597 2022-02-04 14:15:05.000000 ieseg_credscore-0.23.6/ieseg_credscore/OBG.py
+-rw-rw-rw-   0        0        0    46380 2023-06-27 12:50:14.000000 ieseg_credscore-0.23.6/ieseg_credscore/WOE.py
+-rw-rw-rw-   0        0        0       58 2023-06-27 12:18:23.000000 ieseg_credscore-0.23.6/ieseg_credscore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:51:22.920884 ieseg_credscore-0.23.6/ieseg_credscore.egg-info/
+-rw-rw-rw-   0        0        0     2942 2023-06-27 12:51:22.000000 ieseg_credscore-0.23.6/ieseg_credscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-27 12:51:22.000000 ieseg_credscore-0.23.6/ieseg_credscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:51:22.000000 ieseg_credscore-0.23.6/ieseg_credscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 12:51:22.000000 ieseg_credscore-0.23.6/ieseg_credscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 12:51:22.000000 ieseg_credscore-0.23.6/ieseg_credscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-27 12:51:22.948792 ieseg_credscore-0.23.6/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-06-27 12:51:15.000000 ieseg_credscore-0.23.6/setup.py
```

### Comparing `ieseg_credscore-0.23.5/LICENSE.rst` & `ieseg_credscore-0.23.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.5/PKG-INFO` & `ieseg_credscore-0.23.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg_credscore
-Version: 0.23.5
+Version: 0.23.6
 Summary: Credit Scoring - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Credit Scoring IESEG
 Description-Content-Type: text/markdown
```

### Comparing `ieseg_credscore-0.23.5/README.md` & `ieseg_credscore-0.23.6/README.md`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.5/ieseg_credscore/OBG.py` & `ieseg_credscore-0.23.6/ieseg_credscore/OBG.py`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.5/ieseg_credscore/WOE.py` & `ieseg_credscore-0.23.6/ieseg_credscore/WOE.py`

 * *Files 0% similar despite different names*

```diff
@@ -655,20 +655,20 @@
              
     #### Check for correct variable specification and
     #### generate requested output, in case specification is correct
     
     ### Display warning message in case of incorrect predictor variable specification
     
     if (dfrm.iloc[:,1].dtypes.kind in 'bifc') == False and (dfrm.iloc[:,1].dtypes=="category")==False:
-    	warnings.warn("Incorrect variable specification.\nPredictor variable needs to be a numeric variable or a factor.")
+        warnings.warn("Incorrect variable specification.\nPredictor variable needs to be a numeric variable or a factor.")
 
     ### Generate requested output, in case specification is correct
     else:
         ## Function passes the final binning solution as look-up table
-        look_up_table
+        return look_up_table
         
     return binning
 
 def woe_binning (df, target_var, pred_var, min_perc_total, min_perc_class, stop_limit, abbrev_fact_levels, event_class):
 #### Warning message and defaults in case parameters are not specified
     if df.isnull().values.any()==True or type(target_var) is str == False or type(pred_var) is str == False:
         warnings.warn("Incorrect specification of data frame and/or variables.")
```

### Comparing `ieseg_credscore-0.23.5/ieseg_credscore.egg-info/PKG-INFO` & `ieseg_credscore-0.23.6/ieseg_credscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg-credscore
-Version: 0.23.5
+Version: 0.23.6
 Summary: Credit Scoring - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Credit Scoring IESEG
 Description-Content-Type: text/markdown
```

### Comparing `ieseg_credscore-0.23.5/setup.py` & `ieseg_credscore-0.23.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ieseg_credscore',
-    version='0.23.5',
+    version='0.23.6',
     license='MIT',
     author="Philipp Borchert",
     author_email='p.borchert@ieseg.fr',
     packages=find_packages(),
     description = 'Credit Scoring - IESEG School of Management',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

