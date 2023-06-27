# Comparing `tmp/pybw-23.6.26.tar.gz` & `tmp/pybw-23.6.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybw-23.6.26.tar", last modified: Mon Jun 26 16:13:04 2023, max compression
+gzip compressed data, was "pybw-23.6.27.1.tar", last modified: Tue Jun 27 04:53:21 2023, max compression
```

## Comparing `pybw-23.6.26.tar` & `pybw-23.6.27.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.083360 pybw-23.6.26/
--rw-rw-rw-   0        0        0      577 2023-03-14 13:35:46.000000 pybw-23.6.26/- command.txt
--rw-rw-rw-   0        0        0     1167 2023-03-13 12:06:00.000000 pybw-23.6.26/LICENSE
--rw-rw-rw-   0        0        0       17 2023-03-13 14:36:52.000000 pybw-23.6.26/MANIFEST.in
--rw-rw-rw-   0        0        0      754 2023-06-26 16:13:04.081359 pybw-23.6.26/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-03-13 12:06:00.000000 pybw-23.6.26/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:03.901716 pybw-23.6.26/pybw/
--rw-rw-rw-   0        0        0        0 2023-03-13 14:57:12.000000 pybw-23.6.26/pybw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:03.952348 pybw-23.6.26/pybw/ccnb_mod/
--rw-rw-rw-   0        0        0        0 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.011352 pybw-23.6.26/pybw/ccnb_mod/bvseLi/
--rw-rw-rw-   0        0        0    22034 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVAnalysis.py
--rw-rw-rw-   0        0        0    24506 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py
--rw-rw-rw-   0        0        0     5071 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVSEParam.dat
--rw-rw-rw-   0        0        0    25155 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/Structure.py
--rw-rw-rw-   0        0        0     9177 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.037354 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/
--rw-rw-rw-   0        0        0    14330 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc
--rw-rw-rw-   0        0        0    15658 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc
--rw-rw-rw-   0        0        0    22032 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc
--rw-rw-rw-   0        0        0     8727 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    45065 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/bvmparam.dat
--rw-rw-rw-   0        0        0    31592 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/bvse.dat
--rw-rw-rw-   0        0        0     6681 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/elements.dat
--rw-rw-rw-   0        0        0     7678 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/temp.py
--rw-rw-rw-   0        0        0    17720 2023-03-18 14:08:38.000000 pybw-23.6.26/pybw/ccnb_mod/ccnb_mod.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.043356 pybw-23.6.26/pybw/core/
--rw-rw-rw-   0        0        0     2551 2023-06-26 15:51:36.000000 pybw-23.6.26/pybw/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.051356 pybw-23.6.26/pybw/scholar/
--rw-rw-rw-   0        0        0     1714 2023-04-10 07:40:49.000000 pybw-23.6.26/pybw/scholar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.066357 pybw-23.6.26/pybw/tricks/
--rw-rw-rw-   0        0        0      114 2023-06-26 15:52:27.000000 pybw-23.6.26/pybw/tricks/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-06-26 15:54:12.000000 pybw-23.6.26/pybw/tricks/lazy_import.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:03.837711 pybw-23.6.26/pybw/utils/
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.073358 pybw-23.6.26/pybw/utils/pymatgen/
--rw-rw-rw-   0        0        0     7582 2023-03-14 13:35:46.000000 pybw-23.6.26/pybw/utils/pymatgen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:03.937347 pybw-23.6.26/pybw.egg-info/
--rw-rw-rw-   0        0        0      754 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      963 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       15 2023-03-13 12:06:00.000000 pybw-23.6.26/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 16:13:04.083360 pybw-23.6.26/setup.cfg
--rw-rw-rw-   0        0        0     3052 2023-06-26 16:01:11.000000 pybw-23.6.26/setup.py
--rwxrwxrwx   0        0        0      357 2023-06-26 16:12:48.000000 pybw-23.6.26/upload_pypi.bat
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:21.033726 pybw-23.6.27.1/
+-rw-rw-rw-   0        0        0      577 2023-03-14 13:35:46.000000 pybw-23.6.27.1/- command.txt
+-rw-rw-rw-   0        0        0     1167 2023-03-13 12:06:00.000000 pybw-23.6.27.1/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-03-13 14:36:52.000000 pybw-23.6.27.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      756 2023-06-27 04:53:21.032727 pybw-23.6.27.1/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-03-13 12:06:00.000000 pybw-23.6.27.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:20.880715 pybw-23.6.27.1/pybw/
+-rw-rw-rw-   0        0        0        0 2023-03-13 14:57:12.000000 pybw-23.6.27.1/pybw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:20.920718 pybw-23.6.27.1/pybw/ccnb_mod/
+-rw-rw-rw-   0        0        0        0 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:20.971721 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/
+-rw-rw-rw-   0        0        0    22034 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/BVAnalysis.py
+-rw-rw-rw-   0        0        0    24506 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py
+-rw-rw-rw-   0        0        0     5071 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/BVSEParam.dat
+-rw-rw-rw-   0        0        0    25155 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/Structure.py
+-rw-rw-rw-   0        0        0     9177 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:20.997742 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/
+-rw-rw-rw-   0        0        0    14330 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc
+-rw-rw-rw-   0        0        0    15658 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc
+-rw-rw-rw-   0        0        0    22032 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8727 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    45065 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/bvmparam.dat
+-rw-rw-rw-   0        0        0    31592 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/bvse.dat
+-rw-rw-rw-   0        0        0     6681 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/elements.dat
+-rw-rw-rw-   0        0        0     7678 2023-04-04 04:49:42.000000 pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/temp.py
+-rw-rw-rw-   0        0        0    17720 2023-03-18 14:08:38.000000 pybw-23.6.27.1/pybw/ccnb_mod/ccnb_mod.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:21.002741 pybw-23.6.27.1/pybw/core/
+-rw-rw-rw-   0        0        0     2551 2023-06-26 15:51:36.000000 pybw-23.6.27.1/pybw/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:21.007727 pybw-23.6.27.1/pybw/scholar/
+-rw-rw-rw-   0        0        0     1714 2023-04-10 07:40:49.000000 pybw-23.6.27.1/pybw/scholar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:21.017725 pybw-23.6.27.1/pybw/tricks/
+-rw-rw-rw-   0        0        0      114 2023-06-26 15:52:27.000000 pybw-23.6.27.1/pybw/tricks/__init__.py
+-rw-rw-rw-   0        0        0     1118 2023-06-27 04:52:33.000000 pybw-23.6.27.1/pybw/tricks/lazy_import.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:20.834713 pybw-23.6.27.1/pybw/utils/
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:21.026726 pybw-23.6.27.1/pybw/utils/pymatgen/
+-rw-rw-rw-   0        0        0     7582 2023-03-14 13:35:46.000000 pybw-23.6.27.1/pybw/utils/pymatgen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:53:20.908716 pybw-23.6.27.1/pybw.egg-info/
+-rw-rw-rw-   0        0        0      756 2023-06-27 04:53:20.000000 pybw-23.6.27.1/pybw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2023-06-27 04:53:20.000000 pybw-23.6.27.1/pybw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 04:53:20.000000 pybw-23.6.27.1/pybw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-27 04:53:20.000000 pybw-23.6.27.1/pybw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-06-27 04:53:20.000000 pybw-23.6.27.1/pybw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       15 2023-03-13 12:06:00.000000 pybw-23.6.27.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 04:53:21.034727 pybw-23.6.27.1/setup.cfg
+-rw-rw-rw-   0        0        0     3054 2023-06-27 04:53:09.000000 pybw-23.6.27.1/setup.py
+-rwxrwxrwx   0        0        0      364 2023-06-26 16:13:53.000000 pybw-23.6.27.1/upload_pypi.bat
```

### Comparing `pybw-23.6.26/- command.txt` & `pybw-23.6.27.1/- command.txt`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/LICENSE` & `pybw-23.6.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/PKG-INFO` & `pybw-23.6.27.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybw
-Version: 23.6.26
+Version: 23.6.27.1
 Summary: pybw
 Home-page: https://gitee.com/pubowei/pybw
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/pybw
 Project-URL: Package, https://pypi.org/project/pybw
```

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVAnalysis.py` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/BVAnalysis.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVSEParam.dat` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/BVSEParam.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/Structure.py` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/Structure.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__init__.py` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__init__.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/bvmparam.dat` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/bvmparam.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/bvse.dat` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/bvse.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/elements.dat` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/elements.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/bvseLi/temp.py` & `pybw-23.6.27.1/pybw/ccnb_mod/bvseLi/temp.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/ccnb_mod/ccnb_mod.py` & `pybw-23.6.27.1/pybw/ccnb_mod/ccnb_mod.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/core/__init__.py` & `pybw-23.6.27.1/pybw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/scholar/__init__.py` & `pybw-23.6.27.1/pybw/scholar/__init__.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw/tricks/lazy_import.py` & `pybw-23.6.27.1/pybw/tricks/lazy_import.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from joblib import Parallel, delayed
 # from func_timeout import func_set_timeout, func_timeout
 
 
 ## ------ Data Analysis ------
 import re
 import random
+import json
+import yaml
 import numpy as np
 try:
     import pandas as pd
 except:
     pass
 try:
     import polars as pl
@@ -40,14 +42,15 @@
 # plt.rcParams['axes.unicode_minus'] = False
 plt.ion()
 # import scienceplots
 plt.style.use('ggplot')
 
 import seaborn as sns
 
+
 ## ------ Scientific Calculation ------
 import math
 from decimal import Decimal
 
 
 ## ------ Audio Video ------
 # from moviepy.editor import VideoFileClip, AudioFileClip
```

### Comparing `pybw-23.6.26/pybw/utils/pymatgen/__init__.py` & `pybw-23.6.27.1/pybw/utils/pymatgen/__init__.py`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/pybw.egg-info/PKG-INFO` & `pybw-23.6.27.1/pybw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybw
-Version: 23.6.26
+Version: 23.6.27.1
 Summary: pybw
 Home-page: https://gitee.com/pubowei/pybw
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/pybw
 Project-URL: Package, https://pypi.org/project/pybw
```

### Comparing `pybw-23.6.26/pybw.egg-info/SOURCES.txt` & `pybw-23.6.27.1/pybw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybw-23.6.26/setup.py` & `pybw-23.6.27.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name='pybw',
-    version='23.6.26',
+    version='23.6.27.1',
     python_requires='>=3.6',
     
     author='Bowei Pu',
     author_email='pubowei@foxmail.com',
     
     description='pybw',
     long_description=readme,
```

