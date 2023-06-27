# Comparing `tmp/moosez-2.1.2.tar.gz` & `tmp/moosez-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.1.2.tar", last modified: Tue Jun 27 13:53:56 2023, max compression
+gzip compressed data, was "moosez-2.1.3.tar", last modified: Tue Jun 27 15:14:19 2023, max compression
```

## Comparing `moosez-2.1.2.tar` & `moosez-2.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:53:56.562087 moosez-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:53:47.000000 moosez-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 13:53:56.562087 moosez-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-27 13:53:47.000000 moosez-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:53:56.562087 moosez-2.1.2/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 13:53:47.000000 moosez-2.1.2/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:53:56.562087 moosez-2.1.2/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 13:53:56.000000 moosez-2.1.2/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 13:53:56.000000 moosez-2.1.2/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:53:56.000000 moosez-2.1.2/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 13:53:56.000000 moosez-2.1.2/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-27 13:53:56.000000 moosez-2.1.2/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 13:53:56.000000 moosez-2.1.2/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:53:56.562087 moosez-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-27 13:53:47.000000 moosez-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:14:19.850398 moosez-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 15:14:03.000000 moosez-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 15:14:19.850398 moosez-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-27 15:14:03.000000 moosez-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:14:19.846397 moosez-2.1.3/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 15:14:03.000000 moosez-2.1.3/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:14:19.850398 moosez-2.1.3/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 15:14:19.000000 moosez-2.1.3/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 15:14:19.000000 moosez-2.1.3/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:14:19.000000 moosez-2.1.3/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 15:14:19.000000 moosez-2.1.3/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-27 15:14:19.000000 moosez-2.1.3/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 15:14:19.000000 moosez-2.1.3/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:14:19.850398 moosez-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-27 15:14:03.000000 moosez-2.1.3/setup.py
```

### Comparing `moosez-2.1.2/LICENSE` & `moosez-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/PKG-INFO` & `moosez-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.2
+Version: 2.1.3
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.2/README.md` & `moosez-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez/constants.py` & `moosez-2.1.3/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez/display.py` & `moosez-2.1.3/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez/download.py` & `moosez-2.1.3/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez/file_utilities.py` & `moosez-2.1.3/moosez/file_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     :param modality_tag: The modality tag to be selected.
     :return: The list of selected files.
     """
     selected_files = []
     for subject in moose_compliant_subjects:
         files = os.listdir(subject)
         for file in files:
-            if file.startswith(modality_tag):
+            if file.startswith(modality_tag) and file.endswith('.nii') or file.endswith('.nii.gz'):
                 selected_files.append(os.path.join(subject, file))
     return selected_files
 
 
 def organise_files_by_modality(moose_compliant_subjects: list, modalities: list, moose_dir) -> None:
     """
     Organises the files by modality.
```

### Comparing `moosez-2.1.2/moosez/image_conversion.py` & `moosez-2.1.3/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez/image_processing.py` & `moosez-2.1.3/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez/input_validation.py` & `moosez-2.1.3/moosez/input_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     compliant.
     :return: The list of subject paths that are moose compliant.
     """
     # go through each subject in the parent directory
     moose_compliant_subjects = []
     for subject_path in subject_paths:
         # go through each subject and see if the files have the appropriate modality suffixes
-        files = os.listdir(subject_path)
+        # files = os.listdir(subject_path)
+        # get the nifti files in the subject_path
+        files = [file for file in os.listdir(subject_path) if file.endswith('.nii')]
         suffixes = [file.startswith(tag) for tag in modality_tags for file in files]
         if sum(suffixes) == len(modality_tags):
             moose_compliant_subjects.append(subject_path)
     print(f"{constants.ANSI_ORANGE} Number of moose compliant subjects: {len(moose_compliant_subjects)} out of "
           f"{len(subject_paths)} {constants.ANSI_RESET}")
     logging.info(f" Number of moose compliant subjects: {len(moose_compliant_subjects)} out of "
                  f"{len(subject_paths)}")
```

### Comparing `moosez-2.1.2/moosez/moosez.py` & `moosez-2.1.3/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez/predict.py` & `moosez-2.1.3/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez/resources.py` & `moosez-2.1.3/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.2/moosez.egg-info/PKG-INFO` & `moosez-2.1.3/moosez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.2
+Version: 2.1.3
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.2/setup.py` & `moosez-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.1.2',
+    version='2.1.3',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

