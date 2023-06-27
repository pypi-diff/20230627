# Comparing `tmp/automation-utilities-1.3.2.tar.gz` & `tmp/automation-utilities-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.3.2.tar", last modified: Tue Jun 27 12:16:58 2023, max compression
+gzip compressed data, was "automation-utilities-1.3.3.tar", last modified: Tue Jun 27 20:35:23 2023, max compression
```

## Comparing `automation-utilities-1.3.2.tar` & `automation-utilities-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:16:58.901688 automation-utilities-1.3.2/
-drwxrwxrwx   0        0        0        0 2023-06-27 12:16:58.895540 automation-utilities-1.3.2/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-06-27 12:16:58.000000 automation-utilities-1.3.2/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-27 12:16:58.000000 automation-utilities-1.3.2/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:16:58.000000 automation-utilities-1.3.2/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 12:16:58.000000 automation-utilities-1.3.2/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-06-27 12:16:58.901688 automation-utilities-1.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 12:16:58.899858 automation-utilities-1.3.2/automation_utilities/
--rw-rw-rw-   0        0        0     1162 2023-06-26 17:51:15.000000 automation-utilities-1.3.2/automation_utilities/Data.py
--rw-rw-rw-   0        0        0      590 2023-06-27 12:14:03.000000 automation-utilities-1.3.2/automation_utilities/Files.py
--rw-rw-rw-   0        0        0      143 2023-06-26 15:50:11.000000 automation-utilities-1.3.2/automation_utilities/Input.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.2/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-27 12:16:58.901688 automation-utilities-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      248 2023-06-27 12:15:06.000000 automation-utilities-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:35:23.042883 automation-utilities-1.3.3/
+drwxrwxrwx   0        0        0        0 2023-06-27 20:35:23.040890 automation-utilities-1.3.3/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-06-27 20:35:23.041883 automation-utilities-1.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 20:35:23.035724 automation-utilities-1.3.3/automation_utilities/
+-rw-rw-rw-   0        0        0     1237 2023-06-27 18:45:24.000000 automation-utilities-1.3.3/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 12:14:03.000000 automation-utilities-1.3.3/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0      143 2023-06-26 15:50:11.000000 automation-utilities-1.3.3/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.3/automation_utilities/PhoneNumbers.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.3/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 20:35:23.042883 automation-utilities-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-06-27 20:35:21.000000 automation-utilities-1.3.3/setup.py
```

### Comparing `automation-utilities-1.3.2/automation_utilities/Data.py` & `automation-utilities-1.3.3/automation_utilities/Data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import json
 import threading
 
 
 class Data:
-    """This class was made to deal with data used in automation projects"""
-
     lock = threading.Lock()
 
     def __init__(self, file_name: str):
         self.file_name = file_name
-        self.data = json.load(open(file_name, 'r'))
+        try:
+            self.data = json.load(open(file_name, 'r'))
+        except FileNotFoundError:
+            self.data = {}
         self._privte = 15
 
     def get(self, key, from_list: list = None, loop: bool = False):
+        if key not in self.data.keys():
+            self.data[key] = 0
         if isinstance(self.data[key], int):
             Data.lock.acquire()
             self.data[key] += 1
             json.dump(self.data, open(self.file_name, 'w'), indent=2)
             Data.lock.release()
             try:
                 return self.data[key] - 1 if from_list is None else from_list[self.data[key] - 1]
```

### Comparing `automation-utilities-1.3.2/automation_utilities/Files.py` & `automation-utilities-1.3.3/automation_utilities/Files.py`

 * *Files identical despite different names*

