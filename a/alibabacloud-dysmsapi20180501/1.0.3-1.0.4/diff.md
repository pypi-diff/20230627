# Comparing `tmp/alibabacloud_dysmsapi20180501-1.0.3.tar.gz` & `tmp/alibabacloud_dysmsapi20180501-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dysmsapi20180501-1.0.3.tar", last modified: Mon Dec 27 03:08:11 2021, max compression
+gzip compressed data, was "dist/alibabacloud_dysmsapi20180501-1.0.4.tar", last modified: Tue Jun 27 07:48:45 2023, max compression
```

## Comparing `alibabacloud_dysmsapi20180501-1.0.3.tar` & `alibabacloud_dysmsapi20180501-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      217 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501/
--rw-r--r--   0 root         (0) root         (0)       21 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20431 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501/client.py
--rw-r--r--   0 root         (0) root         (0)    29916 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2021-12-27 03:08:11.000000 alibabacloud_dysmsapi20180501-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36170 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501/client.py
+-rw-r--r--   0 root         (0) root         (0)    39312 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-06-27 07:48:45.000000 alibabacloud_dysmsapi20180501-1.0.4/setup.py
```

### Comparing `alibabacloud_dysmsapi20180501-1.0.3/LICENSE` & `alibabacloud_dysmsapi20180501-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20180501-1.0.3/PKG-INFO` & `alibabacloud_dysmsapi20180501-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dysmsapi20180501
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud Dysmsapi (20180501) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dysmsapi20180501-1.0.3/README-CN.md` & `alibabacloud_dysmsapi20180501-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20180501-1.0.3/README.md` & `alibabacloud_dysmsapi20180501-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20180501-1.0.3/alibabacloud_dysmsapi20180501.egg-info/PKG-INFO` & `alibabacloud_dysmsapi20180501-1.0.4/alibabacloud_dysmsapi20180501.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dysmsapi20180501
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud Dysmsapi (20180501) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dysmsapi20180501-1.0.3/setup.py` & `alibabacloud_dysmsapi20180501-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dysmsapi20180501.
 
-Created on 27/12/2021
+Created on 27/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dysmsapi20180501"
 NAME = "alibabacloud_dysmsapi20180501" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dysmsapi (20180501) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

