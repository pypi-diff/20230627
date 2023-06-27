# Comparing `tmp/image_segmenter-0.1.1.tar.gz` & `tmp/image_segmenter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_segmenter-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "image_segmenter-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `image_segmenter-0.1.1.tar` & `image_segmenter-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     3238 2023-06-27 17:46:52.551846 image_segmenter-0.1.1/.gitignore
--rw-r--r--   0        0        0     1084 2023-06-27 17:49:01.418964 image_segmenter-0.1.1/LICENSE
--rw-r--r--   0        0        0     2450 2023-06-27 17:18:02.552909 image_segmenter-0.1.1/README.md
--rw-r--r--   0        0        0    10045 2023-06-27 18:20:28.265604 image_segmenter-0.1.1/image_segmenter.py
--rw-r--r--   0        0        0      613 2023-06-27 17:50:24.835137 image_segmenter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       32 2023-06-09 00:01:47.107516 image_segmenter-0.1.1/requirements.txt
--rw-r--r--   0        0        0     6260 2023-06-09 04:08:03.799087 image_segmenter-0.1.1/voc_writer.py
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 image_segmenter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-06-27 17:46:52.551846 image_segmenter-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1084 2023-06-27 17:49:01.418964 image_segmenter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2450 2023-06-27 17:18:02.552909 image_segmenter-0.2.0/README.md
+-rw-r--r--   0        0        0      104 2023-06-27 18:30:42.025604 image_segmenter-0.2.0/image_segmenter/__init__.py
+-rw-r--r--   0        0        0    10020 2023-06-27 18:29:21.725604 image_segmenter-0.2.0/image_segmenter/image_segmenter.py
+-rw-r--r--   0        0        0     6343 2023-06-27 18:29:25.975604 image_segmenter-0.2.0/image_segmenter/voc_writer.py
+-rw-r--r--   0        0        0      613 2023-06-27 17:50:24.835137 image_segmenter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-06-09 00:01:47.107516 image_segmenter-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 image_segmenter-0.2.0/PKG-INFO
```

### Comparing `image_segmenter-0.1.1/.gitignore` & `image_segmenter-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.1/LICENSE` & `image_segmenter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.1/README.md` & `image_segmenter-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.1/image_segmenter.py` & `image_segmenter-0.2.0/image_segmenter/image_segmenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 email: rich.baird@utah.edu
 homepage: rbaird.me
 repository: https://github.com/richbai90/image_annotator
 date: 2023-06-08
 description: A class for annotating images with bounding boxes using various image processing techniques.
 """
 
-__version__ = '0.1.1'
-
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 from os import path, listdir
 from .voc_writer import VOCWriter
 
 class ImageSegmenter:
```

### Comparing `image_segmenter-0.1.1/pyproject.toml` & `image_segmenter-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.1/voc_writer.py` & `image_segmenter-0.2.0/image_segmenter/voc_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import xml.etree.cElementTree as ET
 import numpy as np
 from os import path
 
+"""
+A module for writing VOC files for use with the ImageSegmenter class.
+"""
+
 # create an enum for the different bounding box formats
 class BBoxFmt():
     '''
     An enum for the different bounding box formats that can be used.
     
     Values
     ------
```

### Comparing `image_segmenter-0.1.1/PKG-INFO` & `image_segmenter-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: image_segmenter
-Version: 0.1.1
-Summary: author: Rich Baird
+Version: 0.2.0
+Summary: Image Segmenter
 Author-email: Rich Baird <rich@rbaird.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/richbai90/image_segmenter.git
 Project-URL: Repository, https://github.com/richbai90/image_segmenter.git
 
 # ImageSegmenter
```

