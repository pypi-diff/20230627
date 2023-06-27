# Comparing `tmp/Digital_Farming_Solution-0.1.1.tar.gz` & `tmp/Digital_Farming_Solution-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Farming_Solution-0.1.1.tar", last modified: Sun Jun 25 17:01:12 2023, max compression
+gzip compressed data, was "Digital_Farming_Solution-0.1.2.tar", last modified: Tue Jun 27 10:31:50 2023, max compression
```

## Comparing `Digital_Farming_Solution-0.1.1.tar` & `Digital_Farming_Solution-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 17:01:11.815259 Digital_Farming_Solution-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-25 17:01:11.559445 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution/
--rw-rw-rw-   0        0        0     4450 2023-06-25 17:00:31.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution/Select_options.py
--rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:01:11.807277 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/
--rw-rw-rw-   0        0        0      609 2023-06-25 17:01:08.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-25 17:01:10.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 17:01:08.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-25 17:01:08.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      609 2023-06-25 17:01:11.815259 Digital_Farming_Solution-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-25 17:01:11.815259 Digital_Farming_Solution-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-06-25 10:53:53.000000 Digital_Farming_Solution-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:31:50.838976 Digital_Farming_Solution-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-27 10:31:50.696801 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution/
+-rw-rw-rw-   0        0        0     6912 2023-06-27 10:30:05.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution/Select_options.py
+-rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:31:50.791151 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-06-27 10:31:49.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-27 10:31:50.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:31:49.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-27 10:31:49.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-06-27 10:31:50.806305 Digital_Farming_Solution-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-27 10:31:50.840947 Digital_Farming_Solution-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-06-27 10:31:05.000000 Digital_Farming_Solution-0.1.2/setup.py
```

### Comparing `Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/PKG-INFO` & `Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital-Farming-Solution
-Version: 0.1.1
+Version: 0.1.2
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.1/PKG-INFO` & `Digital_Farming_Solution-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital_Farming_Solution
-Version: 0.1.1
+Version: 0.1.2
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.1/setup.py` & `Digital_Farming_Solution-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Digital_Farming_Solution",
-    version="0.1.1",
+    version="0.1.2",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
     description=" The packages are helps to the DFS Teams to perform some of the task easily.",
     long_description= 'By importing this packages we can work on easily and  get some meaningfull information.It is more siutable for the dataframe works and it will returnns the Dataframe.',
     long_description_content_type="text/markdown",
     packages=["Digital_Farming_Solution"],
     classifiers=[
```

