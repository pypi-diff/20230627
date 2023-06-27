# Comparing `tmp/cloudpy_org-1.3.4.tar.gz` & `tmp/cloudpy_org-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.3.4.tar", last modified: Sun Jun 25 19:38:52 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.3.5.tar", last modified: Tue Jun 27 06:29:21 2023, max compression
```

## Comparing `cloudpy_org-1.3.4.tar` & `cloudpy_org-1.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 19:38:52.637284 cloudpy_org-1.3.4/
--rw-rw-rw-   0        0        0      935 2023-06-25 19:38:52.637284 cloudpy_org-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 19:38:52.543538 cloudpy_org-1.3.4/cloudpy_org/
--rw-rw-rw-   0        0        0      111 2023-06-25 19:34:30.000000 cloudpy_org-1.3.4/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    74554 2023-06-25 19:38:44.000000 cloudpy_org-1.3.4/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:38:52.621658 cloudpy_org-1.3.4/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 19:38:52.637284 cloudpy_org-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-06-25 19:29:27.000000 cloudpy_org-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:29:21.715669 cloudpy_org-1.3.5/
+-rw-rw-rw-   0        0        0      935 2023-06-27 06:29:21.715669 cloudpy_org-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 06:29:21.621917 cloudpy_org-1.3.5/cloudpy_org/
+-rw-rw-rw-   0        0        0      111 2023-06-25 19:34:30.000000 cloudpy_org-1.3.5/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    72789 2023-06-27 06:23:40.000000 cloudpy_org-1.3.5/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:29:21.700042 cloudpy_org-1.3.5/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-06-27 06:29:20.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-27 06:29:21.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 06:29:20.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-27 06:29:20.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-27 06:29:20.000000 cloudpy_org-1.3.5/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 06:29:21.715669 cloudpy_org-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-06-27 06:25:03.000000 cloudpy_org-1.3.5/setup.py
```

### Comparing `cloudpy_org-1.3.4/PKG-INFO` & `cloudpy_org-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.3.4
+Version: 1.3.5
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.4/cloudpy_org/tools.py` & `cloudpy_org-1.3.5/cloudpy_org/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Find documentation at https://www.cloudpy.org
 """
-cloudpy_org_version='1.3.4'
+cloudpy_org_version='1.3.5'
 import os
 import json
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings('ignore')
 warnings.simplefilter('ignore')
 import pandas as pd
@@ -407,16 +407,14 @@
                 self.__session = boto3.Session(aws_access_key_id=spd[0]
                                          ,aws_secret_access_key=spd[1])
                 self.__s3_client = boto3.client('s3'
                                                 ,aws_access_key_id=spd[0]
                                                 ,aws_secret_access_key=spd[1]
                                                 ,region_name=region_name)
                 del spd
-                #print("AWS framework manager client ready to initialize.")
-                spd = []
             except Exception as e:
                 print('Error:',str(e))
                 self.__session = None
                 self.__s3_client = None
             
     #__________________________________________________________________________
     def domain_commands(self,domain_name:str=None)->None:
@@ -1163,47 +1161,31 @@
         if len(secret_key) > 10:
             k = 'JQxrs8sWqn3JIWlIL8nTlw-302SfmV7RmlZ-T-gB5c4=oiwn8TU5-NcDKzVq'
             self.cppt = processing_tools(data=xpt.basic_dicstr_to_dict(xpt.decrypt(secret_key,self.__do(k,10,False)[1] + self.__do(k,10,False)[0][0:4])))
         else:
             self.cppt = processing_tools()
     #___________________________________________________________________
     def initialize_service(self,service_token:str,version:str=cloudpy_org_version,test_file_name:str=None):
-        error_message = 'Could not initialize the service. Please verify you are using the right service token.'
+        self.__initialize_error_message = 'Could not initialize the service. Please verify you are using the right service token.'
+        self.args_by_key,self.dx = {},{}
         try:
             for i in range(0,1):
                 self.args_by_key,self.dx = {},{}
-                self.__api_encrypted_caller = ''\
-                'gAAAAABkh-dZKOI8qSh47zj54htxA_Ib_ag4gI99hdxDuHo7oWktIOaQ7U63M13qURWqXrbxJ-X8ZFXXn7Lmifq_uI8Sqe_l1CE-'\
-                'BHe39zTrwk6ZJWaDrUwDeXi1Xm_7SEYffuZ75hp7yV9x8qMRTo2nhYFs4chOlTU-gojLp3iosWzlAaxtS8WE6mnxxOn8u7RAcoxg'\
-                'H-Omya51HagtAL3Ho2137D5qIf3LDhr_IFSlnZTkNw-WgMjS3LwUdXgAsSRddZQSzxNlsa7ame28tyGee4Qwg4dg2PCuegG9_1r8'\
-                'WTXYm_U8QVySZt5fRt1qDUzLl9MFDmlMCnjUn5GknLqXYvCY3z4GNNlfBqaxZUpbFE4pV3OZ6NI-cb6V0JiX6rACvxjDIIwecDg2'\
-                'oaEa1Jw-xKBQ86EnFx2j1PcMMtvJlX75xCCR789-v75GfAejN6ZWVjzDwanI2qy5IL63tigukTnufpDuesc3NZUMM4V0B_LbSw0a'\
-                'Ic7tzFKAaRxE3uFiz9J8yAbAkbOGu6pGpWcEXgtvtQe0A4l1fiQznqAhE23o4R0QJ3YHTC7JTuTfi32S3Sjel9jexsyOyRFUdcuO'\
-                'zeminNCLLpIUDG8BYFhy0-jwMvrWnUB2b_NPqlBpKx9EJZwHrga2XgVhRxfHgnSD3vcZqNv4jLhGZdCwfUuRIArKTbmwzddthPZN'\
-                'f8W21ejufOxcvR2JWw7MfKiPpTNlunRsdEq8QLHAwNawjuEiYlK-vrGm0MsSIZmP55nOwzE5SbHNtPgLomZMVDxgKh2xixfq59Ux'\
-                'uVyieJozGM-XPJhjziU6AlAdboUHyo6LJeBV95sdF7VomSLBWbFokTFBKOaY7upqtt7ix1WquS4JwrCRRJcUL4AYrM3njJe9U4Cv'\
-                '9ZGAO5bpKOOwRJRiXkMtLpCCoLg-NqioU59zAgEnGVuT85MqZYzJiH7Xeu9LcEqZ1UDff3kkxpol8piry73P5Jip6hJ9GwW1CulV'\
-                'd8uT-CR_EoVxM9qy0bpY49yMLfq8SmgKz2iKVDo-DOw4IG2UvQ4sr21j242MWT36lwVhl6LZpiFjTTc8vGGogrGcpRclzitVjmEd'\
-                '3zx7TTtHg_Z6SuT8KyNyO6tUsLci9CsPPWJMgjdA-UZgDYuMCYbLWxffZmK1SYg1zDAutfVf6DOlKIwnJOa3QPWyM8SBBT68nxu0'\
-                '20DEgsRt1kPjDiLsbK_TU6PB0H5pUJcTG4Z2JdHmFzgb6uBsUPrrSMcx2BCGxjrggpAC-v5mPO5_RU2IMWVNDLhiAzBKdv1ivtCu'\
-                'H_tDJdfneJHVZ1ucxS8vc7Jz26OUDfT7oDoxLRerO8o6Prm_zKdrVbNgvACpl3fWATCv2nJYyV-PBI_uupWJ6nz-X56Rb3KMt64_'\
-                'HY8BL-3QQclPw1vv05LUGkeGmHgFcJKzS6L6EbkVLCAf3Ar3Z6JeeaZ0Mi77zvaUofaoab7XLatBHg0z7wHpsiynESTKlafaZRTA'\
-                'rH_1U5Au9KWV0kWSxXRu8unqCpfs_okOVuYaoBvqc4Reo2i6NPthfXYqagNlGfYuLYLhsx1szF2Cg86_7KedwMtU8c2roAAN3eGN'\
-                'hhTkLS6xQOK_'
+                self.__api_encrypted_caller = self.__sc[2]
                 self.__get_dynamic_response(service_token=service_token,version=version,test_file_name=test_file_name)
                 self.find_methods_arguments()
                 self.set_valid_characters()
                 self.version = self.get_version()
             if self.__service_initialized:   
-                return 'AWS framework manager client service initialized.'
+                return 'AWS framework manager client: service initialized.'
             else:
-                return error_message
+                return self.__initialize_error_message
         except Exception as e:
             #print("error 01:",str(e))
-            return error_message
+            return self.__initialize_error_message
     #___________________________________________________________________
     def __load_local_code(self,file_name):
         with open(os.getcwd() + "/" + file_name, 'r') as f:
             rslt = json.loads(f.read())
         return rslt
     #___________________________________________________________________
     def __k(self,tagStr:str):
@@ -1226,17 +1208,25 @@
                     print("testing dynamic respose..")
             exec(dc)
             del self.last_k
             self.__service_initialized = True
         except Exception as e:
             #print("error 02:",str(e))
             self.__service_initialized = False
-        self.dynamic_code_response = self.ddxx[service_token + self.ddkk]
-        del self.ddkk
-        del self.ddxx
+        try:
+            self.dynamic_code_response = self.ddxx[service_token + self.ddkk]
+            del self.ddkk
+            del self.ddxx
+        except:
+            self.dynamic_code_response = {}
+        try:
+            del self.ddkk
+            del self.ddxx
+        except:
+            ...
     #___________________________________________________________________
     def _decorator(decorator_param):
         def inner_func(self,dk):
             k = dk + "_is_function"
             dc = "self.dx['@k'] = self.dynamic_exec(dynamic_key='@dynamic_key'@these_args)"
             dc = dc.replace("@dynamic_key",dk)\
             .replace("@k",k)\
```

### Comparing `cloudpy_org-1.3.4/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.3.5/cloudpy_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.3.4
+Version: 1.3.5
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.4/setup.py` & `cloudpy_org-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.3.4",
+    version="1.3.5",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

