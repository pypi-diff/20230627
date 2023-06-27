# Comparing `tmp/iza-0.0.3.tar.gz` & `tmp/iza-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iza-0.0.3.tar", last modified: Sun Jun 25 21:25:25 2023, max compression
+gzip compressed data, was "iza-0.0.5.tar", last modified: Tue Jun 27 21:35:10 2023, max compression
```

## Comparing `iza-0.0.3.tar` & `iza-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:25:25.463561 iza-0.0.3/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iza-0.0.3/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 iza-0.0.3/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-25 21:25:25.463426 iza-0.0.3/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1348 2023-06-24 20:51:36.000000 iza-0.0.3/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:25:25.461841 iza-0.0.3/iza/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-25 21:25:01.000000 iza-0.0.3/iza/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    13717 2023-06-25 21:25:01.000000 iza-0.0.3/iza/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2046 2023-06-25 21:25:01.000000 iza-0.0.3/iza/commands.py
--rw-r--r--   0 solst      (501) staff       (20)    14824 2023-06-25 21:25:01.000000 iza-0.0.3/iza/nbs.py
--rw-r--r--   0 solst      (501) staff       (20)     4983 2023-06-25 21:25:01.000000 iza-0.0.3/iza/plots.py
--rw-r--r--   0 solst      (501) staff       (20)      448 2023-06-25 21:25:01.000000 iza-0.0.3/iza/rich.py
--rw-r--r--   0 solst      (501) staff       (20)     8038 2023-06-25 21:25:01.000000 iza-0.0.3/iza/static.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-25 21:25:01.000000 iza-0.0.3/iza/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     3092 2023-06-25 21:25:01.000000 iza-0.0.3/iza/types.py
--rw-r--r--   0 solst      (501) staff       (20)    38180 2023-06-25 21:25:01.000000 iza-0.0.3/iza/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:25:25.463216 iza-0.0.3/iza.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      377 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       70 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 20:04:21.000000 iza-0.0.3/iza.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        4 2023-06-25 21:25:25.000000 iza-0.0.3/iza.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      816 2023-06-25 21:24:59.000000 iza-0.0.3/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 21:25:25.463605 iza-0.0.3/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-06-24 19:23:39.000000 iza-0.0.3/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 21:35:10.460799 iza-0.0.5/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iza-0.0.5/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 iza-0.0.5/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-27 21:35:10.460653 iza-0.0.5/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1348 2023-06-24 20:51:36.000000 iza-0.0.5/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 21:35:10.459148 iza-0.0.5/iza/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 21:34:57.000000 iza-0.0.5/iza/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    20748 2023-06-27 21:34:57.000000 iza-0.0.5/iza/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     2046 2023-06-27 21:34:57.000000 iza-0.0.5/iza/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)     2264 2023-06-27 21:34:57.000000 iza-0.0.5/iza/imp.py
+-rw-r--r--   0 solst      (501) staff       (20)    14824 2023-06-27 21:34:57.000000 iza-0.0.5/iza/nbs.py
+-rw-r--r--   0 solst      (501) staff       (20)     4983 2023-06-27 21:34:57.000000 iza-0.0.5/iza/plots.py
+-rw-r--r--   0 solst      (501) staff       (20)      448 2023-06-27 21:34:57.000000 iza-0.0.5/iza/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)     8171 2023-06-27 21:34:57.000000 iza-0.0.5/iza/static.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-27 21:34:57.000000 iza-0.0.5/iza/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     4383 2023-06-27 21:34:57.000000 iza-0.0.5/iza/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    54404 2023-06-27 21:34:57.000000 iza-0.0.5/iza/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 21:35:10.460424 iza-0.0.5/iza.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-27 21:35:10.000000 iza-0.0.5/iza.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      388 2023-06-27 21:35:10.000000 iza-0.0.5/iza.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 21:35:10.000000 iza-0.0.5/iza.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       70 2023-06-27 21:35:10.000000 iza-0.0.5/iza.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 20:04:21.000000 iza-0.0.5/iza.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       75 2023-06-27 21:35:10.000000 iza-0.0.5/iza.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        4 2023-06-27 21:35:10.000000 iza-0.0.5/iza.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      899 2023-06-27 21:34:55.000000 iza-0.0.5/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 21:35:10.460842 iza-0.0.5/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-06-24 19:23:39.000000 iza-0.0.5/setup.py
```

### Comparing `iza-0.0.3/LICENSE` & `iza-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iza-0.0.3/PKG-INFO` & `iza-0.0.5/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iza
-Version: 0.0.3
+Version: 0.0.5
 Summary: chaos package of utilities; a nod to izalith
 Home-page: https://github.com/dsm-72/iza
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iza-0.0.3/README.md` & `iza-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `iza-0.0.3/iza/commands.py` & `iza-0.0.5/iza/commands.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.3/iza/nbs.py` & `iza-0.0.5/iza/nbs.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.3/iza/plots.py` & `iza-0.0.5/iza/plots.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.3/iza/static.py` & `iza-0.0.5/iza/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
            'EXT_TXT', 'EXT_JSON', 'EXT_ZIP', 'EXT_IPYNB', 'SEED', 'ITEM', 'TIME', 'LABEL', 'SERIES', 'SAMPLES',
            'CONDITION', 'CONDITIONS', 'HVG', 'PCA', 'UMAP', 'TSNE', 'PHATE', 'MAGIC', 'CELL', 'BARCODE', 'BARCODES',
            'ID', 'MITO', 'RIBO', 'GENE', 'GENE_ID', 'GENE_IDS', 'GENE_SYMBOL', 'HIGHLY_VARIABLE', 'ENSEMBL',
            'ENSEMBL_ID', 'HUMAN', 'MOUSE', 'HUMAN_TF', 'MOUSE_TF', 'HUMAN_GENE_SYMBOL', 'HUMAN_ENSEMBLE_ID',
            'MOUSE_ENSEMBLE_ID', 'BATCH', 'TIMEPOINT', 'TOTAL_COUNTS', 'DOUBLET', 'DOUBLET_SCORES', 'PREDICTED_DOUBLETS',
            'PRENORM', 'DETECTED', 'SCALED_NORMALIZED', 'COUNTS', 'PCT', 'PERCENT', 'PCT_COUNTS', 'PCT_COUNTS_MITO',
            'PCT_COUNTS_RIBO', 'X', 'X_', 'X_PRENORM', 'X_DETECTED', 'X_SCALED_NORMALIZED', 'X_MAGIC', 'X_PCA',
-           'X_PCA_HVG', 'X_PHATE', 'X_PHATE_HVG', 'ADATA', 'MATRIX', 'FEATURES', 'SENSITIVITY', 'LINEAGE_ESC',
-           'LINEAGE_PREGERM', 'LINEAGE_NEURAL_CREST', 'LINEAGE_NEURAL_PROG', 'LINEAGE_ENDO', 'LINEAGE_MESO',
-           'LINEAGE_CARDIAC', 'LINEAGE_HEMA', 'LINEAGE_SOMITES', 'LINEAGE_TROPHOBLAST', 'LINEAGE_ALL', 'LINEAGE_NAMES',
-           'MARKERS_ESC', 'MARKERS_PREGERM', 'MARKERS_NEURAL_CREST', 'MARKERS_NEURAL_PROG', 'MARKERS_ENDO',
-           'MARKERS_MESO', 'MARKERS_CARDIAC', 'MARKERS_HEMA', 'MARKERS_SOMITES', 'MARKERS_TROPHOBLAST', 'MARKERS_LISTS',
-           'MARKERS_ALL', 'LINEAGE_MARKERS', 'RC_PARAMS']
+           'X_PCA_HVG', 'X_PHATE', 'X_PHATE_HVG', 'ADATA', 'MATRIX', 'FEATURES', 'SENSITIVITY',
+           'AMAZON_BUCKET_FLUENTBIO', 'LINEAGE_ESC', 'LINEAGE_PREGERM', 'LINEAGE_NEURAL_CREST', 'LINEAGE_NEURAL_PROG',
+           'LINEAGE_ENDO', 'LINEAGE_MESO', 'LINEAGE_CARDIAC', 'LINEAGE_HEMA', 'LINEAGE_SOMITES', 'LINEAGE_TROPHOBLAST',
+           'LINEAGE_ALL', 'LINEAGE_NAMES', 'MARKERS_ESC', 'MARKERS_PREGERM', 'MARKERS_NEURAL_CREST',
+           'MARKERS_NEURAL_PROG', 'MARKERS_ENDO', 'MARKERS_MESO', 'MARKERS_CARDIAC', 'MARKERS_HEMA', 'MARKERS_SOMITES',
+           'MARKERS_TROPHOBLAST', 'MARKERS_LISTS', 'MARKERS_ALL', 'LINEAGE_MARKERS', 'RC_PARAMS']
 
 # %% ../nbs/01_static.ipynb 5
 import os, sys, pkg_resources
 
 # %% ../nbs/01_static.ipynb 6
 '''----------------------------------------------------
 NOTE: RELATIVE DEFINITIONS
@@ -181,63 +181,66 @@
 # %% ../nbs/01_static.ipynb 27
 ADATA = 'adata'
 MATRIX = 'matrix'
 FEATURES = 'features'
 SENSITIVITY = 'sensitivity'
 
 # %% ../nbs/01_static.ipynb 29
-import itertools
+AMAZON_BUCKET_FLUENTBIO = 'https://fbs-public.s3.us-east-2.amazonaws.com'
 
 # %% ../nbs/01_static.ipynb 31
+import itertools
+
+# %% ../nbs/01_static.ipynb 33
 LINEAGE_ESC = 'esc'
 LINEAGE_PREGERM = 'pregerm'
 LINEAGE_NEURAL_CREST = 'neural_crest'
 LINEAGE_NEURAL_PROG = 'neural_prog'
 LINEAGE_ENDO = 'endo'
 LINEAGE_MESO = 'meso'
 LINEAGE_CARDIAC = 'cardiac'
 LINEAGE_HEMA = 'hema'
 LINEAGE_SOMITES = 'somites'
 LINEAGE_TROPHOBLAST = 'trophblast'
 LINEAGE_ALL = 'all'
 
-# %% ../nbs/01_static.ipynb 32
+# %% ../nbs/01_static.ipynb 34
 LINEAGE_NAMES = [
     LINEAGE_ESC, LINEAGE_PREGERM, LINEAGE_NEURAL_CREST,
     LINEAGE_NEURAL_PROG, LINEAGE_ENDO, LINEAGE_MESO,
     LINEAGE_CARDIAC, LINEAGE_HEMA, LINEAGE_SOMITES,
     LINEAGE_TROPHOBLAST, LINEAGE_ALL
 ]
 
-# %% ../nbs/01_static.ipynb 34
+# %% ../nbs/01_static.ipynb 36
 MARKERS_ESC = ['POU5F1', 'PRDM14', 'NANOG', 'SOX2', 'DPPA4', 'NR2F6', 'OTX2']
 MARKERS_PREGERM = ['TP53','NR6A1','GBX2','ZIC2','ZIC5']
 MARKERS_NEURAL_CREST = ['PAX3','FOXD3','ITGA4','EDNRB','SOX9','SOX10']
 MARKERS_NEURAL_PROG = ['NES','MAP2','PAX6','SOX1','ZBTB16','ONECUT1', 'ONECUT2','NR2F1','ISL1','NPAS1','EN2','SOX2','NEUROD1']
 MARKERS_ENDO = ['EOMES','FOXA2','SOX17','GATA4','GATA6','HHEX']
 MARKERS_MESO = ['MIXL1','CER1']
 MARKERS_CARDIAC = ['NKX2-5','GATA4','MYBPC2','TTN','TNNT2','MYH6','TBX5']
 MARKERS_HEMA = ['NKX2-5','TAL1','SOX17','CD34','PECAM1','CD69','CXCR4','CDH5','KDR','LMO2']
 MARKERS_SOMITES = ['WT1','TBX18','TBX15','PDGFRA','SIX2','TBX5']
 MARKERS_TROPHOBLAST = ['GATA3','TP63','ITGA6','CDH1']
 
-# %% ../nbs/01_static.ipynb 35
+# %% ../nbs/01_static.ipynb 37
 MARKERS_LISTS =  [
     MARKERS_ESC, MARKERS_PREGERM, MARKERS_NEURAL_CREST,
     MARKERS_NEURAL_PROG, MARKERS_ENDO, MARKERS_MESO, 
     MARKERS_CARDIAC, MARKERS_HEMA, MARKERS_SOMITES, 
     MARKERS_TROPHOBLAST,
 ]
 MARKERS_ALL = list(itertools.chain(*MARKERS_LISTS))
 MARKERS_LISTS.append(MARKERS_ALL)
 
-# %% ../nbs/01_static.ipynb 37
+# %% ../nbs/01_static.ipynb 39
 LINEAGE_MARKERS = dict(zip(LINEAGE_NAMES, MARKERS_LISTS))
 
-# %% ../nbs/01_static.ipynb 40
+# %% ../nbs/01_static.ipynb 42
 RC_PARAMS = {
     'axes.axisbelow': False,
     'axes.edgecolor': 'lightgrey',
     'axes.facecolor': 'None',
     'axes.grid': False,
     'axes.labelcolor': 'dimgrey',
     'axes.spines.right': False,
```

### Comparing `iza-0.0.3/iza/utils.py` & `iza-0.0.5/iza/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_utils.ipynb.
 
 # %% auto 0
-__all__ = ['isiter', 'allinstance', 'allsametype', 'isin', 'arein', 'str_just_alpha', 'str_just_numeric', 'strip_punc',
-           'filter_kwargs_for_func', 'filter_kwargs_for_class', 'wrangle_kwargs_for_func', 'wrangle_kwargs_for_class',
-           'get_user', 'collapse_user', 'check_ext', 'drop_ext', 'is_tar', 'is_gz', 'is_targz', 'is_tarball',
-           'filter_for_gz_files', 'get_gz_files_in_dir', 'decompress_tarball', 'decompress_gunzip', 'undo_gz',
-           'make_missing_dirs', 'dir_dirs', 'decompress_directory_of_gunzipped_files',
-           'decompress_tarball_of_gunzipped_files', 'stream_file', 'download_and_decompress_tarball_of_gunzipped_files',
-           'make_temp_file', 'Slice', 'Directory', 'is_matrix', 'undo_npmatrix', 'is_series', 'is_series_like', 'is_np',
-           'is_device', 'is_cpu', 'is_mps', 'is_tensor', 'is_torch', 'config_exp_logger', 'exp_log_filename',
-           'exp_param_filename', 'list_exps', 'gen_exp_name', 'load_exp_params', 'save_exp_params', 'setup_exp',
-           'is_config_subset', 'find_exps']
+__all__ = ['DecompressFunc', 'isiter', 'allinstance', 'allsametype', 'isin', 'arein', 'str_just_alpha', 'str_just_numeric',
+           'strip_punc', 'filter_kwargs_for_func', 'filter_kwargs_for_class', 'wrangle_kwargs_for_func',
+           'wrangle_kwargs_for_class', 'is_pathlib', 'is_pathlike', 'is_path', 'str_to_path', 'path_to_str',
+           'to_abs_expanded', 'sort_file_first', 'sort_directory_first', 'get_user', 'collapse_user', 'check_ext',
+           'drop_ext', 'is_tar', 'is_gz', 'is_targz', 'is_tarball', 'filter_for_gz_files', 'get_gz_files_in_dir',
+           'decompress_tarball', 'decompress_gunzip', 'undo_gz', 'RecursiveDecompressor', 'make_missing_dirs',
+           'dir_dirs', 'decompress_directory_of_gunzipped_files', 'decompress_tarball_of_gunzipped_files',
+           'stream_file', 'download_and_decompress_tarball_of_gunzipped_files', 'make_temp_file', 'urljoin', 'Slice',
+           'base_init_tree', 'rich_init_tree', 'init_tree', 'base_entry_fn', 'rich_entry_fn', 'entry_fn',
+           'walk_dir_tree', 'DirectoryTree', 'RichDirectory', 'Directory', 'is_matrix', 'undo_npmatrix', 'is_series',
+           'is_series_like', 'is_np', 'is_device', 'is_cpu', 'is_mps', 'is_tensor', 'is_torch', 'undo_sparse',
+           'to_ndarray', 'AdataExtractor', 'config_exp_logger', 'exp_log_filename', 'exp_param_filename', 'list_exps',
+           'gen_exp_name', 'load_exp_params', 'save_exp_params', 'setup_exp', 'is_config_subset', 'find_exps',
+           'ArchiveDownloader']
 
 # %% ../nbs/02_utils.ipynb 5
 import inspect, string
 from dataclasses import dataclass, field
 
 import numpy as np, pandas as pd
 
@@ -82,81 +86,131 @@
     # update with kwargs of our class
     params.update(kwargs or {})
     # filter for only the params that other class accepts
     params = filter_kwargs_for_class(cls, **params)
     return params
 
 # %% ../nbs/02_utils.ipynb 12
-import os, sys, pwd, atexit, tempfile, inspect
+import os, sys, pwd, atexit, tempfile, inspect, pathlib
 import requests, tarfile, gzip, shutil
-
+from dataclasses import dataclass, field
 from tqdm.auto import tqdm
 
-from typing import Optional, List, Union, Iterable, Tuple
+from typing import Optional, List, Union, Iterable, Tuple, Any, Callable
 
 # %% ../nbs/02_utils.ipynb 13
 from iza.static import (
     EXT_GZ, EXT_TAR, EXT_TAR_GZ,
 )
 
+from iza.types import (
+    PathType, PathLike
+)
+
 # %% ../nbs/02_utils.ipynb 15
+def is_pathlib(path:Any) -> bool:
+    """Check if the input is a path"""
+    return isinstance(path, PathType)
+
+def is_pathlike(path:Any) -> bool:
+    """Check if the input is a path"""
+    return isinstance(path, (PathLike))
+
+def is_path(path:Any, existance:Optional[bool]) -> bool:
+    """Check if the input is a path"""
+    exists_q = os.path.exists(os.path.expanduser(path))
+    return is_pathlike(path) and (exists_q if existance else True)
+
+def str_to_path(path:str) -> PathType:
+    """Convert a string to a pathlib.Path object"""
+    return pathlib.Path(path)
+
+def path_to_str(path: PathType) -> str:
+    """Convert a pathlib.Path object to a string"""
+    return os.fspath(path)
+
+def to_abs_expanded(dirname:Optional[PathLike]=None) -> PathType:
+    if dirname is None:
+        dirname = os.getcwd()
+
+    dirname = os.path.expanduser(dirname) 
+    dirname = os.path.abspath(dirname) 
+
+    if not is_pathlib(dirname):
+        dirname = pathlib.Path(dirname)
+
+    return dirname
+
+def sort_file_first(path: PathType):
+    return (not path.is_file(), path.name.lower())
+
+def sort_directory_first(path: PathType):
+    return (path.is_file(), path.name.lower())
+
+
+# %% ../nbs/02_utils.ipynb 17
 def get_user() -> str:
     user = pwd.getpwuid(os.getuid())[0]
     return user
 
 def collapse_user(path: str) -> str:
     _, rest = path.split(get_user())    
     return '~' + rest
 
-# %% ../nbs/02_utils.ipynb 17
+# %% ../nbs/02_utils.ipynb 19
 def check_ext(filename:str, extension:str) -> bool:
+    if is_pathlib(filename):
+        filename = path_to_str(filename)
     has_extension = extension in filename 
     splits = filename.split(extension)
     is_end_of_str = len(splits) >= 2 and splits[-1] == ''
     is_end_of_str = filename.endswith(extension)
     return has_extension and is_end_of_str
 
 def drop_ext(filename:str, extension:Optional[str]=None) -> str:
+    if is_pathlib(filename):
+        filename = path_to_str(filename)
+        
     file = os.path.basename(filename)
     if extension is None:
         file, *_ = file.split('.')
     else:
         file = filename.replace(extension, '')
     return os.path.join(os.path.dirname(filename), file)
 
-# %% ../nbs/02_utils.ipynb 18
+# %% ../nbs/02_utils.ipynb 20
 def is_tar(filename:str) -> bool:
     return check_ext(filename, EXT_TAR)
 
 def is_gz(filename:str) -> bool:
     return check_ext(filename, EXT_GZ)
 
 def is_targz(filename:str) -> bool:
     return check_ext(filename, EXT_TAR_GZ)
 
 def is_tarball(filename:str) -> bool:
     return is_tar(filename) or is_targz(filename)
 
 
-# %% ../nbs/02_utils.ipynb 19
+# %% ../nbs/02_utils.ipynb 21
 def filter_for_gz_files(files:List[str]) -> List[str]:
     return list(filter(lambda f: is_gz(f), files))
 
 def get_gz_files_in_dir(dirname:str) -> List[str]:
     all_files = []
 
     for (root, dirs, files) in os.walk(dirname):   
         fullpaths = [os.path.join(root, file) for file in files]
         all_files.extend(fullpaths)
     
     gz_files = filter_for_gz_files(all_files)
     return gz_files
 
-# %% ../nbs/02_utils.ipynb 21
-def decompress_tarball(filename:str) -> Tuple[str, Optional[EOFError]]:
+# %% ../nbs/02_utils.ipynb 23
+def decompress_tarball(filename:str, remove:bool=False) -> Tuple[str, Optional[EOFError]]:
     '''
     Returns
     -------
         dirname : str
             The name of the archive e.g. `~/Downloads/fluentbio.tar.gz` would
             yield `~/Downloads/fluentbio`
 
@@ -164,22 +218,27 @@
     Notes
     -----
     FluentBio has a weird gzip so it complains when it is 
         actually fine
     '''
     error = None
     decompress_dir = os.path.dirname(filename)
-    dirname = drop_ext(filename, EXT_TAR_GZ)
+    ext = EXT_TAR_GZ if is_targz(filename) else EXT_TAR if is_tar(filename) else EXT_GZ
+
+    dirname = drop_ext(filename, ext)
     try:
         with tarfile.open(filename) as tarball:
             tarball.extractall(decompress_dir)
             tarball.close()
 
     except EOFError as error:
         pass
+    
+    if os.path.isdir(dirname) and remove:
+        os.remove(filename)
 
     return dirname, error
 
 
 def decompress_gunzip(filename:str, remove:bool=False) -> Tuple[str, Optional[EOFError]]:
     '''
     Returns
@@ -204,36 +263,121 @@
         pass
 
     if os.path.isfile(decompressed_file) and remove:
         os.remove(filename)
 
     return decompressed_file, error
 
-def undo_gz(filename: str) -> str:
-    if is_gz(filename):
-        filename, _ = decompress_gunzip(filename, remove=True)
+def undo_gz(filename: str, remove:bool=False) -> str:
+    if is_targz(filename):
+        filename, _ = decompress_tarball(filename, remove)
+    elif is_gz(filename):
+        filename, _ = decompress_gunzip(filename, remove)
+    elif is_tar(filename):
+        pass
     elif is_tarball(filename):
-        filename, _ = decompress_tarball(filename)
+        filename, _ = decompress_tarball(filename, remove)
     return filename
 
-# %% ../nbs/02_utils.ipynb 23
+# %% ../nbs/02_utils.ipynb 24
+DecompressFunc = Callable[[str, bool], str]
+
+@dataclass
+class RecursiveDecompressor:
+    dirname: PathType
+    entries: Optional[List[str]] = field(default_factory=list, repr=False)
+    strategy: Optional[DecompressFunc] = field(default=undo_gz, repr=False)
+    remove: Optional[bool] = field(default=True, repr=False)
+    progress: Optional[Any] = field(default=None, repr=False, init=True)
+
+    total: Optional[int] = field(default=None, repr=False, init=False)
+    done: Optional[int] = field(default=None, repr=False, init=False)
+    task: Optional[Any] = field(default=None, repr=False, init=False)
+
+    def __post_init__(self):
+        if not is_pathlib(self.dirname): 
+            self.dirname = pathlib.Path(self.dirname)
+            
+        if self.entries is None: 
+            self.entries = os.listdir(self.dirname)
+
+        self.done = 0
+        self.total = len(self.entries)
+
+    def execute(self):
+        return self.decompress()
+
+    def update_total(self, increment: int):
+        self.total += increment
+        if self.progress is not None:
+            self.progress.update(self.task, total=self.total)
+        else:
+            self.tqdm_bar.total = self.total
+            self.tqdm_bar.refresh()
+
+    def decrease_total(self):
+        self.total -= 1
+        if self.progress is not None:
+            self.progress.update(self.task, total=self.total)
+        else:
+            self.tqdm_bar.total = self.total
+            self.tqdm_bar.refresh()
+
+    def decompress(self):
+        files = [self.dirname / entry for entry in self.entries]
+
+        if self.progress is not None:
+            with self.progress:
+                self.task = self.progress.add_task("[cyan]Extracting...", total=self.total)
+                for file in files:
+                    self.recurse(file)
+                    self.progress.advance(self.task)
+        else:
+            with tqdm(total=self.total, desc='Extracting') as self.tqdm_bar:
+                for file in files:
+                    self.recurse(file)
+                    self.tqdm_bar.update()
+
+    def recurse(self, current:PathLike):
+        filename = path_to_str(current)
+        nextfile = self.strategy(filename, self.remove)
+        self.done += 1
+        nextfile = pathlib.Path(nextfile)
+        
+        # If the decompressed file is a directory, recursively decompress it
+        if nextfile.is_dir():
+            for root, dirs, files in os.walk(nextfile):
+                for f in files:
+                    self.update_total(1)
+                    self.recurse(pathlib.Path(root) / f)
+                    
+        elif self.remove:
+            if filename in self.entries:
+                self.entries.remove(filename)
+            self.decrease_total()
+
+
+# %% ../nbs/02_utils.ipynb 26
 def make_missing_dirs(dirs:List[str]):
     if isinstance(dirs, str):
         dirs = [dirs]
         
+    elif is_pathlib(dirs):
+        dirs = [dirs]
+        
     for d in dirs:
         if not os.path.exists(d):
             os.makedirs(d)
             
 def dir_dirs(dirname:str) -> List[str]:
     entries = os.listdir(dirname)
     is_subdir = lambda e : os.path.isdir(os.path.join(dirname, e))
     return list(filter(is_subdir, entries))
 
-# %% ../nbs/02_utils.ipynb 24
+# %% ../nbs/02_utils.ipynb 27
 def decompress_directory_of_gunzipped_files(
     dirname:str, desc:Optional[str]=None, remove:Optional[bool]=False
 ) -> None:
     if desc is None:
         desc = dirname.split('/')[-1]
 
     gz_files = get_gz_files_in_dir(dirname)
@@ -249,15 +393,15 @@
 
     if desc is None:
         desc = dirname.split('/')[-1]
 
     # NOTE: decompress all internal .gz files
     decompress_directory_of_gunzipped_files(dirname, desc, remove)
 
-# %% ../nbs/02_utils.ipynb 26
+# %% ../nbs/02_utils.ipynb 29
 def stream_file(uri:str, filename:Optional[str]=None, desc:Optional[str]=None) -> None:
     '''
     Parameters
     ----------
     uri : str
         The URI to download
 
@@ -283,15 +427,15 @@
     with tqdm.wrapattr(
         open(filename, 'wb'), 'write', 
         miniters=1, desc=desc, total=total
     ) as fout:
         for chunk in response.iter_content(chunk_size=4096):
             fout.write(chunk)
 
-# %% ../nbs/02_utils.ipynb 28
+# %% ../nbs/02_utils.ipynb 31
 def download_and_decompress_tarball_of_gunzipped_files(
     uri:str, download_dir:str=None, desc:Optional[str]=None, remove:Optional[bool]=False
 ):
     filename = os.path.basename(uri)
     fullpath = os.path.join(download_dir, filename)
 
     if desc is None:
@@ -303,29 +447,36 @@
 
     if desc is None:
         description = f'Decompressing {filename}'
     # NOTE: filtered_matrix.tar.gz --> filtered_matrix/**/file.tsv
     decompress_tarball_of_gunzipped_files(fullpath, desc, remove)
 
 
-# %% ../nbs/02_utils.ipynb 30
+# %% ../nbs/02_utils.ipynb 33
 def make_temp_file(**kwargs: Any) -> tempfile.NamedTemporaryFile:
     temp = tempfile.NamedTemporaryFile(**kwargs)
     @atexit.register
     def delete_temp() -> None:
         temp.close()
     return temp
 
-# %% ../nbs/02_utils.ipynb 32
+# %% ../nbs/02_utils.ipynb 35
+from urllib3.util.url import parse_url
+
+# %% ../nbs/02_utils.ipynb 36
+def urljoin(*parts: str) -> str:
+    return parse_url('/'.join(s.strip('/') for s in parts)).url
+
+# %% ../nbs/02_utils.ipynb 38
 from dataclasses import dataclass, field
 import numpy as np, pandas as pd
 
 from typing import List, Union, Tuple
 
-# %% ../nbs/02_utils.ipynb 35
+# %% ../nbs/02_utils.ipynb 41
 @dataclass
 class Slice:
     """A class for representing a slice and providing conversion to other formats."""
     slc: slice = field(default_factory=slice)
 
     @property
     def start(self):
@@ -412,111 +563,202 @@
             return self.totuple()
         elif dtype in {'dict', dict}:
             return self.todict()
         elif dtype in {'slice', slice}:
             return self.toslice()
         return self
 
-# %% ../nbs/02_utils.ipynb 37
-import os
+# %% ../nbs/02_utils.ipynb 43
+import os, pathlib 
 from pathlib import Path
 from dataclasses import dataclass, field, KW_ONLY
-from typing import Optional, List, ClassVar
+from typing import Optional, List, ClassVar, Any, TypeAlias, Callable
+from enum import StrEnum
 
-# %% ../nbs/02_utils.ipynb 40
-@dataclass
-class Directory:
-    dirname: str
+# %% ../nbs/02_utils.ipynb 44
+from iza.types import (
+    PathLike, PathType,
+    DirectoryTreeStrings, TreeEntryFunc,
+    RichTree, RichText, RichConsole, RichProgress
+)
+from .static import EXT_PY
 
-    _: KW_ONLY
-    _SPACE : ClassVar[str] = '    '
-    _BRANCH: ClassVar[str] = '│   '    
-    _TEE   : ClassVar[str] = '├── '
-    _LAST  : ClassVar[str] = '└── '
+#| export
+from .imp import RichImp
+from ipos.imp import is_mod, is_var_imp, Module, Imp
 
-        
-    def make_tree(self, dirname:Path, prefix:str=''):
-        '''
-        A recursive generator, given a directory Path object
-        will yield a visual tree structure line by line
-        with each line prefixed by the same characters
-        Notes
-        -----
-        Adapted from https://stackoverflow.com/a/59109706/5623899
-        '''
+# %% ../nbs/02_utils.ipynb 45
+try:    
+    from rich.tree import Tree
+    from rich.text import Text    
+    from rich.filesize import decimal
+    from rich import get_console
+    from rich.console import Console
+    from rich.progress import Progress
+
+except ImportError:
+    Tree = None
+    Text = None 
+    Progress = None
 
-        contents = list(dirname.iterdir())
-        # NOTE: contents each get pointers that are ├── with a final └── :
-        pointers = [self._TEE] * (len(contents) - 1) + [self._LAST]
-        for pointer, path in zip(pointers, contents):
-            yield f'{prefix}{pointer}{path.name}'
-
-            # NOTE: extend the prefix and recurse:
-            if path.is_dir(): 
-                # NOTE: space because last, └── , above so no more |
-                extension = self._BRANCH if pointer == self._TEE else self._SPACE 
-                
-                yield from self.make_tree(path, prefix=f'{prefix}{extension}')
+# %% ../nbs/02_utils.ipynb 49
+def base_init_tree(dirname: str):
+    return None
 
-    def get_tree_lines(self, dirname:Optional[str]=None) -> List[str]:
-        dirname = self.prepare_dirname(dirname)
-        tree = self.make_tree(dirname)
-        lines = [line for line in tree]
-        return lines
+def rich_init_tree(dirname):
+    return Tree(f'[link file://{dirname}]{dirname}', guide_style='bold bright_blue')
 
-    def make_tree_str(self, dirname:Optional[str]=None) -> str:
-        dirname = self.prepare_dirname(dirname)
-        lines = self.get_tree_lines(dirname)
-        tree_str = '\n'.join([str(dirname), *lines])
-        return tree_str
-        
-    def prepare_dirname(self, dirname:Optional[str]=None) -> Path:
-        if dirname is None:
-            dirname = self.dirname
+def init_tree(dirname):
+    try:
+        return rich_init_tree(dirname)
+    except:
+        return base_init_tree(dirname)
+
+# %% ../nbs/02_utils.ipynb 51
+def base_entry_fn(path:Path, prefix:str='', pointer:str='', suffix:str='') -> str:
+    name = path.name
+    return f'{prefix}{pointer}{name}{suffix}'
+
+def rich_entry_fn(path:Path, prefix:str='', pointer:str='', suffix:str='') -> str:
+    text = Text(path.name)
+    size = decimal(path.stat().st_size)
+    text.stylize(f'link file://{path}')
+    text.append(f' ({size})', 'cyan')
+    return text
 
-        dirname = os.path.expanduser(dirname) 
-        dirname = os.path.abspath(dirname) 
+def entry_fn(path:Path, prefix:str='', pointer:str='', suffix:str='') -> str:
+    try:
+        return rich_entry_fn(path, prefix, pointer, suffix)
+    except:
+        return base_entry_fn(path, prefix, pointer, suffix)
 
-        if not isinstance(dirname, Path):
-            dirname = Path(dirname)
 
-        return dirname
+# %% ../nbs/02_utils.ipynb 53
+def walk_dir_tree(
+    dirname: PathLike, 
+    prefix: str = '',
+    hidden: Optional[bool] = False, 
+    tree: Optional[RichTree] = None,
+    entry_fn: TreeEntryFunc = entry_fn,
+):    
+    '''
+    A recursive generator, given a directory Path object
+    will yield a visual tree structure line by line
+    with each line prefixed by the same characters
+    Notes
+    -----
+    Adapted from https://stackoverflow.com/a/59109706/5623899
+    '''
+    # NOTE: sort_directory_first, to_abs_expanded, rich_file defined in _02_utils/_08_modules.ipynb
+    dirname = Path(to_abs_expanded(dirname))
+    contents = sorted(Path(dirname).iterdir(), key=sort_directory_first)
+    
+    SPACE, BRANCH, TEE, LAST = DirectoryTreeStrings
+    pointers = [TEE] * (len(contents) - 1) + [LAST]
+    
+    for pointer, path in zip(pointers, contents):
+        # Remove hidden files
+        if path.name.startswith('.') and not hidden:
+            continue
+        
+        name = entry_fn(path, prefix, pointer, suffix='')
+        yield name
+        
+        branch = None
+        if tree is not None:
+            branch = tree.add(entry_fn(path))
+    
+        if path.is_dir():
+            # NOTE: space because last, └── , above so no more |
+            extension = BRANCH if pointer == TEE else SPACE
+            yield from walk_dir_tree(path, prefix=f'{prefix}{extension}', hidden=hidden, tree=branch, entry_fn=entry_fn)
 
-    def print(self, dirname:Optional[str]=None) -> None:
-        dirname = self.prepare_dirname(dirname)
-        tree_str = self.make_tree_str(dirname)
+# %% ../nbs/02_utils.ipynb 55
+@dataclass
+class DirectoryTree:
+    dirname: str
+    
+    hidden: Optional[bool] = False
+    entry_fn: Optional[TreeEntryFunc] = field(default=entry_fn)
+    tree: Optional[RichTree] = field(init=False, default=None)
+    
+    def __post_init__(self):
+        # NOTE: defined in _02_utils/_01_files.ipynb
+        self.dirname = Path(to_abs_expanded(self.dirname))
+        if self.tree is None:
+            self.tree = init_tree(self.dirname)
+
+    def tree_generator(self):
+        yield from walk_dir_tree(
+            self.dirname, hidden=self.hidden, 
+            tree=self.tree, entry_fn=self.entry_fn
+        )
+        
+    def get_tree_lines(self) -> List[str]:        
+        tree_gen = self.tree_generator()
+        lines = [line for line in tree_gen]
+        return lines
+    
+    def make_tree_str(self) -> str:        
+        lines = self.get_tree_lines()
+        tree_str = '\n'.join([str(self.dirname), *lines])
+        return tree_str
+   
+    def print(self) -> None:        
+        tree_str = self.make_tree_str()        
         print(tree_str)
         return
 
-    def __repr__(self):
-        dirname = self.dirname
-        dirname = self.prepare_dirname(dirname)
-        tree_str = self.make_tree_str(dirname)        
-        return tree_str        
+    def __repr__(self):        
+        tree_str = self.make_tree_str()        
+        return tree_str  
+
+# %% ../nbs/02_utils.ipynb 56
+@dataclass
+class RichDirectory(DirectoryTree):
+    _: KW_ONLY
+    console: Optional[RichConsole] = field(default_factory=Console, init=True, repr=False)    
+    _imp: Imp = field(default_factory=RichImp, init=False, repr=False)
+    def __post_init__(self):
+        super().__post_init__()
+        self._imp = RichImp()
+    
+        if self.console is None and is_mod(self._imp._module):
+            self.console = get_console()
+
+    def print_rich(self) -> None:    
+        lines = self.get_tree_lines()
+        self.console.print(self.tree)
 
-# %% ../nbs/02_utils.ipynb 42
+# %% ../nbs/02_utils.ipynb 57
+@dataclass
+class Directory(DirectoryTree):
+    dirname: PathLike
+    pass
+
+# %% ../nbs/02_utils.ipynb 59
 import os
 from pathlib import Path
 from dataclasses import dataclass, field, KW_ONLY
 from typing import Optional, List, ClassVar
 
-# %% ../nbs/02_utils.ipynb 44
+# %% ../nbs/02_utils.ipynb 61
 import pandas as pd
 
-# %% ../nbs/02_utils.ipynb 45
+# %% ../nbs/02_utils.ipynb 62
 from iza.static import (
     ADATA, MATRIX, BARCODES, FEATURES, EXT_H5, EXT_MTX, EXT_TSV,
     GENE_SYMBOL, ENSEMBL_ID
 )
 from iza.types import (
     AnnData
 )
 from tqdm.auto import tqdm
 
-# %% ../nbs/02_utils.ipynb 46
+# %% ../nbs/02_utils.ipynb 63
 try: 
     import scanpy as sc, scprep
 
     # NOTE: Directory defined in _02_utils/_02_directory.ipynb
     @dataclass
     class FilterMatrixDirectory(Directory):
         _: KW_ONLY
@@ -606,15 +848,15 @@
                             matrix, columns=features.index, index = barcodes.index
                         )
                         del matrix
 
                     case 'adata':
                         adata = sc.AnnData(X=data.values, obs=barcodes, var=features, dtype='float32')
                         adata.write(self.adata_filename)
-
+                        
                     case _:
                         pass
 
             return adata
 
         def get_adata(self) -> AnnData:
             adata = sc.read_h5ad(self.adata_filename)
@@ -631,23 +873,23 @@
         
 
         def __post_init__(self):    
             raise ImportError('FilterMatrixDirectory requires scprep and scanpy to be installed')
         
     pass
 
-# %% ../nbs/02_utils.ipynb 48
+# %% ../nbs/02_utils.ipynb 65
 import os
 import numpy as np, pandas as pd
 from typing import Optional, List, ClassVar, Any
 
-# %% ../nbs/02_utils.ipynb 49
+# %% ../nbs/02_utils.ipynb 66
 from .types import Tensor, Device, SeriesLike, ndarray
 
-# %% ../nbs/02_utils.ipynb 52
+# %% ../nbs/02_utils.ipynb 69
 def is_matrix(arr: SeriesLike) -> bool:
     '''
     Checks whether or not `arr` is a np.matrix
     
     Parameters
     ----------    
     arr : SeriesLike
@@ -727,15 +969,15 @@
     Returns
     -------
     result : bool
     '''
     return isinstance(arr_q, ndarray)
 
 
-# %% ../nbs/02_utils.ipynb 53
+# %% ../nbs/02_utils.ipynb 70
 def is_device(device_q: Device) -> bool:
     '''
     Checks whether or not `device_q` is a valid
     pytorch device type.
     
     Parameters
     ----------    
@@ -822,25 +1064,60 @@
     
     See Also
     --------
     is_tensor
     '''
     return is_tensor(tensor_q)
 
-# %% ../nbs/02_utils.ipynb 55
+# %% ../nbs/02_utils.ipynb 71
+def undo_sparse(arr: SeriesLike) -> SeriesLike:  
+    '''
+    Given a arr tries to make it a dense array
+    
+    Parameters
+    ----------    
+    arr : SeriesLike
+        
+    
+    Returns
+    -------
+    arr : ndarray
+    '''
+    if hasattr(arr, 'toarray'):
+        arr = arr.toarray()
+
+    if hasattr(arr, 'todense'):
+        arr = arr.todense()
+
+    return arr
+
+def to_ndarray(arr):
+    if is_np(arr):
+        return arr
+        
+    arr = undo_npmatrix(arr)
+    
+    arr = undo_sparse(arr)
+
+    if not is_np(arr):
+        arr = np.array(arr)
+
+    return arr
+
+# %% ../nbs/02_utils.ipynb 73
 import os, random
 import numpy as np
 
 from dataclasses import dataclass, field, KW_ONLY
 from typing import Optional, List, ClassVar, Any
 
-# %% ../nbs/02_utils.ipynb 56
+# %% ../nbs/02_utils.ipynb 74
 from .types import Tensor, Device, SeriesLike, ndarray
 
-# %% ../nbs/02_utils.ipynb 58
+# %% ../nbs/02_utils.ipynb 76
 try:
     import torch
     def ensure_device(device: Device) -> Device:
         '''
         Given a valid device type attempts to instantiant 
         a pytorch device object i.e. `device='cpu'` will
         return `torch.device('cpu')`.
@@ -1110,15 +1387,15 @@
     coerce_mps_dtype = lambda dtype, device, assume_on_mps: dtype
     ensure_mps_dtype = identity
     move_to = lambda tensor, other, dtype, do_dtype: tensor
     pass
 
 
 
-# %% ../nbs/02_utils.ipynb 59
+# %% ../nbs/02_utils.ipynb 77
 try:
     import torch, pytorch_lightning as pl
     def set_seeds(seed: int) -> None:
         '''
         Calls a bunch of seed functions with `seed`
         
         Parameters
@@ -1130,18 +1407,110 @@
         np.random.seed(seed)    
         pl.seed_everything(seed)
 except ImportError as err:
      def set_seeds(seed: int) -> None:
          random.seed(seed)
          np.random.seed(seed)
 
-# %% ../nbs/02_utils.ipynb 61
+# %% ../nbs/02_utils.ipynb 79
+from dataclasses import dataclass, field
+import numpy as np, pandas as pd
+
+from typing import List, Any, Optional
+
+# %% ../nbs/02_utils.ipynb 80
+from .types import AnnData, ndarray, DataFrame
+from .static import X_MAGIC, PHATE, X_PHATE
+
+# %% ../nbs/02_utils.ipynb 82
+@dataclass
+class AdataExtractor:
+    adata: AnnData
+    layer: Optional[str] = X_MAGIC
+    x_emb: Optional[str] = X_PHATE
+
+    dim_str: Optional[str] = None
+    use_hvg: Optional[bool] = True
+
+    @property
+    def has_hvg(self):
+        return hasattr(self.adata, 'var') and hasattr(self.adata.var, 'highly_variable')
+    
+    @property
+    def has_emb(self):
+        return hasattr(self.adata, 'obsm') and self.x_emb in self.adata.obsm.keys()
+
+    def get_layer(self) -> ndarray:
+        layer = self.sdata().layers.get(self.layer, None)
+
+        if layer is None:
+            layer = self.sdata().X
+
+        if hasattr(layer, 'toarray'):
+            layer = layer.toarray()
+
+        if hasattr(layer, 'todense'):
+            layer = layer.todense()
+
+        return layer
+    
+    def get_emb(self) -> ndarray:
+        emb = self.sdata().obsm.get(self.x_emb, None)
+        if emb is None:
+            raise ValueError(f'No embedding found in adata.obsm {self.sdata().obsm.keys()}')
+
+        # NOTE: defined in _02_utils/_05_guards.ipynb
+        emb = to_ndarray(emb)
+        return emb
+
+    @property
+    def axis_str(self):
+        if self.dim_str:
+            return self.dim_str
+        return self.x_emb.replace('X_', '').upper()
+    
+    @property
+    def emb_cols(self):
+        ndim = self.get_emb().shape[1]
+        cols = [f'{self.axis_str}_{i+1}' for i in range(ndim)]
+        return cols
+        
+    def sdata(self):
+        if self.use_hvg and self.has_hvg:
+            return self.adata[:, self.adata.var.highly_variable]
+        return self.adata
+    
+    def get_df_cnt(self) -> DataFrame:
+        layer = self.get_layer()
+
+        cols = self.sdata().var.index
+        idxs = self.sdata().obs.index
+        df = pd.DataFrame(layer, index=idxs, columns=cols)
+        return df
+    
+    def get_df_emb(self) -> DataFrame:
+        emb = self.get_emb()
+        
+        cols = self.emb_cols
+        idxs = self.sdata().obs.index
+        df = pd.DataFrame(emb, index=idxs, columns=cols)
+        return df
+    
+    @property
+    def df_cnt(self):
+        return self.get_df_cnt()
+    
+    @property
+    def df_emb(self):
+        return self.get_df_emb()
+
+# %% ../nbs/02_utils.ipynb 85
 import os, yaml, datetime, logging
 
-# %% ../nbs/02_utils.ipynb 62
+# %% ../nbs/02_utils.ipynb 86
 def config_exp_logger(path):
     '''
     Arguments:
     ----------
         path (str): full path to experiment, i.e. 
             `<path-to-experiments-dir>/<experiment-timestamp>`
     Returns:
@@ -1302,7 +1671,166 @@
     results = []
     for exp in exps:
         exp_name = os.path.join(path, exp)
         exp_params = load_exp_params(exp_param_filename(exp_name))
         if is_config_subset(exp_params, params):
             results.append(exp)
     return results
+
+# %% ../nbs/02_utils.ipynb 88
+import os, pathlib, itertools
+from pathlib import Path
+from dataclasses import dataclass, field, KW_ONLY
+from typing import Optional, List, ClassVar, Any, TypeAlias, Union
+
+from ipos.imp import is_mod, is_var_imp, Module
+
+# %% ../nbs/02_utils.ipynb 89
+from iza.types import (
+    PathLike, PathType,
+    RichConsole, RichProgress, RichText, RichTree
+)
+from .static import EXT_PY
+from .imp import RichImp
+
+# %% ../nbs/02_utils.ipynb 93
+@dataclass
+class ArchiveDownloader:    
+    _: KW_ONLY
+    rootdir: str
+    archive: str
+    entries: Union[str, list[str]]
+    savedir: str
+    extract: bool = False
+    cleanup: bool = False
+    compound_archive: bool = False
+    archives: Optional[list[str]] = None
+    console: Optional[RichConsole] = None
+    progress: Optional[RichProgress] = None
+
+    _rich: Module = field(init=False, repr=False, default=None)
+    has_rich: bool = field(init=False, repr=False, default=None)
+
+    
+
+    def __post_init__(self):    
+        r = RichImp()
+        self._rich = r._module
+        self.has_rich = is_mod(self._rich)
+
+        self.entries = self.entries if isinstance(self.entries, list) else [self.entries]        
+        self.console = get_console()        
+        self.progress = self.get_progress()
+    
+        self.savedir = Path(self.savedir).expanduser()
+        make_missing_dirs(self.savedir)
+
+    def get_progress(self):
+        progress = getattr(self, 'progress', None)
+        if progress is not None:
+            return progress
+
+        if self.has_rich and is_var_imp('Progress'):
+                self.progress = Progress(console=self.console)
+                return self.progress
+
+        return None
+
+    @property
+    def path(self) -> str:
+        return urljoin(self.rootdir, self.archive)
+
+    @property
+    def urls(self) -> list[str]:
+        urls = []
+        if self.compound_archive and self.archives is not None:
+            for archive, entry in itertools.product(self.archives, self.entries):
+                urls.append(urljoin(self.rootdir, archive, entry))
+        else:
+            urls = [urljoin(self.path, entry) for entry in self.entries]
+        return urls
+
+    def download_missing_files(self) -> None:        
+        total_files = len(self.urls)
+        if self.has_rich and self.progress:
+            with self.progress:
+                task = self.progress.add_task("[cyan]Downloading...", total=total_files)
+                for url in self.urls:
+                    filename = Path(parse_url(url).path).name
+                    fullpath = self.savedir / filename
+                    if not fullpath.exists():
+                        stream_file(url, str(fullpath))
+                        self.progress.advance(task)
+                    else:
+                        self.progress.advance(task)
+        else:            
+            for url in tqdm(self.urls, desc='Downloading'):       
+                filename = Path(parse_url(url).path).name
+                fullpath = self.savedir / filename
+                if not fullpath.exists():
+                    stream_file(url, str(fullpath))
+                
+
+    def calc_n_to_extract(self) -> int:
+        files = [self.savedir / entry for entry in self.entries]
+        files = get_gz_files_in_dir(self.savedir)
+        total = 0
+        for file in files:
+            if is_tarball(file):
+                total += 1
+            elif is_gz(file):
+                total += 1
+        return total                
+
+    def extract_files(self) -> None:
+        recurser = RecursiveDecompressor(
+            dirname=self.savedir, 
+            entries=self.entries,
+            strategy=undo_gz,
+            remove=self.cleanup,             
+            progress=self.progress
+        )
+        recurser.decompress()
+        return
+        files = [self.savedir / entry for entry in self.entries]
+        files = get_gz_files_in_dir(self.savedir)
+        total = self.calc_n_to_extract()
+        if self.has_rich and self.progress:
+            with self.progress:
+                task = self.progress.add_task("[cyan]Extracting...", total=total)
+                for file in files:
+                    undo_gz(file, remove=self.cleanup)                    
+                    self.progress.advance(task)
+        else:
+            for file in tqdm(files, desc='Extracting'):
+                undo_gz(file, remove=self.cleanup)
+
+    def execute(self) -> None:
+        if self.has_rich and self.console:
+            self.console.print(f"Processing archive: [bold cyan]{self.archive}[/bold cyan]")
+        else:
+            print(f"Processing archive: {self.archive}")
+
+        self.download_missing_files()
+        if self.extract:
+            self.extract_files()
+
+        if self.has_rich and self.console:
+            dir = RichDirectory(self.savedir, console=self.console)
+            dir.print_rich()
+        else:
+            dir = Directory(self.savedir)
+            dir.print()
+
+# %% ../nbs/02_utils.ipynb 97
+#| eval: False
+try:
+    import typer
+    app = typer.Typer()
+
+    @app.command()
+    def download(rootdir: str, archive: str, entries: List[str], savedir: str, extract: bool = False, cleanup: bool = False):
+        downloader = ArchiveDownloader(rootdir, archive, entries, savedir, extract, cleanup)
+        downloader.execute()
+
+except ImportError:
+    pass
```

### Comparing `iza-0.0.3/iza.egg-info/PKG-INFO` & `iza-0.0.5/iza.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iza
-Version: 0.0.3
+Version: 0.0.5
 Summary: chaos package of utilities; a nod to izalith
 Home-page: https://github.com/dsm-72/iza
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iza-0.0.3/settings.ini` & `iza-0.0.5/settings.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = iza
 lib_name = iza
-version = 0.0.3
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = iza
 nbs_path = nbs
 recursive = True
@@ -30,8 +30,9 @@
 console_scripts = iza=iza.commands:app
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
+requirements = pandas seaborn scikit-learn numpy nbformat rich typer requests tqdm
```

### Comparing `iza-0.0.3/setup.py` & `iza-0.0.5/setup.py`

 * *Files identical despite different names*

