# Comparing `tmp/idsw-1.0.3.tar.gz` & `tmp/idsw-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idsw-1.0.3.tar", last modified: Fri Jul 22 19:08:47 2022, max compression
+gzip compressed data, was "idsw-1.1.tar", last modified: Tue Jun 27 17:19:57 2023, max compression
```

## Comparing `idsw-1.0.3.tar` & `idsw-1.1.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-07-22 19:08:47.017184 idsw-1.0.3/
--rw-rw-rw-   0        0        0     1139 2022-07-09 14:47:38.000000 idsw-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       24 2022-07-09 14:54:50.000000 idsw-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      783 2022-07-22 19:08:47.017184 idsw-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      467 2022-07-10 00:55:48.000000 idsw-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-07-22 19:08:46.979898 idsw-1.0.3/etl/
--rw-rw-rw-   0        0        0        0 2022-07-08 15:31:26.000000 idsw-1.0.3/etl/__init__.py
--rw-rw-rw-   0        0        0  1050019 2022-07-22 17:02:44.000000 idsw-1.0.3/etl/etl.py
-drwxrwxrwx   0        0        0        0 2022-07-22 19:08:47.004500 idsw-1.0.3/idsw.egg-info/
--rw-rw-rw-   0        0        0      783 2022-07-22 19:08:46.000000 idsw-1.0.3/idsw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2022-07-22 19:08:46.000000 idsw-1.0.3/idsw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-22 19:08:46.000000 idsw-1.0.3/idsw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      289 2022-07-22 19:08:46.000000 idsw-1.0.3/idsw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2022-07-22 19:08:46.000000 idsw-1.0.3/idsw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      288 2022-07-22 00:34:37.000000 idsw-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-07-22 19:08:47.018912 idsw-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      947 2022-07-22 19:03:52.000000 idsw-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-22 19:08:47.011125 idsw-1.0.3/text_preprocessing/
--rw-rw-rw-   0        0        0        0 2022-07-08 15:31:26.000000 idsw-1.0.3/text_preprocessing/__init__.py
--rw-rw-rw-   0        0        0   116527 2022-07-18 18:05:39.000000 idsw-1.0.3/text_preprocessing/text_preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:19:57.849037 idsw-1.1/
+-rw-rw-rw-   0        0        0     1139 2022-07-09 14:47:38.000000 idsw-1.1/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-07-09 14:54:50.000000 idsw-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      781 2023-06-27 17:19:57.848037 idsw-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2022-07-10 00:55:48.000000 idsw-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:19:57.834214 idsw-1.1/idsw.egg-info/
+-rw-rw-rw-   0        0        0      781 2023-06-27 17:19:57.000000 idsw-1.1/idsw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-27 17:19:57.000000 idsw-1.1/idsw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:19:57.000000 idsw-1.1/idsw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      423 2023-06-27 17:19:57.000000 idsw-1.1/idsw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 17:19:57.000000 idsw-1.1/idsw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      422 2023-06-27 15:52:09.000000 idsw-1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:19:57.849678 idsw-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-14 18:54:41.000000 idsw-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:19:57.840453 idsw-1.1/text_preprocessing/
+-rw-rw-rw-   0        0        0        0 2022-07-08 15:31:26.000000 idsw-1.1/text_preprocessing/__init__.py
+-rw-rw-rw-   0        0        0   116527 2022-07-18 18:05:39.000000 idsw-1.1/text_preprocessing/text_preprocessing.py
```

### Comparing `idsw-1.0.3/LICENSE` & `idsw-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idsw-1.0.3/PKG-INFO` & `idsw-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idsw
-Version: 1.0.3
+Version: 1.1
 Summary: Industrial Data Science Workflow: full workflow for ETL, statistics, and Machine learning modelling of (usually) time-stamped industrial facilities data.
 Author: Marco César Prado Soares, Gabriel Fernandes Luz
 Author-email: marcosoares.feq@gmail.com, gfluz94@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `idsw-1.0.3/idsw.egg-info/PKG-INFO` & `idsw-1.1/idsw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idsw
-Version: 1.0.3
+Version: 1.1
 Summary: Industrial Data Science Workflow: full workflow for ETL, statistics, and Machine learning modelling of (usually) time-stamped industrial facilities data.
 Author: Marco César Prado Soares, Gabriel Fernandes Luz
 Author-email: marcosoares.feq@gmail.com, gfluz94@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `idsw-1.0.3/setup.py` & `idsw-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Check the project Github: https://github.com/marcosoares-92/IndustrialDataScienceWorkflow
 """
 with open("requirements.txt", "r") as file:
     required_packages = [package.strip() for package in file.readlines()]
 
 setuptools.setup(
     name="idsw",
-    version="1.0.3",
+    version="1.1",
     author="Marco César Prado Soares, Gabriel Fernandes Luz",
     author_email="marcosoares.feq@gmail.com, gfluz94@gmail.com",
     description=long_description,
     long_description=long_description,
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.7",
```

### Comparing `idsw-1.0.3/text_preprocessing/text_preprocessing.py` & `idsw-1.1/text_preprocessing/text_preprocessing.py`

 * *Files identical despite different names*

