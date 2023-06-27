# Comparing `tmp/moosez-2.0.9.tar.gz` & `tmp/moosez-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.0.9.tar", last modified: Mon Jun 12 16:44:33 2023, max compression
+gzip compressed data, was "moosez-2.1.0.tar", last modified: Tue Jun 27 13:04:27 2023, max compression
```

## Comparing `moosez-2.0.9.tar` & `moosez-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:44:33.884248 moosez-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 16:44:21.000000 moosez-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 16:44:33.884248 moosez-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-06-12 16:44:21.000000 moosez-2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:44:33.884248 moosez-2.0.9/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:44:33.884248 moosez-2.0.9/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:44:33.884248 moosez-2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 16:44:21.000000 moosez-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:27.916004 moosez-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:04:14.000000 moosez-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 13:04:27.916004 moosez-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-27 13:04:14.000000 moosez-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:27.912004 moosez-2.1.0/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 13:04:14.000000 moosez-2.1.0/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:27.916004 moosez-2.1.0/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 13:04:27.000000 moosez-2.1.0/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:04:27.916004 moosez-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-27 13:04:14.000000 moosez-2.1.0/setup.py
```

### Comparing `moosez-2.0.9/LICENSE` & `moosez-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.0.9/PKG-INFO` & `moosez-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.9
+Version: 2.1.0
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.0.9/moosez/constants.py` & `moosez-2.1.0/moosez/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,28 +29,35 @@
 
 # COLOR CODES
 ANSI_ORANGE = '\033[38;5;208m'
 ANSI_GREEN = '\033[38;5;40m'
 ANSI_VIOLET = '\033[38;5;141m'
 ANSI_RESET = '\033[0m'
 
-
 # SUPPORTED TRACERS (limited patch)
 
 TRACER_FDG = 'FDG'
 
-
 # FOLDER NAMES
 
 SEGMENTATIONS_FOLDER = 'segmentations'
 
-
 # PREPROCESSING PARAMETERS
 
-VOXEL_SPACING = [1.5, 1.5, 1.5]
-
+CLINICAL_VOXEL_SPACING = [1.5, 1.5, 1.5]
+PRECLINICAL_VOXEL_SPACING = [0.15, 0.15, 0.15]
+MATRIX_THRESHOLD = 200 * 200 * 600
+Z_AXIS_THRESHOLD = 200
+MARGIN_PADDING = 20
+INTERPOLATION = 'bspline'
+CHUNK_THRESHOLD = 200
 
 # FILE NAMES PREFIX
 
 ORGANS_MULTILABEL_SUFFIX = 'Organs-Multilabel-'
 LUNGS_MULTILABEL_SUFFIX = 'Lungs-Multilabel-'
 MULTILABEL_SUFFIX = 'MULTILABEL-'
+
+# FILE NAMES
+
+RESAMPLED_IMAGE_FILE_NAME = 'resampled_image.nii.gz'
+RESAMPLED_MASK_FILE_NAME = 'resampled_mask.nii.gz'
```

### Comparing `moosez-2.0.9/moosez/display.py` & `moosez-2.1.0/moosez/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to show predefined display
 # messages.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import logging
-from moosez import constants
+
 import pyfiglet
+
 from moosez import constants
 
 
 def logo():
     """
     Display MOOSE logo
     :return:
     """
     print(' ')
     logo_color_code = constants.ANSI_VIOLET
     slogan_color_code = constants.ANSI_VIOLET
-    result = logo_color_code + pyfiglet.figlet_format("MOOSE 2.0", font="smslant").rstrip() + "\033[0m"
-    text = slogan_color_code + "A part of the ENHANCE community. Join us at www.enhance.pet to build the future of " \
+    result = logo_color_code + pyfiglet.figlet_format(" MOOSE 2.0", font="smslant").rstrip() + "\033[0m"
+    text = slogan_color_code + " A part of the ENHANCE community. Join us at www.enhance.pet to build the future of " \
                                "PET imaging together." + "\033[0m"
     print(result)
     print(text)
     print(' ')
 
 
 def expected_modality(model_name: str) -> dict:
@@ -65,15 +66,14 @@
         model["Model name"] = model_name
         return model
 
     logging.error(" Requested model is not available. Please check the model name.")
     return {"Error": "Requested model is not available. Please check the model name."}
 
 
-
 def citation():
     """
         Display manuscript citation
         :return:
         """
     print(f"{constants.ANSI_VIOLET} CITATION:{constants.ANSI_RESET}")
     print(" ")
@@ -114,8 +114,7 @@
         f"{constants.ANSI_ORANGE} Warning: Subjects which don't have the required modalities [check file suffix] "
         f"will be skipped. {constants.ANSI_RESET}")
     warning_message = " Skipping subjects without the required modalities (check file suffix).\n" \
                       " These subjects will be excluded from analysis and their data will not be used."
     logging.warning(warning_message)
 
     return modalities
-
```

### Comparing `moosez-2.0.9/moosez/download.py` & `moosez-2.1.0/moosez/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import logging
 import os
-from rich.progress import Progress
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Author: Lalith Kumar Shiyam Sundar
 # Institution: Medical University of Vienna
 # Research Group: Quantitative Imaging and Medical Physics (QIMP) Team
 # Date: 13.02.2023
 # Version: 2.0.0
@@ -17,18 +16,18 @@
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to download the necessary
 # binaries and models for the moosez.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 import requests
-from tqdm import tqdm
+
 from moosez import constants
 from moosez import resources
-
+from rich.progress import Progress
 
 def binary(system_info, url):
     """
     Downloads the binary for the current system.
     :param system_info: A dictionary containing the system information.
     :param url: The url to download the binary from.
     """
@@ -37,14 +36,15 @@
     response = requests.get(url + binary_name)
 
     with open(binary_name, "wb") as f:
         f.write(response.content)
 
 
 
+
 def model(model_name, model_path):
     """
     Downloads the model for the current system.
     :param model_name: The name of the model to download.
     :param model_path: The path to store the model.
     """
     model_info = resources.MODELS[model_name]
@@ -56,25 +56,25 @@
         logging.info(f" Downloading {directory}")
         # show progress using rich
         response = requests.get(url, stream=True)
         total_size = int(response.headers.get("Content-Length", 0))
         chunk_size = 1024 * 10
 
         with Progress() as progress:
-            task = progress.add_task("[cyan] Downloading...", total=total_size)
+            task = progress.add_task(f"[cyan] Downloading {model_name}...", total=total_size)
             for chunk in response.iter_content(chunk_size=chunk_size):
                 open(filename, "ab").write(chunk)
                 progress.update(task, advance=chunk_size)
 
         # Unzip the model
         import zipfile
         with Progress() as progress:
             with zipfile.ZipFile(filename, 'r') as zip_ref:
                 total_size = sum((file.file_size for file in zip_ref.infolist()))
-                task = progress.add_task("[cyan] Extracting...", total=total_size)
+                task = progress.add_task(f"[cyan] Extracting {model_name}...", total=total_size)
                 # Get the parent directory of 'directory'
                 parent_directory = os.path.dirname(directory)
                 for file in zip_ref.infolist():
                     zip_ref.extract(file, parent_directory)
                     extracted_size = file.file_size
                     progress.update(task, advance=extracted_size)
```

### Comparing `moosez-2.0.9/moosez/file_utilities.py` & `moosez-2.1.0/moosez/file_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to perform file operations.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import os
+import shutil
 import sys
 from datetime import datetime
-import shutil
 from multiprocessing import Pool
+
 from moosez import constants
-from halo import Halo
 
 
 def create_directory(directory_path: str):
     """
     Creates a directory at the specified path.
     :param directory_path: The path to the directory.
     """
```

### Comparing `moosez-2.0.9/moosez/image_conversion.py` & `moosez-2.1.0/moosez/image_conversion.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,27 +13,21 @@
 # This module handles image conversion for the moosez.
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to perform image conversion.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
-import logging
-import re
-import subprocess
 import os
-from halo import Halo
+import sys
 import SimpleITK
 import pydicom
-from moosez import constants
-from multiprocessing import Pool
-from typing import List
-from tqdm import tqdm
 from rich.progress import Progress
-
+import dicom2nifti
+from moosez import constants
 
 
 def read_dicom_folder(folder_path: str) -> SimpleITK.Image:
     """
     Reads a folder of DICOM files and returns the image
 
     :param folder_path: str, Directory to get DICOM files from
@@ -55,20 +49,20 @@
     """
     subject_name = os.path.basename(os.path.dirname(input_path))
     output_image_basename = "output"
     output_image = None  # initialize output_image
     if os.path.isdir(input_path):
         image_probe = os.listdir(input_path)[0]
         modality_tag = pydicom.read_file(os.path.join(input_path, image_probe)).Modality
-        if image_probe.endswith(('IMA', 'dcm')):
-            output_image = read_dicom_folder(input_path)
-            if modality_tag == 'PT':
-                output_image_basename = f"{constants.TRACER_FDG}_PET_{subject_name}.nii"
-            elif modality_tag == 'CT':
-                output_image_basename = f"{modality_tag}_{subject_name}.nii"
+        if modality_tag == 'PT':
+            output_image_basename = f"{constants.TRACER_FDG}_PET_{subject_name}.nii"
+        elif modality_tag == 'CT':
+            output_image_basename = f"{modality_tag}_{subject_name}.nii"
+        dcm2niix(input_path, output_image_basename)
+        return
     elif os.path.isfile(input_path):
         if input_path.endswith('.nii.gz') or input_path.endswith('.nii'):
             return
         output_image = SimpleITK.ReadImage(input_path)
         output_image_basename = f"{os.path.splitext(os.path.basename(input_path))[0]}.nii"
     else:
         return
@@ -99,10 +93,19 @@
                         image_path = os.path.join(subject_path, image)
                         non_nifti_to_nifti(image_path)
                     elif os.path.isfile(os.path.join(subject_path, image)):
                         image_path = os.path.join(subject_path, image)
                         non_nifti_to_nifti(image_path)
             else:
                 continue
-            progress.update(task, advance=1, description=f"[cyan]Processing {subject}...")
+            progress.update(task, advance=1, description=f"[cyan] Processing {subject}...")
 
 
+def dcm2niix(input_path: str, output_image_basename: str) -> None:
+    """
+    Converts DICOM images into Nifti images using dcm2niix
+    :param input_path: Path to the folder with the dicom files to convert
+    """
+    output_dir = os.path.dirname(input_path)
+    output_file = os.path.join(output_dir, output_image_basename)
+
+    dicom2nifti.dicom_series_to_nifti(input_path, output_file, reorient_nifti=True)
```

### Comparing `moosez-2.0.9/moosez/input_validation.py` & `moosez-2.1.0/moosez/input_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # and meets the required specifications.
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to perform input validation.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
-import os
-from moosez import constants
 import logging
-import nibabel as nib
 import multiprocessing
+import os
+
+import nibabel as nib
+
+from moosez import constants
 
 
 def check_directory_exists(directory_path: str):
     """
     Checks if the specified directory exists.
     :param directory_path: The path to the directory.
     :raises: Exception if the directory does not exist.
@@ -54,31 +56,43 @@
           f"{len(subject_paths)} {constants.ANSI_RESET}")
     logging.info(f" Number of moose compliant subjects: {len(moose_compliant_subjects)} out of "
                  f"{len(subject_paths)}")
 
     return moose_compliant_subjects
 
 
-def check_file_for_nnunet_compatibility(filename, input_dir):
+
+def check_file_for_nnunet_compatibility(filename: str, input_dir: str) -> None:
+    """
+    Checks if the file is nnUNet compatible. If not, compresses the file and renames it to include the required tag.
+
+    Parameters:
+        filename (str): The name of the file to check.
+        input_dir (str): The path to the directory containing the file.
+
+    Returns:
+        None
+    """
     if filename.endswith('.nii.gz') and not filename.endswith('_0000.nii.gz'):
-        # if the file is not already in the desired format
+        # Rename the file to include the required tag
         new_filename = filename.replace('.nii.gz', '_0000.nii.gz')
         os.rename(os.path.join(input_dir, filename), os.path.join(input_dir, new_filename))
     elif not filename.endswith('.gz'):
-        # if the file is not compressed, compress it
+        # Compress the file if it is not already compressed
         img = nib.load(os.path.join(input_dir, filename))
         new_filename = filename + '.gz'
         nib.save(img, os.path.join(input_dir, new_filename))
         os.remove(os.path.join(input_dir, filename))
         if not new_filename.endswith('_0000.nii.gz'):
-            # if the file is not already in the desired format
+            # Rename the file to include the required tag
             new_filename_with_zeroes = new_filename.replace('.nii.gz', '_0000.nii.gz')
             os.rename(os.path.join(input_dir, new_filename), os.path.join(input_dir, new_filename_with_zeroes))
 
 
+
 def make_nnunet_compatible(input_dir: str) -> None:
     """
     Checks the files in the specified directory to ensure they comply with the nnUNet requirements. If a file does not
     comply, it is compressed (if it is not already) and renamed to include the required tag.
 
     Parameters:
         input_dir (str): The path to the directory containing the files to check.
```

### Comparing `moosez-2.0.9/moosez/moosez.py` & `moosez-2.1.0/moosez/moosez.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #
 # Usage:
 # The main function in this module is executed when the mooseZ is run.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import argparse
-import colorama
 import logging
 import os
 import time
 from datetime import datetime
 
 import colorama
 from halo import Halo
```

### Comparing `moosez-2.0.9/moosez/resources.py` & `moosez-2.1.0/moosez/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     },
     "clin_ct_vessels": {
         "url": "https://example.com/vessels_model.zip",
         "filename": "clin_ct_vessels_model.zip",
         "directory": "clin_ct_vessels_model",
     },
     "clin_ct_organs": {
-        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/MOOSEv2_05062023_Organs.zip",
+        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/MOOSEv2_bspline_organs23062023.zip",
         "filename": "Dataset123_Organs.zip",
         "directory": "Dataset123_Organs",
     },
     "clin_pt_fdg_tumor": {
         "url": "https://example.com/fdg_tumor_model.zip",
         "filename": "clin_pt_fdg_tumor_model.zip",
         "directory": "clin_pt_fdg_tumor_model",
@@ -73,30 +73,30 @@
     },
     "clin_fdg_pt_ct_all": {
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/MOOSE-files-24062022.zip",
         "filename": "clin_fdg_pt_ct_all_model.zip",
         "directory": "clin_fdg_pt_ct_all_model",
     },
     "preclin_mr_all": {
-        "url": "https://example.com/mr_all_model.zip",
-        "filename": "preclin_mr_all_model.zip",
-        "directory": "preclin_mr_all_model",
+        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/preclin_mr_14062023.zip",
+        "filename": "Dataset234_Preclin.zip",
+        "directory": "Dataset234_Preclin",
     },
 
 }
 
 
 def check_cuda() -> str:
     """
-    This function checks if cuda is available in the device and prints the device name and number of cuda devices
-    available in the device.
-    :return: str
+    This function checks if CUDA is available on the device and prints the device name and number of CUDA devices
+    available on the device.
+
+    Returns:
+        str: The device to run predictions on, either "cpu" or "cuda".
     """
     if not torch.cuda.is_available():
-        print(f'{constants.ANSI_ORANGE} Cuda not available in this device, will run predictions on CPU'
-              f'{constants.ANSI_RESET}')
+        print(f"{constants.ANSI_ORANGE}CUDA not available on this device. Predictions will be run on CPU.{constants.ANSI_RESET}")
         return "cpu"
     else:
         device_count = torch.cuda.device_count()
-        print(f'{constants.ANSI_GREEN} Cuda (no. of gpus: {device_count}) available in this device, will run '
-              f'predictions on GPU {constants.ANSI_RESET}')
+        print(f"{constants.ANSI_GREEN} CUDA is available on this device with {device_count} GPU(s). Predictions will be run on GPU.{constants.ANSI_RESET}")
         return "cuda"
```

### Comparing `moosez-2.0.9/moosez.egg-info/PKG-INFO` & `moosez-2.1.0/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.9
+Version: 2.1.0
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.0.9/setup.py` & `moosez-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.0.9',
+    version='2.1.0',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
@@ -44,15 +44,17 @@
         'mpire~=2.3.3',
         'openpyxl~=3.0.9',
         'matplotlib',
         'pyfiglet~=0.8.post1',
         'natsort~=8.1.0',
         'pillow>=9.2.0',
         'colorama~=0.4.6',
-        'rich'
+        'dask~=2023.6.0',
+        'rich',
+        'dicom2nifti~=2.4.8'
     ],
     entry_points={
         'console_scripts': [
             'moosez=moosez.moosez:main',
         ],
     },
 )
```

