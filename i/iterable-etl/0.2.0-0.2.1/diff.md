# Comparing `tmp/iterable_etl-0.2.0.tar.gz` & `tmp/iterable_etl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable_etl-0.2.0.tar", last modified: Thu Jun 22 19:09:55 2023, max compression
+gzip compressed data, was "iterable_etl-0.2.1.tar", last modified: Tue Jun 27 21:39:02 2023, max compression
```

## Comparing `iterable_etl-0.2.0.tar` & `iterable_etl-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      307 2023-06-09 16:43:58.000000 iterable_etl-0.2.0/MANIFEST.in
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1519 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/README_PUBLIC.md
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/iterable_etl/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       22 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/iterable_etl/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      155 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/__main__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1006 2023-06-21 21:57:04.000000 iterable_etl-0.2.0/iterable_etl/iterable_etl.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/iterable_etl/libs/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.2.0/iterable_etl/libs/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      667 2023-06-21 21:57:04.000000 iterable_etl-0.2.0/iterable_etl/libs/cnst.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1900 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/iterable_etl/libs/dbg.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1047 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/iterable_etl/libs/network.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1403 2023-06-21 21:57:04.000000 iterable_etl-0.2.0/iterable_etl/libs/spark.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      928 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/libs/transform.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/iterable_etl/tables/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.2.0/iterable_etl/tables/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      843 2023-06-21 17:33:07.000000 iterable_etl-0.2.0/iterable_etl/tables/campaign_history.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1370 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/tables/campaign_list_history.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1723 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/tables/campaign_metrics.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      769 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/tables/list.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2279 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/iterable_etl/tables/list_user_history.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/iterable_etl.egg-info/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      717 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       75 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/requires.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       13 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/top_level.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      426 2023-06-22 19:09:55.189529 iterable_etl-0.2.0/setup.cfg
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1050 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/setup.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/tests/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.2.0/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:39:02.136939 iterable_etl-0.2.1/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.2.1/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2027 2023-06-27 21:39:02.136939 iterable_etl-0.2.1/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1519 2023-06-14 17:30:32.000000 iterable_etl-0.2.1/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:39:02.132939 iterable_etl-0.2.1/iterable_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-27 21:37:44.000000 iterable_etl-0.2.1/iterable_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      155 2023-06-14 17:33:42.000000 iterable_etl-0.2.1/iterable_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1233 2023-06-27 19:27:08.000000 iterable_etl-0.2.1/iterable_etl/iterable_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:39:02.136939 iterable_etl-0.2.1/iterable_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.2.1/iterable_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      729 2023-06-27 18:55:02.000000 iterable_etl-0.2.1/iterable_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1900 2023-06-22 19:06:27.000000 iterable_etl-0.2.1/iterable_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1213 2023-06-27 18:55:02.000000 iterable_etl-0.2.1/iterable_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1403 2023-06-21 19:49:44.000000 iterable_etl-0.2.1/iterable_etl/libs/spark.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      928 2023-06-14 17:33:42.000000 iterable_etl-0.2.1/iterable_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:39:02.136939 iterable_etl-0.2.1/iterable_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.2.1/iterable_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      843 2023-06-14 17:39:05.000000 iterable_etl-0.2.1/iterable_etl/tables/campaign_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1370 2023-06-14 17:39:18.000000 iterable_etl-0.2.1/iterable_etl/tables/campaign_list_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1723 2023-06-14 17:39:50.000000 iterable_etl-0.2.1/iterable_etl/tables/campaign_metrics.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      769 2023-06-14 17:40:00.000000 iterable_etl-0.2.1/iterable_etl/tables/list.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2279 2023-06-27 18:55:02.000000 iterable_etl-0.2.1/iterable_etl/tables/list_user_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1544 2023-06-27 21:38:23.000000 iterable_etl-0.2.1/iterable_etl/tables/user_history.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:39:02.132939 iterable_etl-0.2.1/iterable_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2027 2023-06-27 21:39:02.000000 iterable_etl-0.2.1/iterable_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      753 2023-06-27 21:39:02.000000 iterable_etl-0.2.1/iterable_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-27 21:39:02.000000 iterable_etl-0.2.1/iterable_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-27 21:39:02.000000 iterable_etl-0.2.1/iterable_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-27 21:39:02.000000 iterable_etl-0.2.1/iterable_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      426 2023-06-27 21:39:02.136939 iterable_etl-0.2.1/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1050 2023-06-27 21:37:44.000000 iterable_etl-0.2.1/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:39:02.136939 iterable_etl-0.2.1/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.2.1/tests/__init__.py
```

### Comparing `iterable_etl-0.2.0/PKG-INFO` & `iterable_etl-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable_etl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.2.0/README_PUBLIC.md` & `iterable_etl-0.2.1/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl/iterable_etl.py` & `iterable_etl-0.2.1/iterable_etl/iterable_etl.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import click
 
 from iterable_etl.tables.campaign_history import campaign_history_df
 from iterable_etl.tables.campaign_list_history import campaign_list_history_df
 from iterable_etl.tables.campaign_metrics import campaign_metrics_df
 from iterable_etl.tables.list import list_df
 from iterable_etl.tables.list_user_history import list_user_history_df
+from iterable_etl.tables.user_history import user_history_df
 
 
 @click.command()
 @click.option("--table")
 def main(table: str) -> None:
     """program"""
     if table == "campaign_history":
@@ -18,14 +19,18 @@
         campaign_metrics_df()
     elif table == "list":
         list_df()
     elif table == "campaign_list_history":
         campaign_list_history_df()
     elif table == "list_user_history":
         list_user_history_df()
+    elif table == "user_history":
+        start_date = "2023-06-25"
+        end_date = "2023-06-27"
+        user_history_df(start_date=start_date, end_date=end_date)
     elif table == "ALL":
         campaign_history_df()
         campaign_metrics_df()
         list_df()
         campaign_list_history_df()
         list_user_history_df()
     else:
```

### Comparing `iterable_etl-0.2.0/iterable_etl/libs/cnst.py` & `iterable_etl-0.2.1/iterable_etl/libs/cnst.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, Dict
 
 urls = {
     "lists": "https://api.iterable.com/api/lists",
     "campaigns": "https://api.iterable.com/api/campaigns",
     "metrics": "https://api.iterable.com/api/campaigns/metrics",
     "lists_get_users": "https://api.iterable.com/api/lists/getUsers?listId=",
+    "export": "https://api.iterable.com/api/export/data.csv",
 }
 
 
 def get_headers() -> Dict[str, Any]:
     """header config for Iterable API"""
     headers = {
         "Api-Key": os.environ.get("ITERABLE_KEY"),
```

### Comparing `iterable_etl-0.2.0/iterable_etl/libs/dbg.py` & `iterable_etl-0.2.1/iterable_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl/libs/network.py` & `iterable_etl-0.2.1/iterable_etl/libs/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,7 +31,13 @@
     data = get_data(api_url, headers)
     return data.json()
 
 
 def get_data_text(api_url: str, headers: Dict[str, str]) -> str:
     data = get_data(api_url, headers)
     return data.text
+
+
+def get_data_csv(api_url: str, headers: Dict[str, str]) -> str:
+    data = get_data(api_url, headers)
+    content = data.content.decode("utf-8")
+    return content
```

### Comparing `iterable_etl-0.2.0/iterable_etl/libs/spark.py` & `iterable_etl-0.2.1/iterable_etl/libs/spark.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl/libs/transform.py` & `iterable_etl-0.2.1/iterable_etl/libs/transform.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl/tables/campaign_history.py` & `iterable_etl-0.2.1/iterable_etl/tables/campaign_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl/tables/campaign_list_history.py` & `iterable_etl-0.2.1/iterable_etl/tables/campaign_list_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl/tables/campaign_metrics.py` & `iterable_etl-0.2.1/iterable_etl/tables/campaign_metrics.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl/tables/list.py` & `iterable_etl-0.2.1/iterable_etl/tables/list.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl/tables/list_user_history.py` & `iterable_etl-0.2.1/iterable_etl/tables/list_user_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.0/iterable_etl.egg-info/PKG-INFO` & `iterable_etl-0.2.1/iterable_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable-etl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.2.0/iterable_etl.egg-info/SOURCES.txt` & `iterable_etl-0.2.1/iterable_etl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 iterable_etl/libs/transform.py
 iterable_etl/tables/__init__.py
 iterable_etl/tables/campaign_history.py
 iterable_etl/tables/campaign_list_history.py
 iterable_etl/tables/campaign_metrics.py
 iterable_etl/tables/list.py
 iterable_etl/tables/list_user_history.py
+iterable_etl/tables/user_history.py
 tests/__init__.py
```

### Comparing `iterable_etl-0.2.0/setup.py` & `iterable_etl-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="iterable_etl",
-    version="0.2.0",
+    version="0.2.1",
     description="Replicate iterable data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

