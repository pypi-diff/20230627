# Comparing `tmp/DeepStorm-1.0.4.tar.gz` & `tmp/DeepStorm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepStorm-1.0.4.tar", last modified: Tue Jun 27 08:14:13 2023, max compression
+gzip compressed data, was "DeepStorm-1.0.5.tar", last modified: Tue Jun 27 08:15:58 2023, max compression
```

## Comparing `DeepStorm-1.0.4.tar` & `DeepStorm-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:14:13.274529 DeepStorm-1.0.4/
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:14:13.258529 DeepStorm-1.0.4/DeepStorm/
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:14:13.270529 DeepStorm-1.0.4/DeepStorm/Layers/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      277 2023-06-03 09:32:57.000000 DeepStorm-1.0.4/DeepStorm/Layers/Base.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     4058 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Layers/BatchNormalization.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     8026 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Layers/Conv.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      706 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Layers/Dropout.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      552 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Layers/Flatten.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1778 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Layers/FullyConnected.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)    13656 2023-06-03 07:37:12.000000 DeepStorm-1.0.4/DeepStorm/Layers/Helpers.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      873 2023-06-03 07:37:12.000000 DeepStorm-1.0.4/DeepStorm/Layers/Initializers.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     3585 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Layers/Pooling.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      279 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Layers/ReLU.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      931 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Layers/SoftMax.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      146 2023-06-03 07:37:12.000000 DeepStorm-1.0.4/DeepStorm/Layers/__init__.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     6010 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Model.py
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:14:13.274529 DeepStorm-1.0.4/DeepStorm/Optimization/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      386 2023-06-21 15:39:13.000000 DeepStorm-1.0.4/DeepStorm/Optimization/Loss.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1779 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/DeepStorm/Optimization/Optimizers.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       33 2023-06-03 07:37:12.000000 DeepStorm-1.0.4/DeepStorm/Optimization/__init__.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        5 2023-06-27 08:13:55.000000 DeepStorm-1.0.4/DeepStorm/VERSION
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2023-06-03 07:37:12.000000 DeepStorm-1.0.4/DeepStorm/__init__.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1029 2023-06-03 07:37:12.000000 DeepStorm-1.0.4/DeepStorm/logger.py
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:14:13.262529 DeepStorm-1.0.4/DeepStorm.egg-info/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     3438 2023-06-27 08:14:13.000000 DeepStorm-1.0.4/DeepStorm.egg-info/PKG-INFO
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      821 2023-06-27 08:14:13.000000 DeepStorm-1.0.4/DeepStorm.egg-info/SOURCES.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-06-27 08:14:13.000000 DeepStorm-1.0.4/DeepStorm.egg-info/dependency_links.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-06-27 08:08:20.000000 DeepStorm-1.0.4/DeepStorm.egg-info/not-zip-safe
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       68 2023-06-27 08:14:13.000000 DeepStorm-1.0.4/DeepStorm.egg-info/requires.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       10 2023-06-27 08:14:13.000000 DeepStorm-1.0.4/DeepStorm.egg-info/top_level.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1079 2023-06-03 07:37:12.000000 DeepStorm-1.0.4/LICENSE
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      301 2023-06-27 08:09:42.000000 DeepStorm-1.0.4/MANIFEST.in
--rw-rw-r--   0 hassan    (1000) hassan    (1000)    71954 2023-06-27 08:04:56.000000 DeepStorm-1.0.4/NeuralNetworkTests.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     3438 2023-06-27 08:14:13.274529 DeepStorm-1.0.4/PKG-INFO
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     2716 2023-06-27 08:13:38.000000 DeepStorm-1.0.4/README.md
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      104 2023-06-03 07:37:12.000000 DeepStorm-1.0.4/pyproject.toml
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       67 2023-05-24 10:20:55.000000 DeepStorm-1.0.4/requirements.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       38 2023-06-27 08:14:13.274529 DeepStorm-1.0.4/setup.cfg
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1809 2023-06-27 08:05:02.000000 DeepStorm-1.0.4/setup.py
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:15:58.960229 DeepStorm-1.0.5/
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:15:58.944230 DeepStorm-1.0.5/DeepStorm/
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:15:58.956230 DeepStorm-1.0.5/DeepStorm/Layers/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      277 2023-06-03 09:32:57.000000 DeepStorm-1.0.5/DeepStorm/Layers/Base.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     4058 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Layers/BatchNormalization.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     8026 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Layers/Conv.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      706 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Layers/Dropout.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      552 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Layers/Flatten.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1778 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Layers/FullyConnected.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)    13656 2023-06-03 07:37:12.000000 DeepStorm-1.0.5/DeepStorm/Layers/Helpers.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      873 2023-06-03 07:37:12.000000 DeepStorm-1.0.5/DeepStorm/Layers/Initializers.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     3585 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Layers/Pooling.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      279 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Layers/ReLU.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      931 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Layers/SoftMax.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      146 2023-06-03 07:37:12.000000 DeepStorm-1.0.5/DeepStorm/Layers/__init__.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     6010 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Model.py
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:15:58.960229 DeepStorm-1.0.5/DeepStorm/Optimization/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      386 2023-06-21 15:39:13.000000 DeepStorm-1.0.5/DeepStorm/Optimization/Loss.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1779 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/DeepStorm/Optimization/Optimizers.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       33 2023-06-03 07:37:12.000000 DeepStorm-1.0.5/DeepStorm/Optimization/__init__.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        5 2023-06-27 08:15:47.000000 DeepStorm-1.0.5/DeepStorm/VERSION
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2023-06-03 07:37:12.000000 DeepStorm-1.0.5/DeepStorm/__init__.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1029 2023-06-03 07:37:12.000000 DeepStorm-1.0.5/DeepStorm/logger.py
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-06-27 08:15:58.948230 DeepStorm-1.0.5/DeepStorm.egg-info/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     3440 2023-06-27 08:15:58.000000 DeepStorm-1.0.5/DeepStorm.egg-info/PKG-INFO
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      821 2023-06-27 08:15:58.000000 DeepStorm-1.0.5/DeepStorm.egg-info/SOURCES.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-06-27 08:15:58.000000 DeepStorm-1.0.5/DeepStorm.egg-info/dependency_links.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-06-27 08:08:20.000000 DeepStorm-1.0.5/DeepStorm.egg-info/not-zip-safe
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       68 2023-06-27 08:15:58.000000 DeepStorm-1.0.5/DeepStorm.egg-info/requires.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       10 2023-06-27 08:15:58.000000 DeepStorm-1.0.5/DeepStorm.egg-info/top_level.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1079 2023-06-03 07:37:12.000000 DeepStorm-1.0.5/LICENSE
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      301 2023-06-27 08:09:42.000000 DeepStorm-1.0.5/MANIFEST.in
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)    71954 2023-06-27 08:04:56.000000 DeepStorm-1.0.5/NeuralNetworkTests.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     3440 2023-06-27 08:15:58.960229 DeepStorm-1.0.5/PKG-INFO
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     2718 2023-06-27 08:15:08.000000 DeepStorm-1.0.5/README.md
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      104 2023-06-03 07:37:12.000000 DeepStorm-1.0.5/pyproject.toml
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       67 2023-05-24 10:20:55.000000 DeepStorm-1.0.5/requirements.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       38 2023-06-27 08:15:58.960229 DeepStorm-1.0.5/setup.cfg
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1809 2023-06-27 08:05:02.000000 DeepStorm-1.0.5/setup.py
```

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/BatchNormalization.py` & `DeepStorm-1.0.5/DeepStorm/Layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/Conv.py` & `DeepStorm-1.0.5/DeepStorm/Layers/Conv.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/Dropout.py` & `DeepStorm-1.0.5/DeepStorm/Layers/Dropout.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/Flatten.py` & `DeepStorm-1.0.5/DeepStorm/Layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/FullyConnected.py` & `DeepStorm-1.0.5/DeepStorm/Layers/FullyConnected.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/Helpers.py` & `DeepStorm-1.0.5/DeepStorm/Layers/Helpers.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/Initializers.py` & `DeepStorm-1.0.5/DeepStorm/Layers/Initializers.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/Pooling.py` & `DeepStorm-1.0.5/DeepStorm/Layers/Pooling.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Layers/SoftMax.py` & `DeepStorm-1.0.5/DeepStorm/Layers/SoftMax.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Model.py` & `DeepStorm-1.0.5/DeepStorm/Model.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/Optimization/Optimizers.py` & `DeepStorm-1.0.5/DeepStorm/Optimization/Optimizers.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm/logger.py` & `DeepStorm-1.0.5/DeepStorm/logger.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/DeepStorm.egg-info/PKG-INFO` & `DeepStorm-1.0.5/DeepStorm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepStorm
-Version: 1.0.4
+Version: 1.0.5
 Summary: Deep Learning framework from scratch
 Home-page: https://github.com/HassanRady/DeepStorm
 Author: Hassan Rady
 Author-email: hassan.khaled.rady@gmail.com
 License: MIT license
 Keywords: Tweets
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,15 +22,15 @@
 # DeepStorm: Deep Learning Framework
 
 ## Summary:
 Deep Learning Framework from scratch, with an API of a combination of pytorch and keras APIs, only uses numpy for tensor operations.
 
 ## Pip install:
 ```sh
-pip install DLstorm
+pip install DeepStorm
 ```
 
 ## Layers & DL classes in framework:
 - Conv2d
 - MaxPool2d
 - BatchNorm2d
 - Flatten
```

### Comparing `DeepStorm-1.0.4/DeepStorm.egg-info/SOURCES.txt` & `DeepStorm-1.0.5/DeepStorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/LICENSE` & `DeepStorm-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/NeuralNetworkTests.py` & `DeepStorm-1.0.5/NeuralNetworkTests.py`

 * *Files identical despite different names*

### Comparing `DeepStorm-1.0.4/PKG-INFO` & `DeepStorm-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepStorm
-Version: 1.0.4
+Version: 1.0.5
 Summary: Deep Learning framework from scratch
 Home-page: https://github.com/HassanRady/DeepStorm
 Author: Hassan Rady
 Author-email: hassan.khaled.rady@gmail.com
 License: MIT license
 Keywords: Tweets
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,15 +22,15 @@
 # DeepStorm: Deep Learning Framework
 
 ## Summary:
 Deep Learning Framework from scratch, with an API of a combination of pytorch and keras APIs, only uses numpy for tensor operations.
 
 ## Pip install:
 ```sh
-pip install DLstorm
+pip install DeepStorm
 ```
 
 ## Layers & DL classes in framework:
 - Conv2d
 - MaxPool2d
 - BatchNorm2d
 - Flatten
```

### Comparing `DeepStorm-1.0.4/README.md` & `DeepStorm-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # DeepStorm: Deep Learning Framework
 
 ## Summary:
 Deep Learning Framework from scratch, with an API of a combination of pytorch and keras APIs, only uses numpy for tensor operations.
 
 ## Pip install:
 ```sh
-pip install DLstorm
+pip install DeepStorm
 ```
 
 ## Layers & DL classes in framework:
 - Conv2d
 - MaxPool2d
 - BatchNorm2d
 - Flatten
```

### Comparing `DeepStorm-1.0.4/setup.py` & `DeepStorm-1.0.5/setup.py`

 * *Files identical despite different names*

