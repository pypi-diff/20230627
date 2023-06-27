# Comparing `tmp/sam_ml-py-0.6.0.tar.gz` & `tmp/sam_ml-py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.6.0.tar", last modified: Sat Jun 24 09:47:20 2023, max compression
+gzip compressed data, was "sam_ml-py-0.7.0.tar", last modified: Tue Jun 27 15:15:52 2023, max compression
```

## Comparing `sam_ml-py-0.6.0.tar` & `sam_ml-py-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.823865 sam_ml-py-0.6.0/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.827865 sam_ml-py-0.6.0/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.827865 sam_ml-py-0.6.0/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/XGBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:15:52.693506 sam_ml-py-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-27 15:15:52.693506 sam_ml-py-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:15:52.681506 sam_ml-py-0.7.0/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:15:52.681506 sam_ml-py-0.7.0/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:15:52.685506 sam_ml-py-0.7.0/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:15:52.693506 sam_ml-py-0.7.0/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/XGBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:15:52.693506 sam_ml-py-0.7.0/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-27 15:15:52.000000 sam_ml-py-0.7.0/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-27 15:15:52.000000 sam_ml-py-0.7.0/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:15:52.000000 sam_ml-py-0.7.0/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 15:15:52.000000 sam_ml-py-0.7.0/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 15:15:52.000000 sam_ml-py-0.7.0/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:15:52.693506 sam_ml-py-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 15:15:42.000000 sam_ml-py-0.7.0/setup.py
```

### Comparing `sam_ml-py-0.6.0/LICENSE` & `sam_ml-py-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/PKG-INFO` & `sam_ml-py-0.7.0/sam_ml_py.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sam_ml-py
-Version: 0.6.0
+Name: sam-ml-py
+Version: 0.7.0
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -13,14 +13,30 @@
 
 [![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
 a library created by Samuel Brinkmann
 
 ## getting started
 
+0. pre-installations *(needed for [smac](https://github.com/automl/SMAC3) library)*
+
+You need to install `swig` for the *smag* library that is used for hyperparameter tuning.
+
+Linux *(see [smac installation guide](https://automl.github.io/SMAC3/main/1_installation.html))*:
+
+```
+apt-get install swig
+```
+
+MacOS (with [homebrew](https://formulae.brew.sh/formula/swig)):
+
+```
+brew install swig
+```
+
 1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
 2. now you can import the package, e.g.:
```

### Comparing `sam_ml-py-0.6.0/sam_ml/config/logging.py` & `sam_ml-py-0.7.0/sam_ml/config/logging.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/data/embeddings.py` & `sam_ml-py-0.7.0/sam_ml/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/data/feature_selection.py` & `sam_ml-py-0.7.0/sam_ml/data/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/data/sampling.py` & `sam_ml-py-0.7.0/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/data/scaler.py` & `sam_ml-py-0.7.0/sam_ml/data/scaler.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.7.0/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/AdaBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/BaggingClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.7.0/sam_ml/models/BernoulliNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.7.0/sam_ml/models/ClassifierTest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import sys
 import warnings
-from copy import copy
 from typing import Union
 
 import pandas as pd
 
 # to deactivate pygame promt 
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
 
@@ -44,15 +43,15 @@
     warnings.simplefilter("ignore")
     os.environ["PYTHONWARNINGS"] = "ignore" # Also affects subprocesses
 
 
 class CTest:
     """ AutoML class """
 
-    def __init__(self, models: Union[str, list[Classifier]] = "search", vectorizer: Union[str, Embeddings_builder] = None, scaler: Union[str, Scaler] = None, selector: Union[str, Selector] = None, sampler: Union[str, Sampler] = None):
+    def __init__(self, models: Union[str, list[Classifier]] = "all", vectorizer: Union[str, Embeddings_builder] = None, scaler: Union[str, Scaler] = None, selector: Union[str, Selector] = None, sampler: Union[str, Sampler] = None):
         """
         @params:
             models:
 
                 - list of Wrapperclass models from this library
 
                 - 'all': use all Wrapperclass models (18+ models)
@@ -324,115 +323,51 @@
         scoring: str = "accuracy",
         avg: str = "macro",
         pos_label: Union[int, str] = -1,
         secondary_scoring: str = None,
         strength: int = 3,
         small_data_eval: bool = False,
         cv_num: int = 3,
+        leave_loadbar: bool = True,
     ) -> dict:
+        """
+        @params:
+            x_train: DataFrame with train features
+            y_train: Series with train labels
+            x_test: DataFrame with test features
+            y_test: Series with test labels
+
+            n_trails: number of parameter sets to test
+
+            scoring: metrics to evaluate the models
+            avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
+            pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
+            secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
+            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
+
+            small_data_eval: if True: trains model on all datapoints except one and does this for all datapoints (recommended for datasets with less than 150 datapoints)
+
+            cv_num: number of different splits per crossvalidation (only used when small_data_eval=False)
+
+            leave_loadbar: shall the loading bar of the randomCVsearch of each individual model be visible after training (True - load bar will still be visible)
+        """
         for key in tqdm(self.models.keys(), desc="randomCVsearch"):
-            best_hyperparameters, best_score = self.models[key].randomCVsearch(x_train, y_train, n_trails, scoring, avg, pos_label, secondary_scoring, strength, small_data_eval, cv_num, True)
+            best_hyperparameters, best_score = self.models[key].randomCVsearch(x_train, y_train, n_trails, scoring, avg, pos_label, secondary_scoring, strength, small_data_eval, cv_num, leave_loadbar)
             logger.info(f"{self.models[key].model_name} - score: {best_score} ({scoring}) - parameters: {best_hyperparameters}")
-            model_best = copy(self.models[key])
-            model_best.set_params(**best_hyperparameters)
-            train_score, train_time = model_best.train(x_train, y_train, console_out=False)
-            scores = model_best.evaluate(x_test, y_test, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength, console_out=False)
-            
-            scores["train_time"] = train_time
-            scores["train_score"] = train_score
-            scores["best_score (rCVs)"] = best_score
-            scores["best_hyperparameters (rCVs)"] = best_hyperparameters
-            self.scores[key] = scores
+            if best_hyperparameters != {}:
+                model_best = self.models[key].get_deepcopy()
+                model_best.set_params(**best_hyperparameters)
+                train_score, train_time = model_best.train(x_train, y_train, console_out=False)
+                scores = model_best.evaluate(x_test, y_test, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength, console_out=False)
+                
+                scores["train_time"] = train_time
+                scores["train_score"] = train_score
+                scores["best_score (rCVs)"] = best_score
+                scores["best_hyperparameters (rCVs)"] = best_hyperparameters
+                self.scores[key] = scores
         sorted_scores = self.output_scores_as_pd(sort_by=[scoring, "s_score", "train_time"], console_out=False)
         best_model_type = sorted_scores.iloc[0].name
         best_model_value = sorted_scores.iloc[0][scoring]
         best_model_hyperparameters = sorted_scores.iloc[0]["best_hyperparameters (rCVs)"]
         logger.info(f"best model type {best_model_type} - {scoring}: {best_model_value} - parameters: {best_model_hyperparameters}")
         self.__finish_sound()
         return self.scores
-
-
-    # def find_best_model(
-    #     self,
-    #     x_train: pd.DataFrame,
-    #     y_train: pd.Series,
-    #     x_test: pd.DataFrame,
-    #     y_test: pd.Series,
-    #     cv_kind: str = "no",
-    #     scoring: str = "accuracy",
-    #     avg: str = "macro",
-    #     pos_label: Union[int, str] = -1,
-    #     rand_search: bool = True,
-    #     n_iter_num: int = 75,
-    #     cv_num: int = 10,
-    #     console_out: bool = False,
-    #     secondary_scoring: str = None,
-    #     strength: int = 3,
-    # ) -> Pipeline:
-    #     """
-    #     @param:
-    #         cv_kind: which kind of cross validation shall be used to create the scores to find the best model type
-    #             'no': use eval_models on x_train, y_train, x_test, y_test
-    #             'small': use eval_models_cv with small_data_eval=True on x_train, y_train
-    #             'multi': use eval_models_cv with small_data_eval=False on x_train, y_train
-    #         scoring: "accuracy" / "precision" / "recall" / "s_score" / "l_score"
-
-    #         avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
-    #         pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
-    #         rand_search: True: RandomizedSearchCV, False: GridSearchCV
-    #         n_iter_num: Combinations to try out if rand_search=True
-    #         cv_num: number of different splits
-    #         console_out: outputs intermidiate results into the console
-    #         secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
-    #         strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
-
-    #     @return:
-    #         - prints parameters and metrics of best model
-    #         - saves best model in self.best_model
-    #         - returns best model
-    #     """
-
-    #     if cv_kind == "no":
-    #         logger.debug("creating scores using 'eval_models()'")
-    #         self.eval_models(x_train, y_train, x_test, y_test, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
-    #     elif cv_kind == "small":
-    #         logger.debug("creating scores using 'eval_models_cv(small_data_eval=True)'")
-    #         self.eval_models_cv(x_train, y_train, avg=avg, pos_label=pos_label, small_data_eval=True, secondary_scoring=secondary_scoring, strength=strength)
-    #     elif cv_kind == "multi":
-    #         logger.debug("creating scores using 'eval_models_cv(small_data_eval=False)'")
-    #         self.eval_models_cv(x_train, y_train, avg=avg, pos_label=pos_label, small_data_eval=False, secondary_scoring=secondary_scoring, strength=strength, cv_num=cv_num)
-    #     else:
-    #         logger.error(f"wrong input '{cv_kind}' for cv_kind")
-    #         return
-
-    #     sorted_scores = self.output_scores_as_pd(sort_by=[scoring, "s_score"])
-    #     best_model_type = sorted_scores.iloc[0].name
-    #     best_model_value = sorted_scores.iloc[0][scoring]
-
-    #     print()
-    #     print(f"best model type ({scoring}): ", best_model_type, " - ", best_model_value)
-    #     print()
-
-    #     logger.info(f"hyperparametertuning for best model type (rand_search = {rand_search}) - started")
-    #     self.models[best_model_type].gridsearch(
-    #         x_train,
-    #         y_train,
-    #         scoring=scoring,
-    #         train_afterwards=True,
-    #         avg=avg,
-    #         pos_label=pos_label,
-    #         rand_search=rand_search,
-    #         n_iter_num=n_iter_num,
-    #         cv_num=cv_num,
-    #         console_out=console_out,
-    #         secondary_scoring=secondary_scoring,
-    #         strength=strength,
-    #     )
-    #     logger.info(f"hyperparametertuning for best model type (rand_search = {rand_search}) - finished")
-
-    #     # Set self.best_model = hyperparameter tuned model
-    #     self.best_model = self.models[best_model_type]
-
-    #     self.best_model.evaluate(x_test, y_test, avg=avg, pos_label=pos_label)
-    #     self.best_model.feature_importance()
-    #     self.__finish_sound()
-    #     return self.best_model
```

### Comparing `sam_ml-py-0.6.0/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/ExtraTreesClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.7.0/sam_ml/models/GaussianNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/GaussianProcessClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.7.0/sam_ml/models/GradientBoostingMachine.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,11 +36,11 @@
             "n_estimators": Integer("n_estimators", (20, 1500), log=True, default=100),
             "max_depth": Integer("max_depth", (1, 15), distribution=Normal(5, 3), default=3),
             "min_samples_split": Integer("min_samples_split", (2, 100), log=True, default=2),
             "min_samples_leaf": Integer("min_samples_leaf", (1, 100), log=True, default=1),
             "max_features": Categorical("max_features", ["auto", "sqrt", "log2"], default="auto"),
             "subsample": Float("subsample", (0.7, 1), default=1),
             "criterion": Categorical("criterion", ["friedman_mse", "squared_error"], default="friedman_mse"),
-            "loss": Categorical("loss", ["log_loss", "deviance", "exponential"], default="log_loss"),
+            "loss": Categorical("loss", ["log_loss", "deviance"], default="log_loss"),
             "learning_rate": Float("learning_rate", (0.005, 0.3), log=True, default=0.1),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.6.0/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.7.0/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.7.0/sam_ml/models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/MLPClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.7.0/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/SupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/XGBoostClassifier.py` & `sam_ml-py-0.7.0/sam_ml/models/XGBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/__init__.py` & `sam_ml-py-0.7.0/sam_ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml/models/main_classifier.py` & `sam_ml-py-0.7.0/sam_ml/models/main_classifier.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-from copy import copy
 from datetime import timedelta
 from statistics import mean
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from ConfigSpace import Configuration, ConfigurationSpace
 from matplotlib import pyplot as plt
 from sklearn.metrics import (accuracy_score, classification_report,
                              make_scorer, precision_score, recall_score)
-from sklearn.model_selection import (GridSearchCV, RandomizedSearchCV,
-                                     cross_validate)
-# from smac import (HyperparameterOptimizationFacade, MultiFidelityFacade,
-#                   RandomFacade, Scenario)
+from sklearn.model_selection import cross_validate
+from smac import HyperparameterOptimizationFacade, Scenario
 from tqdm.auto import tqdm
 
 from sam_ml.config import setup_logger
 
 from .main_model import Model
 from .scorer import l_scoring, s_scoring
 
 logger = setup_logger(__name__)
 
 
 class Classifier(Model):
     """ Classifier parent class """
 
-    def __init__(self, model_object = None, model_name: str = "classifier", model_type: str = "Classifier", grid: dict[str, list] = {}, is_pipeline: bool = False):
+    def __init__(self, model_object = None, model_name: str = "classifier", model_type: str = "Classifier", grid: ConfigurationSpace = ConfigurationSpace()):
         """
         @params:
-            model_object: model with 'fit' and 'predict' method
+            model_object: model with 'fit', 'predict', 'set_params', and 'get_params' method (see sklearn API)
             model_name: name of the model
             model_type: kind of estimator (e.g. 'RFC' for RandomForestClassifier)
             grid: hyperparameter grid for the model
         """
         super().__init__(model_object, model_name, model_type)
         self._grid = grid
-        self.is_pipeline = is_pipeline
         self.cv_scores: dict[str, float] = {}
         self.rCVsearch_results: pd.DataFrame|None = None
 
     def __repr__(self) -> str:
         params: str = ""
         param_dict = self.get_params(False)
         for key in param_dict:
@@ -117,14 +113,16 @@
             avg: average to use for precision and recall score (e.g. "micro", None, "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. pos_label is used by s_score/l_score
 
             console_out: shall the result be printed into the console
 
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
             strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
+
+        @return: dictionary with keys with scores: 'accuracy', 'precision', 'recall', 's_score', 'l_score'
         """
         pred = self.predict(x_test)
 
         # Calculate Accuracy, Precision and Recall Metrics
         accuracy = accuracy_score(y_test, pred)
         precision = precision_score(y_test, pred, average=avg, pos_label=pos_label)
         recall = recall_score(y_test, pred, average=avg, pos_label=pos_label)
@@ -146,14 +144,54 @@
             "precision": precision,
             "recall": recall,
             "s_score": s_score,
             "l_score": l_score,
         }
 
         return self.test_score
+    
+    def evaluate_score(
+        self,
+        x_test: pd.DataFrame,
+        y_test: pd.Series,
+        scoring: str = "accuracy",
+        avg: str = None,
+        pos_label: Union[int, str] = -1,
+        secondary_scoring: str = None,
+        strength: int = 3,
+    ) -> float:
+        """
+        @param:
+            x_test, y_test: Data to evaluate model
+            scoring: metrics to evaluate the models ("accuracy", "precision", "recall", "s_score", "l_score")
+
+            avg: average to use for precision and recall score (e.g. "micro", None, "weighted", "binary")
+            pos_label: if avg="binary", pos_label says which class to score. pos_label is used by s_score/l_score
+            secondary_scoring: weights the scoring (only for 's_score'/'l_score')
+            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
+
+        @return: score as float
+        """
+        pred = self.predict(x_test)
+
+        # Calculate score
+        if scoring == "accuracy":
+            score = accuracy_score(y_test, pred)
+        elif scoring == "precision":
+            score = precision_score(y_test, pred, average=avg, pos_label=pos_label)
+        elif scoring == "recall":
+            score = recall_score(y_test, pred, average=avg, pos_label=pos_label)
+        elif scoring == "s_score":
+            score = s_scoring(y_test, pred, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
+        elif scoring == "l_score":
+            score = l_scoring(y_test, pred, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
+        else:
+            raise ValueError(f"scoring='{scoring}' is not supported -> only  'accuracy', 'precision', 'recall', 's_score', or 'l_score' ")
+
+        return score
 
     def cross_validation(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         cv_num: int = 10,
         avg: str = "macro",
@@ -172,15 +210,15 @@
 
             console_out: shall the result be printed into the console
 
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
             strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return:
-            dictionary with "accuracy", "precision", "recall", "s_score", "l_score", "avg train score", "avg train time"
+            dictionary with "accuracy", "precision", "recall", "s_score", "l_score", train_score", "train_time"
         """
         logger.debug(f"cross validation {self.model_name} - started")
 
         precision_scorer = make_scorer(precision_score, average=avg, pos_label=pos_label)
         recall_scorer = make_scorer(recall_score, average=avg, pos_label=pos_label)
         s_scorer = make_scorer(s_scoring, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
         l_scorer = make_scorer(l_scoring, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
@@ -257,15 +295,15 @@
             leave_loadbar: shall the loading bar of the training be visible after training (True - load bar will still be visible)
             console_out: shall the result be printed into the console
 
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
             strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return:
-            dictionary with "accuracy", "precision", "recall", "s_score", "l_score", "avg train score", "avg train time"
+            dictionary with "accuracy", "precision", "recall", "s_score", "l_score", train_score", "train_time"
         """
         logger.debug(f"cross validation {self.model_name} - started")
 
         predictions = []
         true_values = []
         t_scores = []
         t_times = []
@@ -345,63 +383,86 @@
         else:
             feature_importances.plot.bar(ax=ax)
         ax.set_title("Feature importances of " + str(self.model_name))
         ax.set_ylabel("use of coefficients as importance scores")
         fig.tight_layout()
         plt.show()
     
-    # def smac_search(
-    #         self,
-    #         x_train: pd.DataFrame, 
-    #         y_train: pd.Series
-    # ):
-    #     # Next, we create an object, holding general information about the run
-    #     scenario = Scenario(
-    #         self.grid,
-    #         n_trials=5,  # We want to run max 50 trials (combination of config and seed)
-    #         deterministic=True,
-    #         min_budget=5,
-    #         max_budget=25,
-    #     )
-
-    #     # We want to run the facade's default initial design, but we want to change the number
-    #     # of initial configs to 5.
-    #     initial_design = MultiFidelityFacade.get_initial_design(scenario)
-
-    #     # define target function
-    #     def grid_train(config: Configuration, seed: int, budget) -> float:
-    #         print(config)
-    #         print(seed)
-    #         print(budget)
-    #         params = self.get_params()
-    #         #print(params)
-    #         params.update(config)
-    #         #print(params)
-    #         model = type(self)(**params)
-    #         score = model.cross_validation(x_train, y_train, console_out=False, cv_num=2)
-    #         print(1 - score["accuracy"])
-    #         return 1 - score["accuracy"]  # SMAC always minimizes (the smaller the better)
-
-    #     # Now we use SMAC to find the best hyperparameters
-    #     smac = MultiFidelityFacade(
-    #         scenario,
-    #         grid_train,
-    #         initial_design=initial_design,
-    #         overwrite=True,  # If the run exists, we overwrite it; alternatively, we can continue from last state
-    #     )
-
-    #     incumbent = smac.optimize()
-
-    #     # Get cost of default configuration
-    #     default_cost = smac.validate(self.grid.get_default_configuration())
-    #     print(f"Default cost: {default_cost}")
-
-    #     # Let's calculate the cost of the incumbent
-    #     incumbent_cost = smac.validate(incumbent)
-    #     print(f"Incumbent cost: {incumbent_cost}")
+    def smac_search(
+        self,
+        x_train: pd.DataFrame, 
+        y_train: pd.Series,
+        n_trails: int = 50,
+        cv_num: int = 5,
+        scoring: str = "accuracy",
+        avg: str = "macro",
+        pos_label: Union[int, str] = -1,
+        secondary_scoring: str = None,
+        strength: int = 3,
+        small_data_eval: bool = False,
+        walltime_limit: float = 600,
+    ) -> Configuration:
+        """
+        @params:
+            x_train: DataFrame with train features
+            y_train: Series with labels
+
+            n_trails: max number of parameter sets to test
+            cv_num: number of different splits per crossvalidation (only used when small_data_eval=False)
+
+            scoring: metrics to evaluate the models ("accuracy", "precision", "recall", "s_score", "l_score")
+            avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
+            pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
+            secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
+            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
+
+            small_data_eval: if True: trains model on all datapoints except one and does this for all datapoints (recommended for datasets with less than 150 datapoints)
+            
+            walltime_limit: the maximum time in seconds that SMAC is allowed to run
+
+        @return: ConfigSpace.Configuration with best hyperparameters (can be used like dict)
+        """
+        logger.debug("starting smac_search")
+        # NormalInteger in grid are not supported and Classifier in Categorical
+        if self.model_type in ("RFC", "ABC", "BC", "ETC", "GBM", "XGBC"):
+            logger.error(f"The model type '{self.model_type}' is currently not supported")
+            return {}
+
+        scenario = Scenario(
+            self.grid,
+            n_trials=n_trails,
+            deterministic=True,
+            walltime_limit=walltime_limit,
+        )
+
+        initial_design = HyperparameterOptimizationFacade.get_initial_design(scenario, n_configs=5)
+        logger.debug(f"initial_design: {initial_design.select_configurations()}")
+
+        # define target function
+        def grid_train(config: Configuration, seed: int) -> float:
+            logger.debug(f"config: {config}")
+            model = self.get_deepcopy()
+            model.set_params(**config)
+            if small_data_eval:
+                score = model.cross_validation_small_data(x_train, y_train, console_out=False, leave_loadbar=False, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
+            else:
+                score = model.cross_validation(x_train, y_train, console_out=False, cv_num=cv_num, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
+            return 1 - score[scoring]  # SMAC always minimizes (the smaller the better)
+
+        # use SMAC to find the best hyperparameters
+        smac = HyperparameterOptimizationFacade(
+            scenario,
+            grid_train,
+            initial_design=initial_design,
+            overwrite=True,  # If the run exists, we overwrite it; alternatively, we can continue from last state
+        )
+
+        incumbent = smac.optimize()
+        logger.debug("finished smac_search")
+        return incumbent
 
     def randomCVsearch(
         self,
         x_train: pd.DataFrame,
         y_train: pd.Series,
         n_trails: int = 10,
         scoring: str = "accuracy",
@@ -409,20 +470,43 @@
         pos_label: Union[int, str] = -1,
         secondary_scoring: str = None,
         strength: int = 3,
         small_data_eval: bool = False,
         cv_num: int = 5,
         leave_loadbar: bool = True,
     ) -> tuple[dict, float]:
+        """
+        @params:
+            x_train: DataFrame with train features
+            y_train: Series with labels
+
+            n_trails: number of parameter sets to test
+
+            scoring: metrics to evaluate the models ("accuracy", "precision", "recall", "s_score", "l_score")
+            avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
+            pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
+            secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
+            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
+
+            small_data_eval: if True: trains model on all datapoints except one and does this for all datapoints (recommended for datasets with less than 150 datapoints)
+
+            cv_num: number of different splits per crossvalidation (only used when small_data_eval=False)
+
+            leave_loadbar: shall the loading bar of the different parameter sets be visible after training (True - load bar will still be visible)
+
+        @return: dictionary with best hyperparameters and float of best_score
+        """
+        logger.debug("starting randomCVsearch")
         results = []
         configs = self.get_random_configs(n_trails)
         at_least_one_run: bool = False
         try:
             for config in tqdm(configs, desc=f"randomCVsearch ({self.model_name})", leave=leave_loadbar):
-                model = copy(self)
+                logger.debug(f"config: {config}")
+                model = self.get_deepcopy()
                 model.set_params(**config)
                 if small_data_eval:
                     score = model.cross_validation_small_data(x_train, y_train, console_out=False, leave_loadbar=False, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
                 else:
                     score = model.cross_validation(x_train, y_train, cv_num=cv_num, console_out=False, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
                 config_dict = dict(config)
                 config_dict[scoring] = score[scoring]
@@ -441,120 +525,11 @@
         for col in self.rCVsearch_results.columns:
             value = self.rCVsearch_results[col].iloc[0]
             if str(value) != "nan":
                 best_hyperparameters[col] = value
 
         best_score = best_hyperparameters[scoring]
         best_hyperparameters.pop(scoring)
+
+        logger.debug("finished randomCVsearch")
         
         return best_hyperparameters, best_score
-
-    # def gridsearch(
-    #     self,
-    #     x_train: pd.DataFrame,
-    #     y_train: pd.Series,
-    #     grid: dict = None,
-    #     scoring: str = "accuracy",
-    #     avg: str = "macro",
-    #     pos_label: Union[int, str] = -1,
-    #     cv_num: int = 10,
-    #     verbose: int = 0,
-    #     rand_search: bool = True,
-    #     n_iter_num: int = 75,
-    #     console_out: bool = True,
-    #     train_afterwards: bool = True,
-    #     secondary_scoring: str = None,
-    #     strength: int = 3,
-    # ):
-    #     """
-    #     @param:
-    #         x_train: DataFrame with train features
-    #         y_train: Series with labels
-
-    #         grid: dictonary of parameters to tune (default: default parameter dictionary self.grid)
-
-    #         scoring: metrics to evaluate the models
-    #         avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
-    #         pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
-
-    #         rand_search: True: RandomizedSearchCV, False: GridSearchCV
-    #         n_iter_num: Combinations to try out if rand_search=True
-
-    #         cv_num: number of different splits
-
-    #         verbose: log level (higher number --> more logs)
-    #         console_out: output the the results of the different iterations
-    #         train_afterwards: train the best model after finding it
-
-    #         secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
-    #         strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
-
-    #     @return:
-    #         set self.model = best model from search
-    #     """
-    #     if grid is None:
-    #         grid = self.grid
-
-    #     if console_out:
-    #         print()
-    #         print("grid: ", grid)
-    #         print()
-
-    #     if scoring == "precision":
-    #         scoring = make_scorer(precision_score, average=avg, pos_label=pos_label)
-    #     elif scoring == "recall":
-    #         scoring = make_scorer(recall_score, average=avg, pos_label=pos_label)
-    #     elif scoring == "s_score":
-    #         scoring = make_scorer(s_scoring, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
-    #     elif scoring == "l_score":
-    #         scoring = make_scorer(l_scoring, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
-
-    #     if rand_search:
-    #         grid_search = RandomizedSearchCV(
-    #             estimator=self,
-    #             param_distributions=grid,
-    #             n_iter=n_iter_num,
-    #             cv=cv_num,
-    #             verbose=verbose,
-    #             random_state=42,
-    #             n_jobs=-1,
-    #             scoring=scoring,
-    #         )
-    #     else:
-    #         grid_search = GridSearchCV(
-    #             estimator=self,
-    #             param_grid=grid,
-    #             n_jobs=-1,
-    #             cv=cv_num,
-    #             verbose=verbose,
-    #             scoring=scoring,
-    #             error_score=0,
-    #         )
-    #     logger.debug(f"hyperparameter tuning {self.model_name} - started")
-    #     grid_result = grid_search.fit(x_train, y_train)
-    #     logger.debug(f"hyperparameter tuning {self.model_name} - finished")
-
-    #     if console_out:
-    #         means = grid_result.cv_results_["mean_test_score"]
-    #         stds = grid_result.cv_results_["std_test_score"]
-    #         params = grid_result.cv_results_["params"]
-    #         print()
-    #         for mean, stdev, param in zip(means, stds, params):
-    #             print("mean: %f (stdev: %f) with: %r" % (mean, stdev, param))
-    #         print()
-
-    #     self.model = grid_result.best_estimator_.model
-    #     if self.is_pipeline:
-    #         self.vectorizer = grid_result.best_estimator_.vectorizer
-    #         self.scaler = grid_result.best_estimator_.scaler
-    #         self.selector = grid_result.best_estimator_.selector
-    #         self.sampler = grid_result.best_estimator_.sampler
-    #         self._classifier = (self.model, self.model_type, self._grid)
-
-    #     print()
-    #     print("Best: %f using %s" % (grid_result.best_score_, grid_result.best_params_))
-    #     print()
-
-    #     if train_afterwards:
-    #         logger.debug(f"best model training {self.model_name} - started")
-    #         self.train(x_train, y_train, console_out=False)
-    #         logger.debug(f"best model training {self.model_name} - finished")
```

### Comparing `sam_ml-py-0.6.0/sam_ml/models/main_model.py` & `sam_ml-py-0.7.0/sam_ml/models/main_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pickle
 import time
+from copy import deepcopy
 from datetime import timedelta
 from typing import Union
 
 import pandas as pd
 
 from sam_ml.config import setup_logger
 
@@ -11,17 +12,17 @@
 
 class Model:
     """ Model parent class """
 
     def __init__(self, model_object = None, model_name: str = "model", model_type: str = "Model"):
         """
         @params:
-            model_object: model with 'fit' and 'predict' method
+            model_object: model with 'fit', 'predict', 'set_params', and 'get_params' method (see sklearn API)
             model_name: name of the model
-            model_type: kind of estimator  (e.g. 'RFC' for RandomForestClassifier)
+            model_type: kind of estimator (e.g. 'RFC' for RandomForestClassifier)
         """
         self.model = model_object
         self.model_name = model_name
         self.model_type = model_type
         self.trained: bool = False
         self.train_score: float = None
         self.train_time: str = None
@@ -73,14 +74,18 @@
         return self
 
     def evaluate(self, x_test: pd.DataFrame, y_test: pd.Series, console_out: bool = True) -> float:
         self.test_score = self.model.score(x_test, y_test)
         if console_out:
             print("Test score: ", self.test_score)
         return self.test_score
+    
+    def get_deepcopy(self):
+        """function to create a deepcopy of object"""
+        return deepcopy(self)
 
     def save_model(self, path: str, only_estimator: bool = False):
         """ 
         function to pickle and save the Class object 
         
         @params:
             path: path to save the model with suffix '.pkl'
```

### Comparing `sam_ml-py-0.6.0/sam_ml/models/scorer.py` & `sam_ml-py-0.7.0/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.7.0/sam_ml_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.6.0/setup.py` & `sam_ml-py-0.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.6.0",
+    version="0.7.0",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
@@ -24,15 +24,15 @@
         "pygame",
         "ipywidgets",
         "tqdm",
         "statsmodels",
         "sentence-transformers",
         "xgboost",
         "ConfigSpace", # for hyperparameter tuning spaces
-        #"smac", # for hyperparameter tuning
+        "smac", # for hyperparameter tuning
     ],
     extras_require={"test": ["pytest", "pylint!=2.5.0", "isort", "refurb", "black"],},
     author="Samuel Brinkmann",
     license="MIT",
     tests_require=["pytest==4.4.1"],
     setup_requires=["pytest-runner"],
 )
```

