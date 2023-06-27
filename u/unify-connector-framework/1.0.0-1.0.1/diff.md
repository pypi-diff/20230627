# Comparing `tmp/unify-connector-framework-1.0.0.tar.gz` & `tmp/unify-connector-framework-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-connector-framework-1.0.0.tar", last modified: Mon Jun 26 21:54:32 2023, max compression
+gzip compressed data, was "dist/unify-connector-framework-1.0.1.tar", last modified: Tue Jun 27 18:17:08 2023, max compression
```

## Comparing `unify-connector-framework-1.0.0.tar` & `unify-connector-framework-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1690 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unifyconnectorframework/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      799 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15890 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/connector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10771 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/connector_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1691 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/logging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17963 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/organization_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1690 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      553 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unifyconnectorframework/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2023-06-27 18:17:02.000000 unify-connector-framework-1.0.1/unifyconnectorframework/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      787 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/config_not_found_error.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15890 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/connector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10771 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/connector_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1691 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/logging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17963 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/organization_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/utils.py
```

### Comparing `unify-connector-framework-1.0.0/LICENSE` & `unify-connector-framework-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.0/PKG-INFO` & `unify-connector-framework-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-connector-framework
-Version: 1.0.0
+Version: 1.0.1
 Summary: Develop connectors for Element Unify with the Connector Framework
 Home-page: https://github.com/ElementAnalytics/unify-python-agents-common
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-connector-framework-1.0.0/README.md` & `unify-connector-framework-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.0/setup.py` & `unify-connector-framework-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.0/unify_connector_framework.egg-info/PKG-INFO` & `unify-connector-framework-1.0.1/unify_connector_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-connector-framework
-Version: 1.0.0
+Version: 1.0.1
 Summary: Develop connectors for Element Unify with the Connector Framework
 Home-page: https://github.com/ElementAnalytics/unify-python-agents-common
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-connector-framework-1.0.0/unifyconnectorframework/__init__.py` & `unify-connector-framework-1.0.1/unifyconnectorframework/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 
 """
 Defines package information
 """
 from .organization_client import DatasetOperation, OrganizationClient
 from .connector_handler import ConnectorHandler
 from .connector import Connector
+from .config_not_found_error import ConfigNotFoundError
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

### Comparing `unify-connector-framework-1.0.0/unifyconnectorframework/connector.py` & `unify-connector-framework-1.0.1/unifyconnectorframework/connector.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.0/unifyconnectorframework/connector_handler.py` & `unify-connector-framework-1.0.1/unifyconnectorframework/connector_handler.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.0/unifyconnectorframework/logging.py` & `unify-connector-framework-1.0.1/unifyconnectorframework/logging.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.0/unifyconnectorframework/organization_client.py` & `unify-connector-framework-1.0.1/unifyconnectorframework/organization_client.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.0/unifyconnectorframework/utils.py` & `unify-connector-framework-1.0.1/unifyconnectorframework/utils.py`

 * *Files identical despite different names*

