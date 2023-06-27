# Comparing `tmp/image_segmenter-0.1.0.tar.gz` & `tmp/image_segmenter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_segmenter-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "image_segmenter-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `image_segmenter-0.1.0.tar` & `image_segmenter-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3238 2023-06-27 17:46:52.551846 image_segmenter-0.1.0/.gitignore
--rw-r--r--   0        0        0     1084 2023-06-27 17:49:01.418964 image_segmenter-0.1.0/LICENSE
--rw-r--r--   0        0        0     2450 2023-06-27 17:18:02.552909 image_segmenter-0.1.0/README.md
--rw-r--r--   0        0        0    10044 2023-06-27 18:06:37.052294 image_segmenter-0.1.0/image_segmenter.py
--rw-r--r--   0        0        0      613 2023-06-27 17:50:24.835137 image_segmenter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-06-09 00:01:47.107516 image_segmenter-0.1.0/requirements.txt
--rw-r--r--   0        0        0     6260 2023-06-09 04:08:03.799087 image_segmenter-0.1.0/voc_writer.py
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 image_segmenter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-06-27 17:46:52.551846 image_segmenter-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1084 2023-06-27 17:49:01.418964 image_segmenter-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2450 2023-06-27 17:18:02.552909 image_segmenter-0.1.1/README.md
+-rw-r--r--   0        0        0    10045 2023-06-27 18:20:28.265604 image_segmenter-0.1.1/image_segmenter.py
+-rw-r--r--   0        0        0      613 2023-06-27 17:50:24.835137 image_segmenter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-06-09 00:01:47.107516 image_segmenter-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     6260 2023-06-09 04:08:03.799087 image_segmenter-0.1.1/voc_writer.py
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 image_segmenter-0.1.1/PKG-INFO
```

### Comparing `image_segmenter-0.1.0/.gitignore` & `image_segmenter-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.0/LICENSE` & `image_segmenter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.0/README.md` & `image_segmenter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.0/image_segmenter.py` & `image_segmenter-0.1.1/image_segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 email: rich.baird@utah.edu
 homepage: rbaird.me
 repository: https://github.com/richbai90/image_annotator
 date: 2023-06-08
 description: A class for annotating images with bounding boxes using various image processing techniques.
 """
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 from os import path, listdir
-from voc_writer import VOCWriter
+from .voc_writer import VOCWriter
 
 class ImageSegmenter:
     """
     A class for annotating images with bounding boxes using various image processing techniques.
     """
 
     def __init__(self):
```

### Comparing `image_segmenter-0.1.0/pyproject.toml` & `image_segmenter-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.0/voc_writer.py` & `image_segmenter-0.1.1/voc_writer.py`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.1.0/PKG-INFO` & `image_segmenter-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_segmenter
-Version: 0.1.0
+Version: 0.1.1
 Summary: author: Rich Baird
 Author-email: Rich Baird <rich@rbaird.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/richbai90/image_segmenter.git
 Project-URL: Repository, https://github.com/richbai90/image_segmenter.git
```

