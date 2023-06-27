# Comparing `tmp/automation-utilities-1.3.1.tar.gz` & `tmp/automation-utilities-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.3.1.tar", last modified: Mon Jun 26 16:02:29 2023, max compression
+gzip compressed data, was "automation-utilities-1.3.2.tar", last modified: Tue Jun 27 12:16:58 2023, max compression
```

## Comparing `automation-utilities-1.3.1.tar` & `automation-utilities-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:02:29.955626 automation-utilities-1.3.1/
-drwxrwxrwx   0        0        0        0 2023-06-26 16:02:29.949715 automation-utilities-1.3.1/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-06-26 16:02:29.000000 automation-utilities-1.3.1/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-26 16:02:29.000000 automation-utilities-1.3.1/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:02:29.000000 automation-utilities-1.3.1/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-26 16:02:29.000000 automation-utilities-1.3.1/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-06-26 16:02:29.954618 automation-utilities-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 16:02:29.953274 automation-utilities-1.3.1/automation_utilities/
--rw-rw-rw-   0        0        0     1049 2023-06-26 16:02:27.000000 automation-utilities-1.3.1/automation_utilities/Data.py
--rw-rw-rw-   0        0        0      354 2023-06-26 15:50:11.000000 automation-utilities-1.3.1/automation_utilities/Files.py
--rw-rw-rw-   0        0        0      143 2023-06-26 15:50:11.000000 automation-utilities-1.3.1/automation_utilities/Input.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.1/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-26 16:02:29.955626 automation-utilities-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      248 2023-06-26 16:02:27.000000 automation-utilities-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:58.901688 automation-utilities-1.3.2/
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:58.895540 automation-utilities-1.3.2/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-06-27 12:16:58.000000 automation-utilities-1.3.2/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-27 12:16:58.000000 automation-utilities-1.3.2/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:16:58.000000 automation-utilities-1.3.2/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 12:16:58.000000 automation-utilities-1.3.2/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-06-27 12:16:58.901688 automation-utilities-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:58.899858 automation-utilities-1.3.2/automation_utilities/
+-rw-rw-rw-   0        0        0     1162 2023-06-26 17:51:15.000000 automation-utilities-1.3.2/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 12:14:03.000000 automation-utilities-1.3.2/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0      143 2023-06-26 15:50:11.000000 automation-utilities-1.3.2/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.2/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:16:58.901688 automation-utilities-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      248 2023-06-27 12:15:06.000000 automation-utilities-1.3.2/setup.py
```

### Comparing `automation-utilities-1.3.1/automation_utilities/Data.py` & `automation-utilities-1.3.2/automation_utilities/Data.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,25 +8,28 @@
     lock = threading.Lock()
 
     def __init__(self, file_name: str):
         self.file_name = file_name
         self.data = json.load(open(file_name, 'r'))
         self._privte = 15
 
-    def get(self, key, from_list: list = None):
+    def get(self, key, from_list: list = None, loop: bool = False):
         if isinstance(self.data[key], int):
             Data.lock.acquire()
             self.data[key] += 1
             json.dump(self.data, open(self.file_name, 'w'), indent=2)
             Data.lock.release()
             try:
                 return self.data[key] - 1 if from_list is None else from_list[self.data[key] - 1]
-            except IndexError:
-                self.reset(key)
-                return from_list[self.data[key] - 1]
+            except IndexError as IE:
+                if loop:
+                    self.reset(key)
+                    return from_list[self.data[key] - 1]
+                else:
+                    raise IE
         else:
             return self.data[key]
 
     def reset(self, key):
         self.data[key] = 0
         Data.lock.acquire()
         json.dump(self.data, open(self.file_name, 'w'), indent=2)
```

