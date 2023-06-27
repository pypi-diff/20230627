# Comparing `tmp/fiftyone_pipeline_engines_fiftyone-4.4.5.tar.gz` & `tmp/fiftyone_pipeline_engines_fiftyone-4.4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiftyone_pipeline_engines_fiftyone-4.4.5.tar", last modified: Fri Feb 17 12:00:44 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_engines_fiftyone-4.4.6.0.tar", last modified: Tue Jun 27 13:33:38 2023, max compression
```

## Comparing `fiftyone_pipeline_engines_fiftyone-4.4.5.tar` & `fiftyone_pipeline_engines_fiftyone-4.4.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/
--rw-r--r--   0 vsts      (1001) docker     (116)     1820 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)    13974 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone/share_usage.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4367 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3005 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     1820 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)      520 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       63 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       35 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     2675 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:38.052445 fiftyone_pipeline_engines_fiftyone-4.4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-27 13:33:38.052445 fiftyone_pipeline_engines_fiftyone-4.4.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:38.052445 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone/share_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:38.052445 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-27 13:33:38.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-27 13:33:38.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:33:38.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 13:33:38.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 13:33:38.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:33:38.052445 fiftyone_pipeline_engines_fiftyone-4.4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines_fiftyone-4.4.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.5/PKG-INFO` & `fiftyone_pipeline_engines_fiftyone-4.4.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_engines_fiftyone
-Version: 4.4.5
+Version: 4.4.6.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
-Description: # Pipeline Engines Fiftyone
-        
-        ![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Engines**
-        
-        [Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
-        
-        ## Introduction
-        
-        The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
-        
-        ## This package fiftyone_pipeline_engines_fiftyone
-        
-        It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
-        
-        ## Requirements 
-        
-        * Python 3.5+
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+
+# Pipeline Engines Fiftyone
+
+![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Engines**
+
+[Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
+
+## Introduction
+
+The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
+
+## This package fiftyone_pipeline_engines_fiftyone
+
+It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
+
+## Requirements 
+
+* Python 3.5+
+
+
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone/share_usage.py` & `fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone/share_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,32 +31,36 @@
 import json
 import requests
 import gzip
 import sys
 import platform
 import datetime
 import pkg_resources
+from concurrent.futures import ThreadPoolExecutor
 
 # The maximum length of a piece of evidence's value which can be
 # added to the usage data being sent.
 SHARE_USAGE_MAX_EVIDENCE_LENGTH = 512
 
 SHARE_USAGE_VERSION = '1.1'
 
+# The default number of seconds to wait for the server connection before failing the request when sending usage data
+REQUEST_TIMEOUT = 60
 
 class ShareUsage(Engine):
     def __init__(
         self,
         interval = 1200,
         requested_package_size = 10,
         cookie = None,
         query_whitelist = [],
         header_blacklist = [],
         share_percentage = 1,
-        endpoint = "https://devices-v4.51degrees.com/new.ashx"):
+        endpoint = "https://devices-v4.51degrees.com/new.ashx",
+        request_timeout=REQUEST_TIMEOUT):
         """!
         Constructor for ShareUsage element
         
         @type interval: int
         @param interval: If exactly the same evidence values are seen 
         multiple times within this time limit (in seconds) then they 
         will only be shared once.
@@ -95,25 +99,35 @@
         self.datakey = "shareusage"
 
         self.interval = interval
         self.requested_package_size = requested_package_size
         self.cookie = cookie
         self.share_percentage = share_percentage
         self.endpoint = endpoint
+        self.request_timeout = request_timeout
 
         # Add the share usage tracker which detects when
         # to send up sharing data
 
         self.tracker = ShareUsageTracker(interval = interval)
 
         # Initialise share data list 
         self.share_data = []
 
         self.constant_xml = None
-    
+
+        # Reusable thread pool for sending usage in background
+        # According to the doc on ThreadPoolExecutor - all threads will be joined before the interpreter can exit
+        # this ensures that all the data will be sent correctly before the actual exit happens
+
+        self.thread_pool = ThreadPoolExecutor(thread_name_prefix='ShareUsage')
+
+    def __del__(self):
+        self.thread_pool.shutdown(wait=True)
+
     def get_constant_xml(self):
         if self.constant_xml is None:
             coreVersion = pkg_resources.get_distribution("fiftyone_pipeline_core").version
             osVersion = f"{ReplacedString(platform.system()).result} {ReplacedString(platform.release()).result}"
             pyVersion = ReplacedString(platform.python_version()).result
 
             xml = ""
@@ -177,25 +191,29 @@
         """
 
         share_data = self.share_data
         self.share_data = []
 
         data = f'<Devices version="{SHARE_USAGE_VERSION}">{"".join(share_data)}</Devices>'
 
-        thread = threading.Thread(
-            target=self.send_thread,
-            args=[self.endpoint, data],
-            daemon=True,
-            name="ShareUsage POST")
-        thread.start()
+        self.thread_pool.submit(self.send_thread, self.endpoint, data)
 
     def send_thread(self, endpoint, data):
         data = gzip.compress(bytearray(data, encoding='utf8'))
 
-        requests.post(endpoint, headers={"Content-Encoding": "gzip", "Content-Type": "text/xml"}, data=data)
+        # setting a reasonable time out and catching any exceptions
+        try:
+            requests.post(endpoint, headers={"Content-Encoding": "gzip", "Content-Type": "text/xml"}, data=data,
+                          timeout=self.request_timeout)
+        except Exception as e:
+            print(e)
+            self._log(
+                "error",
+                f"ShareUsage failed sending {len(data)} bytes of data: {e}"
+            )
 
 
     def add_to_share_usage(self, data):
         """!
         Internal method which adds to the share usage bundle (generating XML)
         @type key: dict
         @param key: data value store of current evidence in FlowData
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py` & `fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py` & `fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO` & `fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-engines-fiftyone
-Version: 4.4.5
+Version: 4.4.6.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
-Description: # Pipeline Engines Fiftyone
-        
-        ![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Engines**
-        
-        [Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
-        
-        ## Introduction
-        
-        The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
-        
-        ## This package fiftyone_pipeline_engines_fiftyone
-        
-        It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
-        
-        ## Requirements 
-        
-        * Python 3.5+
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+
+# Pipeline Engines Fiftyone
+
+![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Engines**
+
+[Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
+
+## Introduction
+
+The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
+
+## This package fiftyone_pipeline_engines_fiftyone
+
+It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
+
+## Requirements 
+
+* Python 3.5+
+
+
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.5/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt` & `fiftyone_pipeline_engines_fiftyone-4.4.6.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.5/setup.py` & `fiftyone_pipeline_engines_fiftyone-4.4.6.0/setup.py`

 * *Files identical despite different names*

