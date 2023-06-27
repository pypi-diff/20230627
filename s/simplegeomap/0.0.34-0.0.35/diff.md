# Comparing `tmp/simplegeomap-0.0.34.tar.gz` & `tmp/simplegeomap-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplegeomap-0.0.34.tar", last modified: Fri Jun 23 07:54:18 2023, max compression
+gzip compressed data, was "dist/simplegeomap-0.0.35.tar", last modified: Tue Jun 27 06:02:16 2023, max compression
```

## Comparing `simplegeomap-0.0.34.tar` & `simplegeomap-0.0.35.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.34/README.md
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/
--rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/dependency_links.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/top_level.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)       45 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/requires.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/SOURCES.txt
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap/
--rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.34/simplegeomap/__init__.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     7137 2023-06-23 07:43:24.000000 simplegeomap-0.0.34/simplegeomap/simplegeomap.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     7636 2023-06-23 07:44:48.000000 simplegeomap-0.0.34/simplegeomap/util.py
--rw-rw-r--   0 burak     (1000) burak     (1000)      618 2023-06-23 07:53:19.000000 simplegeomap-0.0.34/setup.py
--rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/setup.cfg
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.35/README.md
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/simplegeomap.egg-info/
+-rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/simplegeomap.egg-info/dependency_links.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/simplegeomap.egg-info/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/simplegeomap.egg-info/top_level.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)       45 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/simplegeomap.egg-info/requires.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/simplegeomap.egg-info/SOURCES.txt
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/simplegeomap/
+-rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.35/simplegeomap/__init__.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     7137 2023-06-23 07:43:24.000000 simplegeomap-0.0.35/simplegeomap/simplegeomap.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     7636 2023-06-23 07:44:48.000000 simplegeomap-0.0.35/simplegeomap/util.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)      618 2023-06-27 06:01:24.000000 simplegeomap-0.0.35/setup.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-27 06:02:16.000000 simplegeomap-0.0.35/setup.cfg
```

### Comparing `simplegeomap-0.0.34/PKG-INFO` & `simplegeomap-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.34
+Version: 0.0.35
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.34/README.md` & `simplegeomap-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.34/simplegeomap.egg-info/PKG-INFO` & `simplegeomap-0.0.35/simplegeomap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.34
+Version: 0.0.35
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.34/simplegeomap/simplegeomap.py` & `simplegeomap-0.0.35/simplegeomap/simplegeomap.py`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.34/simplegeomap/util.py` & `simplegeomap-0.0.35/simplegeomap/util.py`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.34/setup.py` & `simplegeomap-0.0.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 readme=open("README.md").read()
 
 setuptools.setup(
     name='simplegeomap',    
-    version='0.0.34',
+    version='0.0.35',
     description="Simple offline map plot utility, for country borders, elevation, water",
     long_description=readme,
     long_description_content_type="text/markdown",    
     install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','zarr'],
     include_package_data=True,
     url="https://github.com/burakbayramli/simplegeomap",
     author="Burak Bayramli",
```

