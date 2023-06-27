# Comparing `tmp/utilities_hki-0.1.4.tar.gz` & `tmp/utilities_hki-0.1.5.tar.gz`

## Comparing `utilities_hki-0.1.4.tar` & `utilities_hki-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/requirements.txt
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/__init__.py
--rwxr-xr-x   0        0        0    71506 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/analy_utils.py
--rwxr-xr-x   0        0        0     2729 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/db_utils.py
--rwxr-xr-x   0        0        0     2944 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/email_utils.py
--rwxr-xr-x   0        0        0     5268 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/fb_utils.py
--rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/data/gmm_2022-10-23.joblib
--rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/data/gmm_2023-04-02.joblib
--rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
--rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/.gitignore
--rwxr-xr-x   0        0        0    34522 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/LICENSE.txt
--rwxr-xr-x   0        0        0     4424 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/README.md
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 utilities_hki-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/requirements.txt
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/__init__.py
+-rwxr-xr-x   0        0        0    71505 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/analy_utils.py
+-rwxr-xr-x   0        0        0     2729 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/db_utils.py
+-rwxr-xr-x   0        0        0     2944 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/email_utils.py
+-rwxr-xr-x   0        0        0     5268 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/fb_utils.py
+-rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/data/gmm_2022-10-23.joblib
+-rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/data/gmm_2023-04-02.joblib
+-rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
+-rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/.gitignore
+-rwxr-xr-x   0        0        0    34522 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/LICENSE.txt
+-rwxr-xr-x   0        0        0     4424 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/README.md
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 utilities_hki-0.1.5/PKG-INFO
```

### Comparing `utilities_hki-0.1.4/src/utilities_hki/analy_utils.py` & `utilities_hki-0.1.5/src/utilities_hki/analy_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1331,15 +1331,15 @@
 
     df = visitors.copy()
 
     # get summary data
     df.actions = df.action_category_flow.apply(
         lambda x: len([i for i in x.split(',') if not i.startswith('session-') and i != 'None']))
     for action in ['pageview', 'download', 'outlink_click', 'buyetf_click',
-                   'brokerlink_click', 'video_action', 'form_actions']:
+                   'brokerlink_click', 'video_action', 'form_action']:
         df[action + 's'] = df.action_category_flow.apply(
             lambda x: len([i for i in x.split(',') if i.endswith('_' + action)]))
     for duration in ['visit_duration', 'action_duration',
                      'page_duration', 'page_action_duration']:
         df[duration] = df[duration].apply(lambda x: sum(x))
 
     df.timestamp = df.timestamp.explode().astype(str).groupby('visitor_id').apply(
```

### Comparing `utilities_hki-0.1.4/src/utilities_hki/db_utils.py` & `utilities_hki-0.1.5/src/utilities_hki/db_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/src/utilities_hki/email_utils.py` & `utilities_hki-0.1.5/src/utilities_hki/email_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/src/utilities_hki/fb_utils.py` & `utilities_hki-0.1.5/src/utilities_hki/fb_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/src/utilities_hki/data/gmm_2022-10-23.joblib` & `utilities_hki-0.1.5/src/utilities_hki/data/gmm_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/src/utilities_hki/data/gmm_2023-04-02.joblib` & `utilities_hki-0.1.5/src/utilities_hki/data/gmm_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib` & `utilities_hki-0.1.5/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib` & `utilities_hki-0.1.5/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/LICENSE.txt` & `utilities_hki-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/README.md` & `utilities_hki-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.4/pyproject.toml` & `utilities_hki-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "utilities_hki"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Francisco Pena" },
   { name="Colleen Treado" },
 ]
 description = "Global utilities for Humankind data science"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `utilities_hki-0.1.4/PKG-INFO` & `utilities_hki-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilities_hki
-Version: 0.1.4
+Version: 0.1.5
 Summary: Global utilities for Humankind data science
 Project-URL: Homepage, https://github.com/humankind-datascience/utilities-hki
 Author: Francisco Pena, Colleen Treado
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

