# Comparing `tmp/dcentrapi-0.2.94.tar.gz` & `tmp/dcentrapi-0.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.94.tar", last modified: Tue Jun 27 11:39:54 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.95.tar", last modified: Tue Jun 27 13:33:37 2023, max compression
```

## Comparing `dcentrapi-0.2.94.tar` & `dcentrapi-0.2.95.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 11:39:54.864017 dcentrapi-0.2.94/
--rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.94/LICENSE.rst
--rw-r--r--   0 oded       (502) staff       (20)     6742 2023-06-27 11:39:54.863886 dcentrapi-0.2.94/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.94/README.md
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 11:39:54.862787 dcentrapi-0.2.94/dcentrapi/
--rw-r--r--   0 oded       (502) staff       (20)      829 2023-06-26 05:46:25.000000 dcentrapi-0.2.94/dcentrapi/Base.py
--rw-r--r--   0 oded       (502) staff       (20)      405 2023-06-27 11:25:45.000000 dcentrapi-0.2.94/dcentrapi/__init__.py
--rw-r--r--   0 oded       (502) staff       (20)      196 2023-06-27 11:39:48.000000 dcentrapi-0.2.94/dcentrapi/common.py
--rw-r--r--   0 oded       (502) staff       (20)     8769 2023-06-27 11:25:45.000000 dcentrapi-0.2.94/dcentrapi/eventPolling.py
--rw-r--r--   0 oded       (502) staff       (20)      533 2023-06-27 11:25:45.000000 dcentrapi-0.2.94/dcentrapi/gasMonitor.py
--rw-r--r--   0 oded       (502) staff       (20)      567 2023-06-27 11:25:45.000000 dcentrapi-0.2.94/dcentrapi/hackMitigation.py
--rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.94/dcentrapi/merkleTree.py
--rw-r--r--   0 oded       (502) staff       (20)     3115 2023-06-27 11:25:45.000000 dcentrapi-0.2.94/dcentrapi/rpcAggregation.py
--rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.94/dcentrapi/test.py
--rw-r--r--   0 oded       (502) staff       (20)      845 2023-06-27 11:25:45.000000 dcentrapi-0.2.94/dcentrapi/web3Index.py
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 11:39:54.863698 dcentrapi-0.2.94/dcentrapi.egg-info/
--rw-r--r--   0 oded       (502) staff       (20)     6742 2023-06-27 11:39:54.000000 dcentrapi-0.2.94/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)      425 2023-06-27 11:39:54.000000 dcentrapi-0.2.94/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-27 11:39:54.000000 dcentrapi-0.2.94/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-27 11:39:54.000000 dcentrapi-0.2.94/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-27 11:39:54.000000 dcentrapi-0.2.94/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-27 11:39:54.864060 dcentrapi-0.2.94/setup.cfg
--rw-r--r--   0 oded       (502) staff       (20)     1159 2023-06-27 11:39:48.000000 dcentrapi-0.2.94/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 13:33:37.761097 dcentrapi-0.2.95/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.95/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6742 2023-06-27 13:33:37.760954 dcentrapi-0.2.95/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.95/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 13:33:37.759837 dcentrapi-0.2.95/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      771 2023-06-27 12:04:51.000000 dcentrapi-0.2.95/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      397 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)      130 2023-06-27 12:04:51.000000 dcentrapi-0.2.95/dcentrapi/common.py
+-rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      525 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)      559 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.95/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-27 12:04:51.000000 dcentrapi-0.2.95/dcentrapi/requests_dappi.py
+-rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.95/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 13:33:37.760730 dcentrapi-0.2.95/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6742 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      453 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-27 13:33:37.761141 dcentrapi-0.2.95/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1110 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/setup.py
```

### Comparing `dcentrapi-0.2.94/LICENSE.rst` & `dcentrapi-0.2.95/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.94/PKG-INFO` & `dcentrapi-0.2.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.94
+Version: 0.2.95
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.2.94/README.md` & `dcentrapi-0.2.95/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.94/dcentrapi/Base.py` & `dcentrapi-0.2.95/dcentrapi/Base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from dcentrapi.common import get_dapi_version
-
-
 class Base:
     def __init__(self, stage, username=None, key=None):
-        self.__version__ = get_dapi_version()
+        self.__version__ = "0.2.94"
 
         if stage == "develop":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://test-api.dcentralab.com/"
             self.web3index_url = "https://test-api.web3index.info/"
         if stage == "staging":
             self.headers = {"Authorization": username + "," + key}
```

### Comparing `dcentrapi-0.2.94/dcentrapi/eventPolling.py` & `dcentrapi-0.2.95/dcentrapi/eventPolling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Union, List, Dict
-from dcentrapi.modules.requests_dappi import requests_get, requests_post
+from dcentrapi.requests_dappi import requests_get, requests_post
 from dcentrapi.Base import Base
 
 
 class EventPolling(Base):
     def get_collection(self, collection_name: str):
         url = self.url + "event_polling/collection"
         data = {"collection_name": collection_name}
```

### Comparing `dcentrapi-0.2.94/dcentrapi/gasMonitor.py` & `dcentrapi-0.2.95/dcentrapi/gasMonitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcentrapi.Base import Base
-from dcentrapi.modules.requests_dappi import requests_get
+from dcentrapi.requests_dappi import requests_get
 
 
 class GasMonitor(Base):
 
     def get_optimal_gas_price(self, network_name, minutes, stats=None, values=None):
         url = self.url + "gas_monitor/optimal_gas_price_for_network"
         data = {
```

### Comparing `dcentrapi-0.2.94/dcentrapi/merkleTree.py` & `dcentrapi-0.2.95/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.94/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.95/dcentrapi/rpcAggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcentrapi.Base import Base
-from dcentrapi.modules.requests_dappi import requests_get, requests_post
+from dcentrapi.requests_dappi import requests_get, requests_post
 
 
 class RpcAggregation(Base):
     def get_token_balance(self, user, token, network, rpc_url=None):
         url = self.url + "tokenBalance"
         data = {"network": network, "user": user, "token": token, "rpc_url": rpc_url}
         response = requests_get(url, params=data, headers=self.headers)
```

### Comparing `dcentrapi-0.2.94/dcentrapi/test.py` & `dcentrapi-0.2.95/dcentrapi/test.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.94/dcentrapi/web3Index.py` & `dcentrapi-0.2.95/dcentrapi/web3Index.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcentrapi.Base import Base
-from dcentrapi.modules.requests_dappi import requests_get
+from dcentrapi.requests_dappi import requests_get
 
 
 class Web3Index(Base):
     def get_pairs(self, network_name: str, token_address: str):
         url = self.web3index_url + "pairs" + f"/{network_name}/{token_address}"
         response = requests_get(url, headers=self.headers)
         return response.json()
```

### Comparing `dcentrapi-0.2.94/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.95/dcentrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.94
+Version: 0.2.95
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.2.94/setup.py` & `dcentrapi-0.2.95/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 import re
 
-# from dcentrapi.common import get_dapi_version
-
 
 def get_property(prop, project):
     result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
     return result.group(1)
 
 
 DESCRIPTION = 'Dcentralab Pypi packages'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 project_name = 'dcentrapi'
-VERSION = "0.2.94"
+VERSION = "0.2.95"
 
 
 # Setting up
 setup(
     name="dcentrapi",
     version=VERSION,
     author="Dcentralab (Niv Shitrit)",
```

