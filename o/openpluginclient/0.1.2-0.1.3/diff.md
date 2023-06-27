# Comparing `tmp/openpluginclient-0.1.2.tar.gz` & `tmp/openpluginclient-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpluginclient-0.1.2.tar", last modified: Tue Jun 27 16:45:23 2023, max compression
+gzip compressed data, was "openpluginclient-0.1.3.tar", last modified: Tue Jun 27 17:31:19 2023, max compression
```

## Comparing `openpluginclient-0.1.2.tar` & `openpluginclient-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:23.585126 openpluginclient-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 16:45:23.585126 openpluginclient-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:23.581125 openpluginclient-0.1.2/openpluginclient/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 16:45:10.000000 openpluginclient-0.1.2/openpluginclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-27 16:45:10.000000 openpluginclient-0.1.2/openpluginclient/openpluginclient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:10.000000 openpluginclient-0.1.2/openpluginclient/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:23.585126 openpluginclient-0.1.2/openpluginclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 16:45:23.000000 openpluginclient-0.1.2/openpluginclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-27 16:45:23.000000 openpluginclient-0.1.2/openpluginclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:45:23.000000 openpluginclient-0.1.2/openpluginclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 16:45:23.000000 openpluginclient-0.1.2/openpluginclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:45:23.000000 openpluginclient-0.1.2/openpluginclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 16:45:23.585126 openpluginclient-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 16:45:10.000000 openpluginclient-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:23.585126 openpluginclient-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:10.000000 openpluginclient-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-27 16:45:10.000000 openpluginclient-0.1.2/tests/test_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/openpluginclient/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/openpluginclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/openpluginclient/openpluginclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/openpluginclient/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/openpluginclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/tests/test_completion.py
```

### Comparing `openpluginclient-0.1.2/PKG-INFO` & `openpluginclient-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openpluginclient
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for accessing ChatGPT plugins via API
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Client for accessing ChatGPT plugins via OpenPlugin API
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openpluginclient-0.1.2/openpluginclient/openpluginclient.py` & `openpluginclient-0.1.3/openpluginclient/openpluginclient.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import json
 import requests
 import os
+from pathlib import Path
 
 SUPPORTED_MODELS = ["gpt-4-0613", "gpt-3.5-turbo-0613"]
 DEVELOPMENT = False
 if (os.getenv("DEVELOPMENT") == "true"):
     DEVELOPMENT = True
 
 def get_supported_plugins():
-    current_dir = os.getcwd()
-    print("current_dir", current_dir)
-    file_path = os.path.join(current_dir, 'pypi-client', 'openpluginclient', 'plugins.json')
-    print("file_path", file_path)
+    file_path = Path(__file__).parent / "plugins.json"
     with open(file_path, 'r') as f:
         return json.load(f)
 
 def openplugin_completion(early_access_token: str, plugin_name: str = None, fail_silently: bool = False, **chatgpt_args):
     # Ensure an early access token is provided.
     if not early_access_token:
         raise ValueError(f"An early access token must be provided.")
```

### Comparing `openpluginclient-0.1.2/openpluginclient.egg-info/PKG-INFO` & `openpluginclient-0.1.3/openpluginclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openpluginclient
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for accessing ChatGPT plugins via API
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Client for accessing ChatGPT plugins via OpenPlugin API
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openpluginclient-0.1.2/setup.py` & `openpluginclient-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openpluginclient', 
-        version="0.1.2",
+        version="0.1.3",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Python package for accessing ChatGPT plugins via API',
         long_description='Client for accessing ChatGPT plugins via OpenPlugin API',
         packages=find_packages(),
         package_data={
             "openplugin": ["*.json"],  # include all .json files in the openplugin package
```

### Comparing `openpluginclient-0.1.2/tests/test_completion.py` & `openpluginclient-0.1.3/tests/test_completion.py`

 * *Files identical despite different names*

