# Comparing `tmp/impulsePy-3.0.0.tar.gz` & `tmp/impulsePy-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\impulsePy-3.0.0.tar", last modified: Thu Jun 22 07:48:57 2023, max compression
+gzip compressed data, was "dist\impulsePy-3.1.0.tar", last modified: Tue Jun 27 06:54:24 2023, max compression
```

## Comparing `impulsePy-3.0.0.tar` & `impulsePy-3.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:48:57.000000 impulsePy-3.0.0/
--rw-rw-rw-   0        0        0      740 2023-06-22 07:48:57.000000 impulsePy-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-22 07:40:36.000000 impulsePy-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy/
--rw-rw-rw-   0        0        0    21363 2023-06-22 07:37:13.000000 impulsePy-3.0.0/impulsePy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/
--rw-rw-rw-   0        0        0      740 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 07:48:57.000000 impulsePy-3.0.0/impulsePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 07:48:57.000000 impulsePy-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-06-22 07:38:30.000000 impulsePy-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:54:24.000000 impulsePy-3.1.0/
+-rw-rw-rw-   0        0        0      774 2023-06-27 06:54:24.000000 impulsePy-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-27 06:51:36.000000 impulsePy-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 06:54:24.000000 impulsePy-3.1.0/impulsePy/
+-rw-rw-rw-   0        0        0    21701 2023-06-27 06:43:22.000000 impulsePy-3.1.0/impulsePy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:54:24.000000 impulsePy-3.1.0/impulsePy.egg-info/
+-rw-rw-rw-   0        0        0      774 2023-06-27 06:54:24.000000 impulsePy-3.1.0/impulsePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-27 06:54:24.000000 impulsePy-3.1.0/impulsePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 06:54:24.000000 impulsePy-3.1.0/impulsePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 06:54:24.000000 impulsePy-3.1.0/impulsePy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 06:54:24.000000 impulsePy-3.1.0/impulsePy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 06:54:24.000000 impulsePy-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-06-27 06:51:12.000000 impulsePy-3.1.0/setup.py
```

### Comparing `impulsePy-3.0.0/PKG-INFO` & `impulsePy-3.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: impulsePy
-Version: 3.0.0
+Version: 3.1.0
 Summary: Library for controlling Impulse
 Home-page: UNKNOWN
 Author: DENSsolutions
 Author-email: merijn.pen@DENSsolutions.com
 License: UNKNOWN
 Description: # impulsePy
         
         This python library is compatible with Impulse version 1.4 and earlier.
         The module offers real-time access to all data from Impulse controlled devices.
         It offers controls for:
-        - Heat
+        - Heat (normal heating & liquid heating)
         - Bias
         - Gas
         - Liquid
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `impulsePy-3.0.0/impulsePy/__init__.py` & `impulsePy-3.1.0/impulsePy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import logging
 import os
 from time import sleep
 
 _logger = logging.getLogger(__name__)
 
-version = "3.0.0" # Added LSS controls and data
+version = "3.1.0" # Added LSS controls and data, including line control
 
 controlEndpoint = "tcp://127.0.0.1:5557"
 dataEndpoint = "tcp://127.0.0.1:5556"
 
 profilesPath = os.path.expanduser('~\\Documents\\Impulse\\Profiles\\')
 profilesPath = profilesPath.replace("\\","/")
 
@@ -350,51 +350,61 @@
         return returnMessage["resultCode"]
 
 class liquid():
     def __init__(self):
         self.stimulus = 'liquid'
         self.data = device(self.stimulus)
         
-    def setHumidity(self, setPoint):
-        controlDict = {
-            '$type': 'control.liquid.v2.setHumidity',
-            'humidity': setPoint
-        }
-        resultCode = sendControl(controlDict)['resultCode']
-        return resultCode
-
+    #v0 and v1 commands (LSS)
     def setPF(self, version, outletPressure, flow):
         controlDict = {
             '$type': 'control.liquid.'+version+'.pressureFlow.apply',
             'flow': flow,
             'outletPressure': outletPressure
         }            
         resultCode = sendControl(controlDict)['resultCode']
         return resultCode
-    
-    def setPFC(self, version, outletPressure, flow, concentration):
+
+    def setIOP(self, version, inletPressure, outletPressure):
+        controlDict = {
+            '$type': 'control.liquid.'+version+'.inletOutletPressure.apply',
+            'inletPressure1': inletPressure,
+            'outletPressure': outletPressure
+        }        
+        resultCode = sendControl(controlDict)['resultCode']
+        return resultCode
+
+    #v2 commands (LSS advanced)
+    def setHumidity(self, setPoint):
+        controlDict = {
+            '$type': 'control.liquid.v2.setHumidity',
+            'humidity': setPoint
+        }
+        resultCode = sendControl(controlDict)['resultCode']
+        return resultCode
+   
+    def setPFC(self, outletPressure, flow, concentration):
         controlDict = {
             '$type': 'control.liquid.v2.pressureFlow.apply',
             'flow': flow,
             'concentration': concentration,
             'outletPressure': outletPressure
         }       
         resultCode = sendControl(controlDict)['resultCode']
         return resultCode
-    
-    def setIOP(self, version, inletPressure, outletPressure):
+ 
+    def setLine(self, line):
         controlDict = {
-            '$type': 'control.liquid.'+version+'.inletOutletPressure.apply',
-            'inletPressure1': inletPressure,
-            'outletPressure': outletPressure
-        }        
+            '$type': 'control.liquid.setLine',
+            'line': line # possible values: liquid, gas
+        }       
         resultCode = sendControl(controlDict)['resultCode']
         return resultCode
-
-    def setI2OP(self, version, inletPressure1, inletPressure2, outletPressure):
+    
+    def setI2OP(self, inletPressure1, inletPressure2, outletPressure):
         controlDict = {
             '$type': 'control.liquid.v2.inletOutletPressure.apply',
             'inletPressure1': inletPressure1,
             'inletPressure2': inletPressure2,
             'outletPressure': outletPressure
         }        
         resultCode = sendControl(controlDict)['resultCode']
```

### Comparing `impulsePy-3.0.0/impulsePy.egg-info/PKG-INFO` & `impulsePy-3.1.0/impulsePy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: impulsePy
-Version: 3.0.0
+Version: 3.1.0
 Summary: Library for controlling Impulse
 Home-page: UNKNOWN
 Author: DENSsolutions
 Author-email: merijn.pen@DENSsolutions.com
 License: UNKNOWN
 Description: # impulsePy
         
         This python library is compatible with Impulse version 1.4 and earlier.
         The module offers real-time access to all data from Impulse controlled devices.
         It offers controls for:
-        - Heat
+        - Heat (normal heating & liquid heating)
         - Bias
         - Gas
         - Liquid
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `impulsePy-3.0.0/setup.py` & `impulsePy-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impulsePy", # Replace with your own username
-    version="3.0.0",
+    version="3.1.0",
     author="DENSsolutions",
     author_email="merijn.pen@DENSsolutions.com",
     description="Library for controlling Impulse",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

