# Comparing `tmp/adaboost-model-0.2.0.tar.gz` & `tmp/adaboost-model-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Lenovo\source\repos\sis-model\packaging\dist\.tmp-zmnm0qp6\adaboost-model-0.2.0.tar", last modified: Tue Jun 27 16:02:12 2023, max compression
+gzip compressed data, was "C:\Users\Lenovo\source\repos\sis-model\packaging\dist\.tmp-yolz52n5\adaboost-model-0.2.1.tar", last modified: Tue Jun 27 17:12:52 2023, max compression
```

## Comparing `adaboost-model-0.2.0.tar` & `adaboost-model-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 16:02:12.163359 adaboost-model-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-06-27 15:55:58.000000 adaboost-model-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      588 2023-06-27 16:02:12.163359 adaboost-model-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-06-27 15:55:33.000000 adaboost-model-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 16:02:12.163359 adaboost-model-0.2.0/adaboost_model.egg-info/
--rw-rw-rw-   0        0        0      588 2023-06-27 16:02:12.000000 adaboost-model-0.2.0/adaboost_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-06-27 16:02:12.000000 adaboost-model-0.2.0/adaboost_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 16:02:12.000000 adaboost-model-0.2.0/adaboost_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 16:02:12.000000 adaboost-model-0.2.0/adaboost_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      714 2023-06-27 16:00:49.000000 adaboost-model-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 16:02:12.163359 adaboost-model-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 17:12:52.877994 adaboost-model-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 15:55:58.000000 adaboost-model-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      588 2023-06-27 17:12:52.876997 adaboost-model-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-06-27 15:55:33.000000 adaboost-model-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:12:52.875987 adaboost-model-0.2.1/adaboost_model.egg-info/
+-rw-rw-rw-   0        0        0      588 2023-06-27 17:12:52.000000 adaboost-model-0.2.1/adaboost_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-06-27 17:12:52.000000 adaboost-model-0.2.1/adaboost_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:12:52.000000 adaboost-model-0.2.1/adaboost_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:12:52.000000 adaboost-model-0.2.1/adaboost_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      714 2023-06-27 17:12:09.000000 adaboost-model-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:12:52.877994 adaboost-model-0.2.1/setup.cfg
```

### Comparing `adaboost-model-0.2.0/LICENSE` & `adaboost-model-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adaboost-model-0.2.0/PKG-INFO` & `adaboost-model-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: adaboost-model
-Version: 0.2.0
+Version: 0.2.1
 Summary: Academic Performance Prediction
 Author-email: Queency Koh <queencykoh@gmail.com>
 Project-URL: Homepage, https://github.com/queency-koh/sis-model
 Project-URL: Bug Tracker, https://github.com/queency-koh/sis-model/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: ==3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Academic Performance Prediction using Adaboost Model
```

### Comparing `adaboost-model-0.2.0/adaboost_model.egg-info/PKG-INFO` & `adaboost-model-0.2.1/adaboost_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: adaboost-model
-Version: 0.2.0
+Version: 0.2.1
 Summary: Academic Performance Prediction
 Author-email: Queency Koh <queencykoh@gmail.com>
 Project-URL: Homepage, https://github.com/queency-koh/sis-model
 Project-URL: Bug Tracker, https://github.com/queency-koh/sis-model/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: ==3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Academic Performance Prediction using Adaboost Model
```

### Comparing `adaboost-model-0.2.0/pyproject.toml` & `adaboost-model-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["numpy>=1.18.1,<1.19.2","pandas>=0.25.3,<1.3.5","scikit-learn>=0.22.1,<1.1.2","joblib>=0.14.1,<1.0.0","setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adaboost-model"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Queency Koh", email="queencykoh@gmail.com" },
 ]
 description = "Academic Performance Prediction"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = "==3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

