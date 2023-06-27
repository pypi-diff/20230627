# Comparing `tmp/alibabacloud_gateway_oss_py2-0.0.8.tar.gz` & `tmp/alibabacloud_gateway_oss_py2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_oss_py2-0.0.8.tar", last modified: Wed Oct 26 01:52:39 2022, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_oss_py2-0.0.9.tar", last modified: Tue Jun 27 11:54:19 2023, max compression
```

## Comparing `alibabacloud_gateway_oss_py2-0.0.8.tar` & `alibabacloud_gateway_oss_py2-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 01:52:39.000000 alibabacloud_gateway_oss_py2-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1020 2022-10-26 01:52:39.000000 alibabacloud_gateway_oss_py2-0.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 01:52:39.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss/
--rw-r--r--   0 root         (0) root         (0)       22 2022-10-26 01:52:38.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15686 2022-10-26 01:52:38.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 01:52:39.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2022-10-26 01:52:38.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      339 2022-10-26 01:52:38.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-26 01:52:38.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      498 2022-10-26 01:52:38.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-10-26 01:52:38.000000 alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-26 01:52:39.000000 alibabacloud_gateway_oss_py2-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3272 2022-10-26 01:52:38.000000 alibabacloud_gateway_oss_py2-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16304 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      498 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-06-27 11:54:19.000000 alibabacloud_gateway_oss_py2-0.0.9/setup.py
```

### Comparing `alibabacloud_gateway_oss_py2-0.0.8/PKG-INFO` & `alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_gateway_oss_py2
-Version: 0.0.8
+Name: alibabacloud-gateway-oss-py2
+Version: 0.0.9
 Summary: Alibaba Cloud OSS SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,oss,py2
```

### Comparing `alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss/client.py` & `alibabacloud_gateway_oss_py2-0.0.9/alibabacloud_gateway_oss/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from __future__ import unicode_literals
 
 from Tea.exceptions import TeaException
 from alibabacloud_darabonba_encode_util.encoder import Encoder
 from alibabacloud_darabonba_signature_util.signer import Signer
-from Tea.core import TeaCore
 from Tea.converter import TeaConverter
+from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_util.client import Client as UtilClient
+from alibabacloud_darabonba_map.client import Client as MapClient
 from alibabacloud_darabonba_string.client import Client as StringClient
 from alibabacloud_tea_xml.client import Client as XMLClient
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 from alibabacloud_oss_util.client import Client as OSSUtilClient
-from alibabacloud_darabonba_map.client import Client as MapClient
 from alibabacloud_darabonba_array.client import Client as ArrayClient
 
 
 class Client(SPIClient):
     _default_signed_params = None  # type: list[str]
     _except_signed_params = None  # type: list[str]
 
@@ -60,15 +60,16 @@
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
 
     def modify_configuration(self, context, attribute_map):
@@ -79,14 +80,23 @@
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
+                new_key = 'x-oss-meta-%s' % TeaConverter.to_unicode(key)
+                request.headers[new_key] = meta_data.get(key)
         config = context.configuration
         credential = request.credential
         access_key_id = credential.get_access_key_id()
         access_key_secret = credential.get_access_key_secret()
         security_token = credential.get_security_token()
         if not UtilClient.empty(security_token):
             request.headers['x-oss-security-token'] = security_token
@@ -290,13 +300,13 @@
         content_md_5 = headers.get('content-md5')
         if UtilClient.is_unset(content_md_5):
             content_md_5 = ''
         canonicalized_headers = '%s%s\n%s\n%s\n' % (TeaConverter.to_unicode(canonicalized_headers), TeaConverter.to_unicode(content_md_5), TeaConverter.to_unicode(content_type), TeaConverter.to_unicode(headers.get('date')))
         keys = MapClient.key_set(headers)
         sorted_headers = ArrayClient.asc_sort(keys)
         for header in sorted_headers:
-            if StringClient.contains(StringClient.to_lower(header), 'x-oss-'):
+            if StringClient.contains(StringClient.to_lower(header), 'x-oss-') and not UtilClient.is_unset(headers.get(header)):
                 canonicalized_headers = '%s%s:%s\n' % (TeaConverter.to_unicode(canonicalized_headers), TeaConverter.to_unicode(header), TeaConverter.to_unicode(headers.get(header)))
         return canonicalized_headers
 
     def get_signature_v2(self, bucket_name, pathname, method, query, headers, secret):
         return ''
```

### Comparing `alibabacloud_gateway_oss_py2-0.0.8/alibabacloud_gateway_oss_py2.egg-info/PKG-INFO` & `alibabacloud_gateway_oss_py2-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-gateway-oss-py2
-Version: 0.0.8
+Name: alibabacloud_gateway_oss_py2
+Version: 0.0.9
 Summary: Alibaba Cloud OSS SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,oss,py2
```

### Comparing `alibabacloud_gateway_oss_py2-0.0.8/setup.py` & `alibabacloud_gateway_oss_py2-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,38 +21,38 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gateway_oss_py2.
 
-Created on 25/10/2022
+Created on 27/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gateway_oss"
 NAME = "alibabacloud_gateway_oss_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OSS SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-gateway"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_gateway_spi_py2>=0.0.1, <1.0.0",
-    "alibabacloud_credentials_py2>=0.0.1, <1.0.0",
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
+    "alibabacloud_credentials_py2>=0.1.1, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_oss_util_py2>=0.0.1, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_tea_xml_py2>=0.0.2, <1.0.0",
     "alibabacloud_darabonba_string_py2>=0.0.4, <1.0.0",
-    "alibabacloud_darabonba_map_py2>=0.0.1, <1.0.0",
-    "alibabacloud_darabonba_array_py2>=0.0.5, <1.0.0",
-    "alibabacloud_darabonba_encode_util_py2>=0.0.1, <1.0.0",
-    "alibabacloud_darabonba_signature_util_py2>=0.0.3, <1.0.0"
+    "alibabacloud_darabonba_map_py2>=0.0.2, <1.0.0",
+    "alibabacloud_darabonba_array_py2>=0.1.0, <1.0.0",
+    "alibabacloud_darabonba_encode_util_py2>=0.0.2, <1.0.0",
+    "alibabacloud_darabonba_signature_util_py2>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
         with open("README.md") as fp:
```

