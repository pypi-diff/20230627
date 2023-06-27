# Comparing `tmp/fiftyone_pipeline_core-4.4.5.tar.gz` & `tmp/fiftyone_pipeline_core-4.4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiftyone_pipeline_core-4.4.5.tar", last modified: Fri Feb 17 12:00:43 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_core-4.4.6.0.tar", last modified: Tue Jun 27 13:33:37 2023, max compression
```

## Comparing `fiftyone_pipeline_core-4.4.5.tar` & `fiftyone_pipeline_core-4.4.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/
--rw-r--r--   0 vsts      (1001) docker     (116)       59 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (116)     2920 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/
--rw-r--r--   0 vsts      (1001) docker     (116)    16980 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/JavaScriptResource.mustache
--rwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2869 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/aspectproperty_value.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2078 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     3433 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/elementdata.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2600 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/elementdata_dictionary.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     3011 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/evidence.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2427 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/evidence_keyfilter.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     8094 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/flowdata.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     4770 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/flowelement.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1726 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/flowerror.py
--rw-r--r--   0 vsts      (1001) docker     (116)     7413 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/javascriptbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (116)     7438 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/jsonbundler.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     3046 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/logger.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2170 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/messages.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     5057 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/pipeline.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     6440 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/pipelinebuilder.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3009 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/sequenceelement.py
--rw-r--r--   0 vsts      (1001) docker     (116)     8565 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/setheaderelement.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2934 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/web.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     2920 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)     1055 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       14 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       23 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2023-02-17 12:00:43.000000 fiftyone_pipeline_core-4.4.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     2797 2023-02-17 12:00:32.000000 fiftyone_pipeline_core-4.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:37.648442 fiftyone_pipeline_core-4.4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-27 13:33:37.648442 fiftyone_pipeline_core-4.4.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:37.644442 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/JavaScriptResource.mustache
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/aspectproperty_value.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3433 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/elementdata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/elementdata_dictionary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3011 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/evidence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2427 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/evidence_keyfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8094 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/flowdata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4770 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/flowelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/flowerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/javascriptbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/jsonbundler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/messages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5057 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6440 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/pipelinebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/sequenceelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/setheaderelement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2934 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:37.648442 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-27 13:33:37.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-27 13:33:37.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:33:37.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 13:33:37.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 13:33:37.000000 fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:33:37.648442 fiftyone_pipeline_core-4.4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-27 13:33:32.000000 fiftyone_pipeline_core-4.4.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fiftyone_pipeline_core-4.4.5/PKG-INFO` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
-Name: fiftyone_pipeline_core
-Version: 4.4.5
+Name: fiftyone-pipeline-core
+Version: 4.4.6.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package definds the essential components of the Pipeline API such as flow elements, flow data and evidence. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
-Description: # Pipeline Core
-        
-        ![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Core**
-        
-        [Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
-        
-        ## Introduction
-        
-        The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
-        
-        ## This package fiftyone_pipeline_core
-        
-        This package defines the essential components of the Pipeline API such as `flow elements`, `flow data` and `evidence`. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
-        
-        It can be used on its own or with the following additional packages.
-        
-        - **fiftyone_pipeline_engines** - Adds a specialized type of flow element called an engine which allows for additional features including an auto-updating data file for properties, a service called when a requested property is missing and a caching system.
-        
-        Engines created by 51Degrees:
-        
-        - [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
-        - [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
-        
-        ## Requirements
-        
-        * Python 3.5+
-        * The `flask` python library to run the web examples 
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# Pipeline Core
+
+![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Core**
+
+[Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
+
+## Introduction
+
+The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
+
+## This package fiftyone_pipeline_core
+
+This package defines the essential components of the Pipeline API such as `flow elements`, `flow data` and `evidence`. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
+
+It can be used on its own or with the following additional packages.
+
+- **fiftyone_pipeline_engines** - Adds a specialized type of flow element called an engine which allows for additional features including an auto-updating data file for properties, a service called when a requested property is missing and a caching system.
+
+Engines created by 51Degrees:
+
+- [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
+- [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
+
+## Requirements
+
+* Python 3.5+
+* The `flask` python library to run the web examples 
+
+
```

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/JavaScriptResource.mustache` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/JavaScriptResource.mustache`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/aspectproperty_value.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/aspectproperty_value.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/elementdata.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/elementdata.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/elementdata_dictionary.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/elementdata_dictionary.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/evidence.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/evidence.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/evidence_keyfilter.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/evidence_keyfilter.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/flowdata.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/flowdata.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/flowelement.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/flowelement.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/flowerror.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/flowerror.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/javascriptbuilder.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/javascriptbuilder.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/jsonbundler.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/jsonbundler.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/logger.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/logger.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/messages.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/messages.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/pipeline.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/pipeline.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/pipelinebuilder.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/pipelinebuilder.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/sequenceelement.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/sequenceelement.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/setheaderelement.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/setheaderelement.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core/web.py` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core/web.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core.egg-info/PKG-INFO` & `fiftyone_pipeline_core-4.4.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
-Name: fiftyone-pipeline-core
-Version: 4.4.5
+Name: fiftyone_pipeline_core
+Version: 4.4.6.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package definds the essential components of the Pipeline API such as flow elements, flow data and evidence. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
-Description: # Pipeline Core
-        
-        ![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Core**
-        
-        [Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
-        
-        ## Introduction
-        
-        The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
-        
-        ## This package fiftyone_pipeline_core
-        
-        This package defines the essential components of the Pipeline API such as `flow elements`, `flow data` and `evidence`. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
-        
-        It can be used on its own or with the following additional packages.
-        
-        - **fiftyone_pipeline_engines** - Adds a specialized type of flow element called an engine which allows for additional features including an auto-updating data file for properties, a service called when a requested property is missing and a caching system.
-        
-        Engines created by 51Degrees:
-        
-        - [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
-        - [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
-        
-        ## Requirements
-        
-        * Python 3.5+
-        * The `flask` python library to run the web examples 
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# Pipeline Core
+
+![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Core**
+
+[Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
+
+## Introduction
+
+The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
+
+## This package fiftyone_pipeline_core
+
+This package defines the essential components of the Pipeline API such as `flow elements`, `flow data` and `evidence`. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
+
+It can be used on its own or with the following additional packages.
+
+- **fiftyone_pipeline_engines** - Adds a specialized type of flow element called an engine which allows for additional features including an auto-updating data file for properties, a service called when a requested property is missing and a caching system.
+
+Engines created by 51Degrees:
+
+- [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
+- [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
+
+## Requirements
+
+* Python 3.5+
+* The `flask` python library to run the web examples 
+
+
```

### Comparing `fiftyone_pipeline_core-4.4.5/fiftyone_pipeline_core.egg-info/SOURCES.txt` & `fiftyone_pipeline_core-4.4.6.0/fiftyone_pipeline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.5/setup.py` & `fiftyone_pipeline_core-4.4.6.0/setup.py`

 * *Files identical despite different names*

