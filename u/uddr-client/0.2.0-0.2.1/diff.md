# Comparing `tmp/uddr_client-0.2.0.tar.gz` & `tmp/uddr_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uddr_client-0.2.0.tar", last modified: Thu Jun 22 21:58:34 2023, max compression
+gzip compressed data, was "uddr_client-0.2.1.tar", last modified: Tue Jun 27 21:34:45 2023, max compression
```

## Comparing `uddr_client-0.2.0.tar` & `uddr_client-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.824825 uddr_client-0.2.0/
--rw-r--r--   0 shane     (1000) shane     (1000)     1071 2023-06-14 04:19:49.000000 uddr_client-0.2.0/LICENSE.md
--rw-r--r--   0 shane     (1000) shane     (1000)     4191 2023-06-22 21:58:34.824825 uddr_client-0.2.0/PKG-INFO
--rw-r--r--   0 shane     (1000) shane     (1000)     3576 2023-06-22 21:56:00.000000 uddr_client-0.2.0/README.md
--rw-r--r--   0 shane     (1000) shane     (1000)       38 2023-06-22 21:58:34.824825 uddr_client-0.2.0/setup.cfg
--rw-r--r--   0 shane     (1000) shane     (1000)      948 2023-06-22 21:58:18.000000 uddr_client-0.2.0/setup.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/uddr_client/
--rw-r--r--   0 shane     (1000) shane     (1000)       37 2023-06-09 19:52:19.000000 uddr_client-0.2.0/src/uddr_client/__init__.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/uddr_client/api/
--rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/api/__init__.py
--rw-r--r--   0 shane     (1000) shane     (1000)    18903 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/api/api_client.py
--rw-r--r--   0 shane     (1000) shane     (1000)     2593 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/client.py
--rw-r--r--   0 shane     (1000) shane     (1000)     3065 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/connection.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/uddr_client/doh/
--rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/doh/__init__.py
--rw-r--r--   0 shane     (1000) shane     (1000)     4886 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/doh/doh_client.py
--rw-r--r--   0 shane     (1000) shane     (1000)     1062 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/doh/ioc_parser.py
--rw-r--r--   0 shane     (1000) shane     (1000)     1481 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/response.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/uddr_client.egg-info/
--rw-r--r--   0 shane     (1000) shane     (1000)     4191 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/PKG-INFO
--rw-r--r--   0 shane     (1000) shane     (1000)      501 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/SOURCES.txt
--rw-r--r--   0 shane     (1000) shane     (1000)        1 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/dependency_links.txt
--rw-r--r--   0 shane     (1000) shane     (1000)       53 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/requires.txt
--rw-r--r--   0 shane     (1000) shane     (1000)       12 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/top_level.txt
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-27 21:34:45.946167 uddr_client-0.2.1/
+-rw-r--r--   0 shane     (1000) shane     (1000)     1071 2023-06-14 04:19:49.000000 uddr_client-0.2.1/LICENSE.md
+-rw-r--r--   0 shane     (1000) shane     (1000)     4191 2023-06-27 21:34:45.946167 uddr_client-0.2.1/PKG-INFO
+-rw-r--r--   0 shane     (1000) shane     (1000)     3576 2023-06-22 21:56:00.000000 uddr_client-0.2.1/README.md
+-rw-r--r--   0 shane     (1000) shane     (1000)       38 2023-06-27 21:34:45.946167 uddr_client-0.2.1/setup.cfg
+-rw-r--r--   0 shane     (1000) shane     (1000)      952 2023-06-27 21:32:58.000000 uddr_client-0.2.1/setup.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-27 21:34:45.936167 uddr_client-0.2.1/src/
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-27 21:34:45.936167 uddr_client-0.2.1/src/uddr_client/
+-rw-r--r--   0 shane     (1000) shane     (1000)       37 2023-06-09 19:52:19.000000 uddr_client-0.2.1/src/uddr_client/__init__.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-27 21:34:45.936167 uddr_client-0.2.1/src/uddr_client/api/
+-rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.1/src/uddr_client/api/__init__.py
+-rw-r--r--   0 shane     (1000) shane     (1000)    18903 2023-06-22 21:56:00.000000 uddr_client-0.2.1/src/uddr_client/api/api_client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     2593 2023-06-22 21:56:00.000000 uddr_client-0.2.1/src/uddr_client/client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     3065 2023-06-22 21:56:00.000000 uddr_client-0.2.1/src/uddr_client/connection.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-27 21:34:45.946167 uddr_client-0.2.1/src/uddr_client/doh/
+-rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.1/src/uddr_client/doh/__init__.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     4886 2023-06-22 21:56:00.000000 uddr_client-0.2.1/src/uddr_client/doh/doh_client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     1909 2023-06-27 21:27:27.000000 uddr_client-0.2.1/src/uddr_client/doh/ioc_parser.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     1481 2023-06-22 21:56:00.000000 uddr_client-0.2.1/src/uddr_client/response.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-27 21:34:45.936167 uddr_client-0.2.1/src/uddr_client.egg-info/
+-rw-r--r--   0 shane     (1000) shane     (1000)     4191 2023-06-27 21:34:45.000000 uddr_client-0.2.1/src/uddr_client.egg-info/PKG-INFO
+-rw-r--r--   0 shane     (1000) shane     (1000)      501 2023-06-27 21:34:45.000000 uddr_client-0.2.1/src/uddr_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)        1 2023-06-27 21:34:45.000000 uddr_client-0.2.1/src/uddr_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)       53 2023-06-27 21:34:45.000000 uddr_client-0.2.1/src/uddr_client.egg-info/requires.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)       12 2023-06-27 21:34:45.000000 uddr_client-0.2.1/src/uddr_client.egg-info/top_level.txt
```

### Comparing `uddr_client-0.2.0/LICENSE.md` & `uddr_client-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.0/PKG-INFO` & `uddr_client-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uddr_client
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python client for the UDDR API.
 Home-page: https://github.com/sbarbett/uddr_client
 Author: Shane Barbetta
 Author-email: shane@barbetta.me
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `uddr_client-0.2.0/README.md` & `uddr_client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.0/setup.py` & `uddr_client-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="uddr_client", 
-    version="0.2.0",  
+    version="0.2.1",  
     description="A Python client for the UDDR API.", 
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown', 
     author="Shane Barbetta", 
     author_email="shane@barbetta.me",  
     url="https://github.com/sbarbett/uddr_client", 
     license="MIT", 
@@ -20,10 +20,10 @@
     ],
     package_dir={"": "src"},  
     packages=find_packages(where="src"),  
     python_requires=">=3.7", 
     install_requires=[
         "pandas>=2.0.2",
         "xmltodict>=0.13.0",
-	"python-decouple>=3.8",
+	    "python-decouple>=3.8",
     ],
 )
```

### Comparing `uddr_client-0.2.0/src/uddr_client/api/api_client.py` & `uddr_client-0.2.1/src/uddr_client/api/api_client.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.0/src/uddr_client/client.py` & `uddr_client-0.2.1/src/uddr_client/client.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.0/src/uddr_client/connection.py` & `uddr_client-0.2.1/src/uddr_client/connection.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.0/src/uddr_client/doh/doh_client.py` & `uddr_client-0.2.1/src/uddr_client/doh/doh_client.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.0/src/uddr_client/response.py` & `uddr_client-0.2.1/src/uddr_client/response.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.0/src/uddr_client.egg-info/PKG-INFO` & `uddr_client-0.2.1/src/uddr_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uddr-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python client for the UDDR API.
 Home-page: https://github.com/sbarbett/uddr_client
 Author: Shane Barbetta
 Author-email: shane@barbetta.me
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

