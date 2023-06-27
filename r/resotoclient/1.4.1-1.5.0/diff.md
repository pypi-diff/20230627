# Comparing `tmp/resotoclient-1.4.1.tar.gz` & `tmp/resotoclient-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoclient-1.4.1.tar", max compression
+gzip compressed data, was "resotoclient-1.5.0.tar", max compression
```

## Comparing `resotoclient-1.4.1.tar` & `resotoclient-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-09 13:17:30.428599 resotoclient-1.4.1/LICENSE
--rw-r--r--   0        0        0     1243 2023-05-09 13:17:30.428599 resotoclient-1.4.1/README.md
--rw-r--r--   0        0        0     2083 2023-05-09 13:17:30.428599 resotoclient-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    20715 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/__init__.py
--rw-r--r--   0        0        0    23316 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/async_client.py
--rw-r--r--   0        0        0     6219 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/ca.py
--rw-r--r--   0        0        0     2813 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/http_client/__init__.py
--rw-r--r--   0        0        0    12959 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/http_client/aiohttp_client.py
--rw-r--r--   0        0        0     1282 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/http_client/event_loop_thread.py
--rw-r--r--   0        0        0      693 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/json_utils.py
--rw-r--r--   0        0        0     3813 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/jwt_utils.py
--rw-r--r--   0        0        0     2283 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/models.py
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 resotoclient-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 08:53:30.129541 resotoclient-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1243 2023-06-27 08:53:30.129541 resotoclient-1.5.0/README.md
+-rw-r--r--   0        0        0     2156 2023-06-27 08:53:30.133541 resotoclient-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    20715 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/__init__.py
+-rw-r--r--   0        0        0    23316 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/async_client.py
+-rw-r--r--   0        0        0     6219 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/ca.py
+-rw-r--r--   0        0        0     2813 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/http_client/__init__.py
+-rw-r--r--   0        0        0    12959 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/http_client/aiohttp_client.py
+-rw-r--r--   0        0        0     1282 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/http_client/event_loop_thread.py
+-rw-r--r--   0        0        0      693 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/json_utils.py
+-rw-r--r--   0        0        0     3813 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/jwt_utils.py
+-rw-r--r--   0        0        0     2363 2023-06-27 08:53:30.133541 resotoclient-1.5.0/resotoclient/models.py
+-rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 resotoclient-1.5.0/PKG-INFO
```

### Comparing `resotoclient-1.4.1/LICENSE` & `resotoclient-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/README.md` & `resotoclient-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/pyproject.toml` & `resotoclient-1.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resotoclient"
-version = "1.4.1"
+version = "1.5.0"
 description = "Resoto Python client library"
 authors = ["Some Engineering Inc."]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/someengineering/resotoclient-python"
 repository = "https://github.com/someengineering/resotoclient-python"
 packages = [
@@ -54,14 +54,15 @@
 flake8 = "^6.0.0"
 black = ">=22.12.0"
 flake8-bandit = "^4.1.1"
 flake8-bugbear = "^23.3.23"
 pep8-naming = "^0.13.3"
 networkx = "^2.8"
 six = "^1.16.0"
+urllib3 = "^1.26.15" # poetry itself stopped working with latest urllib3
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.19.0"
 
 [tool.pyright]
 include = ["resotoclient", "tests"]
 exclude = ["**/node_modules",
```

### Comparing `resotoclient-1.4.1/resotoclient/__init__.py` & `resotoclient-1.5.0/resotoclient/__init__.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/resotoclient/async_client.py` & `resotoclient-1.5.0/resotoclient/async_client.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/resotoclient/ca.py` & `resotoclient-1.5.0/resotoclient/ca.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/resotoclient/http_client/__init__.py` & `resotoclient-1.5.0/resotoclient/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/resotoclient/http_client/aiohttp_client.py` & `resotoclient-1.5.0/resotoclient/http_client/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/resotoclient/http_client/event_loop_thread.py` & `resotoclient-1.5.0/resotoclient/http_client/event_loop_thread.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/resotoclient/json_utils.py` & `resotoclient-1.5.0/resotoclient/json_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/resotoclient/jwt_utils.py` & `resotoclient-1.5.0/resotoclient/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.1/resotoclient/models.py` & `resotoclient-1.5.0/resotoclient/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 @dataclass
 class Property:
     name: str
     kind: str
     required: bool = False
     description: Optional[str] = None
     synthetic: Optional[JsObject] = None
+    metadata: Optional[JsObject] = None
 
 
 @dataclass
 class Kind:
     fqn: str
     runtime_kind: Optional[str]
     properties: Optional[List[Property]]
     bases: Optional[List[str]]
     aggregate_root: Optional[bool] = False
     successor_kinds: Optional[Dict[str, List[str]]] = None
+    metadata: Optional[JsObject] = None
 
 
 @dataclass
 class Model:
     kinds: Mapping[str, Kind]
```

### Comparing `resotoclient-1.4.1/PKG-INFO` & `resotoclient-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoclient
-Version: 1.4.1
+Version: 1.5.0
 Summary: Resoto Python client library
 Home-page: https://github.com/someengineering/resotoclient-python
 License: Apache-2.0
 Author: Some Engineering Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -14,15 +14,14 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Provides-Extra: extras
 Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: certifi (>=2017.4.17)
 Requires-Dist: cryptography (>=36.0.2)
```

