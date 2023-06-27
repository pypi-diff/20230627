# Comparing `tmp/Adobe_Lib_Manual-4.0.tar.gz` & `tmp/Adobe_Lib_Manual-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Adobe_Lib_Manual-4.0.tar", last modified: Tue Jun 27 18:13:18 2023, max compression
+gzip compressed data, was "Adobe_Lib_Manual-4.1.tar", last modified: Tue Jun 27 18:23:51 2023, max compression
```

## Comparing `Adobe_Lib_Manual-4.0.tar` & `Adobe_Lib_Manual-4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 18:13:18.114630 Adobe_Lib_Manual-4.0/
-drwxrwxrwx   0        0        0        0 2023-06-27 18:13:18.035973 Adobe_Lib_Manual-4.0/Adobe_Lib_Manual.egg-info/
--rw-rw-rw-   0        0        0      504 2023-06-27 18:13:17.000000 Adobe_Lib_Manual-4.0/Adobe_Lib_Manual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-06-27 18:13:17.000000 Adobe_Lib_Manual-4.0/Adobe_Lib_Manual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 18:13:17.000000 Adobe_Lib_Manual-4.0/Adobe_Lib_Manual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-27 18:13:17.000000 Adobe_Lib_Manual-4.0/Adobe_Lib_Manual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10147 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      504 2023-06-27 18:13:18.114630 Adobe_Lib_Manual-4.0/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-06-27 17:37:10.000000 Adobe_Lib_Manual-4.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 18:13:18.099000 Adobe_Lib_Manual-4.0/aanalytics2/
--rw-rw-rw-   0        0        0      170 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/__init__.py
--rw-rw-rw-   0        0        0       23 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/__version__.py
--rw-rw-rw-   0        0        0     2808 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/aanalytics14.py
--rw-rw-rw-   0        0        0   160368 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/aanalytics2.py
--rw-rw-rw-   0        0        0      678 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/config.py
--rw-rw-rw-   0        0        0     7934 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/configs.py
--rw-rw-rw-   0        0        0    11275 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/connector.py
--rw-rw-rw-   0        0        0    12515 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/ingestion.py
--rw-rw-rw-   0        0        0    10473 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/projects.py
--rw-rw-rw-   0        0        0    17339 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/requestCreator.py
--rw-rw-rw-   0        0        0     3778 2023-06-27 17:39:20.000000 Adobe_Lib_Manual-4.0/aanalytics2/token_provider.py
--rw-rw-rw-   0        0        0     9958 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/aanalytics2/workspace.py
--rw-rw-rw-   0        0        0       42 2023-06-27 18:13:18.114630 Adobe_Lib_Manual-4.0/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-06-27 18:13:09.000000 Adobe_Lib_Manual-4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 18:13:18.114630 Adobe_Lib_Manual-4.0/test/
--rw-rw-rw-   0        0        0        0 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/test/__init__.py
--rw-rw-rw-   0        0        0      883 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/test/test_configuration.py
--rw-rw-rw-   0        0        0     2470 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.0/test/test_core_analytics.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:23:51.208546 Adobe_Lib_Manual-4.1/
+drwxrwxrwx   0        0        0        0 2023-06-27 18:23:51.128757 Adobe_Lib_Manual-4.1/Adobe_Lib_Manual.egg-info/
+-rw-rw-rw-   0        0        0      528 2023-06-27 18:23:51.000000 Adobe_Lib_Manual-4.1/Adobe_Lib_Manual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-06-27 18:23:51.000000 Adobe_Lib_Manual-4.1/Adobe_Lib_Manual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:23:51.000000 Adobe_Lib_Manual-4.1/Adobe_Lib_Manual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 18:23:51.000000 Adobe_Lib_Manual-4.1/Adobe_Lib_Manual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10147 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      528 2023-06-27 18:23:51.208546 Adobe_Lib_Manual-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-06-27 17:37:10.000000 Adobe_Lib_Manual-4.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 18:23:51.184827 Adobe_Lib_Manual-4.1/aanalytics2/
+-rw-rw-rw-   0        0        0      170 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/__version__.py
+-rw-rw-rw-   0        0        0     2808 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/aanalytics14.py
+-rw-rw-rw-   0        0        0   160368 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/aanalytics2.py
+-rw-rw-rw-   0        0        0      678 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/config.py
+-rw-rw-rw-   0        0        0     7934 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/configs.py
+-rw-rw-rw-   0        0        0    11275 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/connector.py
+-rw-rw-rw-   0        0        0    12515 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/ingestion.py
+-rw-rw-rw-   0        0        0    10473 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/projects.py
+-rw-rw-rw-   0        0        0    17339 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/requestCreator.py
+-rw-rw-rw-   0        0        0     3778 2023-06-27 17:39:20.000000 Adobe_Lib_Manual-4.1/aanalytics2/token_provider.py
+-rw-rw-rw-   0        0        0     9958 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/aanalytics2/workspace.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 18:23:51.208546 Adobe_Lib_Manual-4.1/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-06-27 18:23:47.000000 Adobe_Lib_Manual-4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:23:51.192843 Adobe_Lib_Manual-4.1/test/
+-rw-rw-rw-   0        0        0        0 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/test/__init__.py
+-rw-rw-rw-   0        0        0      883 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/test/test_configuration.py
+-rw-rw-rw-   0        0        0     2470 2023-06-27 17:17:00.000000 Adobe_Lib_Manual-4.1/test/test_core_analytics.py
```

### Comparing `Adobe_Lib_Manual-4.0/Adobe_Lib_Manual.egg-info/SOURCES.txt` & `Adobe_Lib_Manual-4.1/Adobe_Lib_Manual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/LICENSE` & `Adobe_Lib_Manual-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/aanalytics14.py` & `Adobe_Lib_Manual-4.1/aanalytics2/aanalytics14.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/aanalytics2.py` & `Adobe_Lib_Manual-4.1/aanalytics2/aanalytics2.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/config.py` & `Adobe_Lib_Manual-4.1/aanalytics2/config.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/configs.py` & `Adobe_Lib_Manual-4.1/aanalytics2/configs.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/connector.py` & `Adobe_Lib_Manual-4.1/aanalytics2/connector.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/ingestion.py` & `Adobe_Lib_Manual-4.1/aanalytics2/ingestion.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/projects.py` & `Adobe_Lib_Manual-4.1/aanalytics2/projects.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/requestCreator.py` & `Adobe_Lib_Manual-4.1/aanalytics2/requestCreator.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/token_provider.py` & `Adobe_Lib_Manual-4.1/aanalytics2/token_provider.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/aanalytics2/workspace.py` & `Adobe_Lib_Manual-4.1/aanalytics2/workspace.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/setup.py` & `Adobe_Lib_Manual-4.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='Adobe_Lib_Manual',
-  version='4.0',
+  version='4.1',
   description='abc',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Ajay Pandey',
   author_email='ajaypanday678@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `Adobe_Lib_Manual-4.0/test/test_configuration.py` & `Adobe_Lib_Manual-4.1/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `Adobe_Lib_Manual-4.0/test/test_core_analytics.py` & `Adobe_Lib_Manual-4.1/test/test_core_analytics.py`

 * *Files identical despite different names*

