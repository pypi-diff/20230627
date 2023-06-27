# Comparing `tmp/cloudpy_org-1.3.5.tar.gz` & `tmp/cloudpy_org-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.3.5.tar", last modified: Tue Jun 27 06:29:21 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.3.6.tar", last modified: Tue Jun 27 07:12:47 2023, max compression
```

## Comparing `cloudpy_org-1.3.5.tar` & `cloudpy_org-1.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 06:29:21.715669 cloudpy_org-1.3.5/
--rw-rw-rw-   0        0        0      935 2023-06-27 06:29:21.715669 cloudpy_org-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 06:29:21.621917 cloudpy_org-1.3.5/cloudpy_org/
--rw-rw-rw-   0        0        0      111 2023-06-25 19:34:30.000000 cloudpy_org-1.3.5/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    72789 2023-06-27 06:23:40.000000 cloudpy_org-1.3.5/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 06:29:21.700042 cloudpy_org-1.3.5/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2023-06-27 06:29:20.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-27 06:29:21.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 06:29:20.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-27 06:29:20.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-27 06:29:20.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 06:29:21.715669 cloudpy_org-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-06-27 06:25:03.000000 cloudpy_org-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:12:47.948359 cloudpy_org-1.3.6/
+-rw-rw-rw-   0        0        0      935 2023-06-27 07:12:47.932731 cloudpy_org-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:12:47.854606 cloudpy_org-1.3.6/cloudpy_org/
+-rw-rw-rw-   0        0        0      111 2023-06-25 19:34:30.000000 cloudpy_org-1.3.6/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    72887 2023-06-27 07:12:21.000000 cloudpy_org-1.3.6/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:12:47.917116 cloudpy_org-1.3.6/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-06-27 07:12:47.000000 cloudpy_org-1.3.6/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-27 07:12:47.000000 cloudpy_org-1.3.6/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:12:47.000000 cloudpy_org-1.3.6/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-27 07:12:47.000000 cloudpy_org-1.3.6/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-27 07:12:47.000000 cloudpy_org-1.3.6/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:12:47.948359 cloudpy_org-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-06-27 07:11:32.000000 cloudpy_org-1.3.6/setup.py
```

### Comparing `cloudpy_org-1.3.5/PKG-INFO` & `cloudpy_org-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.3.5
+Version: 1.3.6
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.5/cloudpy_org/tools.py` & `cloudpy_org-1.3.6/cloudpy_org/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Find documentation at https://www.cloudpy.org
 """
-cloudpy_org_version='1.3.5'
+cloudpy_org_version='1.3.6'
 import os
 import json
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings('ignore')
 warnings.simplefilter('ignore')
 import pandas as pd
@@ -1488,12 +1488,16 @@
         return str(rslt)
 def aws_framework_manager_client(username_or_email:str="",pwd:str="",local:bool=False):
     url_base = "https://www.cloudpy.org/"
     if local:
         url_base = "http://localhost/"
     url = url_base + "gen_authentication_token"
     token = requests.post(url_base + "gen_authentication_token",json = {"username_or_email":username_or_email,"pwd":pwd} ,verify=False).text
-    secret_key = requests.post(url_base + "authenticate_with_token",json={"token":token},verify=False).text
-    service_token= requests.post(url_base + "gen_service_token",json={"secret_key":secret_key},verify=False).text
-    fm = aws_framework_manager(secret_key=secret_key)
-    print(fm.initialize_service(service_token=service_token))
+    if "wrong" in token.lower():
+        fm = None
+        print(token)
+    else:
+        secret_key = requests.post(url_base + "authenticate_with_token",json={"token":token},verify=False).text
+        service_token= requests.post(url_base + "gen_service_token",json={"secret_key":secret_key},verify=False).text
+        fm = aws_framework_manager(secret_key=secret_key)
+        print(fm.initialize_service(service_token=service_token))
     return fm
```

### Comparing `cloudpy_org-1.3.5/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.3.6/cloudpy_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.3.5
+Version: 1.3.6
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.5/setup.py` & `cloudpy_org-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.3.5",
+    version="1.3.6",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

