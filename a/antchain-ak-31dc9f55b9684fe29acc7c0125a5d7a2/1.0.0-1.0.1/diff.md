# Comparing `tmp/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0.tar.gz` & `tmp/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0.tar", last modified: Tue Jun 27 03:58:43 2023, max compression
+gzip compressed data, was "dist/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1.tar", last modified: Tue Jun 27 09:13:09 2023, max compression
```

## Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0.tar` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-27 03:58:42.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-27 03:58:42.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-06-27 03:58:42.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-27 03:58:42.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-27 03:58:42.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22124 2023-06-27 03:58:42.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/client.py
--rw-r--r--   0 root         (0) root         (0)    15155 2023-06-27 03:58:42.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-27 03:58:43.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-06-27 03:58:42.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-27 09:13:08.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-27 09:13:08.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-06-27 09:13:08.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-27 09:13:08.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-27 09:13:08.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22124 2023-06-27 09:13:08.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/client.py
+-rw-r--r--   0 root         (0) root         (0)    15462 2023-06-27 09:13:08.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-27 09:13:09.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-06-27 09:13:08.000000 antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/setup.py
```

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/LICENSE` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/PKG-INFO` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_31dc9f55b9684fe29acc7c0125a5d7a2 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/README-CN.md` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/README.md` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/PKG-INFO` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-31dc9f55b9684fe29acc7c0125a5d7a2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_31dc9f55b9684fe29acc7c0125a5d7a2 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/SOURCES.txt` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/client.py` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_31dc9f55b9684fe29acc7c0125a5d7a2',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_31dc9f55b9684fe29acc7c0125a5d7a2',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/models.py` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/antchain_sdk_ak_31dc9f55b9684fe29acc7c0125a5d7a2/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,25 +200,28 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         status: str = None,
         result_url: str = None,
+        failed_reason: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 隐私计算模型执行状态
         self.status = status
         # 结果文件路径
         self.result_url = result_url
+        # 失败的原因
+        self.failed_reason = failed_reason
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -231,28 +234,32 @@
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         if self.status is not None:
             result['status'] = self.status
         if self.result_url is not None:
             result['result_url'] = self.result_url
+        if self.failed_reason is not None:
+            result['failed_reason'] = self.failed_reason
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('result_url') is not None:
             self.result_url = m.get('result_url')
+        if m.get('failed_reason') is not None:
+            self.failed_reason = m.get('failed_reason')
         return self
 
 
 class UploadAntcloudAdomAppmarketFileRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.0/setup.py` & `antchain_ak_31dc9f55b9684fe29acc7c0125a5d7a2-1.0.1/setup.py`

 * *Files identical despite different names*

