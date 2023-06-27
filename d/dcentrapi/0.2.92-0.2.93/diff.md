# Comparing `tmp/dcentrapi-0.2.92.tar.gz` & `tmp/dcentrapi-0.2.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.92.tar", last modified: Tue Jun 27 09:02:48 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.93.tar", last modified: Tue Jun 27 11:28:21 2023, max compression
```

## Comparing `dcentrapi-0.2.92.tar` & `dcentrapi-0.2.93.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 09:02:48.416629 dcentrapi-0.2.92/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.92/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 09:02:48.416457 dcentrapi-0.2.92/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.92/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 09:02:48.414308 dcentrapi-0.2.92/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.92/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      399 2023-06-27 09:02:30.000000 dcentrapi-0.2.92/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      196 2023-06-27 09:02:34.000000 dcentrapi-0.2.92/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     8763 2023-06-27 09:02:30.000000 dcentrapi-0.2.92/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      527 2023-06-27 08:46:56.000000 dcentrapi-0.2.92/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      561 2023-06-27 08:47:15.000000 dcentrapi-0.2.92/dcentrapi/hackMitigation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.92/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3109 2023-06-27 08:48:22.000000 dcentrapi-0.2.92/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      839 2023-06-27 08:48:44.000000 dcentrapi-0.2.92/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 09:02:48.416183 dcentrapi-0.2.92/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      407 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-27 09:02:48.416686 dcentrapi-0.2.92/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.92/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 11:28:21.588220 dcentrapi-0.2.93/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.93/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6742 2023-06-27 11:28:21.588092 dcentrapi-0.2.93/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.93/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 11:28:21.587134 dcentrapi-0.2.93/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      829 2023-06-26 05:46:25.000000 dcentrapi-0.2.93/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      405 2023-06-27 11:25:45.000000 dcentrapi-0.2.93/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)      196 2023-06-27 11:25:55.000000 dcentrapi-0.2.93/dcentrapi/common.py
+-rw-r--r--   0 oded       (502) staff       (20)     8769 2023-06-27 11:25:45.000000 dcentrapi-0.2.93/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      533 2023-06-27 11:25:45.000000 dcentrapi-0.2.93/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)      567 2023-06-27 11:25:45.000000 dcentrapi-0.2.93/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.93/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)     3115 2023-06-27 11:25:45.000000 dcentrapi-0.2.93/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.93/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)      845 2023-06-27 11:25:45.000000 dcentrapi-0.2.93/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 11:28:21.587916 dcentrapi-0.2.93/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6742 2023-06-27 11:28:21.000000 dcentrapi-0.2.93/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      425 2023-06-27 11:28:21.000000 dcentrapi-0.2.93/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-27 11:28:21.000000 dcentrapi-0.2.93/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-27 11:28:21.000000 dcentrapi-0.2.93/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-27 11:28:21.000000 dcentrapi-0.2.93/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-27 11:28:21.588267 dcentrapi-0.2.93/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1167 2022-12-21 09:08:31.000000 dcentrapi-0.2.93/setup.py
```

### Comparing `dcentrapi-0.2.92/LICENSE.rst` & `dcentrapi-0.2.93/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.92/PKG-INFO` & `dcentrapi-0.2.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.92
+Version: 0.2.93
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.92/README.md` & `dcentrapi-0.2.93/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.92/dcentrapi/Base.py` & `dcentrapi-0.2.93/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.92/dcentrapi/eventPolling.py` & `dcentrapi-0.2.93/dcentrapi/eventPolling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Union, List, Dict
-from dcentrapi.modules.requests import requests_get, requests_post
+from dcentrapi.modules.requests_dappi import requests_get, requests_post
 from dcentrapi.Base import Base
 
 
 class EventPolling(Base):
     def get_collection(self, collection_name: str):
         url = self.url + "event_polling/collection"
         data = {"collection_name": collection_name}
```

### Comparing `dcentrapi-0.2.92/dcentrapi/gasMonitor.py` & `dcentrapi-0.2.93/dcentrapi/gasMonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcentrapi.Base import Base
-from dcentrapi.modules.requests import requests_get
+from dcentrapi.modules.requests_dappi import requests_get
 
 
 class GasMonitor(Base):
 
     def get_optimal_gas_price(self, network_name, minutes, stats=None, values=None):
         url = self.url + "gas_monitor/optimal_gas_price_for_network"
         data = {
```

### Comparing `dcentrapi-0.2.92/dcentrapi/merkleTree.py` & `dcentrapi-0.2.93/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.92/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.93/dcentrapi/rpcAggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcentrapi.Base import Base
-from dcentrapi.modules.requests import requests_get, requests_post
+from dcentrapi.modules.requests_dappi import requests_get, requests_post
 
 
 class RpcAggregation(Base):
     def get_token_balance(self, user, token, network, rpc_url=None):
         url = self.url + "tokenBalance"
         data = {"network": network, "user": user, "token": token, "rpc_url": rpc_url}
         response = requests_get(url, params=data, headers=self.headers)
```

### Comparing `dcentrapi-0.2.92/dcentrapi/web3Index.py` & `dcentrapi-0.2.93/dcentrapi/web3Index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcentrapi.Base import Base
-from dcentrapi.modules.requests import requests_get
+from dcentrapi.modules.requests_dappi import requests_get
 
 
 class Web3Index(Base):
     def get_pairs(self, network_name: str, token_address: str):
         url = self.web3index_url + "pairs" + f"/{network_name}/{token_address}"
         response = requests_get(url, headers=self.headers)
         return response.json()
```

### Comparing `dcentrapi-0.2.92/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.93/dcentrapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.92
+Version: 0.2.93
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.92/setup.py` & `dcentrapi-0.2.93/setup.py`

 * *Files identical despite different names*

