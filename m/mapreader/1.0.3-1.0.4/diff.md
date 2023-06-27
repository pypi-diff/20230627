# Comparing `tmp/mapreader-1.0.3.tar.gz` & `tmp/mapreader-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapreader-1.0.3.tar", last modified: Wed Jun 21 14:25:47 2023, max compression
+gzip compressed data, was "mapreader-1.0.4.tar", last modified: Tue Jun 27 11:21:23 2023, max compression
```

## Comparing `mapreader-1.0.3.tar` & `mapreader-1.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-21 14:25:35.000000 mapreader-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-21 14:25:47.145010 mapreader-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-21 14:25:35.000000 mapreader-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/mapreader/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 14:25:47.145010 mapreader-1.0.3/mapreader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.137010 mapreader-1.0.3/mapreader/annotate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/annotate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.141010 mapreader-1.0.3/mapreader/classify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73307 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    27268 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/classifier_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/custom_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28572 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/load_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.141010 mapreader-1.0.3/mapreader/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38174 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/tile_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/tile_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.141010 mapreader-1.0.3/mapreader/load/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/load/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86859 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/load/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/load/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/mapreader/process/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/process/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/mapreader/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/utils/compute_and_save_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/utils/slice_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.137010 mapreader-1.0.3/mapreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:25:46.000000 mapreader-1.0.3/mapreader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 14:25:47.145010 mapreader-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-21 14:25:35.000000 mapreader-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-21 14:25:35.000000 mapreader-1.0.3/tests/test_annotations_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-21 14:25:35.000000 mapreader-1.0.3/tests/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-21 14:25:35.000000 mapreader-1.0.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-06-21 14:25:35.000000 mapreader-1.0.3/tests/test_sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-21 14:25:35.000000 mapreader-1.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.185683 mapreader-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-27 11:21:07.000000 mapreader-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-27 11:21:23.185683 mapreader-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-27 11:21:07.000000 mapreader-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.185683 mapreader-1.0.4/mapreader/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 11:21:23.185683 mapreader-1.0.4/mapreader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.181683 mapreader-1.0.4/mapreader/annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/annotate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.181683 mapreader-1.0.4/mapreader/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73307 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/classify/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27268 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/classify/classifier_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/classify/custom_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28572 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/classify/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/classify/load_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.181683 mapreader-1.0.4/mapreader/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/download/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/download/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38345 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/download/sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/download/tile_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/download/tile_merging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.185683 mapreader-1.0.4/mapreader/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/load/geo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87045 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/load/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/load/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.185683 mapreader-1.0.4/mapreader/process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/process/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.185683 mapreader-1.0.4/mapreader/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/utils/compute_and_save_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-27 11:21:07.000000 mapreader-1.0.4/mapreader/utils/slice_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.181683 mapreader-1.0.4/mapreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-27 11:21:23.000000 mapreader-1.0.4/mapreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-27 11:21:23.000000 mapreader-1.0.4/mapreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:21:23.000000 mapreader-1.0.4/mapreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 11:21:23.000000 mapreader-1.0.4/mapreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:21:22.000000 mapreader-1.0.4/mapreader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-27 11:21:23.000000 mapreader-1.0.4/mapreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 11:21:23.000000 mapreader-1.0.4/mapreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-27 11:21:23.185683 mapreader-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-27 11:21:07.000000 mapreader-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:21:23.185683 mapreader-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-27 11:21:07.000000 mapreader-1.0.4/tests/test_annotations_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-27 11:21:07.000000 mapreader-1.0.4/tests/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 11:21:07.000000 mapreader-1.0.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-06-27 11:21:07.000000 mapreader-1.0.4/tests/test_sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-27 11:21:07.000000 mapreader-1.0.4/versioneer.py
```

### Comparing `mapreader-1.0.3/LICENSE` & `mapreader-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/PKG-INFO` & `mapreader-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.0.3
+Version: 1.0.4
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.0.3 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.0.4 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `mapreader-1.0.3/README.md` & `mapreader-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/__init__.py` & `mapreader-1.0.4/mapreader/__init__.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/annotate/utils.py` & `mapreader-1.0.4/mapreader/annotate/utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/classify/classifier.py` & `mapreader-1.0.4/mapreader/classify/classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/classify/classifier_context.py` & `mapreader-1.0.4/mapreader/classify/classifier_context.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/classify/custom_models.py` & `mapreader-1.0.4/mapreader/classify/custom_models.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/classify/datasets.py` & `mapreader-1.0.4/mapreader/classify/datasets.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/classify/load_annotations.py` & `mapreader-1.0.4/mapreader/classify/load_annotations.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/download/data_structures.py` & `mapreader-1.0.4/mapreader/download/data_structures.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/download/downloader.py` & `mapreader-1.0.4/mapreader/download/downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/download/downloader_utils.py` & `mapreader-1.0.4/mapreader/download/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/download/sheet_downloader.py` & `mapreader-1.0.4/mapreader/download/sheet_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 import os
 from typing import Union, Optional
 from shapely.geometry import Polygon, LineString, Point, shape
 from shapely.ops import unary_union
-from .data_structures import Coordinate, GridBoundingBox
 from .tile_loading import TileDownloader, DEFAULT_TEMP_FOLDER
 from .tile_merging import TileMerger
-from .downloader_utils import get_coordinate_from_index, get_grid_bb_from_polygon, get_polygon_from_grid_bb
+from .downloader_utils import get_grid_bb_from_polygon, get_polygon_from_grid_bb
 import re
 import matplotlib.pyplot as plt
 # import cartopy.crs as ccrs - would be good to get this fixed (i think by conda package)
 import numpy as np
 import pandas as pd
 import shutil
 from functools import reduce
 from pyproj.crs import CRS
+import matplotlib.image as mpimg
 
 
 
 class SheetDownloader:
     """
     A class to download map sheets using metadata.
     """
@@ -470,17 +470,22 @@
         -------
         bool
             True if file exists, False if not.
         """
         map_name = str("map_" + feature["properties"]["IMAGE"])        
         path_save = self.merger.output_folder
         if os.path.exists(f"{path_save}{map_name}.png"):
-            print(f'[INFO] "{path_save}{map_name}.png" already exists. Skipping download.')
-            return True
+            try:
+                mpimg.imread(f"{path_save}{map_name}.png")
+                print(f'[INFO] "{path_save}{map_name}.png" already exists. Skipping download.')
+                return True
+            except OSError:
+                return False
         return False
+            
 
     def _download_map(self, feature: dict) -> bool:
         """
         Downloads a single map sheet and saves as png file.
 
         Parameters
         ----------
@@ -500,22 +505,27 @@
             print(f'[WARNING] Download of "{map_name}.png" was unsuccessfull.')
         
         shutil.rmtree(DEFAULT_TEMP_FOLDER)
         return success
 
     def _save_metadata(
         self, 
-        feature: dict
-    ) -> list:
+        feature: dict,
+        out_filepath: str,
+    ) -> None:
         """
-        Creates list of selected metadata items.
+        Creates list of selected metadata items and saves to a csv file.
+        If file exists, metadata list is appended.
 
         Parameters
         ----------
         feature : dict
+            The feature for which to extract the metadata from
+        out_filepath : str
+            The path to save metadata csv.
 
         Returns
         -------
         list
             List of selected metadata (to be saved)
         """
 
@@ -531,33 +541,28 @@
 
         #use grid_bb to get coords of actually downloaded tiles
         polygon = get_polygon_from_grid_bb(grid_bb)
         coords = polygon.bounds
 
         crs = self.crs
 
-        return [map_name, map_url, coords, crs, published_date, grid_bb]
-
-    def _create_metadata_df(self, metadata_to_save: list, out_filepath) -> None:
-        """
-        Creates metadata datframe from list of ``metadata_to_save`` and saves as csv.
-
-        Parameters
-        ----------
-        metadata_to_save : list
-            List of metadata to save
-        out_filepath : _type_
-            File path where metadata csv will be saved.
-        """
-        metadata_df = pd.DataFrame(
+        metadata_to_save = [map_name, map_url, coords, crs, published_date, grid_bb]
+        new_metadata_df = pd.DataFrame(
             metadata_to_save,
-            columns=["name", "url", "coordinates", "crs", "published_date", "grid_bb"],
-        )
-        exists = True if os.path.exists(out_filepath) else False
-        metadata_df.to_csv(out_filepath, sep="\t", mode="a", header=not exists)
+            index=["name", "url", "coordinates", "crs", "published_date", "grid_bb"],
+        ).T
+        
+        if os.path.exists(out_filepath):
+            existing_metadata_df = pd.read_csv(out_filepath, sep="\t", index_col=0)
+            metadata_df = pd.concat([existing_metadata_df, new_metadata_df], ignore_index=True)
+            metadata_df.drop_duplicates(subset=["grid_bb"], keep="first", inplace=True)
+        else: 
+            metadata_df = new_metadata_df
+        
+        metadata_df.to_csv(out_filepath, sep="\t")
 
     def _download_map_sheets(self, features: list, path_save: Optional[str] = "maps", metadata_fname: Optional[str] = "metadata.csv", overwrite: Optional[bool] = False):
         """Download map sheets from a list of features.
 
         Parameters
         ----------
         features : list
@@ -566,25 +571,22 @@
             Path to save map sheets, by default "maps"
         metadata_fname : str, optional
             Name to use for metadata file, by default "metadata.csv"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
         """
 
-        metadata_to_save = []
         for feature in features:
             if not overwrite:
                 if self._check_map_sheet_exists(feature):
                     continue
             success = self._download_map(feature)
             if success:
-                metadata_to_save.append(self._save_metadata(feature))
-
-        metadata_path = f"{path_save}/{metadata_fname}"
-        self._create_metadata_df(metadata_to_save, metadata_path)
+                metadata_path = f"{path_save}/{metadata_fname}"
+                self._save_metadata(feature, metadata_path)
 
     def download_all_map_sheets(
         self, path_save: Optional[str] = "maps", metadata_fname: Optional[str] = "metadata.csv", overwrite: Optional[bool] = False,
     ) -> None:
         """
         Downloads all map sheets in metadata.
 
@@ -600,15 +602,15 @@
         if not self.grid_bbs:
             raise ValueError("[ERROR] Please first run ``get_grid_bb()``")
 
         self._initialise_downloader()
         self._initialise_merger(path_save)
 
         features = self.features
-        self._download_map_sheets(features, path_save, metadata_fname)
+        self._download_map_sheets(features, path_save, metadata_fname, overwrite)
 
     def download_map_sheets_by_wfs_ids(
         self,
         wfs_ids: Union[list, int],
         path_save: Optional[str] = "maps",
         metadata_fname: Optional[str] = "metadata.csv",
         overwrite: Optional[bool] = False,
```

### Comparing `mapreader-1.0.3/mapreader/download/tile_loading.py` & `mapreader-1.0.4/mapreader/download/tile_loading.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/download/tile_merging.py` & `mapreader-1.0.4/mapreader/download/tile_merging.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/load/geo_utils.py` & `mapreader-1.0.4/mapreader/load/geo_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/load/images.py` & `mapreader-1.0.4/mapreader/load/images.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,18 +631,21 @@
         Notes
         -----
         The shape of the image is obtained by loading the image from its
         ``image_path`` value and getting its shape.
         """
         tree_level = self._get_tree_level(image_id)
 
-        myimg = mpimg.imread(self.images[tree_level][image_id]["image_path"])
-        # shape = (hwc)
-        myimg_shape = myimg.shape
-        self.images[tree_level][image_id]["shape"] = myimg_shape
+        try: 
+            myimg = mpimg.imread(self.images[tree_level][image_id]["image_path"])
+            # shape = (hwc)
+            myimg_shape = myimg.shape
+            self.images[tree_level][image_id]["shape"] = myimg_shape
+        except OSError:
+            raise ValueError(f'[ERROR] Problem with "{image_id}". Please either redownload or remove from list of images to load.')
 
     def _add_coord_increments_id(
         self, image_id: Union[int, str], verbose: Optional[bool] = False
     ) -> None:
         """
         Add pixel-wise delta longitute (``dlon``) and delta latititude
         (``dlat``) to the metadata of the image with the specified ``image_id``
```

### Comparing `mapreader-1.0.3/mapreader/load/loader.py` & `mapreader-1.0.4/mapreader/load/loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/process/process.py` & `mapreader-1.0.4/mapreader/process/process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/utils/compute_and_save_stats.py` & `mapreader-1.0.4/mapreader/utils/compute_and_save_stats.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader/utils/slice_parallel.py` & `mapreader-1.0.4/mapreader/utils/slice_parallel.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader.egg-info/PKG-INFO` & `mapreader-1.0.4/mapreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.0.3
+Version: 1.0.4
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.0.3 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.0.4 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `mapreader-1.0.3/mapreader.egg-info/SOURCES.txt` & `mapreader-1.0.4/mapreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/mapreader.egg-info/requires.txt` & `mapreader-1.0.4/mapreader.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/setup.py` & `mapreader-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/tests/test_annotations_loader.py` & `mapreader-1.0.4/tests/test_annotations_loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/tests/test_classifier.py` & `mapreader-1.0.4/tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/tests/test_import.py` & `mapreader-1.0.4/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/tests/test_sheet_downloader.py` & `mapreader-1.0.4/tests/test_sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.3/versioneer.py` & `mapreader-1.0.4/versioneer.py`

 * *Files identical despite different names*

