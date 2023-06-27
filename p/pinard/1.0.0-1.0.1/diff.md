# Comparing `tmp/pinard-1.0.0.tar.gz` & `tmp/pinard-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinard-1.0.0.tar", last modified: Tue Jun 27 09:40:13 2023, max compression
+gzip compressed data, was "pinard-1.0.1.tar", last modified: Tue Jun 27 09:58:06 2023, max compression
```

## Comparing `pinard-1.0.0.tar` & `pinard-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.437826 pinard-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    21467 2023-06-27 09:40:03.000000 pinard-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-06-27 09:40:13.437826 pinard-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-27 09:40:03.000000 pinard-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.433826 pinard-1.0.0/pinard/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.433826 pinard-1.0.0/pinard/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/augmentation/_random_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/augmentation/_spline_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/augmentation/augmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.433826 pinard-1.0.0/pinard/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/_data_driven_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/_nirs_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/_random_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.437826 pinard-1.0.0/pinard/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/preprocessing/_nirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/preprocessing/_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/preprocessing/_standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.437826 pinard-1.0.0/pinard/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/sklearn/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/sklearn/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.433826 pinard-1.0.0/pinard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:40:13.437826 pinard-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-27 09:40:03.000000 pinard-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.437826 pinard-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:06.624775 pinard-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    21467 2023-06-27 09:57:52.000000 pinard-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-06-27 09:58:06.624775 pinard-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-27 09:57:52.000000 pinard-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:06.616774 pinard-1.0.1/pinard/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:06.620774 pinard-1.0.1/pinard/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/augmentation/_random_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/augmentation/_spline_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/augmentation/augmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:06.620774 pinard-1.0.1/pinard/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/model_selection/_data_driven_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/model_selection/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/model_selection/_nirs_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/model_selection/_random_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:06.620774 pinard-1.0.1/pinard/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/preprocessing/_nirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/preprocessing/_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/preprocessing/_standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:06.620774 pinard-1.0.1/pinard/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/sklearn/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/sklearn/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-27 09:57:52.000000 pinard-1.0.1/pinard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:06.620774 pinard-1.0.1/pinard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-06-27 09:58:06.000000 pinard-1.0.1/pinard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-27 09:58:06.000000 pinard-1.0.1/pinard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:58:06.000000 pinard-1.0.1/pinard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 09:58:06.000000 pinard-1.0.1/pinard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 09:58:06.000000 pinard-1.0.1/pinard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:58:06.000000 pinard-1.0.1/pinard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:58:06.624775 pinard-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-27 09:57:52.000000 pinard-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:06.624775 pinard-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:57:52.000000 pinard-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-27 09:57:52.000000 pinard-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 09:57:52.000000 pinard-1.0.1/tests/test_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 09:57:52.000000 pinard-1.0.1/tests/test_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-27 09:57:52.000000 pinard-1.0.1/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-27 09:57:52.000000 pinard-1.0.1/tests/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-27 09:57:52.000000 pinard-1.0.1/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-27 09:57:52.000000 pinard-1.0.1/tests/test_utils.py
```

### Comparing `pinard-1.0.0/LICENSE` & `pinard-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/PKG-INFO` & `pinard-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinard
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pinard: a Pipeline for Nirs Analysis ReloadeD.
 Home-page: https://github.com/gbeurier/pinard
 Author: Gregory Beurier
 Author-email: beurier@cirad.fr
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pinard-1.0.0/README.md` & `pinard-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/augmentation/__init__.py` & `pinard-1.0.1/pinard/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/augmentation/_random_augmentation.py` & `pinard-1.0.1/pinard/augmentation/_random_augmentation.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/augmentation/_spline_augmentation.py` & `pinard-1.0.1/pinard/augmentation/_spline_augmentation.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/augmentation/augmenter.py` & `pinard-1.0.1/pinard/augmentation/augmenter.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/model_selection/_data_driven_sampling.py` & `pinard-1.0.1/pinard/model_selection/_data_driven_sampling.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/model_selection/_helpers.py` & `pinard-1.0.1/pinard/model_selection/_helpers.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/model_selection/_nirs_sampling.py` & `pinard-1.0.1/pinard/model_selection/_nirs_sampling.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/model_selection/_random_sampling.py` & `pinard-1.0.1/pinard/model_selection/_random_sampling.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/preprocessing/__init__.py` & `pinard-1.0.1/pinard/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/preprocessing/_nirs.py` & `pinard-1.0.1/pinard/preprocessing/_nirs.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/preprocessing/_scaler.py` & `pinard-1.0.1/pinard/preprocessing/_scaler.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/preprocessing/_standard.py` & `pinard-1.0.1/pinard/preprocessing/_standard.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/sklearn/_pipeline.py` & `pinard-1.0.1/pinard/sklearn/_pipeline.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/sklearn/_utils.py` & `pinard-1.0.1/pinard/sklearn/_utils.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard/utils.py` & `pinard-1.0.1/pinard/utils.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/pinard.egg-info/PKG-INFO` & `pinard-1.0.1/pinard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinard
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pinard: a Pipeline for Nirs Analysis ReloadeD.
 Home-page: https://github.com/gbeurier/pinard
 Author: Gregory Beurier
 Author-email: beurier@cirad.fr
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pinard-1.0.0/pinard.egg-info/SOURCES.txt` & `pinard-1.0.1/pinard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/setup.py` & `pinard-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/tests/conftest.py` & `pinard-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/tests/test_preprocessing.py` & `pinard-1.0.1/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/tests/test_selection.py` & `pinard-1.0.1/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `pinard-1.0.0/tests/test_utils.py` & `pinard-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

