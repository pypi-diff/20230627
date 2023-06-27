# Comparing `tmp/dcentrapi-0.2.95.tar.gz` & `tmp/dcentrapi-0.2.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.95.tar", last modified: Tue Jun 27 13:33:37 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.96.tar", last modified: Tue Jun 27 14:10:01 2023, max compression
```

## Comparing `dcentrapi-0.2.95.tar` & `dcentrapi-0.2.96.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 13:33:37.761097 dcentrapi-0.2.95/
--rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.95/LICENSE.rst
--rw-r--r--   0 oded       (502) staff       (20)     6742 2023-06-27 13:33:37.760954 dcentrapi-0.2.95/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.95/README.md
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 13:33:37.759837 dcentrapi-0.2.95/dcentrapi/
--rw-r--r--   0 oded       (502) staff       (20)      771 2023-06-27 12:04:51.000000 dcentrapi-0.2.95/dcentrapi/Base.py
--rw-r--r--   0 oded       (502) staff       (20)      397 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/__init__.py
--rw-r--r--   0 oded       (502) staff       (20)      130 2023-06-27 12:04:51.000000 dcentrapi-0.2.95/dcentrapi/common.py
--rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/eventPolling.py
--rw-r--r--   0 oded       (502) staff       (20)      525 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/gasMonitor.py
--rw-r--r--   0 oded       (502) staff       (20)      559 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/hackMitigation.py
--rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.95/dcentrapi/merkleTree.py
--rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-27 12:04:51.000000 dcentrapi-0.2.95/dcentrapi/requests_dappi.py
--rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/rpcAggregation.py
--rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.95/dcentrapi/test.py
--rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/dcentrapi/web3Index.py
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-27 13:33:37.760730 dcentrapi-0.2.95/dcentrapi.egg-info/
--rw-r--r--   0 oded       (502) staff       (20)     6742 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)      453 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-27 13:33:37.000000 dcentrapi-0.2.95/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-27 13:33:37.761141 dcentrapi-0.2.95/setup.cfg
--rw-r--r--   0 oded       (502) staff       (20)     1110 2023-06-27 13:32:34.000000 dcentrapi-0.2.95/setup.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 14:10:01.983053 dcentrapi-0.2.96/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.96/LICENSE.rst
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 14:10:01.982902 dcentrapi-0.2.96/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.96/README.md
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 14:10:01.982000 dcentrapi-0.2.96/dcentrapi/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      771 2023-06-27 14:09:32.000000 dcentrapi-0.2.96/dcentrapi/Base.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      405 2023-06-27 13:48:08.000000 dcentrapi-0.2.96/dcentrapi/__init__.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      130 2023-06-27 13:48:08.000000 dcentrapi-0.2.96/dcentrapi/common.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     8714 2023-06-27 14:09:17.000000 dcentrapi-0.2.96/dcentrapi/eventPolling.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-06-27 14:09:05.000000 dcentrapi-0.2.96/dcentrapi/gasMonitor.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      525 2023-06-27 14:08:48.000000 dcentrapi-0.2.96/dcentrapi/hackMitigation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.96/dcentrapi/merkleTree.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3059 2023-06-27 14:06:26.000000 dcentrapi-0.2.96/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      804 2023-06-27 14:06:16.000000 dcentrapi-0.2.96/dcentrapi/web3Index.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 14:10:01.982706 dcentrapi-0.2.96/dcentrapi.egg-info/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 14:10:01.000000 dcentrapi-0.2.96/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      407 2023-06-27 14:10:01.000000 dcentrapi-0.2.96/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-27 14:10:01.000000 dcentrapi-0.2.96/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-27 14:10:01.000000 dcentrapi-0.2.96/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-27 14:10:01.000000 dcentrapi-0.2.96/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-27 14:10:01.983177 dcentrapi-0.2.96/setup.cfg
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1110 2023-06-27 14:05:55.000000 dcentrapi-0.2.96/setup.py
```

### Comparing `dcentrapi-0.2.95/LICENSE.rst` & `dcentrapi-0.2.96/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.95/PKG-INFO` & `dcentrapi-0.2.96/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.95
+Version: 0.2.96
 Summary: Dcentralab Pypi packages
+Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -103,7 +105,9 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+
+
```

### Comparing `dcentrapi-0.2.95/README.md` & `dcentrapi-0.2.96/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.95/dcentrapi/Base.py` & `dcentrapi-0.2.96/dcentrapi/Base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class Base:
     def __init__(self, stage, username=None, key=None):
-        self.__version__ = "0.2.94"
+        self.__version__ = "0.2.96"
 
         if stage == "develop":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://test-api.dcentralab.com/"
             self.web3index_url = "https://test-api.web3index.info/"
         if stage == "staging":
             self.headers = {"Authorization": username + "," + key}
```

### Comparing `dcentrapi-0.2.95/dcentrapi/eventPolling.py` & `dcentrapi-0.2.96/dcentrapi/eventPolling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from typing import Union, List, Dict
-from dcentrapi.requests_dappi import requests_get, requests_post
+
+import requests
+
 from dcentrapi.Base import Base
 
 
 class EventPolling(Base):
     def get_collection(self, collection_name: str):
         url = self.url + "event_polling/collection"
         data = {"collection_name": collection_name}
-        response = requests_post(url, json=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     def get_latest_contract_version(self, contract_name: str):
         url = self.url + "event_polling/get_latest_contract_version"
         data = {"contract_name": contract_name}
-        response = requests_get(url, params=data, headers=self.headers)
+        response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def register_user(self, user_name: str, collection_name: str):
         url = self.url + "event_polling/register_user"
         data = {
             "user_name": user_name,
             "collection_name": collection_name,
         }
-        response = requests_post(url, json=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     def subscribe_contract(
         self,
         contract_name: str,
         contract_address: str,
         network: str,
@@ -43,21 +45,21 @@
             "contract_version": contract_version,
             "network": network,
             "collection_name": collection_name,
             "abi": abi,
             "git_tag": git_tag,
             "webhook_url": webhook_url,
         }
-        response = requests_post(url, json=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     def get_schema(self, contract_name: str, contract_version: str):
         url = self.url + "event_polling/schema"
         data = {"contract_name": contract_name, "contract_version": contract_version}
-        response = requests_get(url, params=data, headers=self.headers)
+        response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def get_events_sum_of_values_in_range(
         self,
         collection_name: str,
         contract_address: str,
         event_name: str,
@@ -70,92 +72,92 @@
             "collection_name": collection_name,
             "contract_address": contract_address,
             "event_name": event_name,
             "field_name": field_name,
             "start_time": start_time,
             "end_time": end_time,
         }
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_collection_sum_of_values_in_range(
         self, collection_name: str, event_name: str, field_name: str, start_time: str, end_time: str
     ):
         url = self.url + "event_polling/collection_sum_of_values_in_range"
         data = {
             "collection_name": collection_name,
             "event_name": event_name,
             "field_name": field_name,
             "start_time": start_time,
             "end_time": end_time,
         }
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_collection_contracts_sum_of_values(
         self, collection_name: str, event_name: str, field_name: str, start_time: str, end_time: str
     ):
         url = self.url + "event_polling/collection_contracts_sum_of_values"
         data = {
             "collection_name": collection_name,
             "event_name": event_name,
             "field_name": field_name,
             "start_time": start_time,
             "end_time": end_time,
         }
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_collection_daily_nof_transactions(self, collection_name: str, start_time: str, end_time: str):
         url = self.url + "event_polling/collection_daily_nof_transactions"
         data = {"collection_name": collection_name, "start_time": start_time, "end_time": end_time}
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_collection_nof_transactions(self, collection_name: str):
         url = self.url + "event_polling/collection_nof_transactions"
         data = {"collection_name": collection_name}
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_collection_nof_transactions_by_time(self, collection_name, start_time, end_time):
         url = self.url + "event_polling/collection_nof_transactions_by_time"
         data = {"collection_name": collection_name, "start_time": start_time, "end_time": end_time}
-        response = requests_get(url, params=data, headers=self.headers)
+        response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def get_collection_nof_users_in_time_range(self, collection_name: str, start_time: str, end_time: str):
         url = self.url + "event_polling/collection_nof_users_in_time_range"
         data = {"collection_name": collection_name, "start_time": start_time, "end_time": end_time}
-        response = requests_get(url, params=data, headers=self.headers)
+        response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def get_contract_nof_transactions(self, collection_name: str, contract_address: str):
         url = self.url + "event_polling/contract_nof_transactions"
         data = {"collection_name": collection_name, "contract_address": contract_address}
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_collection_users_in_time_range(self, collection_name: str, start_time: str, end_time: str):
         url = self.url + "event_polling/collection_users_in_time_range"
         data = {"collection_name": collection_name, "start_time": start_time, "end_time": end_time}
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_contract_users_in_time_range(
         self, collection_name: str, contract_address: str, start_time: str, end_time: str
     ):
         url = self.url + "event_polling/contract_users_in_time_range"
         data = {
             "collection_name": collection_name,
             "contract_address": contract_address,
             "start_time": start_time,
             "end_time": end_time,
         }
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_contracts_events_info(
         self,
         collection_name: str,
         contract_addresses: [str],
         event_names: [str],
@@ -174,37 +176,37 @@
             "end_time": end_time,
             "user_web3_addresses": user_web3_addresses,
             "event_names": event_names,
             "incentive_id": incentive_id,
             "user_address": user_address,
             "sort": sort,
         }
-        response = requests_post(url, json=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     def get_nof_contracts_events_unique_transactions(
         self, collection_name: str, contract_addresses: str, event_names: str
     ):
         url = self.url + "event_polling/contracts_events_info"
         data = {
             "collection_name": collection_name,
             "contract_addresses": contract_addresses,
             "event_names": event_names,
         }
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_nof_token_transfers(self, contract_addresses: [str]):
         url = self.url + "event_polling/token_transfers"
         data = {"contract_addresses": contract_addresses}
-        response = requests_get(url=url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_event_details(self, collection_name: str, list_of_events: [str], event_parameter: str):
         url = self.url + "event_polling/get_event_details"
         data = {
             "collection_name": collection_name,
             "list_of_events": list_of_events,
             "event_parameter": event_parameter,
         }
-        response = requests_post(url=url, json=data, headers=self.headers)
+        response = requests.post(url=url, json=data, headers=self.headers)
         return response.json()
```

### Comparing `dcentrapi-0.2.95/dcentrapi/hackMitigation.py` & `dcentrapi-0.2.96/dcentrapi/hackMitigation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import requests
 from dcentrapi.Base import Base
 from dcentrapi.common import DapiError
-from dcentrapi.requests_dappi import requests_get
 
 
 class HackMitigation(Base):
 
     def are_addresses_blacklisted(self, addresses: [str]):
         url = self.url + "generic_freeze_signal/are_addresses_blacklisted"
         data = {
             "addresses": addresses,
         }
-        response = requests_get(url, json=data, headers=self.headers)
+        response = requests.get(url, json=data, headers=self.headers)
         try:
             return response.json()
         except Exception as e:
             return DapiError(response=response, exception=e)
```

### Comparing `dcentrapi-0.2.95/dcentrapi/merkleTree.py` & `dcentrapi-0.2.96/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.95/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.96/dcentrapi/rpcAggregation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,68 @@
+import requests
+
 from dcentrapi.Base import Base
-from dcentrapi.requests_dappi import requests_get, requests_post
 
 
 class RpcAggregation(Base):
     def get_token_balance(self, user, token, network, rpc_url=None):
         url = self.url + "tokenBalance"
         data = {"network": network, "user": user, "token": token, "rpc_url": rpc_url}
-        response = requests_get(url, params=data, headers=self.headers)
+        response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def get_token_balances_for_user(self, user, tokens: list, network, rpc_url=None):
         url = self.url + "tokenBalancesForUser"
         data = {"network": network, "user": user, "tokens": tokens, "rpc_url": rpc_url}
-        response = requests_post(url, json=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     def get_token_balance_for_users(self, users: list, token, network, rpc_url=None):
         url = self.url + "tokenBalanceForUsers"
         data = {"network": network, "users": users, "token": token, "rpc_url": rpc_url}
-        response = requests_post(url, json=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     def calculate_token_price_from_pair(self, pool, target_token_address, network, rpc_url=None):
         url = self.url + "calculateTokenPriceFromPair"
         data = {"network": network, "lp_token": pool, "target_token_address": target_token_address, "rpc_url": rpc_url}
-        response = requests_get(url, params=data, headers=self.headers)
+        response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def calculate_reserves_amount_from_pair(self, pool, amount, network, rpc_url=None):
         url = self.url + "calculateReservesAmountsFromPair"
         data = {"network": network, "lp_token": pool, "amount": amount, "rpc_url": rpc_url}
-        response = requests_get(url, params=data, headers=self.headers)
+        response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def get_reserves_from_pair(self, pool, network, rpc_url=None):
         url = self.url + "getReservesFromPair"
         data = {"network": network, "lp_token": pool, "rpc_url": rpc_url}
-        response = requests_get(url, params=data, headers=self.headers)
+        response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     # Accepted values for factory_type (May 2023):
     # UNI_V2, UNI_V3, CURVE, BALANCER
 
     def get_reserves_from_pools(self, factory_type, pools: list, network, rpc_url=None):
         url = self.url + "getReservesFromPools"
         data = {
             "factory_type": factory_type,
             "pools": pools,
             "network": network,
             "rpc_url": rpc_url
         }
-        response = requests_post(url, json=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     # Same accepted factory_type values as for get_reserves_from_pools above
     def get_pool_data_from_factory(self, factory_type, factory, indices: list, network, rpc_url=None):
         url = self.url + "getPoolDataFromFactory"
         data = {
             "factory_type": factory_type,
             "factory": factory,
             "indices": indices,
             "network": network,
             "rpc_url": rpc_url
         }
-        response = requests_post(url, json=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
```

### Comparing `dcentrapi-0.2.95/dcentrapi/web3Index.py` & `dcentrapi-0.2.96/dcentrapi/web3Index.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import requests
+
 from dcentrapi.Base import Base
-from dcentrapi.requests_dappi import requests_get
 
 
 class Web3Index(Base):
     def get_pairs(self, network_name: str, token_address: str):
         url = self.web3index_url + "pairs" + f"/{network_name}/{token_address}"
-        response = requests_get(url, headers=self.headers)
+        response = requests.get(url, headers=self.headers)
         return response.json()
 
     def get_factories(self):
         url = self.web3index_url + "factories"
-        response = requests_get(url, headers=self.headers)
+        response = requests.get(url, headers=self.headers)
         return response.json()
 
     def get_token_price_snapshot(self, info):
         # Currently info is token symbol (str), e.g. "XCAD"
         # In future, might also have the base token id (int)
         url = self.web3index_url + "token_price_snapshot" + f"/{info}"
-        response = requests_get(url, headers=self.headers)
+        response = requests.get(url, headers=self.headers)
         return response.json()
```

### Comparing `dcentrapi-0.2.95/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.96/dcentrapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.95
+Version: 0.2.96
 Summary: Dcentralab Pypi packages
+Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -103,7 +105,9 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+
+
```

### Comparing `dcentrapi-0.2.95/setup.py` & `dcentrapi-0.2.96/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return result.group(1)
 
 
 DESCRIPTION = 'Dcentralab Pypi packages'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 project_name = 'dcentrapi'
-VERSION = "0.2.95"
+VERSION = "0.2.96"
 
 
 # Setting up
 setup(
     name="dcentrapi",
     version=VERSION,
     author="Dcentralab (Niv Shitrit)",
```

