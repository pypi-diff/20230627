# Comparing `tmp/utilities_hki-0.1.5.tar.gz` & `tmp/utilities_hki-0.1.6.tar.gz`

## Comparing `utilities_hki-0.1.5.tar` & `utilities_hki-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/requirements.txt
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/__init__.py
--rwxr-xr-x   0        0        0    71505 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/analy_utils.py
--rwxr-xr-x   0        0        0     2729 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/db_utils.py
--rwxr-xr-x   0        0        0     2944 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/email_utils.py
--rwxr-xr-x   0        0        0     5268 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/fb_utils.py
--rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/data/gmm_2022-10-23.joblib
--rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/data/gmm_2023-04-02.joblib
--rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
--rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/.gitignore
--rwxr-xr-x   0        0        0    34522 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/LICENSE.txt
--rwxr-xr-x   0        0        0     4424 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/README.md
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/requirements.txt
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/__init__.py
+-rwxr-xr-x   0        0        0    71816 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/analy_utils.py
+-rwxr-xr-x   0        0        0     2729 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/db_utils.py
+-rwxr-xr-x   0        0        0     2944 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/email_utils.py
+-rwxr-xr-x   0        0        0     5268 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/fb_utils.py
+-rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/data/gmm_2022-10-23.joblib
+-rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/data/gmm_2023-04-02.joblib
+-rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
+-rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/.gitignore
+-rwxr-xr-x   0        0        0    34522 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/LICENSE.txt
+-rwxr-xr-x   0        0        0     4424 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/README.md
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/PKG-INFO
```

### Comparing `utilities_hki-0.1.5/src/utilities_hki/analy_utils.py` & `utilities_hki-0.1.6/src/utilities_hki/analy_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1301,26 +1301,30 @@
     engage_flow = df.engagement_flow.str.split(',').explode()
     engage_flow = engage_flow.map(get_engage_map()).astype(str)
     engage_flow = pd.DataFrame(engage_flow.groupby('visitor_id').apply(lambda x: ','.join(x)))
     
     return engage_flow
 
 
-def build_processed_visitor_data(visits=None, visitors=None):
+def build_processed_visitor_data(visits=None, visitors=None, drop_sessions=False, drop_none=False):
     """
     Build processed visitor-level data set.
 
     Processed visitor data = summary data and numerical sequences representing customer journeys.
     
     Parameters
     ----------
     visits : pd.DataFrame
         Raw visit-level data. If none passed in, must pass in raw visitor-level data instead.
     visitors : pd.DataFrame
         Raw visitor-level data. If none passed in, will build on the fly.
+    drop_sessions : bool
+        Whether to drop 'session-start' and 'session-end' from action flows.
+    drop_none : bool
+        Whether to drop 'None' from action flows.
 
     Returns
     -------
     pd.DataFrame
         Processed visitor-level data.
     """
 
@@ -1354,16 +1358,17 @@
             sorted(df.referrer_type.explode().unique()), key=lambda s: s.split('_')[-1]))},
         ]
     cols = ['day', 'visit_trade_hours', 'device_category', 'referrer_type']
     for i, col in enumerate(cols):
         df[col] = df[col].apply(lambda x: ','.join(list(map(maps[i].get, x))))
         
     # map action and engagement flows to numerical sequences
-    action_flow = map_action_flow(df, drop_none=True)
-    page_flow = map_action_flow(df, colstr='page', action_types=['pageview'], drop_none=True)
+    action_flow = map_action_flow(df, drop_sessions=drop_sessions, drop_none=drop_none)
+    page_flow = map_action_flow(df, colstr='page', action_types=['pageview'],
+                                drop_sessions=drop_sessions, drop_none=drop_none)
     engage_flow = map_engage_flow(df)
 
     # drop original columns and replace with transformations
     df = df.drop(columns=[col for col in df.columns if col in
                           list(action_flow.columns) +
                           list(page_flow.columns) +
                           list(engage_flow.columns)])
```

### Comparing `utilities_hki-0.1.5/src/utilities_hki/db_utils.py` & `utilities_hki-0.1.6/src/utilities_hki/db_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/src/utilities_hki/email_utils.py` & `utilities_hki-0.1.6/src/utilities_hki/email_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/src/utilities_hki/fb_utils.py` & `utilities_hki-0.1.6/src/utilities_hki/fb_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/src/utilities_hki/data/gmm_2022-10-23.joblib` & `utilities_hki-0.1.6/src/utilities_hki/data/gmm_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/src/utilities_hki/data/gmm_2023-04-02.joblib` & `utilities_hki-0.1.6/src/utilities_hki/data/gmm_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib` & `utilities_hki-0.1.6/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib` & `utilities_hki-0.1.6/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/LICENSE.txt` & `utilities_hki-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/README.md` & `utilities_hki-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.5/pyproject.toml` & `utilities_hki-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "utilities_hki"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Francisco Pena" },
   { name="Colleen Treado" },
 ]
 description = "Global utilities for Humankind data science"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `utilities_hki-0.1.5/PKG-INFO` & `utilities_hki-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilities_hki
-Version: 0.1.5
+Version: 0.1.6
 Summary: Global utilities for Humankind data science
 Project-URL: Homepage, https://github.com/humankind-datascience/utilities-hki
 Author: Francisco Pena, Colleen Treado
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

