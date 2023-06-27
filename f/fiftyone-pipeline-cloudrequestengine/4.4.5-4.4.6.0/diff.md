# Comparing `tmp/fiftyone_pipeline_cloudrequestengine-4.4.5.tar.gz` & `tmp/fiftyone_pipeline_cloudrequestengine-4.4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiftyone_pipeline_cloudrequestengine-4.4.5.tar", last modified: Fri Feb 17 12:00:43 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_cloudrequestengine-4.4.6.0.tar", last modified: Tue Jun 27 13:33:38 2023, max compression
```

## Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5.tar` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/
--rw-r--r--   0 vsts      (1001) docker     (116)     2591 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2452 2023-02-17 12:00:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/clouddata.py
--rw-r--r--   0 vsts      (1001) docker     (116)     5107 2023-02-17 12:00:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/cloudengine.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)    14180 2023-02-17 12:00:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1923 2023-02-17 12:00:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2770 2023-02-17 12:00:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/constants.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1345 2023-02-17 12:00:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/requestclient.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     2591 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)      683 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       35 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       37 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2023-02-17 12:00:43.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     2724 2023-02-17 12:00:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:38.244444 fiftyone_pipeline_cloudrequestengine-4.4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-27 13:33:38.244444 fiftyone_pipeline_cloudrequestengine-4.4.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:38.244444 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-27 13:33:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/clouddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-27 13:33:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14180 2023-06-27 13:33:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-27 13:33:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-27 13:33:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-27 13:33:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/requestclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:38.244444 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-27 13:33:38.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-27 13:33:38.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:33:38.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 13:33:38.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 13:33:38.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:33:38.244444 fiftyone_pipeline_cloudrequestengine-4.4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-27 13:33:32.000000 fiftyone_pipeline_cloudrequestengine-4.4.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/PKG-INFO` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_cloudrequestengine
-Version: 4.4.5
+Version: 4.4.6.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package extends the flow element class created by the fiftyone-pipeline-core package into a specialized type of flow element called an engine.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
-Description: # Cloud Request Engine
-        
-        ![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Cloud Request Engine**
-        
-        [Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
-        
-        ## Introduction
-        
-        The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
-        
-        ## Requirements
-        
-        * Python 3.5+
-        
-        ## This package fiftyone_pipeline_cloudrequestengine
-        
-        This package uses the `engines` class created by the `fiftyone-pipeline-engines`. It makes available:
-        
-        * A `Cloud Request Engine` which calls the 51Degrees cloud service to fetch properties and metadata about them based on a provided resource key. Get a resource key at https://configure.51degrees.com/
-        * A `Cloud Engine` template which reads data from the Cloud Request Engine.
-        
-        It is used by the cloud versions of the following 51Degrees engines:
-        
-        - [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
-        - [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
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
+# Cloud Request Engine
+
+![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Cloud Request Engine**
+
+[Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
+
+## Introduction
+
+The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
+
+## Requirements
+
+* Python 3.5+
+
+## This package fiftyone_pipeline_cloudrequestengine
+
+This package uses the `engines` class created by the `fiftyone-pipeline-engines`. It makes available:
+
+* A `Cloud Request Engine` which calls the 51Degrees cloud service to fetch properties and metadata about them based on a provided resource key. Get a resource key at https://configure.51degrees.com/
+* A `Cloud Engine` template which reads data from the Cloud Request Engine.
+
+It is used by the cloud versions of the following 51Degrees engines:
+
+- [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
+- [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
+
+
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/clouddata.py` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/clouddata.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/cloudengine.py` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/constants.py` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/constants.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine/requestclient.py` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine/requestclient.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-cloudrequestengine
-Version: 4.4.5
+Version: 4.4.6.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package extends the flow element class created by the fiftyone-pipeline-core package into a specialized type of flow element called an engine.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
-Description: # Cloud Request Engine
-        
-        ![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Cloud Request Engine**
-        
-        [Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
-        
-        ## Introduction
-        
-        The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
-        
-        ## Requirements
-        
-        * Python 3.5+
-        
-        ## This package fiftyone_pipeline_cloudrequestengine
-        
-        This package uses the `engines` class created by the `fiftyone-pipeline-engines`. It makes available:
-        
-        * A `Cloud Request Engine` which calls the 51Degrees cloud service to fetch properties and metadata about them based on a provided resource key. Get a resource key at https://configure.51degrees.com/
-        * A `Cloud Engine` template which reads data from the Cloud Request Engine.
-        
-        It is used by the cloud versions of the following 51Degrees engines:
-        
-        - [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
-        - [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
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
+# Cloud Request Engine
+
+![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Cloud Request Engine**
+
+[Developer Documentation](https://51degrees.com/pipeline-python/index.html?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Developer Documentation")
+
+## Introduction
+
+The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines) 
+
+## Requirements
+
+* Python 3.5+
+
+## This package fiftyone_pipeline_cloudrequestengine
+
+This package uses the `engines` class created by the `fiftyone-pipeline-engines`. It makes available:
+
+* A `Cloud Request Engine` which calls the 51Degrees cloud service to fetch properties and metadata about them based on a provided resource key. Get a resource key at https://configure.51degrees.com/
+* A `Cloud Engine` template which reads data from the Cloud Request Engine.
+
+It is used by the cloud versions of the following 51Degrees engines:
+
+- [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
+- [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
+
+
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.5/setup.py` & `fiftyone_pipeline_cloudrequestengine-4.4.6.0/setup.py`

 * *Files identical despite different names*

