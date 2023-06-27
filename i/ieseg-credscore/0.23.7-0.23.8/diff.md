# Comparing `tmp/ieseg_credscore-0.23.7.tar.gz` & `tmp/ieseg_credscore-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieseg_credscore-0.23.7.tar", last modified: Tue Jun 27 12:56:17 2023, max compression
+gzip compressed data, was "ieseg_credscore-0.23.8.tar", last modified: Tue Jun 27 13:01:27 2023, max compression
```

## Comparing `ieseg_credscore-0.23.7.tar` & `ieseg_credscore-0.23.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:56:17.059755 ieseg_credscore-0.23.7/
--rw-rw-rw-   0        0        0     1092 2023-06-26 15:40:57.000000 ieseg_credscore-0.23.7/LICENSE.rst
--rw-rw-rw-   0        0        0     2942 2023-06-27 12:56:17.060750 ieseg_credscore-0.23.7/PKG-INFO
--rw-rw-rw-   0        0        0     2606 2023-06-26 16:44:47.000000 ieseg_credscore-0.23.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 12:56:16.982015 ieseg_credscore-0.23.7/ieseg_credscore/
--rw-rw-rw-   0        0        0     4597 2022-02-04 14:15:05.000000 ieseg_credscore-0.23.7/ieseg_credscore/OBG.py
--rw-rw-rw-   0        0        0    46428 2023-06-27 12:54:59.000000 ieseg_credscore-0.23.7/ieseg_credscore/WOE.py
--rw-rw-rw-   0        0        0       58 2023-06-27 12:18:23.000000 ieseg_credscore-0.23.7/ieseg_credscore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:56:17.050783 ieseg_credscore-0.23.7/ieseg_credscore.egg-info/
--rw-rw-rw-   0        0        0     2942 2023-06-27 12:56:16.000000 ieseg_credscore-0.23.7/ieseg_credscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-06-27 12:56:16.000000 ieseg_credscore-0.23.7/ieseg_credscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:56:16.000000 ieseg_credscore-0.23.7/ieseg_credscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 12:56:16.000000 ieseg_credscore-0.23.7/ieseg_credscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 12:56:16.000000 ieseg_credscore-0.23.7/ieseg_credscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-27 12:56:17.070716 ieseg_credscore-0.23.7/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-06-27 12:56:13.000000 ieseg_credscore-0.23.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:01:27.602667 ieseg_credscore-0.23.8/
+-rw-rw-rw-   0        0        0     1092 2023-06-26 15:40:57.000000 ieseg_credscore-0.23.8/LICENSE.rst
+-rw-rw-rw-   0        0        0     2942 2023-06-27 13:01:27.602667 ieseg_credscore-0.23.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-26 16:44:47.000000 ieseg_credscore-0.23.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 13:01:27.520942 ieseg_credscore-0.23.8/ieseg_credscore/
+-rw-rw-rw-   0        0        0     4597 2022-02-04 14:15:05.000000 ieseg_credscore-0.23.8/ieseg_credscore/OBG.py
+-rw-rw-rw-   0        0        0    46382 2023-06-27 13:00:33.000000 ieseg_credscore-0.23.8/ieseg_credscore/WOE.py
+-rw-rw-rw-   0        0        0       58 2023-06-27 12:18:23.000000 ieseg_credscore-0.23.8/ieseg_credscore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:01:27.589710 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/
+-rw-rw-rw-   0        0        0     2942 2023-06-27 13:01:26.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-27 13:01:27.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:01:26.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 13:01:26.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 13:01:26.000000 ieseg_credscore-0.23.8/ieseg_credscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-27 13:01:27.613631 ieseg_credscore-0.23.8/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-06-27 13:01:17.000000 ieseg_credscore-0.23.8/setup.py
```

### Comparing `ieseg_credscore-0.23.7/LICENSE.rst` & `ieseg_credscore-0.23.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.7/PKG-INFO` & `ieseg_credscore-0.23.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg_credscore
-Version: 0.23.7
+Version: 0.23.8
 Summary: Credit Scoring - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Credit Scoring IESEG
 Description-Content-Type: text/markdown
```

### Comparing `ieseg_credscore-0.23.7/README.md` & `ieseg_credscore-0.23.8/README.md`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.7/ieseg_credscore/OBG.py` & `ieseg_credscore-0.23.8/ieseg_credscore/OBG.py`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.7/ieseg_credscore/WOE.py` & `ieseg_credscore-0.23.8/ieseg_credscore/WOE.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,16 +181,14 @@
     dfrm = df[[target_var, pred_var]]# used for iterative merging of bins
     dfrm.columns = ['target_var','predictor_var']
 
     #### Check if numerical variable or factor was provided as predictor and apply appropriate binning technique
 
     ### Binning in case a numerical variable was selected
     if len(dfrm.iloc[:,0].drop_duplicates()) == 2 and (dfrm.iloc[:,1].dtypes.kind in 'bifc') == True:
-        
-
         ## Derive number of initial bins from min.perc.total parameter
         max_bins = math.trunc(1/min_perc_total)
         
         ## Derive cutpoints for bins (with similar frequency)
         cutpoints = dfrm.predictor_var.quantile(np.arange(0,max_bins+1)/max_bins).reset_index(drop=True)
         innercutpoints = [-np.inf] + list(cutpoints[1:len(cutpoints)-1]) + [np.inf]  # add -Inf, +Inf to cutpoints
         cutpoints = list(dict.fromkeys(innercutpoints))
@@ -403,20 +401,15 @@
         if bad == 0 and good == 1:
             look_up_table = look_up_table.rename(index=str, columns={0: "bad", 1: "good"})
         elif good == 0 and bad==1:    
             look_up_table = look_up_table.rename(index=str, columns={0: "good", 1: "bad"})  
         
         binning = pd.concat([(woe_dfrm_final["woe"]).reset_index(drop=False), look_up_table["cutpoints_final"].reset_index(drop=True), look_up_table["upper_cutpoints_final_dfrm"].reset_index(drop=True), look_up_table["iv_total_final"].reset_index(drop=True), look_up_table["good"].reset_index(drop=True), look_up_table["bad"].reset_index(drop=True), look_up_table["col_perc_a"].reset_index(drop=True), look_up_table["col_perc_b"].reset_index(drop=True), woe_dfrm_final["iv_bins"].reset_index(drop=True)], axis=1, sort=False).set_index(["predictor_var_binned"])
     
-    
-    
-    
-    
-    
-    
+
     ### Binning in case a factor was selected        
     if len(dfrm.iloc[:,0].drop_duplicates()) == 2 and (dfrm.iloc[:,1].dtype == 'object')==True:
         dfrm.iloc[:,1] = dfrm.iloc[:,1].astype('category')            
         ## Copy predictor variable to prepare binning/recoding
         dfrm["predictor_var_binned"] = dfrm["predictor_var"]
         
         ## Handling of NAs
```

### Comparing `ieseg_credscore-0.23.7/ieseg_credscore.egg-info/PKG-INFO` & `ieseg_credscore-0.23.8/ieseg_credscore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg-credscore
-Version: 0.23.7
+Version: 0.23.8
 Summary: Credit Scoring - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Credit Scoring IESEG
 Description-Content-Type: text/markdown
```

### Comparing `ieseg_credscore-0.23.7/setup.py` & `ieseg_credscore-0.23.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ieseg_credscore',
-    version='0.23.7',
+    version='0.23.8',
     license='MIT',
     author="Philipp Borchert",
     author_email='p.borchert@ieseg.fr',
     packages=find_packages(),
     description = 'Credit Scoring - IESEG School of Management',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

