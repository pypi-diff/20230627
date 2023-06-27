# Comparing `tmp/alibabacloud_gateway_oss-0.0.8.tar.gz` & `tmp/alibabacloud_gateway_oss-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_oss-0.0.8.tar", last modified: Wed Oct 26 01:52:34 2022, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_oss-0.0.9.tar", last modified: Tue Jun 27 11:54:16 2023, max compression
```

## Comparing `alibabacloud_gateway_oss-0.0.8.tar` & `alibabacloud_gateway_oss-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      886 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss/
--rw-r--r--   0 root         (0) root         (0)       22 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29081 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss.egg-info/
--rw-r--r--   0 root         (0) root         (0)      886 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      454 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2952 2022-10-26 01:52:34.000000 alibabacloud_gateway_oss-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30241 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      454 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-06-27 11:54:16.000000 alibabacloud_gateway_oss-0.0.9/setup.py
```

### Comparing `alibabacloud_gateway_oss-0.0.8/PKG-INFO` & `alibabacloud_gateway_oss-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gateway_oss
-Version: 0.0.8
+Version: 0.0.9
 Summary: Alibaba Cloud OSS SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,oss
```

### Comparing `alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss/client.py` & `alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from alibabacloud_darabonba_signature_util.signer import Signer
 from typing import List, Dict
 from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_gateway_spi import models as spi_models
 from alibabacloud_tea_util.client import Client as UtilClient
+from alibabacloud_darabonba_map.client import Client as MapClient
 from alibabacloud_darabonba_string.client import Client as StringClient
 from alibabacloud_tea_xml.client import Client as XMLClient
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 from alibabacloud_oss_util.client import Client as OSSUtilClient
-from alibabacloud_darabonba_map.client import Client as MapClient
 from alibabacloud_darabonba_array.client import Client as ArrayClient
 
 
 class Client(SPIClient):
     _default_signed_params: List[str] = None
     _except_signed_params: List[str] = None
 
@@ -59,15 +59,16 @@
             'restore',
             'callback',
             'callback-var',
             'policy',
             'encryption',
             'versions',
             'versioning',
-            'versionId'
+            'versionId',
+            'wormId'
         ]
         self._except_signed_params = [
             'list-type',
             'regions'
         ]
 
     def modify_configuration(
@@ -94,14 +95,23 @@
         request = context.request
         host_map = {}
         if not UtilClient.is_unset(request.host_map):
             host_map = request.host_map
         bucket_name = host_map.get('bucket')
         if UtilClient.is_unset(bucket_name):
             bucket_name = ''
+        if not UtilClient.is_unset(request.headers.get('x-oss-meta-*')):
+            tmp = UtilClient.parse_json(request.headers.get('x-oss-meta-*'))
+            map_data = UtilClient.assert_as_map(tmp)
+            meta_data = UtilClient.stringify_map_value(map_data)
+            meta_key_set = MapClient.key_set(meta_data)
+            request.headers['x-oss-meta-*'] = None
+            for key in meta_key_set:
+                new_key = f'x-oss-meta-{key}'
+                request.headers[new_key] = meta_data.get(key)
         config = context.configuration
         credential = request.credential
         access_key_id = credential.get_access_key_id()
         access_key_secret = credential.get_access_key_secret()
         security_token = credential.get_security_token()
         if not UtilClient.empty(security_token):
             request.headers['x-oss-security-token'] = security_token
@@ -141,14 +151,23 @@
         request = context.request
         host_map = {}
         if not UtilClient.is_unset(request.host_map):
             host_map = request.host_map
         bucket_name = host_map.get('bucket')
         if UtilClient.is_unset(bucket_name):
             bucket_name = ''
+        if not UtilClient.is_unset(request.headers.get('x-oss-meta-*')):
+            tmp = UtilClient.parse_json(request.headers.get('x-oss-meta-*'))
+            map_data = UtilClient.assert_as_map(tmp)
+            meta_data = UtilClient.stringify_map_value(map_data)
+            meta_key_set = MapClient.key_set(meta_data)
+            request.headers['x-oss-meta-*'] = None
+            for key in meta_key_set:
+                new_key = f'x-oss-meta-{key}'
+                request.headers[new_key] = meta_data.get(key)
         config = context.configuration
         credential = request.credential
         access_key_id = await credential.get_access_key_id_async()
         access_key_secret = await credential.get_access_key_secret_async()
         security_token = await credential.get_security_token_async()
         if not UtilClient.empty(security_token):
             request.headers['x-oss-security-token'] = security_token
@@ -591,15 +610,15 @@
         content_md_5 = headers.get('content-md5')
         if UtilClient.is_unset(content_md_5):
             content_md_5 = ''
         canonicalized_headers = f"{canonicalized_headers}{content_md_5}\n{content_type}\n{headers.get('date')}\n"
         keys = MapClient.key_set(headers)
         sorted_headers = ArrayClient.asc_sort(keys)
         for header in sorted_headers:
-            if StringClient.contains(StringClient.to_lower(header), 'x-oss-'):
+            if StringClient.contains(StringClient.to_lower(header), 'x-oss-') and not UtilClient.is_unset(headers.get(header)):
                 canonicalized_headers = f'{canonicalized_headers}{header}:{headers.get(header)}\n'
         return canonicalized_headers
 
     async def build_canonicalized_headers_async(
         self,
         headers: Dict[str, str],
     ) -> str:
@@ -610,15 +629,15 @@
         content_md_5 = headers.get('content-md5')
         if UtilClient.is_unset(content_md_5):
             content_md_5 = ''
         canonicalized_headers = f"{canonicalized_headers}{content_md_5}\n{content_type}\n{headers.get('date')}\n"
         keys = MapClient.key_set(headers)
         sorted_headers = ArrayClient.asc_sort(keys)
         for header in sorted_headers:
-            if StringClient.contains(StringClient.to_lower(header), 'x-oss-'):
+            if StringClient.contains(StringClient.to_lower(header), 'x-oss-') and not UtilClient.is_unset(headers.get(header)):
                 canonicalized_headers = f'{canonicalized_headers}{header}:{headers.get(header)}\n'
         return canonicalized_headers
 
     def get_signature_v2(
         self,
         bucket_name: str,
         pathname: str,
```

### Comparing `alibabacloud_gateway_oss-0.0.8/alibabacloud_gateway_oss.egg-info/PKG-INFO` & `alibabacloud_gateway_oss-0.0.9/alibabacloud_gateway_oss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gateway-oss
-Version: 0.0.8
+Version: 0.0.9
 Summary: Alibaba Cloud OSS SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,oss
```

### Comparing `alibabacloud_gateway_oss-0.0.8/setup.py` & `alibabacloud_gateway_oss-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,38 +20,38 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gateway_oss.
 
-Created on 25/10/2022
+Created on 27/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gateway_oss"
 NAME = "alibabacloud_gateway_oss" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OSS SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-gateway"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_gateway_spi>=0.0.1, <1.0.0",
-    "alibabacloud_credentials>=0.2.0, <1.0.0",
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_credentials>=0.3.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_tea_xml>=0.0.2, <1.0.0",
     "alibabacloud_darabonba_string>=0.0.4, <1.0.0",
     "alibabacloud_darabonba_map>=0.0.1, <1.0.0",
-    "alibabacloud_darabonba_array>=0.0.5, <1.0.0",
-    "alibabacloud_darabonba_encode_util>=0.0.1, <1.0.0",
-    "alibabacloud_darabonba_signature_util>=0.0.3, <1.0.0"
+    "alibabacloud_darabonba_array>=0.1.0, <1.0.0",
+    "alibabacloud_darabonba_encode_util>=0.0.2, <1.0.0",
+    "alibabacloud_darabonba_signature_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

