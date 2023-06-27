# Comparing `tmp/hubmap-sdk-1.0.3.tar.gz` & `tmp/hubmap-sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubmap-sdk-1.0.3.tar", last modified: Wed Apr 19 14:53:02 2023, max compression
+gzip compressed data, was "hubmap-sdk-1.0.4.tar", last modified: Tue Jun 27 19:44:27 2023, max compression
```

## Comparing `hubmap-sdk-1.0.3.tar` & `hubmap-sdk-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:53:02.202153 hubmap-sdk-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3298 2023-04-19 14:53:02.202153 hubmap-sdk-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2862 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:53:02.201152 hubmap-sdk-1.0.3/hubmap_sdk/
--rw-r--r--   0 root         (0) root         (0)      345 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/client.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/collection.py
--rw-r--r--   0 root         (0) root         (0)      206 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/dataset.py
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/donor.py
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/entity.py
--rw-r--r--   0 root         (0) root         (0)    19599 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/entitysdk.py
--rw-r--r--   0 root         (0) root         (0)      205 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/sample.py
--rw-r--r--   0 root         (0) root         (0)     4229 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/sdk_helper.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/searchsdk.py
--rw-r--r--   0 root         (0) root         (0)      205 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:53:02.202153 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3298 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      442 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 14:53:02.202153 hubmap-sdk-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      880 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/setup.py
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-06-27 19:44:27.288907 hubmap-sdk-1.0.4/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1074 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/LICENSE
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3298 2023-06-27 19:44:27.288907 hubmap-sdk-1.0.4/PKG-INFO
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2862 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/README.md
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-06-27 19:44:27.286907 hubmap-sdk-1.0.4/hubmap_sdk/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      392 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/__init__.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/client.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      208 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/collection.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      206 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/dataset.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      204 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/donor.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      180 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/entity.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    19599 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/entitysdk.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      210 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/publication.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      205 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/sample.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     4340 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/sdk_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2548 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/searchsdk.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      205 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/hubmap_sdk/upload.py
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-06-27 19:44:27.287907 hubmap-sdk-1.0.4/hubmap_sdk.egg-info/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3298 2023-06-27 19:44:27.000000 hubmap-sdk-1.0.4/hubmap_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      468 2023-06-27 19:44:27.000000 hubmap-sdk-1.0.4/hubmap_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)        1 2023-06-27 19:44:27.000000 hubmap-sdk-1.0.4/hubmap_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)       78 2023-06-27 19:44:27.000000 hubmap-sdk-1.0.4/hubmap_sdk.egg-info/requires.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)       11 2023-06-27 19:44:27.000000 hubmap-sdk-1.0.4/hubmap_sdk.egg-info/top_level.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)       38 2023-06-27 19:44:27.288907 hubmap-sdk-1.0.4/setup.cfg
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      880 2023-06-27 19:42:25.000000 hubmap-sdk-1.0.4/setup.py
```

### Comparing `hubmap-sdk-1.0.3/LICENSE` & `hubmap-sdk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hubmap-sdk-1.0.3/PKG-INFO` & `hubmap-sdk-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Client Libary to use HuBMAP web services
 Author: Hubmap
 Author-email: api-developers@hubmapconsortium.org
 Keywords: HuBMAP Sdk,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hubmap-sdk Version: 1.0.3 Summary: Python Client
+Metadata-Version: 2.1 Name: hubmap-sdk Version: 1.0.4 Summary: Python Client
 Libary to use HuBMAP web services Author: Hubmap Author-email: api-
 developers@hubmapconsortium.org Keywords: HuBMAP Sdk,python Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # hubmap-sdk --
 - A Python interface to the various HuBMAP web services ### Overview The hubmap
 sdk is a client library that allows for easy integration of the API's
```

### Comparing `hubmap-sdk-1.0.3/README.md` & `hubmap-sdk-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hubmap-sdk-1.0.3/hubmap_sdk/entitysdk.py` & `hubmap-sdk-1.0.4/hubmap_sdk/entitysdk.py`

 * *Files identical despite different names*

### Comparing `hubmap-sdk-1.0.3/hubmap_sdk/sdk_helper.py` & `hubmap-sdk-1.0.4/hubmap_sdk/sdk_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import json.decoder
 
 import requests
-from hubmap_sdk import Donor, Dataset, Sample, Collection, Upload
+from hubmap_sdk import Donor, Dataset, Sample, Collection, Upload, Publication
 
 
 
 def make_entity(output):
     if output['entity_type'].lower() == 'dataset':
         new_instance = Dataset(output)
     if output['entity_type'].lower() == 'donor':
         new_instance = Donor(output)
     if output['entity_type'].lower() == 'sample':
         new_instance = Sample(output)
     if output['entity_type'].lower() == 'collection':
         new_instance = Collection(output)
     if output['entity_type'].lower() == 'upload':
         new_instance = Upload(output)
+    if output['entity_type'].lower() == 'publication':
+        new_instance = Publication(output)
     return new_instance
 
 
 def make_request(method_type, instance, url, optional_argument=None, data=None):
     if optional_argument is None:
         optional_argument = ''
     try:
```

### Comparing `hubmap-sdk-1.0.3/hubmap_sdk/searchsdk.py` & `hubmap-sdk-1.0.4/hubmap_sdk/searchsdk.py`

 * *Files identical despite different names*

### Comparing `hubmap-sdk-1.0.3/hubmap_sdk.egg-info/PKG-INFO` & `hubmap-sdk-1.0.4/hubmap_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Client Libary to use HuBMAP web services
 Author: Hubmap
 Author-email: api-developers@hubmapconsortium.org
 Keywords: HuBMAP Sdk,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hubmap-sdk Version: 1.0.3 Summary: Python Client
+Metadata-Version: 2.1 Name: hubmap-sdk Version: 1.0.4 Summary: Python Client
 Libary to use HuBMAP web services Author: Hubmap Author-email: api-
 developers@hubmapconsortium.org Keywords: HuBMAP Sdk,python Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # hubmap-sdk --
 - A Python interface to the various HuBMAP web services ### Overview The hubmap
 sdk is a client library that allows for easy integration of the API's
```

### Comparing `hubmap-sdk-1.0.3/setup.py` & `hubmap-sdk-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hubmap-sdk",
-    version="1.0.3",
+    version="1.0.4",
     author="Hubmap",
     author_email="api-developers@hubmapconsortium.org",
     description="Python Client Libary to use HuBMAP web services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['hubmap_sdk'],
     keywords=[
```

