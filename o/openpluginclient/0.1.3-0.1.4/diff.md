# Comparing `tmp/openpluginclient-0.1.3.tar.gz` & `tmp/openpluginclient-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpluginclient-0.1.3.tar", last modified: Tue Jun 27 17:31:19 2023, max compression
+gzip compressed data, was "openpluginclient-0.1.4.tar", last modified: Tue Jun 27 17:40:48 2023, max compression
```

## Comparing `openpluginclient-0.1.3.tar` & `openpluginclient-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/openpluginclient/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/openpluginclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/openpluginclient/openpluginclient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/openpluginclient/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/openpluginclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 17:31:19.000000 openpluginclient-0.1.3/openpluginclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:19.411441 openpluginclient-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-27 17:31:08.000000 openpluginclient-0.1.3/tests/test_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:40:48.754436 openpluginclient-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 17:40:48.754436 openpluginclient-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:40:48.754436 openpluginclient-0.1.4/openpluginclient/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 17:40:37.000000 openpluginclient-0.1.4/openpluginclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-27 17:40:37.000000 openpluginclient-0.1.4/openpluginclient/openpluginclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-06-27 17:40:37.000000 openpluginclient-0.1.4/openpluginclient/plugins.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:40:37.000000 openpluginclient-0.1.4/openpluginclient/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:40:48.754436 openpluginclient-0.1.4/openpluginclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 17:40:48.000000 openpluginclient-0.1.4/openpluginclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-27 17:40:48.000000 openpluginclient-0.1.4/openpluginclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:40:48.000000 openpluginclient-0.1.4/openpluginclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 17:40:48.000000 openpluginclient-0.1.4/openpluginclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 17:40:48.000000 openpluginclient-0.1.4/openpluginclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:40:48.754436 openpluginclient-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-27 17:40:37.000000 openpluginclient-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:40:48.754436 openpluginclient-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:40:37.000000 openpluginclient-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-27 17:40:37.000000 openpluginclient-0.1.4/tests/test_completion.py
```

### Comparing `openpluginclient-0.1.3/PKG-INFO` & `openpluginclient-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openpluginclient
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for accessing ChatGPT plugins via API
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Client for accessing ChatGPT plugins via OpenPlugin API
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openpluginclient-0.1.3/openpluginclient/openpluginclient.py` & `openpluginclient-0.1.4/openpluginclient/openpluginclient.py`

 * *Files identical despite different names*

### Comparing `openpluginclient-0.1.3/openpluginclient.egg-info/PKG-INFO` & `openpluginclient-0.1.4/openpluginclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openpluginclient
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for accessing ChatGPT plugins via API
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Client for accessing ChatGPT plugins via OpenPlugin API
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openpluginclient-0.1.3/setup.py` & `openpluginclient-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openpluginclient', 
-        version="0.1.3",
+        version="0.1.4",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Python package for accessing ChatGPT plugins via API',
         long_description='Client for accessing ChatGPT plugins via OpenPlugin API',
         packages=find_packages(),
         package_data={
-            "openplugin": ["*.json"],  # include all .json files in the openplugin package
+            "openpluginclient": ["*.json"],  # include all .json files in the openplugin package
         },
         exclude=['tests'],
         install_requires=[
             'requests'
         ], # add any additional packages
         
         keywords=[
```

### Comparing `openpluginclient-0.1.3/tests/test_completion.py` & `openpluginclient-0.1.4/tests/test_completion.py`

 * *Files identical despite different names*

