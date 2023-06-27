# Comparing `tmp/marketplace_sdk-0.3.6.tar.gz` & `tmp/marketplace_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketplace_sdk-0.3.6.tar", last modified: Tue Jun 13 11:59:24 2023, max compression
+gzip compressed data, was "marketplace_sdk-0.4.0.tar", last modified: Tue Jun 27 09:58:40 2023, max compression
```

## Comparing `marketplace_sdk-0.3.6.tar` & `marketplace_sdk-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.573458 marketplace_sdk-0.3.6/logos/
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/logos/MARVEL.png
--rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/logos/MarketPlace.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.573458 marketplace_sdk-0.3.6/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.573458 marketplace_sdk-0.3.6/marketplace/app/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/marketplace/app/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/marketplace/message_broker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/message_broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/message_broker/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/message_broker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.836193 marketplace_sdk-0.4.0/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/logos/MARVEL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/logos/MarketPlace.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.836193 marketplace_sdk-0.4.0/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.836193 marketplace_sdk-0.4.0/marketplace/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/marketplace/app/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/marketplace/message_broker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/message_broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/message_broker/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/message_broker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/setup.py
```

### Comparing `marketplace_sdk-0.3.6/LICENSE` & `marketplace_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/PKG-INFO` & `marketplace_sdk-0.4.0/marketplace_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: marketplace_sdk
-Version: 0.3.6
+Name: marketplace-sdk
+Version: 0.4.0
 Summary: Software Development Toolkit to communicate with the Materials MarketPlace platform.
 Home-page: https://github.com/materials-marketplace/python-sdk
 Author: Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 Author-email: simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `marketplace_sdk-0.3.6/README.md` & `marketplace_sdk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/logos/MARVEL.png` & `marketplace_sdk-0.4.0/logos/MARVEL.png`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/logos/MarketPlace.png` & `marketplace_sdk-0.4.0/logos/MarketPlace.png`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/marketplace/app/__init__.py` & `marketplace_sdk-0.4.0/marketplace/app/__init__.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/marketplace/app/utils.py` & `marketplace_sdk-0.4.0/marketplace/app/utils.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/marketplace/app/v0/base.py` & `marketplace_sdk-0.4.0/marketplace/app/v0/base.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/marketplace/app/v0/object_storage.py` & `marketplace_sdk-0.4.0/marketplace/app/v0/object_storage.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/marketplace/app/v0/transformation.py` & `marketplace_sdk-0.4.0/marketplace/app/v0/transformation.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/marketplace/client.py` & `marketplace_sdk-0.4.0/marketplace/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from urllib.parse import urljoin
 
 import requests
 from requests import Response
 
 from .version import __version__
 
-MP_DEFAULT_HOST = "https://www.materials-marketplace.eu/"
+MP_DEFAULT_HOST = "https://materials-marketplace.eu/"
 
 
 class MarketPlaceClient:
     """Interact with the MarketPlace platform."""
 
     def __init__(self, marketplace_host_url=None, access_token=None):
         marketplace_host_url = marketplace_host_url or os.environ.get(
```

### Comparing `marketplace_sdk-0.3.6/marketplace/message_broker/rpc_server.py` & `marketplace_sdk-0.4.0/marketplace/message_broker/rpc_server.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/marketplace_sdk.egg-info/PKG-INFO` & `marketplace_sdk-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: marketplace-sdk
-Version: 0.3.6
+Name: marketplace_sdk
+Version: 0.4.0
 Summary: Software Development Toolkit to communicate with the Materials MarketPlace platform.
 Home-page: https://github.com/materials-marketplace/python-sdk
 Author: Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 Author-email: simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `marketplace_sdk-0.3.6/marketplace_sdk.egg-info/SOURCES.txt` & `marketplace_sdk-0.4.0/marketplace_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.6/setup.cfg` & `marketplace_sdk-0.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = marketplace_sdk
-version = v0.3.6
+version = v0.4.0
 description = Software Development Toolkit to communicate with the Materials MarketPlace platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/materials-marketplace/python-sdk
 author = Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 author_email = simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 license = MIT
```

