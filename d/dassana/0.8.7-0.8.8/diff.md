# Comparing `tmp/dassana-0.8.7.tar.gz` & `tmp/dassana-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dassana-0.8.7.tar", last modified: Tue Jun 20 06:20:02 2023, max compression
+gzip compressed data, was "dassana-0.8.8.tar", last modified: Tue Jun 27 04:20:34 2023, max compression
```

## Comparing `dassana-0.8.7.tar` & `dassana-0.8.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:20:02.314661 dassana-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 06:20:02.314661 dassana-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 06:19:53.000000 dassana-0.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:20:02.314661 dassana-0.8.7/dassana/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/dassana_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/data_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:20:02.314661 dassana-0.8.7/dassana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 06:20:02.314661 dassana-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-20 06:19:53.000000 dassana-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:20:34.030220 dassana-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 04:20:34.030220 dassana-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 04:20:21.000000 dassana-0.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:20:34.030220 dassana-0.8.8/dassana/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/dassana_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/data_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-27 04:20:21.000000 dassana-0.8.8/dassana/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:20:34.030220 dassana-0.8.8/dassana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-27 04:20:34.000000 dassana-0.8.8/dassana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 04:20:33.000000 dassana-0.8.8/dassana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 04:20:34.030220 dassana-0.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-27 04:20:21.000000 dassana-0.8.8/setup.py
```

### Comparing `dassana-0.8.7/dassana/common.py` & `dassana-0.8.8/dassana/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,22 +87,27 @@
 def get_ingestion_details(tenant_id, source, record_type, config_id, metadata, priority, is_snapshot):
     access_token = get_access_token()
 
     headers = {
         "x-dassana-tenant-id": tenant_id,
         "Authorization": f"Bearer {access_token}", 
     }
-    res = requests.post(ingestion_service_url +"/job/", headers=headers, json={
+    json_body = {
         "source": str(source),
         "recordType": str(record_type),
         "configId": str(config_id),
         "is_snapshot": is_snapshot,
-        # "priority": priority,
+        "priority": priority,
         "metadata": metadata
-        })
+        }
+    
+    if json_body["priority"] is None:
+        del json_body["priority"]
+    
+    res = requests.post(ingestion_service_url +"/job/", headers=headers, json=json_body)
     if(res.status_code == 200):
         return res.json()
 
     return 0
 
 def report_status(status, additionalContext, timeTakenInSec, recordsIngested, ingestion_config_id):
     reportingURL = f"https://{app_url}/app/v1/{app_id}/status"
@@ -127,15 +132,15 @@
         resp = requests.Session().post(reportingURL, headers=headers, json=payload, verify=False)
         logging.info(f"Report request status: {resp.status_code}")
     else:
         resp = requests.Session().post(reportingURL, headers=headers, json=payload)
         logging.info(f"Report request status: {resp.status_code}")
 
 class DassanaWriter:
-    def __init__(self, tenant_id, source, record_type, config_id, metadata = {}, priority = 999, is_snapshot = False):
+    def __init__(self, tenant_id, source, record_type, config_id, metadata = {}, priority = None, is_snapshot = False):
         print("Initialized common utility")
 
         self.source = source
         self.record_type = record_type
         self.config_id = config_id
         self.metadata = metadata
         self.priority = priority
```

### Comparing `dassana-0.8.7/dassana/dassana_env.py` & `dassana-0.8.8/dassana/dassana_env.py`

 * *Files identical despite different names*

### Comparing `dassana-0.8.7/dassana/data_pipes.py` & `dassana-0.8.8/dassana/data_pipes.py`

 * *Files identical despite different names*

### Comparing `dassana-0.8.7/dassana/rest.py` & `dassana-0.8.8/dassana/rest.py`

 * *Files identical despite different names*

