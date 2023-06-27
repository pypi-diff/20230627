# Comparing `tmp/ieseg_credscore-0.23.8.tar.gz` & `tmp/ieseg_credscore-0.23.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieseg_credscore-0.23.8.tar", last modified: Tue Jun 27 13:01:27 2023, max compression
+gzip compressed data, was "ieseg_credscore-0.23.9.tar", last modified: Tue Jun 27 13:06:26 2023, max compression
```

## Comparing `ieseg_credscore-0.23.8.tar` & `ieseg_credscore-0.23.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:01:27.602667 ieseg_credscore-0.23.8/
--rw-rw-rw-   0        0        0     1092 2023-06-26 15:40:57.000000 ieseg_credscore-0.23.8/LICENSE.rst
--rw-rw-rw-   0        0        0     2942 2023-06-27 13:01:27.602667 ieseg_credscore-0.23.8/PKG-INFO
--rw-rw-rw-   0        0        0     2606 2023-06-26 16:44:47.000000 ieseg_credscore-0.23.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 13:01:27.520942 ieseg_credscore-0.23.8/ieseg_credscore/
--rw-rw-rw-   0        0        0     4597 2022-02-04 14:15:05.000000 ieseg_credscore-0.23.8/ieseg_credscore/OBG.py
--rw-rw-rw-   0        0        0    46382 2023-06-27 13:00:33.000000 ieseg_credscore-0.23.8/ieseg_credscore/WOE.py
--rw-rw-rw-   0        0        0       58 2023-06-27 12:18:23.000000 ieseg_credscore-0.23.8/ieseg_credscore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:01:27.589710 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/
--rw-rw-rw-   0        0        0     2942 2023-06-27 13:01:26.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-06-27 13:01:27.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:01:26.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 13:01:26.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 13:01:26.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-27 13:01:27.613631 ieseg_credscore-0.23.8/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-06-27 13:01:17.000000 ieseg_credscore-0.23.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:06:26.778292 ieseg_credscore-0.23.9/
+-rw-rw-rw-   0        0        0     1092 2023-06-26 15:40:57.000000 ieseg_credscore-0.23.9/LICENSE.rst
+-rw-rw-rw-   0        0        0     2942 2023-06-27 13:06:26.779302 ieseg_credscore-0.23.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-26 16:44:47.000000 ieseg_credscore-0.23.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 13:06:26.696538 ieseg_credscore-0.23.9/ieseg_credscore/
+-rw-rw-rw-   0        0        0     4597 2022-02-04 14:15:05.000000 ieseg_credscore-0.23.9/ieseg_credscore/OBG.py
+-rw-rw-rw-   0        0        0    46392 2023-06-27 13:06:07.000000 ieseg_credscore-0.23.9/ieseg_credscore/WOE.py
+-rw-rw-rw-   0        0        0       58 2023-06-27 12:18:23.000000 ieseg_credscore-0.23.9/ieseg_credscore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:06:26.766303 ieseg_credscore-0.23.9/ieseg_credscore.egg-info/
+-rw-rw-rw-   0        0        0     2942 2023-06-27 13:06:26.000000 ieseg_credscore-0.23.9/ieseg_credscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-27 13:06:26.000000 ieseg_credscore-0.23.9/ieseg_credscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:06:26.000000 ieseg_credscore-0.23.9/ieseg_credscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 13:06:26.000000 ieseg_credscore-0.23.9/ieseg_credscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 13:06:26.000000 ieseg_credscore-0.23.9/ieseg_credscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-27 13:06:26.790224 ieseg_credscore-0.23.9/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-06-27 13:06:17.000000 ieseg_credscore-0.23.9/setup.py
```

### Comparing `ieseg_credscore-0.23.8/LICENSE.rst` & `ieseg_credscore-0.23.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.8/PKG-INFO` & `ieseg_credscore-0.23.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg_credscore
-Version: 0.23.8
+Version: 0.23.9
 Summary: Credit Scoring - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Credit Scoring IESEG
 Description-Content-Type: text/markdown
```

### Comparing `ieseg_credscore-0.23.8/README.md` & `ieseg_credscore-0.23.9/README.md`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.8/ieseg_credscore/OBG.py` & `ieseg_credscore-0.23.9/ieseg_credscore/OBG.py`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.8/ieseg_credscore/WOE.py` & `ieseg_credscore-0.23.9/ieseg_credscore/WOE.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,16 @@
     df = df[[target_var, pred_var]] # used for final binning
     dfrm = df[[target_var, pred_var]]# used for iterative merging of bins
     dfrm.columns = ['target_var','predictor_var']
 
     #### Check if numerical variable or factor was provided as predictor and apply appropriate binning technique
 
     ### Binning in case a numerical variable was selected
-    if len(dfrm.iloc[:,0].drop_duplicates()) == 2 and (dfrm.iloc[:,1].dtypes.kind in 'bifc') == True:
+    # if len(dfrm.iloc[:,0].drop_duplicates()) == 2 and (dfrm.iloc[:,1].dtypes.kind in 'bifc') == True:
+    if len(dfrm.iloc[:,0].drop_duplicates()) == 2:
         ## Derive number of initial bins from min.perc.total parameter
         max_bins = math.trunc(1/min_perc_total)
         
         ## Derive cutpoints for bins (with similar frequency)
         cutpoints = dfrm.predictor_var.quantile(np.arange(0,max_bins+1)/max_bins).reset_index(drop=True)
         innercutpoints = [-np.inf] + list(cutpoints[1:len(cutpoints)-1]) + [np.inf]  # add -Inf, +Inf to cutpoints
         cutpoints = list(dict.fromkeys(innercutpoints))
@@ -642,26 +643,26 @@
             look_up_table = look_up_table.rename(index=str, columns={0: "bad", 1: "good"})
         elif good == 0 and bad== 1:    
             look_up_table = look_up_table.rename(index=str, columns={0: "good", 1: "bad"})  
             
         binning=look_up_table
             
              
-        #### Check for correct variable specification and
-        #### generate requested output, in case specification is correct
-        
-        ### Display warning message in case of incorrect predictor variable specification
-        
-        if (dfrm.iloc[:,1].dtypes.kind in 'bifc') == False and (dfrm.iloc[:,1].dtypes=="category")==False:
-            warnings.warn("Incorrect variable specification.\nPredictor variable needs to be a numeric variable or a factor.")
+    #### Check for correct variable specification and
+    #### generate requested output, in case specification is correct
+    
+    ### Display warning message in case of incorrect predictor variable specification
+    
+    if (dfrm.iloc[:,1].dtypes.kind in 'bifc') == False and (dfrm.iloc[:,1].dtypes=="category")==False:
+        warnings.warn("Incorrect variable specification.\nPredictor variable needs to be a numeric variable or a factor.")
 
-        ### Generate requested output, in case specification is correct
-        else:
-            ## Function passes the final binning solution as look-up table
-            return look_up_table
+    ### Generate requested output, in case specification is correct
+    else:
+        ## Function passes the final binning solution as look-up table
+        return look_up_table
             
     return binning
 
 def woe_binning (df, target_var, pred_var, min_perc_total, min_perc_class, stop_limit, abbrev_fact_levels, event_class):
 #### Warning message and defaults in case parameters are not specified
     if df.isnull().values.any()==True or type(target_var) is str == False or type(pred_var) is str == False:
         warnings.warn("Incorrect specification of data frame and/or variables.")
```

### Comparing `ieseg_credscore-0.23.8/ieseg_credscore.egg-info/PKG-INFO` & `ieseg_credscore-0.23.9/ieseg_credscore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg-credscore
-Version: 0.23.8
+Version: 0.23.9
 Summary: Credit Scoring - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Credit Scoring IESEG
 Description-Content-Type: text/markdown
```

### Comparing `ieseg_credscore-0.23.8/setup.py` & `ieseg_credscore-0.23.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ieseg_credscore',
-    version='0.23.8',
+    version='0.23.9',
     license='MIT',
     author="Philipp Borchert",
     author_email='p.borchert@ieseg.fr',
     packages=find_packages(),
     description = 'Credit Scoring - IESEG School of Management',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

