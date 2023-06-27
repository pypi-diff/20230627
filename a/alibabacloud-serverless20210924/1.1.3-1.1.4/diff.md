# Comparing `tmp/alibabacloud_serverless20210924-1.1.3.tar.gz` & `tmp/alibabacloud_serverless20210924-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_serverless20210924-1.1.3.tar", last modified: Fri Dec  2 08:58:19 2022, max compression
+gzip compressed data, was "dist/alibabacloud_serverless20210924-1.1.4.tar", last modified: Thu Dec  8 03:07:11 2022, max compression
```

## Comparing `alibabacloud_serverless20210924-1.1.3.tar` & `alibabacloud_serverless20210924-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/
--rw-r--r--   0 root         (0) root         (0)       92 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1043 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114550 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924/client.py
--rw-r--r--   0 root         (0) root         (0)   147612 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2645 2022-12-02 08:58:19.000000 alibabacloud_serverless20210924-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)      161 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1043 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   116772 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924/client.py
+-rw-r--r--   0 root         (0) root         (0)   148936 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2645 2022-12-08 03:07:11.000000 alibabacloud_serverless20210924-1.1.4/setup.py
```

### Comparing `alibabacloud_serverless20210924-1.1.3/LICENSE` & `alibabacloud_serverless20210924-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_serverless20210924-1.1.3/PKG-INFO` & `alibabacloud_serverless20210924-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_serverless20210924
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud serverless (20210924) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_serverless20210924-1.1.3/README-CN.md` & `alibabacloud_serverless20210924-1.1.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_serverless20210924-1.1.3/README.md` & `alibabacloud_serverless20210924-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924/client.py` & `alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,80 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def cancel_task(
+        self,
+        name: str,
+    ) -> serverless_20210924_models.CancelTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.cancel_task_with_options(name, headers, runtime)
+
+    async def cancel_task_async(
+        self,
+        name: str,
+    ) -> serverless_20210924_models.CancelTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.cancel_task_with_options_async(name, headers, runtime)
+
+    def cancel_task_with_options(
+        self,
+        name: str,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> serverless_20210924_models.CancelTaskResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='CancelTask',
+            version='2021-09-24',
+            protocol='HTTPS',
+            pathname=f'/apis/serverlessdeployment/v1/tasks/{OpenApiUtilClient.get_encode_param(name)}/cancel',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            serverless_20210924_models.CancelTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def cancel_task_with_options_async(
+        self,
+        name: str,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> serverless_20210924_models.CancelTaskResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='CancelTask',
+            version='2021-09-24',
+            protocol='HTTPS',
+            pathname=f'/apis/serverlessdeployment/v1/tasks/{OpenApiUtilClient.get_encode_param(name)}/cancel',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            serverless_20210924_models.CancelTaskResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
     def create_application(
         self,
         request: serverless_20210924_models.CreateApplicationRequest,
     ) -> serverless_20210924_models.CreateApplicationResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_application_with_options(request, headers, runtime)
```

### Comparing `alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924/models.py` & `alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2145,14 +2145,58 @@
         if m.get('commit') is not None:
             self.commit = m.get('commit')
         if m.get('on') is not None:
             self.on = m.get('on')
         return self
 
 
+class CancelTaskResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: Task = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = Task()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateApplicationRequest(TeaModel):
     def __init__(
         self,
         auto_deploy: bool = None,
         description: str = None,
         env_vars: Dict[str, str] = None,
         name: str = None,
```

### Comparing `alibabacloud_serverless20210924-1.1.3/alibabacloud_serverless20210924.egg-info/PKG-INFO` & `alibabacloud_serverless20210924-1.1.4/alibabacloud_serverless20210924.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-serverless20210924
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud serverless (20210924) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_serverless20210924-1.1.3/setup.py` & `alibabacloud_serverless20210924-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_serverless20210924.
 
-Created on 02/12/2022
+Created on 08/12/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_serverless20210924"
 NAME = "alibabacloud_serverless20210924" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud serverless (20210924) SDK Library for Python"
```

