# Comparing `tmp/dcentrapi-0.2.91.tar.gz` & `tmp/dcentrapi-0.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.91.tar", last modified: Tue Jun 27 08:49:53 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.92.tar", last modified: Tue Jun 27 09:02:48 2023, max compression
```

## Comparing `dcentrapi-0.2.91.tar` & `dcentrapi-0.2.92.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 08:49:53.525075 dcentrapi-0.2.91/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.91/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 08:49:53.524928 dcentrapi-0.2.91/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.91/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 08:49:53.523963 dcentrapi-0.2.91/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.91/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      332 2023-06-27 07:19:17.000000 dcentrapi-0.2.91/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      196 2023-06-27 08:49:15.000000 dcentrapi-0.2.91/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     8763 2023-06-27 08:46:40.000000 dcentrapi-0.2.91/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      527 2023-06-27 08:46:56.000000 dcentrapi-0.2.91/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      561 2023-06-27 08:47:15.000000 dcentrapi-0.2.91/dcentrapi/hackMitigation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.91/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3109 2023-06-27 08:48:22.000000 dcentrapi-0.2.91/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      839 2023-06-27 08:48:44.000000 dcentrapi-0.2.91/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 08:49:53.524740 dcentrapi-0.2.91/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 08:49:53.000000 dcentrapi-0.2.91/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      407 2023-06-27 08:49:53.000000 dcentrapi-0.2.91/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-27 08:49:53.000000 dcentrapi-0.2.91/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-27 08:49:53.000000 dcentrapi-0.2.91/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-27 08:49:53.000000 dcentrapi-0.2.91/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-27 08:49:53.525127 dcentrapi-0.2.91/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.91/setup.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 09:02:48.416629 dcentrapi-0.2.92/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.92/LICENSE.rst
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 09:02:48.416457 dcentrapi-0.2.92/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.92/README.md
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 09:02:48.414308 dcentrapi-0.2.92/dcentrapi/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.92/dcentrapi/Base.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      399 2023-06-27 09:02:30.000000 dcentrapi-0.2.92/dcentrapi/__init__.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      196 2023-06-27 09:02:34.000000 dcentrapi-0.2.92/dcentrapi/common.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     8763 2023-06-27 09:02:30.000000 dcentrapi-0.2.92/dcentrapi/eventPolling.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      527 2023-06-27 08:46:56.000000 dcentrapi-0.2.92/dcentrapi/gasMonitor.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      561 2023-06-27 08:47:15.000000 dcentrapi-0.2.92/dcentrapi/hackMitigation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.92/dcentrapi/merkleTree.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3109 2023-06-27 08:48:22.000000 dcentrapi-0.2.92/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      839 2023-06-27 08:48:44.000000 dcentrapi-0.2.92/dcentrapi/web3Index.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 09:02:48.416183 dcentrapi-0.2.92/dcentrapi.egg-info/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      407 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-27 09:02:48.000000 dcentrapi-0.2.92/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-27 09:02:48.416686 dcentrapi-0.2.92/setup.cfg
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.92/setup.py
```

### Comparing `dcentrapi-0.2.91/LICENSE.rst` & `dcentrapi-0.2.92/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.91/PKG-INFO` & `dcentrapi-0.2.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.91
+Version: 0.2.92
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.2.91/README.md` & `dcentrapi-0.2.92/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.91/dcentrapi/Base.py` & `dcentrapi-0.2.92/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.91/dcentrapi/eventPolling.py` & `dcentrapi-0.2.92/dcentrapi/eventPolling.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, List, Dict
-from dcentrapi.Base import Base
 from dcentrapi.modules.requests import requests_get, requests_post
+from dcentrapi.Base import Base
 
 
 class EventPolling(Base):
     def get_collection(self, collection_name: str):
         url = self.url + "event_polling/collection"
         data = {"collection_name": collection_name}
         response = requests_post(url, json=data, headers=self.headers)
```

### Comparing `dcentrapi-0.2.91/dcentrapi/gasMonitor.py` & `dcentrapi-0.2.92/dcentrapi/gasMonitor.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.91/dcentrapi/hackMitigation.py` & `dcentrapi-0.2.92/dcentrapi/hackMitigation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.91/dcentrapi/merkleTree.py` & `dcentrapi-0.2.92/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.91/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.92/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.91/dcentrapi/web3Index.py` & `dcentrapi-0.2.92/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.91/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.92/dcentrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.91
+Version: 0.2.92
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.2.91/setup.py` & `dcentrapi-0.2.92/setup.py`

 * *Files identical despite different names*

