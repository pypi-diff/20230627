# Comparing `tmp/scratchcommunication-1.0.2.tar.gz` & `tmp/scratchcommunication-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-1.0.2.tar", last modified: Wed Jun 21 15:42:08 2023, max compression
+gzip compressed data, was "scratchcommunication-1.1.0.tar", last modified: Tue Jun 27 20:34:34 2023, max compression
```

## Comparing `scratchcommunication-1.0.2.tar` & `scratchcommunication-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 15:42:08.000000 scratchcommunication-1.0.2/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:42:08.245807 scratchcommunication-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-21 15:41:58.000000 scratchcommunication-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:34:34.489060 scratchcommunication-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-27 20:34:34.489060 scratchcommunication-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-27 20:34:24.000000 scratchcommunication-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:34:34.489060 scratchcommunication-1.1.0/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 20:34:24.000000 scratchcommunication-1.1.0/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-06-27 20:34:24.000000 scratchcommunication-1.1.0/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-27 20:34:24.000000 scratchcommunication-1.1.0/scratchcommunication/cloud_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 20:34:24.000000 scratchcommunication-1.1.0/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 20:34:24.000000 scratchcommunication-1.1.0/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-27 20:34:24.000000 scratchcommunication-1.1.0/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:34:34.489060 scratchcommunication-1.1.0/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-27 20:34:34.000000 scratchcommunication-1.1.0/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 20:34:34.000000 scratchcommunication-1.1.0/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:34:34.000000 scratchcommunication-1.1.0/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 20:34:34.000000 scratchcommunication-1.1.0/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 20:34:34.000000 scratchcommunication-1.1.0/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:34:34.489060 scratchcommunication-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-27 20:34:24.000000 scratchcommunication-1.1.0/setup.py
```

### Comparing `scratchcommunication-1.0.2/PKG-INFO` & `scratchcommunication-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 1.0.2
+Version: 1.1.0
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-1.0.2/scratchcommunication/cloud.py` & `scratchcommunication-1.1.0/scratchcommunication/cloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Iterable, Literal, Mapping, Union
+from typing import Literal, Union
 from .exceptions import QuickAccessDisabledError
 from websocket import WebSocket
 from threading import Thread
 import json, math, time, requests
 
 NoneType = type(None)
 
@@ -100,15 +100,15 @@
 
     @staticmethod
     def get_cloud_logs(*, project_id : str, limit : int = 100, filter_by_name : Union[str, NoneType] = None, filter_by_name_literal : bool = False) -> list:
         '''
         Use for getting the cloud logs of a project.
         '''
         logs = []
-        filter_by_name = filter_by_name if filter_by_name_literal else "☁ " + filter_by_name.replace("☁ ", "", 1)
+        filter_by_name = filter_by_name if filter_by_name_literal else "☁ " + filter_by_name.replace("☁ ", "", 1) if filter_by_name else None
         offset = 0
         while len(logs) < limit:
             data = requests.get(f"https://clouddata.scratch.mit.edu/logs?projectid={project_id}&limit={limit}&offset={offset}").json()
             logs.extend(data if filter_by_name is None else filter(lambda x: x["name"] == filter_by_name, data))
             offset += len(data)
             if len(data) == 0:
                 break
@@ -157,68 +157,71 @@
         name = name if name_literal else "☁ " + name.replace("☁ ", "", 1)
         time.sleep(max(0, self.wait_until - time.time()))
         self.wait_until = time.time() + 0.1
 
         self._set_variable(name=name, value=value, retry=10)
         self.emit_event("set", name=name.replace("☁ ", "", 1), var=name, value=value, timestamp=time.time())
 
-    def get_variable(self, * name : str, name_literal : bool = False) -> Union[float, int, bool, NoneType]:
+    def get_variable(self, *, name : str, name_literal : bool = False) -> Union[float, int, bool, NoneType]:
         '''
         Use for getting the value of a cloud variable.
         '''
-        if self.receive_from_websocket:
-            return self.values[name]
         name = name if name_literal else "☁ " + name.replace("☁ ", "", 1)
+        if self.receive_from_websocket:
+            try:
+                return self.values[name]
+            except: pass
         try:
-            return self.get_cloud_logs(project_id=self.project_id, limit=1)[0]["value"]
+            return self.get_cloud_logs(project_id=self.project_id, limit=1, filter_by_name=name, filter_by_name_literal=True)[0]["value"]
         except IndexError:
             return self.values[name]
 
     def __getitem__(self, item : str) -> Union[float, int, bool, NoneType]:
         if not self.quickaccess:
             raise QuickAccessDisabledError("Quickaccess is disabled")
         return self.get_variable(name=item)
 
     def __setitem__(self, item : str, value : Union[float, int, bool, NoneType]):
         if not self.quickaccess:
             raise QuickAccessDisabledError("Quickaccess is disabled")
         self.set_variable(name=item, value=value)
     
-    def receive_new_data(self) -> dict:
+    def receive_new_data(self, first : bool = False) -> dict:
         '''
         Use for receiving new cloud data.
         '''
         data = [json.loads(j) for j in self.websocket.recv().split("\n") if j]
+        changed = [i["name"] for i in data if i["method"] == "set" and i["name"] in self.values]
         self.values.update({i["name"]: i["value"] for i in data if i["method"] == "set"})
         for i in data:
             i.pop("project_id")
             i["var"] = i["name"]
             i["name"] = i["name"].replace("☁ ", "", 1)
-            self.emit_event(i.pop("method"), **i)
+            if not first or i["name"] in changed:
+                self.emit_event(i.pop("method"), **i)
         return self.values
 
     def receive_data(self):
         '''
         Use for receiving cloud data.
         '''
         while True:
             try:
                 self._connect()
-                self.websocket.recv()
+                self.receive_new_data(first=True)
                 break
             except: pass
         while True:
             try:
                 self.receive_new_data()
             except Exception as e:
-                #print(e)
                 while True:
                     try:
                         self._connect()
-                        self.websocket.recv()
+                        self.receive_new_data(first=True)
                         break
                     except: pass
 
     def emit_event(self, event : Union[Literal["set", "delete", "connect", "create"], Event], **entries) -> int:
         '''
         Use for emitting events. Returns how many handlers could handle the event.
         '''
```

### Comparing `scratchcommunication-1.0.2/scratchcommunication/session.py` & `scratchcommunication-1.1.0/scratchcommunication/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import warnings
 from .headers import headers
 from .exceptions import InvalidValueError
-from . import cloud
+from . import cloud, cloud_socket
 import requests, json, re
 
 class Session:
     def __init__(self, username : str = None, *, session_id : str):
         self.session_id = session_id
         self.username = username
         self.headers = headers
         self._login()
+
     def _login(self):
         '''
         Don't use this
         '''
         self.cookies = {
             "scratchcsrftoken" : "a",
             "scratchlanguage" : "en",
@@ -25,14 +26,15 @@
         account = requests.post("https://scratch.mit.edu/session", headers=self.headers, cookies={
             "scratchsessionsid": self.session_id,
             "scratchcsrftoken": "a",
             "scratchlanguage": "en",
         }).json()
         self.xtoken = account["user"]["token"]
         self.headers["X-Token"] = self.xtoken
+
     @classmethod
     def login(cls, username : str, password : str):
         '''
         Login from your username and password.
         '''
         try:
             return cls(
@@ -49,12 +51,19 @@
                     }
                 ).headers["Set-Cookie"]).group())
             )
         except AttributeError:
             raise InvalidValueError("Your login was wrong")
         except Exception as e:
             raise Exception("An error occurred while trying to log in.") from e
+        
     def create_cloudconnection(self, project_id : int, **kwargs) -> cloud.CloudConnection:
         '''
         Create a cloud connection to a project.
         '''
         return cloud.CloudConnection(project_id=project_id, session=self, **kwargs)
+
+    def create_cloud_socket(self, project_id : int, *, packet_size : int = 220):
+        '''
+        Create a cloud socket to a project.
+        '''
+        return cloud_socket.CloudSocket(cloud=self.create_cloudconnection(project_id), packet_size=packet_size)
```

### Comparing `scratchcommunication-1.0.2/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-1.1.0/scratchcommunication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 1.0.2
+Version: 1.1.0
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-1.0.2/setup.py` & `scratchcommunication-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scratchcommunication',
-    version='1.0.2',
+    version='1.1.0',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
     long_description='A python module for communicating with scratch projects',
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/scratchcommunication',
     packages=find_packages(exclude=[]),
@@ -18,11 +18,11 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords=['scratch', 'api'],
     install_requires=[
         'requests',
-        'websocket',
+        'websocket-client',
     ],
     python_requires='>=3.6',
 )
```

