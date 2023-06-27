# Comparing `tmp/moosez-2.1.0.tar.gz` & `tmp/moosez-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.1.0.tar", last modified: Tue Jun 27 13:04:27 2023, max compression
+gzip compressed data, was "moosez-2.1.1.tar", last modified: Tue Jun 27 13:38:16 2023, max compression
```

## Comparing `moosez-2.1.0.tar` & `moosez-2.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:27.916004 moosez-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:04:14.000000 moosez-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 13:04:27.916004 moosez-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-27 13:04:14.000000 moosez-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:27.912004 moosez-2.1.0/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:27.916004 moosez-2.1.0/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:04:27.916004 moosez-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-27 13:04:14.000000 moosez-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:38:16.065827 moosez-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:38:06.000000 moosez-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 13:38:16.065827 moosez-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-27 13:38:06.000000 moosez-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:38:16.065827 moosez-2.1.1/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 13:38:06.000000 moosez-2.1.1/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:38:16.065827 moosez-2.1.1/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 13:38:16.000000 moosez-2.1.1/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 13:38:16.000000 moosez-2.1.1/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:38:16.000000 moosez-2.1.1/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 13:38:16.000000 moosez-2.1.1/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-27 13:38:16.000000 moosez-2.1.1/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 13:38:16.000000 moosez-2.1.1/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:38:16.065827 moosez-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-27 13:38:06.000000 moosez-2.1.1/setup.py
```

### Comparing `moosez-2.1.0/LICENSE` & `moosez-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/PKG-INFO` & `moosez-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.0
+Version: 2.1.1
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.0/README.md` & `moosez-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/constants.py` & `moosez-2.1.1/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/display.py` & `moosez-2.1.1/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/download.py` & `moosez-2.1.1/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/file_utilities.py` & `moosez-2.1.1/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/image_conversion.py` & `moosez-2.1.1/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/image_processing.py` & `moosez-2.1.1/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/input_validation.py` & `moosez-2.1.1/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/moosez.py` & `moosez-2.1.1/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.0/moosez/predict.py` & `moosez-2.1.1/moosez/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     elif model_name == "clin_ct_ribs":
         return 202
     elif model_name == "clin_ct_vertebrae":
         return 203
     elif model_name == "clin_ct_muscles":
         return 204
     elif model_name == "clin_ct_lungs":
-        return 124
+        return 333
     elif model_name == "clin_ct_fat":
         return 206
     elif model_name == "clin_ct_vessels":
         return 207
     elif model_name == "clin_ct_organs":
         return 123
     elif model_name == "clin_pt_fdg_tumor":
```

### Comparing `moosez-2.1.0/moosez/resources.py` & `moosez-2.1.1/moosez/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     },
     "clin_ct_muscles": {
         "url": "https://example.com/muscles_model.zip",
         "filename": "clin_ct_muscles_model.zip",
         "directory": "clin_ct_muscles_model",
     },
     "clin_ct_lungs": {
-        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/HMS_3dlungs_10062023.zip",
-        "filename": "Dataset124_HMS_3dlungs.zip",
-        "directory": "Dataset124_HMS_3dlungs",
+        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/clin_ct_lungs_24062023.zip",
+        "filename": "Dataset333_HMS3dlungs.zip",
+        "directory": "Dataset333_HMS3dlungs",
     },
     "clin_ct_fat": {
         "url": "https://example.com/fat_model.zip",
         "filename": "clin_ct_fat_model.zip",
         "directory": "clin_ct_fat_model",
     },
     "clin_ct_vessels": {
```

### Comparing `moosez-2.1.0/moosez.egg-info/PKG-INFO` & `moosez-2.1.1/moosez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.0
+Version: 2.1.1
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.0/setup.py` & `moosez-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.1.0',
+    version='2.1.1',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

