# Comparing `tmp/fiftyone_pipeline_engines-4.4.5.tar.gz` & `tmp/fiftyone_pipeline_engines-4.4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiftyone_pipeline_engines-4.4.5.tar", last modified: Fri Feb 17 12:00:44 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_engines-4.4.6.0.tar", last modified: Tue Jun 27 13:33:37 2023, max compression
```

## Comparing `fiftyone_pipeline_engines-4.4.5.tar` & `fiftyone_pipeline_engines-4.4.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines-4.4.5/
--rw-r--r--   0 vsts      (1001) docker     (116)     2651 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines-4.4.5/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2902 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/aspectdata.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2494 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/aspectdata_dictionary.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2111 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/basic_dictionary_cache.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6556 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/datafile.py
--rw-r--r--   0 vsts      (1001) docker     (116)     9974 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/datafile_update_service.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     1938 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/datakeyed_cache.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     4548 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/engine.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1758 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/lru_cache.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1545 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/missingproperty_service.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2146 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/tracker.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     2651 2023-02-17 12:00:43.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)      734 2023-02-17 12:00:43.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2023-02-17 12:00:43.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       43 2023-02-17 12:00:43.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       26 2023-02-17 12:00:43.000000 fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2023-02-17 12:00:44.000000 fiftyone_pipeline_engines-4.4.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     2726 2023-02-17 12:00:32.000000 fiftyone_pipeline_engines-4.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:37.856447 fiftyone_pipeline_engines-4.4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-27 13:33:37.856447 fiftyone_pipeline_engines-4.4.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:37.852447 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2902 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/aspectdata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/aspectdata_dictionary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2111 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/basic_dictionary_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/datafile_update_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1938 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/datakeyed_cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4548 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/missingproperty_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2146 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:37.856447 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-27 13:33:37.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 13:33:37.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:33:37.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 13:33:37.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 13:33:37.000000 fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:33:37.856447 fiftyone_pipeline_engines-4.4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-27 13:33:32.000000 fiftyone_pipeline_engines-4.4.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fiftyone_pipeline_engines-4.4.5/PKG-INFO` & `fiftyone_pipeline_engines-4.4.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_engines
-Version: 4.4.5
+Version: 4.4.6.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package extends the flow element class created by the fiftyone-pipeline-core package into a specialized type of flow element called an engine.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
-Description: # Pipeline Engines
-        
-        ![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Engines**
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
-        ## This package fiftyone_pipeline_engines
-        
-        This package extends the `flow element` class created by the `fiftyone-pipeline-core` package into a specialized type of flow element called an engine. This allows for additional features including:
-        
-        * An auto-updating data file for properties
-        * A service called when a requested property
-        * A caching system and implementation of an LRU (least recently used) cache
-        
-        Engines created by 51Degrees:
-        
-        - [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
-        - [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
-        
-        ## Requirements 
-        
-        * Python 3.5+
-        * The gitversion lib using `python -m pip install gitversion`
-        
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
+# Pipeline Engines
+
+![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Engines**
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
+## This package fiftyone_pipeline_engines
+
+This package extends the `flow element` class created by the `fiftyone-pipeline-core` package into a specialized type of flow element called an engine. This allows for additional features including:
+
+* An auto-updating data file for properties
+* A service called when a requested property
+* A caching system and implementation of an LRU (least recently used) cache
+
+Engines created by 51Degrees:
+
+- [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
+- [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
+
+## Requirements 
+
+* Python 3.5+
+* The gitversion lib using `python -m pip install gitversion`
+
+
+
```

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/aspectdata.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/aspectdata.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/aspectdata_dictionary.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/aspectdata_dictionary.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/basic_dictionary_cache.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/basic_dictionary_cache.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/datafile.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/datafile.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/datafile_update_service.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/datafile_update_service.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/datakeyed_cache.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/datakeyed_cache.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/engine.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/engine.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/lru_cache.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/lru_cache.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/missingproperty_service.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/missingproperty_service.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines/tracker.py` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines/tracker.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines.egg-info/PKG-INFO` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-engines
-Version: 4.4.5
+Version: 4.4.6.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package extends the flow element class created by the fiftyone-pipeline-core package into a specialized type of flow element called an engine.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
-Description: # Pipeline Engines
-        
-        ![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Engines**
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
-        ## This package fiftyone_pipeline_engines
-        
-        This package extends the `flow element` class created by the `fiftyone-pipeline-core` package into a specialized type of flow element called an engine. This allows for additional features including:
-        
-        * An auto-updating data file for properties
-        * A service called when a requested property
-        * A caching system and implementation of an LRU (least recently used) cache
-        
-        Engines created by 51Degrees:
-        
-        - [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
-        - [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
-        
-        ## Requirements 
-        
-        * Python 3.5+
-        * The gitversion lib using `python -m pip install gitversion`
-        
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
+# Pipeline Engines
+
+![51Degrees](https://51degrees.com/DesktopModules/FiftyOne/Distributor/Logo.ashx?utm_source=github&utm_medium=repository&utm_content=readme_main&utm_campaign=python-open-source "Data rewards the curious") **Python Pipeline Engines**
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
+## This package fiftyone_pipeline_engines
+
+This package extends the `flow element` class created by the `fiftyone-pipeline-core` package into a specialized type of flow element called an engine. This allows for additional features including:
+
+* An auto-updating data file for properties
+* A service called when a requested property
+* A caching system and implementation of an LRU (least recently used) cache
+
+Engines created by 51Degrees:
+
+- [**fiftyone_devicedetection**](https://pypi.org/project/fiftyone-devicedetection/) - Get details about the devices accessing your web page
+- [**fiftyone_location**](https://pypi.org/project/fiftyone-location/) - Get postal address details from the location of devices accessing your web page
+
+## Requirements 
+
+* Python 3.5+
+* The gitversion lib using `python -m pip install gitversion`
+
+
+
```

### Comparing `fiftyone_pipeline_engines-4.4.5/fiftyone_pipeline_engines.egg-info/SOURCES.txt` & `fiftyone_pipeline_engines-4.4.6.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.5/setup.py` & `fiftyone_pipeline_engines-4.4.6.0/setup.py`

 * *Files identical despite different names*

