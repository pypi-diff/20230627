# Comparing `tmp/osint-python-starter-service-2.2.0.tar.gz` & `tmp/osint-python-starter-service-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.2.0.tar", last modified: Fri Jun 23 01:28:42 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.2.1.tar", last modified: Tue Jun 27 14:10:22 2023, max compression
```

## Comparing `osint-python-starter-service-2.2.0.tar` & `osint-python-starter-service-2.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.2.0/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.2.0/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/classes/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-22 23:18:15.000000 osint-python-starter-service-2.2.0/classes/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2841 2023-06-22 23:23:47.000000 osint-python-starter-service-2.2.0/classes/article_raw_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      909 2023-06-22 23:23:46.000000 osint-python-starter-service-2.2.0/classes/metadata_item_ner_en.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1051 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       24 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-06-23 00:55:50.000000 osint-python-starter-service-2.2.0/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.2.0/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.2.0/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6309 2023-06-23 01:20:47.000000 osint-python-starter-service-2.2.0/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5774 2023-06-03 20:59:13.000000 osint-python-starter-service-2.2.0/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3999 2023-06-23 01:22:59.000000 osint-python-starter-service-2.2.0/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1837 2023-06-07 19:08:41.000000 osint-python-starter-service-2.2.0/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.2.0/starter_service/examples/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      602 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1595 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/manual_api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1282 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1220 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1332 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/offset_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1164 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6117 2023-06-23 01:28:24.000000 osint-python-starter-service-2.2.0/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.2.0/starter_service/schemas.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      788 2023-06-23 00:39:02.000000 osint-python-starter-service-2.2.0/starter_service/sub_process.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/starter_service/tests/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.2.0/starter_service/tests/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.2.0/starter_service/tests/employee.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      699 2023-06-03 20:55:03.000000 osint-python-starter-service-2.2.0/starter_service/tests/teet.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2885 2023-06-03 20:45:37.000000 osint-python-starter-service-2.2.0/starter_service/tests/test_avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.2.0/starter_service/tests/tst.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.2.1/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.2.1/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/classes/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-22 23:18:15.000000 osint-python-starter-service-2.2.1/classes/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2841 2023-06-22 23:23:47.000000 osint-python-starter-service-2.2.1/classes/article_raw_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      909 2023-06-22 23:23:46.000000 osint-python-starter-service-2.2.1/classes/metadata_item_ner_en.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1051 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       24 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-06-27 14:09:32.000000 osint-python-starter-service-2.2.1/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.2.1/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.2.1/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6309 2023-06-23 01:20:47.000000 osint-python-starter-service-2.2.1/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5774 2023-06-03 20:59:13.000000 osint-python-starter-service-2.2.1/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4278 2023-06-27 14:08:38.000000 osint-python-starter-service-2.2.1/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1837 2023-06-07 19:08:41.000000 osint-python-starter-service-2.2.1/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.2.1/starter_service/examples/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      602 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1595 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/manual_api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1282 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1220 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1332 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/offset_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1164 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6117 2023-06-23 01:28:24.000000 osint-python-starter-service-2.2.1/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.2.1/starter_service/schemas.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      788 2023-06-23 00:39:02.000000 osint-python-starter-service-2.2.1/starter_service/sub_process.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/starter_service/tests/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.2.1/starter_service/tests/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.2.1/starter_service/tests/employee.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      699 2023-06-03 20:55:03.000000 osint-python-starter-service-2.2.1/starter_service/tests/teet.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2885 2023-06-03 20:45:37.000000 osint-python-starter-service-2.2.1/starter_service/tests/test_avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.2.1/starter_service/tests/tst.py
```

### Comparing `osint-python-starter-service-2.2.0/LICENSE` & `osint-python-starter-service-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/PKG-INFO` & `osint-python-starter-service-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.2.0/README.md` & `osint-python-starter-service-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/classes/article_raw_en.py` & `osint-python-starter-service-2.2.1/classes/article_raw_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/classes/metadata_item_ner_en.py` & `osint-python-starter-service-2.2.1/classes/metadata_item_ner_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/setup.py` & `osint-python-starter-service-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.2.0",
+    version="2.2.1",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.2.0/starter_service/api.py` & `osint-python-starter-service-2.2.1/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/api_server.py` & `osint-python-starter-service-2.2.1/starter_service/api_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/avro_parser.py` & `osint-python-starter-service-2.2.1/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/base_service.py` & `osint-python-starter-service-2.2.1/starter_service/base_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import sys
+import threading
 from abc import ABC, abstractmethod
 from time import sleep
 
 from starter_service.api_server import APIServer
 from starter_service.env import ENV
 from starter_service.kafka_adapter import KafkaAdapter
 from starter_service.schemas import SchemaRegistry
@@ -67,17 +68,22 @@
     def start(self):
         """Start the service"""
         try:
             if self.kafka:
                 self.logger.info("Starting service Kafka...")
                 self.kafka.start()
             self.logger.info("Starting service API...")
-            sleep(3)
             # Wait for kafka to start and register schemas
+            sleep(3)
+
+            # Callback
             self.callback(kafka_error=self.kafka_error, api_error=self.api_error)
+            # Async callback
+            threading.Thread(target=self.async_callback, daemon=True).start()
+
             if self.api:
                 self.api.run()
 
             if self.kafka is None and self.api is None:
                 raise Exception('No services initialized. Shutting down.')
 
         except Exception as e:
@@ -111,7 +117,11 @@
     def api_callback(self, **kwargs):
         """Override this method to callback after service is initialized"""
         pass
 
     def callback(self, **kwargs):
         """Override this method to callback after service is initialized"""
         pass
+
+    def async_callback(self, **kwargs):
+        """Override this method to callback after service is initialized"""
+        pass
```

### Comparing `osint-python-starter-service-2.2.0/starter_service/env.py` & `osint-python-starter-service-2.2.1/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/examples/error.py` & `osint-python-starter-service-2.2.1/starter_service/examples/error.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/examples/manual_api.py` & `osint-python-starter-service-2.2.1/starter_service/examples/manual_api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.2.1/starter_service/examples/manual_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/examples/multi.py` & `osint-python-starter-service-2.2.1/starter_service/examples/multi.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/examples/offset_kafka.py` & `osint-python-starter-service-2.2.1/starter_service/examples/offset_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/examples/single.py` & `osint-python-starter-service-2.2.1/starter_service/examples/single.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.2.1/starter_service/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/schemas.py` & `osint-python-starter-service-2.2.1/starter_service/schemas.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/sub_process.py` & `osint-python-starter-service-2.2.1/starter_service/sub_process.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/tests/employee.py` & `osint-python-starter-service-2.2.1/starter_service/tests/employee.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/tests/teet.py` & `osint-python-starter-service-2.2.1/starter_service/tests/teet.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.0/starter_service/tests/test_avro_parser.py` & `osint-python-starter-service-2.2.1/starter_service/tests/test_avro_parser.py`

 * *Files identical despite different names*

