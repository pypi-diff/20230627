# Comparing `tmp/ncem-0.1.4.tar.gz` & `tmp/ncem-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncem-0.1.4.tar", max compression
+gzip compressed data, was "ncem-0.1.5.tar", max compression
```

## Comparing `ncem-0.1.4.tar` & `ncem-0.1.5.tar`

### file list

```diff
@@ -1,49 +1,74 @@
--rw-r--r--   0        0        0     1517 2022-08-08 13:33:23.518990 ncem-0.1.4/LICENSE
--rw-r--r--   0        0        0     2709 2022-08-08 13:33:23.518990 ncem-0.1.4/README.rst
--rw-r--r--   0        0        0      375 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/__init__.py
--rw-r--r--   0        0        0      271 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/__main__.py
--rw-r--r--   0        0        0       52 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/api/__init__.py
--rw-r--r--   0        0        0      416 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/api/train/__init__.py
--rw-r--r--   0        0        0   157285 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/data.py
--rw-r--r--   0        0        0      719 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/__init__.py
--rw-r--r--   0        0        0   100682 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/base_estimator.py
--rw-r--r--   0        0        0     9932 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/base_estimator_neighbors.py
--rw-r--r--   0        0        0     6811 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/estimator_cvae.py
--rw-r--r--   0        0        0     8603 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/estimator_cvae_ncem.py
--rw-r--r--   0        0        0    10372 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/estimator_deconvolution.py
--rw-r--r--   0        0        0     3901 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/estimator_ed.py
--rw-r--r--   0        0        0     9817 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/estimator_ed_ncem.py
--rw-r--r--   0        0        0    10816 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/estimator_interactions.py
--rw-r--r--   0        0        0     9745 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/estimators/estimator_linear.py
--rw-r--r--   0        0        0      457 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/interpretation/__init__.py
--rw-r--r--   0        0        0    81545 2022-08-08 13:33:23.530991 ncem-0.1.4/ncem/interpretation/interpreter.py
--rw-r--r--   0        0        0      455 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/__init__.py
--rw-r--r--   0        0        0     2075 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/custom_callbacks.py
--rw-r--r--   0        0        0     1001 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/layers/__init__.py
--rw-r--r--   0        0        0     3692 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/layers/gnn_layers.py
--rw-r--r--   0        0        0    21947 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/layers/layer_stacks_lvm.py
--rw-r--r--   0        0        0    18334 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/layers/output_layers.py
--rw-r--r--   0        0        0     1989 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/layers/preproc_input.py
--rw-r--r--   0        0        0     7015 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/layers/single_gnn_layers.py
--rw-r--r--   0        0        0     9174 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/model_cvae.py
--rw-r--r--   0        0        0    14813 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/model_cvae_ncem.py
--rw-r--r--   0        0        0     5971 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/model_ed.py
--rw-r--r--   0        0        0    10541 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/model_ed_ncem.py
--rw-r--r--   0        0        0     6211 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/model_ed_single_ncem.py
--rw-r--r--   0        0        0     4677 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/model_interactions.py
--rw-r--r--   0        0        0     4484 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/models/model_linear.py
--rw-r--r--   0        0        0        0 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/py.typed
--rw-r--r--   0        0        0      387 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/train/__init__.py
--rw-r--r--   0        0        0    58685 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/train/summaries.py
--rw-r--r--   0        0        0    10122 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/train/train_model.py
--rw-r--r--   0        0        0      532 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/unit_test/directories.py
--rw-r--r--   0        0        0     1900 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/unit_test/test_dataloader_local.py
--rw-r--r--   0        0        0     9160 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/unit_test/test_estimator_local.py
--rw-r--r--   0        0        0     3104 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/utils/losses.py
--rw-r--r--   0        0        0     6713 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/utils/metrics.py
--rw-r--r--   0        0        0      278 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/utils/ols_fit.py
--rw-r--r--   0        0        0      916 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/utils/sparse.py
--rw-r--r--   0        0        0     1987 2022-08-08 13:33:23.534991 ncem-0.1.4/ncem/utils/wald_test.py
--rw-r--r--   0        0        0     1813 2022-08-08 13:33:23.534991 ncem-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4066 2022-08-08 13:33:31.403226 ncem-0.1.4/setup.py
--rw-r--r--   0        0        0     3894 2022-08-08 13:33:31.403626 ncem-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-06-27 16:06:44.912943 ncem-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2709 2023-06-27 16:06:44.912943 ncem-0.1.5/README.rst
+-rw-r--r--   0        0        0      375 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/__main__.py
+-rw-r--r--   0        0        0       52 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/api/__init__.py
+-rw-r--r--   0        0        0      446 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/api/train/__init__.py
+-rw-r--r--   0        0        0   157232 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/data.py
+-rw-r--r--   0        0        0      768 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/__init__.py
+-rw-r--r--   0        0        0   101048 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/base_estimator.py
+-rw-r--r--   0        0        0     9842 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/base_estimator_neighbors.py
+-rw-r--r--   0        0        0     6811 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/estimator_cvae.py
+-rw-r--r--   0        0        0     8603 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/estimator_cvae_ncem.py
+-rw-r--r--   0        0        0    10368 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/estimator_deconvolution.py
+-rw-r--r--   0        0        0     3901 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/estimator_ed.py
+-rw-r--r--   0        0        0     9818 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/estimator_ed_ncem.py
+-rw-r--r--   0        0        0    10810 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/estimator_interactions.py
+-rw-r--r--   0        0        0     9745 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/estimators/estimator_linear.py
+-rw-r--r--   0        0        0      457 2023-06-27 16:06:44.924944 ncem-0.1.5/ncem/interpretation/__init__.py
+-rw-r--r--   0        0        0    80734 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/interpretation/interpreter.py
+-rw-r--r--   0        0        0      455 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/__init__.py
+-rw-r--r--   0        0        0     2075 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/custom_callbacks.py
+-rw-r--r--   0        0        0     1007 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/layers/__init__.py
+-rw-r--r--   0        0        0     3692 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/layers/gnn_layers.py
+-rw-r--r--   0        0        0    21947 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/layers/layer_stacks_lvm.py
+-rw-r--r--   0        0        0    18334 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/layers/output_layers.py
+-rw-r--r--   0        0        0     1989 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/layers/preproc_input.py
+-rw-r--r--   0        0        0     7468 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/layers/single_gnn_layers.py
+-rw-r--r--   0        0        0     9256 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/model_cvae.py
+-rw-r--r--   0        0        0    14895 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/model_cvae_ncem.py
+-rw-r--r--   0        0        0     5994 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/model_ed.py
+-rw-r--r--   0        0        0    10564 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/model_ed_ncem.py
+-rw-r--r--   0        0        0     6277 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/model_ed_single_ncem.py
+-rw-r--r--   0        0        0     4677 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/model_interactions.py
+-rw-r--r--   0        0        0     4484 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/models/model_linear.py
+-rw-r--r--   0        0        0      142 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/pl/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/pl/ablation.py
+-rw-r--r--   0        0        0     2596 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/pl/input.py
+-rw-r--r--   0        0        0     7550 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/pl/type_couplings.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/py.typed
+-rw-r--r--   0        0        0      496 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/__init__.py
+-rw-r--r--   0        0        0       29 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/__init__.py
+-rw-r--r--   0        0        0     3225 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/ablation.py
+-rw-r--r--   0        0        0    16856 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/design_matrix.py
+-rw-r--r--   0        0        0    12689 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/linear_model.py
+-rw-r--r--   0        0        0      435 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/ols_fit.py
+-rw-r--r--   0        0        0    14293 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/spline_model.py
+-rw-r--r--   0        0        0     8529 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/testing.py
+-rw-r--r--   0        0        0      534 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/utils.py
+-rw-r--r--   0        0        0     2267 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/backend/vardecomp.py
+-rw-r--r--   0        0        0     2074 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/constants.py
+-rw-r--r--   0        0        0      477 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/glm/__init__.py
+-rw-r--r--   0        0        0        7 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/tf/__init__.py
+-rw-r--r--   0        0        0        7 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/tl/fit/torch/__init__.py
+-rw-r--r--   0        0        0      459 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/train/__init__.py
+-rw-r--r--   0        0        0    59745 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/train/summaries.py
+-rw-r--r--   0        0        0    10192 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/train/train_model.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/__init__.py
+-rw-r--r--   0        0        0     2554 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/data_for_tests.py
+-rw-r--r--   0        0        0      532 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/directories.py
+-rw-r--r--   0        0        0     1976 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/test_dataloader_local.py
+-rw-r--r--   0        0        0     9253 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/test_estimator_local.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/tools/fit/__init__.py
+-rw-r--r--   0        0        0     5755 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/tools/fit/test_glm.py
+-rw-r--r--   0        0        0     5238 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/unit_test/tools/fit/test_spline.py
+-rw-r--r--   0        0        0      426 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/utils/_utils.py
+-rw-r--r--   0        0        0     3104 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/utils/losses.py
+-rw-r--r--   0        0        0     6709 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/utils/metrics.py
+-rw-r--r--   0        0        0      213 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/utils/ols_fit.py
+-rw-r--r--   0        0        0      916 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/utils/sparse.py
+-rw-r--r--   0        0        0     2060 2023-06-27 16:06:44.928943 ncem-0.1.5/ncem/utils/wald_test.py
+-rw-r--r--   0        0        0     1913 2023-06-27 16:06:44.932944 ncem-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4010 1970-01-01 00:00:00.000000 ncem-0.1.5/PKG-INFO
```

### Comparing `ncem-0.1.4/LICENSE` & `ncem-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/README.rst` & `ncem-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/data.py` & `ncem-0.1.5/ncem/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import abc
+import os
 import warnings
 from collections import OrderedDict
-import os
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import matplotlib.colors as colors
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import seaborn as sns
 import squidpy as sq
 from anndata import AnnData, read_h5ad
 from diffxpy.testing.correction import correct
 from matplotlib.ticker import FormatStrFormatter
 from matplotlib.tri import Triangulation
 from omnipath.interactions import import_intercell_network
-from pandas import read_csv, read_excel, DataFrame
+from pandas import DataFrame, read_csv, read_excel
 from scipy import sparse, stats
 from tqdm import tqdm
 
 
-def get_data_custom(interpreter, deconvolution: bool = False, n_eval_nodes_per_graph: int=10):
+def get_data_custom(interpreter, deconvolution: bool = False, n_eval_nodes_per_graph: int = 10):
     interpreter.undefined_node_types = None
     interpreter.img_to_patient_dict = interpreter.data.celldata.uns["img_to_patient_dict"]
     interpreter.complete_img_keys = list(interpreter.data.img_celldata.keys())
 
-    interpreter.a = {k: adata.obsp["adjacency_matrix_connectivities"] for k, adata in interpreter.data.img_celldata.items()}
+    interpreter.a = {
+        k: adata.obsp["adjacency_matrix_connectivities"] for k, adata in interpreter.data.img_celldata.items()
+    }
     interpreter.h_0 = {k: adata.obsm["node_types"] for k, adata in interpreter.data.img_celldata.items()}
     interpreter.h_1 = {k: adata.X for k, adata in interpreter.data.img_celldata.items()}
     interpreter.node_types = {k: adata.obsm["node_types"] for k, adata in interpreter.data.img_celldata.items()}
     interpreter.node_type_names = interpreter.data.celldata.uns["node_type_names"]
     interpreter.n_features_type = list(interpreter.node_types.values())[0].shape[1]
     interpreter.n_features_standard = interpreter.data.celldata.shape[1]
     interpreter.node_feature_names = list(interpreter.data.celldata.var_names)
@@ -55,31 +57,31 @@
     interpreter.n_domains = len(np.unique(list(interpreter.domains.values())))
 
     # Report summary statistics of loaded graph:
     print(
         "Mean of mean node degree per images across images: %f"
         % np.mean([np.mean(v.sum(axis=1)) for k, v in interpreter.a.items()])
     )
-    
+
     # splitting data into test and validation sets, can be ignored for non sender-receiver focused analysis
     interpreter.split_data_node(0.1, 0.1)
     interpreter.n_eval_nodes_per_graph = n_eval_nodes_per_graph
-    interpreter.cell_names = list(interpreter.data.celldata.uns['node_type_names'].values())
+    interpreter.cell_names = list(interpreter.data.celldata.uns["node_type_names"].values())
     if deconvolution:
         interpreter.proportions = {k: adata.obsm["proportions"] for k, adata in interpreter.data.img_celldata.items()}
-    
-    
+
+
 class GraphTools:
     """GraphTools class."""
 
     celldata: AnnData
     img_celldata: Dict[str, AnnData]
 
     def compute_adjacency_matrices(
-        self, radius: int, coord_type: str = 'generic', n_rings: int = 1, transform: str = None
+        self, radius: int, coord_type: str = "generic", n_rings: int = 1, transform: str = None
     ):
         """Compute adjacency matrix for each image in dataset (uses `squidpy.gr.spatial_neighbors`).
 
         Parameters
         ----------
         radius : int
             Radius of neighbors for non-grid data.
@@ -93,27 +95,27 @@
             - `spectral` - spectral transformation of the adjacency matrix.
             - `cosine` - cosine transformation of the adjacency matrix.
             - `None` - no transformation of the adjacency matrix.
         """
         pbar_total = len(self.img_celldata.keys())
         with tqdm(total=pbar_total) as pbar:
             for _k, adata in self.img_celldata.items():
-                if coord_type == 'grid':
+                if coord_type == "grid":
                     radius = None
                 else:
                     n_rings = 1
                 sq.gr.spatial_neighbors(
                     adata=adata,
                     coord_type=coord_type,
                     radius=radius,
                     n_rings=n_rings,
                     transform=transform,
-                    key_added="adjacency_matrix"
+                    key_added="adjacency_matrix",
                 )
-                #print(adata.obsp['adjacency_matrix_connectivities'].sum(axis=1).mean())
+                # print(adata.obsp['adjacency_matrix_connectivities'].sum(axis=1).mean())
                 pbar.update(1)
 
     @staticmethod
     def _transform_a(a):
         """Compute degree transformation of adjacency matrix.
 
         Computes D^(-1) * (A+I), with A an adjacency matrix, I the identity matrix and D the degree matrix.
@@ -321,15 +323,15 @@
                 )
                 interaction_matrix.append(im)
                 pbar.update(1)
         df_concat = pd.concat(interaction_matrix)
         by_row_index = df_concat.groupby(df_concat.index)
         df_means = by_row_index.sum().sort_index(axis=1)
         interactions = np.array(df_means).T
-        self.celldata.uns[f"{cluster_key}_interactions"] = interactions/np.sum(interactions, axis=1)[:, np.newaxis]
+        self.celldata.uns[f"{cluster_key}_interactions"] = interactions / np.sum(interactions, axis=1)[:, np.newaxis]
 
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
         if save:
             save = save + suffix
         sq.pl.interaction_matrix(
             self.celldata,
@@ -745,15 +747,22 @@
             temp_adata = temp_adata[np.argwhere(np.array(temp_adata.obsm["spatial"])[:, 1] < 0).squeeze()]
 
         plt.ioff()
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
         sc.pl.spatial(
-            temp_adata, color=cluster_id, spot_size=spot_size, legend_loc=legend_loc, ax=ax, show=False, title="", frameon=False
+            temp_adata,
+            color=cluster_id,
+            spot_size=spot_size,
+            legend_loc=legend_loc,
+            ax=ax,
+            show=False,
+            title="",
+            frameon=False,
         )
         ax.set_xlabel("")
         ax.set_ylabel("")
         # Save, show and return figure.
         plt.tight_layout()
         if save is not None:
             plt.savefig(save + image_key + suffix)
@@ -877,16 +886,16 @@
         if filter_titles:
             log_pval = log_pval.sort_values(columns, ascending=True).filter(items=filter_titles, axis=0)
         if clip_pvalues:
             log_pval[log_pval < clip_pvalues] = clip_pvalues
         fold_change_df = adata_substates.obs[[cluster_col, f"{target_cell_type} substates"] + sorce_type_names]
         fold_change_df = fold_change_df.replace({"in neighbourhood": 1, "not in neighbourhood": 0})
         for x in fold_change_df.columns:
-            if x.startswith('source type'):
-                fold_change_df[x] = fold_change_df[x].astype('int')
+            if x.startswith("source type"):
+                fold_change_df[x] = fold_change_df[x].astype("int")
         counts = pd.pivot_table(
             fold_change_df,
             index=[f"{target_cell_type} substates"],
             aggfunc=np.sum,
             margins=True,
         ).T
         counts["new_index"] = [x.replace("source type ", "") for x in counts.index]
@@ -1061,32 +1070,43 @@
         n = len(filter_titles)
         axs = axs.flat
         for ax in axs[n:]:
             ax.remove()
         ax = axs[:n]
 
         for i, x in enumerate(filter_titles[:-1]):
-            sc.pl.umap(adata, color=f"source type {x}", title='', show=False, size=size, legend_loc="None", ax=ax[i], frameon=False, hspace=0., wspace=0.)
+            sc.pl.umap(
+                adata,
+                color=f"source type {x}",
+                title="",
+                show=False,
+                size=size,
+                legend_loc="None",
+                ax=ax[i],
+                frameon=False,
+                hspace=0.0,
+                wspace=0.0,
+            )
             ax[i].set_xlabel("")
             ax[i].set_ylabel("")
             ax[i].set_title(x)
         sc.pl.umap(
             adata,
             color=f"source type {filter_titles[-1]}",
-            title='',
+            title="",
             size=size,
             show=False,
             ax=ax[n - 1],
-            frameon=False
+            frameon=False,
         )
         ax[n - 1].set_xlabel("")
         ax[n - 1].set_ylabel("")
         ax[n - 1].set_title(filter_titles[-1])
         # Save, show and return figure.
-        #plt.tight_layout(pad=1.2)
+        # plt.tight_layout(pad=1.2)
         if save is not None:
             plt.savefig(save + suffix)
 
         if show:
             plt.show()
 
         plt.close(fig)
@@ -1165,26 +1185,26 @@
             # adata,
             temp_adata[temp_adata.obs[cluster_id] != target_cell_type],
             spot_size=spot_size,
             ax=ax,
             show=False,
             na_color="whitesmoke",
             title="",
-            frameon=False
+            frameon=False,
         )
         sc.pl.spatial(
             adata_substates,
             color=f"{target_cell_type} substates",
             spot_size=spot_size,
             ax=ax,
             show=False,
             legend_loc=legend_loc,
             title="",
             palette=palette,
-            frameon=False
+            frameon=False,
         )
         ax.invert_yaxis()
         ax.set_xlabel("")
         ax.set_ylabel("")
         # Save, show and return figure.
         plt.tight_layout()
         if save is not None:
@@ -1594,17 +1614,17 @@
             x = np.sqrt(self.celldata.obs[area_key])
 
         if volume_key:
             x = np.cbrt(self.celldata.obs[volume_key])
 
         fig, ax = plt.subplots(1, 1, figsize=figsize)
         sns.histplot(x, ax=ax)
-        plt.axvline(np.mean(x), color='Red', linewidth=2, ax=ax)
+        plt.axvline(np.mean(x), color="Red", linewidth=2, ax=ax)
         min_ylim, max_ylim = plt.ylim()
-        plt.text(np.mean(x) * text_pos[0], max_ylim * text_pos[1], 'mean: {:.2f} $\mu$m'.format(np.mean(x)), ax=ax)
+        plt.text(np.mean(x) * text_pos[0], max_ylim * text_pos[1], "mean: {:.2f} $\mu$m".format(np.mean(x)), ax=ax)
         ax.set_xlabel("")
         ax.set_ylabel("")
 
         plt.tight_layout()
         if save is not None:
             plt.savefig(save + suffix)
 
@@ -1655,28 +1675,28 @@
         """
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
 
         x = []
         with tqdm(total=len(self.img_celldata.keys())) as pbar:
             for adata in self.img_celldata.values():
-                dist = adata.obsp['adjacency_matrix_distances'].todense()
+                dist = adata.obsp["adjacency_matrix_distances"].todense()
                 for i in range(dist.shape[0]):
                     vec = dist[i, :]
                     vec = vec[vec != 0]
                     if vec.shape[1] == 0:
                         continue
                     x.append(np.min(vec))
                 pbar.update(1)
 
         fig, ax = plt.subplots(1, 1, figsize=figsize)
         sns.histplot(x, ax=ax)
-        plt.axvline(np.mean(x), color='Red', linewidth=2, ax=ax)
+        plt.axvline(np.mean(x), color="Red", linewidth=2, ax=ax)
         min_ylim, max_ylim = plt.ylim()
-        plt.text(np.mean(x) * text_pos[0], max_ylim * text_pos[1], 'mean: {:.2f} $\mu$m'.format(np.mean(x)), ax=ax)
+        plt.text(np.mean(x) * text_pos[0], max_ylim * text_pos[1], "mean: {:.2f} $\mu$m".format(np.mean(x)), ax=ax)
         ax.set_xlabel("")
         ax.set_ylabel("")
 
         plt.tight_layout()
         if save is not None:
             plt.savefig(save + suffix)
 
@@ -1695,18 +1715,18 @@
 class DataLoader(GraphTools, PlottingTools):
     """DataLoader class. Inherits all functions from GraphTools and PlottingTools."""
 
     def __init__(
         self,
         data_path: str,
         radius: Optional[int] = None,
-        coord_type: str = 'generic',
+        coord_type: str = "generic",
         n_rings: int = 1,
         label_selection: Optional[List[str]] = None,
-        n_top_genes: Optional[int] = None
+        n_top_genes: Optional[int] = None,
     ):
         """Initialize DataLoader.
 
         Parameters
         ----------
         data_path : str
             Data path.
@@ -1804,29 +1824,28 @@
         # Get global mean of feature intensity across all features:
         global_mean_per_node = self.celldata.X.sum(axis=1).mean(axis=0)
         return {i: global_mean_per_node / np.sum(adata.X, axis=1) for i, adata in self.img_celldata.items()}
 
     @property
     def var_names(self):
         return self.celldata.var_names
-    
+
 
 class customLoader(DataLoader):
-    
     def __init__(
         self,
-        adata, 
-        cluster, 
-        patient, 
+        adata,
+        cluster,
+        patient,
         library_id,
         radius,
-        coord_type='generic',
+        coord_type="generic",
         n_rings=1,
         n_top_genes=None,
-        label_selection=None
+        label_selection=None,
     ):
         self.adata = adata.copy()
         self.cluster = cluster
         self.patient = patient
         self.library_id = library_id
 
         print("Loading data from raw files")
@@ -1843,35 +1862,30 @@
                 len(self.img_celldata),
                 len(self.patients),
                 self.celldata.shape[0],
                 self.celldata.shape[1],
                 len(self.celldata.uns["node_type_names"]),
             )
         )
-    
+
     def _register_celldata(self, n_top_genes):
-        
-        metadata = {
-            "cluster_col_preprocessed": self.cluster,
-            "image_col": self.library_id
-        }
-        
+
+        metadata = {"cluster_col_preprocessed": self.cluster, "image_col": self.library_id}
+
         celldata = self.adata.copy()
         celldata.X = celldata.X.toarray()
         celldata.uns["metadata"] = metadata
-        del celldata.uns['spatial']
+        del celldata.uns["spatial"]
 
         # register node type names
         node_type_names = list(np.unique(celldata.obs[self.cluster]))
         celldata.uns["node_type_names"] = {x: x for x in node_type_names}
         node_types = np.zeros((celldata.shape[0], len(node_type_names)))
         node_type_idx = np.array(
-            [
-                node_type_names.index(x) for x in celldata.obs[self.cluster].values
-            ]  # index in encoding vector
+            [node_type_names.index(x) for x in celldata.obs[self.cluster].values]  # index in encoding vector
         )
         node_types[np.arange(0, node_type_idx.shape[0]), node_type_idx] = 1
         celldata.obsm["node_types"] = node_types
 
         if self.patient:
             img_to_patient_dict = {}
             for p in np.unique(celldata.obs[self.patient]):
@@ -1879,15 +1893,15 @@
                     img_to_patient_dict[i] = p
         else:
             img_to_patient_dict = {"image": "patient"}
         celldata.uns["img_to_patient_dict"] = img_to_patient_dict
         self.img_to_patient_dict = img_to_patient_dict
 
         self.celldata = celldata
-        
+
     def _register_img_celldata(self):
         """Load dictionary of of image-wise celldata objects with {imgage key : anndata object of image}."""
         img_celldata = {}
         if self.library_id:
             for k in np.unique(self.celldata.obs[self.library_id]):
                 img_celldata[str(k)] = self.celldata[self.celldata.obs[self.library_id] == k].copy()
             self.img_celldata = img_celldata
@@ -1919,27 +1933,26 @@
             "label_selection": [],
             "continuous_mean": {},
             "continuous_std": {},
             "label_data_types": {},
         }
         self.celldata.uns["graph_covariates"] = graph_covariates
 
-        
+
 class customLoaderDeconvolution(DataLoader):
-    
     def __init__(
         self,
-        adata, 
-        patient, 
+        adata,
+        patient,
         library_id,
         radius,
-        coord_type='generic',
+        coord_type="generic",
         n_rings=1,
         n_top_genes=None,
-        label_selection=None
+        label_selection=None,
     ):
         self.adata = adata.copy()
         self.patient = patient
         self.library_id = library_id
 
         print("Loading data from raw files")
         self.register_celldata(n_top_genes=n_top_genes)
@@ -1955,22 +1968,22 @@
                 len(self.img_celldata),
                 len(self.patients),
                 self.celldata.shape[0],
                 self.celldata.shape[1],
                 len(self.celldata.uns["node_type_names"]),
             )
         )
-    
+
     def _register_celldata(self, n_top_genes):
-        
+
         metadata = {
-            #"cluster_col_preprocessed": self.cluster,
+            # "cluster_col_preprocessed": self.cluster,
             "image_col": self.library_id
         }
-        
+
         celldata = self.adata.copy()
         celldata.uns["metadata"] = metadata
 
         if self.patient:
             img_to_patient_dict = {}
             for p in np.unique(celldata.obs[self.patient]):
                 for i in np.unique(celldata.obs[celldata.obs[self.patient] == p][self.library_id]):
@@ -1982,15 +1995,15 @@
                     img_to_patient_dict[str(img)] = "patient"
             else:
                 img_to_patient_dict = {"image": "patient"}
         celldata.uns["img_to_patient_dict"] = img_to_patient_dict
         self.img_to_patient_dict = img_to_patient_dict
 
         self.celldata = celldata
-        
+
     def _register_img_celldata(self):
         """Load dictionary of of image-wise celldata objects with {imgage key : anndata object of image}."""
         img_celldata = {}
         if self.library_id:
             for k in np.unique(self.celldata.obs[self.library_id]):
                 img_celldata[str(k)] = self.celldata[self.celldata.obs[self.library_id] == k].copy()
             self.img_celldata = img_celldata
@@ -2173,38 +2186,37 @@
             "pos_cols": ["X", "Y"],
             "cluster_col": "celltype_Level_2",
             "cluster_col_preprocessed": "celltype_Level_2_preprocessed",
             "patient_col": None,
         }
         celldata = read_h5ad(os.path.join(self.data_path, metadata["fn"]))
         feature_cols_hgnc_names = [
-            'CD14',
-            'MS4A1',
-            'IL2RA',
-            'CD3G',
-            'CD4',
-            'PTPRC',
-            'PTPRC',
-            'PTPRC',
-            'CD68',
-            'CD8A',
-            'KRT5',  # 'KRT1', 'KRT14'
-            'FOXP3',
-            'GATA3',
-            'MKI67',
-            'Nuclei',
-            'PDCD1',
-            'CD274',
-            'SMN1',
-            'VIM'
+            "CD14",
+            "MS4A1",
+            "IL2RA",
+            "CD3G",
+            "CD4",
+            "PTPRC",
+            "PTPRC",
+            "PTPRC",
+            "CD68",
+            "CD8A",
+            "KRT5",  # 'KRT1', 'KRT14'
+            "FOXP3",
+            "GATA3",
+            "MKI67",
+            "Nuclei",
+            "PDCD1",
+            "CD274",
+            "SMN1",
+            "VIM",
         ]
         X = DataFrame(celldata.X, columns=feature_cols_hgnc_names)
         celldata = AnnData(
-            X=X, obs=celldata.obs, uns=celldata.uns, obsm=celldata.obsm,
-            varm=celldata.varm, obsp=celldata.obsp
+            X=X, obs=celldata.obs, uns=celldata.uns, obsm=celldata.obsm, varm=celldata.varm, obsp=celldata.obsp
         )
         celldata.var_names_make_unique()
         celldata = celldata[celldata.obs[metadata["image_col"]] != "Dirt"].copy()
         celldata.uns["metadata"] = metadata
         img_keys = list(np.unique(celldata.obs[metadata["image_col"]]))
         celldata.uns["img_keys"] = img_keys
 
@@ -2344,56 +2356,55 @@
             # "X1",
             # "cell_size",
             # "category",
             # "donor",
             # "Cluster",
         ]
         var_names = [
-            'H3-4', 
-            'VIM', 
-            'SMN1', 
-            'SLC3A2', 
-            'NFE2L2', 
-            'CD4', 
-            'CD14', 
-            'PTPRC', 
-            'PDCD1',
-            'PECAM1', 
-            'SDHA', 
-            'MKI67', 
-            'CS', 
-            'RPS6', 
-            'ITGAX', 
-            'CD68', 
-            'CD36', 
-            'ATP5F1A',
-            'CD247', 
-            'ENTPD1', 
-            'VDAC1', 
-            'G6PD', 
-            'XBP1', 
-            'PKM', 
-            'SLC1A5', 
-            'SLC2A1', 
-            'CD8A',
-            'B3GAT1', 
-            'LDHA', 
-            'IDH2', 
-            'HK1', 
-            'CDH1', 
-            'CPT1A', 
-            'CKM', 
-            'ATP1A1',
-            'HIF1A'
+            "H3-4",
+            "VIM",
+            "SMN1",
+            "SLC3A2",
+            "NFE2L2",
+            "CD4",
+            "CD14",
+            "PTPRC",
+            "PDCD1",
+            "PECAM1",
+            "SDHA",
+            "MKI67",
+            "CS",
+            "RPS6",
+            "ITGAX",
+            "CD68",
+            "CD36",
+            "ATP5F1A",
+            "CD247",
+            "ENTPD1",
+            "VDAC1",
+            "G6PD",
+            "XBP1",
+            "PKM",
+            "SLC1A5",
+            "SLC2A1",
+            "CD8A",
+            "B3GAT1",
+            "LDHA",
+            "IDH2",
+            "HK1",
+            "CDH1",
+            "CPT1A",
+            "CKM",
+            "ATP1A1",
+            "HIF1A",
         ]
 
         celldata = AnnData(
-            X=pd.DataFrame(np.array(celldata_df[feature_cols]), columns=var_names), obs=celldata_df[
-                ["point", "cell_id", "cell_size", "donor", "Cluster"]
-            ].astype("category"),
+            X=pd.DataFrame(np.array(celldata_df[feature_cols]), columns=var_names),
+            obs=celldata_df[["point", "cell_id", "cell_size", "donor", "Cluster"]].astype("category"),
         )
 
         celldata.uns["metadata"] = metadata
         img_keys = list(np.unique(celldata_df[metadata["image_col"]]))
         celldata.uns["img_keys"] = img_keys
 
         # register x and y coordinates into obsm
@@ -2808,71 +2819,71 @@
             "CD194 - CCR4 chemokine R:Cyc_14_ch_3",
             "MMP9 - matrix metalloproteinase:Cyc_15_ch_2",
             "CD71 - transferrin R:Cyc_15_ch_4",
             "CD57 - NK cells:Cyc_17_ch_4",
             "MMP12 - matrix metalloproteinase:Cyc_21_ch_4",
         ]
         feature_cols_hgnc_names = [
-            'CD44',
-            'FOXP3',
-            'CD8A',
-            'TP53',
-            'GATA3',
-            'PTPRC',
-            'TBX21',
-            'CTNNB1',
-            'HLA-DR',
-            'CD274',
-            'MKI67',
-            'PTPRC',
-            'CD4',
-            'CR2',
-            'MUC1',
-            'TNFRSF8',
-            'CD2',
-            'VIM',
-            'MS4A1',
-            'LAG3',
-            'ATP1A1',
-            'CD5',
-            'IDO1',
-            'KRT1',
-            'ITGAM',
-            'NCAM1',
-            'ACTA1',
-            'BCL2',
-            'IL2RA',
-            'ITGAX',
-            'PDCD1',
-            'GZMB',
-            'EGFR',
-            'VISTA',
-            'FUT4',
-            'ICOS',
-            'SYP',
-            'GFAP',
-            'CD7',
-            'CD247',
-            'CHGA',
-            'CD163',
-            'PTPRC',
-            'CD68',
-            'PECAM1',
-            'PDPN',
-            'CD34',
-            'CD38',
-            'SDC1',
-            'HOECHST1:Cyc_1_ch_1',  ##
-            'CDX2',
-            'COL6A1',
-            'CCR4',
-            'MMP9',
-            'TFRC',
-            'B3GAT1',
-            'MMP12'
+            "CD44",
+            "FOXP3",
+            "CD8A",
+            "TP53",
+            "GATA3",
+            "PTPRC",
+            "TBX21",
+            "CTNNB1",
+            "HLA-DR",
+            "CD274",
+            "MKI67",
+            "PTPRC",
+            "CD4",
+            "CR2",
+            "MUC1",
+            "TNFRSF8",
+            "CD2",
+            "VIM",
+            "MS4A1",
+            "LAG3",
+            "ATP1A1",
+            "CD5",
+            "IDO1",
+            "KRT1",
+            "ITGAM",
+            "NCAM1",
+            "ACTA1",
+            "BCL2",
+            "IL2RA",
+            "ITGAX",
+            "PDCD1",
+            "GZMB",
+            "EGFR",
+            "VISTA",
+            "FUT4",
+            "ICOS",
+            "SYP",
+            "GFAP",
+            "CD7",
+            "CD247",
+            "CHGA",
+            "CD163",
+            "PTPRC",
+            "CD68",
+            "PECAM1",
+            "PDPN",
+            "CD34",
+            "CD38",
+            "SDC1",
+            "HOECHST1:Cyc_1_ch_1",  ##
+            "CDX2",
+            "COL6A1",
+            "CCR4",
+            "MMP9",
+            "TFRC",
+            "B3GAT1",
+            "MMP12",
         ]
         X = DataFrame(np.array(celldata_df[feature_cols]), columns=feature_cols_hgnc_names)
         celldata = AnnData(X=X, obs=celldata_df[["File Name", "patients", "ClusterName"]])
         celldata.var_names_make_unique()
 
         celldata.uns["metadata"] = metadata
         img_keys = list(np.unique(celldata_df[metadata["image_col"]]))
@@ -3120,44 +3131,44 @@
         self.celldata.uns["graph_covariates"] = graph_covariates
 
 
 class DataLoaderLohoff(DataLoader):
     """DataLoaderLohoff class. Inherits all functions from DataLoader."""
 
     cell_type_merge_dict = {
-        'Allantois': 'Allantois',
-        'Anterior somitic tissues': 'Anterior somitic tissues',
-        'Blood progenitors': 'Blood progenitors',
-        'Cardiomyocytes': 'Cardiomyocytes',
-        'Cranial mesoderm': 'Cranial mesoderm',
-        'Definitive endoderm': 'Definitive endoderm',
-        'Dermomyotome': 'Dermomyotome',
-        'Endothelium': 'Endothelium',
-        'Erythroid': 'Erythroid',
-        'ExE endoderm': 'ExE endoderm',
-        'Forebrain/Midbrain/Hindbrain': 'Forebrain/Midbrain/Hindbrain',
-        'Gut tube': 'Gut tube',
-        'Haematoendothelial progenitors': 'Haematoendothelial progenitors',
-        'Intermediate mesoderm': 'Intermediate mesoderm',
-        'Lateral plate mesoderm': 'Lateral plate mesoderm',
-        'Low quality': 'Low quality',
-        'Mixed mesenchymal mesoderm': 'Mixed mesenchymal mesoderm',
-        'NMP': 'NMP',
-        'Neural crest': 'Neural crest',
-        'Presomitic mesoderm': 'Presomitic mesoderm',
-        'Sclerotome': 'Sclerotome',
-        'Spinal cord': 'Spinal cord',
-        'Splanchnic mesoderm': 'Splanchnic mesoderm',
-        'Surface ectoderm': 'Surface ectoderm'
+        "Allantois": "Allantois",
+        "Anterior somitic tissues": "Anterior somitic tissues",
+        "Blood progenitors": "Blood progenitors",
+        "Cardiomyocytes": "Cardiomyocytes",
+        "Cranial mesoderm": "Cranial mesoderm",
+        "Definitive endoderm": "Definitive endoderm",
+        "Dermomyotome": "Dermomyotome",
+        "Endothelium": "Endothelium",
+        "Erythroid": "Erythroid",
+        "ExE endoderm": "ExE endoderm",
+        "Forebrain/Midbrain/Hindbrain": "Forebrain/Midbrain/Hindbrain",
+        "Gut tube": "Gut tube",
+        "Haematoendothelial progenitors": "Haematoendothelial progenitors",
+        "Intermediate mesoderm": "Intermediate mesoderm",
+        "Lateral plate mesoderm": "Lateral plate mesoderm",
+        "Low quality": "Low quality",
+        "Mixed mesenchymal mesoderm": "Mixed mesenchymal mesoderm",
+        "NMP": "NMP",
+        "Neural crest": "Neural crest",
+        "Presomitic mesoderm": "Presomitic mesoderm",
+        "Sclerotome": "Sclerotome",
+        "Spinal cord": "Spinal cord",
+        "Splanchnic mesoderm": "Splanchnic mesoderm",
+        "Surface ectoderm": "Surface ectoderm",
     }
 
     def _register_celldata(self, n_top_genes: Optional[int] = None):
         """Load AnnData object of complete dataset."""
         metadata = {
-            "lateral_resolution": 1.,
+            "lateral_resolution": 1.0,
             "fn": "preprocessed_lohoff.h5ad",
             "image_col": "embryo",
             "pos_cols": ["x_global", "y_global"],
             "cluster_col": "celltype_mapped_refined",
             "cluster_col_preprocessed": "celltype_mapped_refined",
             "patient_col": "embryo",
         }
@@ -3394,41 +3405,37 @@
             "Vangl2",
             "Vav1",
             "Vcam1",
             "Vwf",
         ]
 
         celldata = AnnData(
-            X=celldata_df[feature_cols],
-            obs=celldata_df[["CellID", "FOV", "CellTypeID_new", "Center_x", "Center_y"]]
+            X=celldata_df[feature_cols], obs=celldata_df[["CellID", "FOV", "CellTypeID_new", "Center_x", "Center_y"]]
         )
 
         celldata.uns["metadata"] = metadata
         img_keys = list(np.unique(celldata_df[metadata["image_col"]]))
         celldata.uns["img_keys"] = img_keys
 
         # register x and y coordinates into obsm
         celldata.obsm["spatial"] = np.array(celldata_df[metadata["pos_cols"]])
 
-        img_to_patient_dict = {
-            str(x): "patient"
-            for x in celldata_df[metadata["image_col"]].values
-        }
+        img_to_patient_dict = {str(x): "patient" for x in celldata_df[metadata["image_col"]].values}
         # img_to_patient_dict = {k: "p_1" for k in img_keys}
         celldata.uns["img_to_patient_dict"] = img_to_patient_dict
         self.img_to_patient_dict = img_to_patient_dict
 
         # add clean cluster column which removes regular expression from cluster_col
         celldata.obs[metadata["cluster_col_preprocessed"]] = list(
             pd.Series(list(celldata.obs[metadata["cluster_col"]]), dtype="str").map(self.cell_type_merge_dict)
         )
         celldata.obs[metadata["cluster_col_preprocessed"]] = celldata.obs[metadata["cluster_col_preprocessed"]].astype(
             "str"
         )
-        #celldata = celldata[celldata.obs[metadata["cluster_col_preprocessed"]] != 'Unknown']
+        # celldata = celldata[celldata.obs[metadata["cluster_col_preprocessed"]] != 'Unknown']
 
         # register node type names
         node_type_names = list(np.unique(celldata.obs[metadata["cluster_col_preprocessed"]]))
         celldata.uns["node_type_names"] = {x: x for x in node_type_names}
         node_types = np.zeros((celldata.shape[0], len(node_type_names)))
         node_type_idx = np.array(
             [
@@ -3497,15 +3504,15 @@
         metadata = {
             "lateral_resolution": 0.1079,
             "fn": "merfish_wt_imputed_fetal_liver.h5ad",
             "image_col": "FOV",
             "pos_cols": ["Center_x", "Center_y"],
             "cluster_col": "CellTypeID_new",
             "cluster_col_preprocessed": "CellTypeID_new_preprocessed",
-            "n_top_genes": n_top_genes
+            "n_top_genes": n_top_genes,
         }
         celldata = read_h5ad(self.data_path + metadata["fn"])
         celldata.uns["metadata"] = metadata
         if n_top_genes:
             sc.pp.highly_variable_genes(celldata, n_top_genes=n_top_genes)
             celldata = celldata[:, celldata.var.highly_variable].copy()
 
@@ -3708,29 +3715,25 @@
             "Vangl2",
             "Vav1",
             "Vcam1",
             "Vwf",
         ]
 
         celldata = AnnData(
-            X=celldata_df[feature_cols],
-            obs=celldata_df[["CellID", "FOV", "CellTypeID_new", "Center_x", "Center_y"]]
+            X=celldata_df[feature_cols], obs=celldata_df[["CellID", "FOV", "CellTypeID_new", "Center_x", "Center_y"]]
         )
 
         celldata.uns["metadata"] = metadata
         img_keys = list(np.unique(celldata_df[metadata["image_col"]]))
         celldata.uns["img_keys"] = img_keys
 
         # register x and y coordinates into obsm
         celldata.obsm["spatial"] = np.array(celldata_df[metadata["pos_cols"]])
 
-        img_to_patient_dict = {
-            str(x): "patient"
-            for x in celldata_df[metadata["image_col"]].values
-        }
+        img_to_patient_dict = {str(x): "patient" for x in celldata_df[metadata["image_col"]].values}
         # img_to_patient_dict = {k: "p_1" for k in img_keys}
         celldata.uns["img_to_patient_dict"] = img_to_patient_dict
         self.img_to_patient_dict = img_to_patient_dict
 
         # add clean cluster column which removes regular expression from cluster_col
         celldata.obs[metadata["cluster_col_preprocessed"]] = list(
             pd.Series(list(celldata.obs[metadata["cluster_col"]]), dtype="str").map(self.cell_type_merge_dict)
@@ -3790,58 +3793,56 @@
         self.celldata.uns["graph_covariates"] = graph_covariates
 
 
 class DataLoader10xVisiumMouseBrain(DataLoader):
     """DataLoader10xVisiumMouseBrain class. Inherits all functions from DataLoader."""
 
     cell_type_merge_dict = {
-        'Cortex_1': 'Cortex 1',
-        'Cortex_2': 'Cortex 2',
-        'Cortex_3': 'Cortex 3',
-        'Cortex_4': 'Cortex 4',
-        'Cortex_5': 'Cortex 5',
-        'Fiber_tract': 'Fiber tract',
-        'Hippocampus': 'Hippocampus',
-        'Hypothalamus_1': 'Hypothalamus 1',
-        'Hypothalamus_2': 'Hypothalamus 2',
-        'Lateral_ventricle': 'Lateral ventricle',
-        'Pyramidal_layer': 'Pyramidal layer',
-        'Pyramidal_layer_dentate_gyrus': 'Pyramidal layer dentate gyrus',
-        'Striatum': 'Striatum',
-        'Thalamus_1': 'Thalamus 1',
-        'Thalamus_2': 'Thalamus 2'
+        "Cortex_1": "Cortex 1",
+        "Cortex_2": "Cortex 2",
+        "Cortex_3": "Cortex 3",
+        "Cortex_4": "Cortex 4",
+        "Cortex_5": "Cortex 5",
+        "Fiber_tract": "Fiber tract",
+        "Hippocampus": "Hippocampus",
+        "Hypothalamus_1": "Hypothalamus 1",
+        "Hypothalamus_2": "Hypothalamus 2",
+        "Lateral_ventricle": "Lateral ventricle",
+        "Pyramidal_layer": "Pyramidal layer",
+        "Pyramidal_layer_dentate_gyrus": "Pyramidal layer dentate gyrus",
+        "Striatum": "Striatum",
+        "Thalamus_1": "Thalamus 1",
+        "Thalamus_2": "Thalamus 2",
     }
 
     def _register_celldata(self, n_top_genes: Optional[int] = None):
         """Load AnnData object of complete dataset."""
         metadata = {
-            "lateral_resolution": 1.,
+            "lateral_resolution": 1.0,
             "fn": "visium_hne_adata.h5ad",
             "image_col": "in_tissue",
             "cluster_col": "cluster",
             "cluster_col_preprocessed": "cluster_preprocessed",
             "patient_col": "in_tissue",
-            "n_top_genes": n_top_genes
+            "n_top_genes": n_top_genes,
         }
 
         celldata = read_h5ad(self.data_path + metadata["fn"]).copy()
         if n_top_genes:
             sc.pp.highly_variable_genes(celldata, n_top_genes=n_top_genes)
             celldata = celldata[:, celldata.var.highly_variable].copy()
 
         celldata.X = celldata.X.toarray()
         celldata.uns["metadata"] = metadata
         celldata.uns["img_keys"] = list(np.unique(celldata.obs[metadata["image_col"]]))
 
         celldata.uns["img_to_patient_dict"] = {"1": "1"}
         self.img_to_patient_dict = {"1": "1"}
 
-        celldata.obs[metadata["cluster_col"]] = celldata.obs[metadata["cluster_col"]].astype(
-            "str"
-        )
+        celldata.obs[metadata["cluster_col"]] = celldata.obs[metadata["cluster_col"]].astype("str")
         # add clean cluster column which removes regular expression from cluster_col
         celldata.obs[metadata["cluster_col_preprocessed"]] = list(
             pd.Series(list(celldata.obs[metadata["cluster_col"]]), dtype="str").map(self.cell_type_merge_dict)
         )
         celldata.obs[metadata["cluster_col_preprocessed"]] = celldata.obs[metadata["cluster_col_preprocessed"]].astype(
             "str"
         )
@@ -3899,38 +3900,33 @@
 
 class DataLoader10xLymphnode(DataLoader):
     """DataLoader10xLymphnode class. Inherits all functions from DataLoader."""
 
     def _register_celldata(self, n_top_genes: Optional[int] = None):
         """Load AnnData object of complete dataset."""
         metadata = {
-            "lateral_resolution": 1.,
+            "lateral_resolution": 1.0,
             "fn": "destVI_lymphnode.h5ad",
-            #"image_col": "batch",
+            # "image_col": "batch",
             "cluster_col": "lymph_node",
             "cluster_col_preprocessed": "lymph_node",
-            "n_top_genes": None
+            "n_top_genes": None,
         }
 
         ad = read_h5ad(self.data_path + metadata["fn"]).copy()
-        metadata['var_names'] = ad.var_names
+        metadata["var_names"] = ad.var_names
 
-        celldata = AnnData(
-            X=ad.obsm['scale'],
-            obs=ad.obs, obsm=ad.obsm
-        )
-        celldata.obsm['spatial'] = celldata.obsm['location']
+        celldata = AnnData(X=ad.obsm["scale"], obs=ad.obs, obsm=ad.obsm)
+        celldata.obsm["spatial"] = celldata.obsm["location"]
         celldata.uns["metadata"] = metadata
 
         celldata.uns["img_to_patient_dict"] = {"1": "1"}
         self.img_to_patient_dict = {"1": "1"}
 
-        celldata.obs[metadata["cluster_col"]] = celldata.obs[metadata["cluster_col"]].astype(
-            "str"
-        )
+        celldata.obs[metadata["cluster_col"]] = celldata.obs[metadata["cluster_col"]].astype("str")
         # register node type names
         node_type_names = list(np.unique(celldata.obs[metadata["cluster_col_preprocessed"]]))
         celldata.uns["node_type_names"] = {x: x for x in node_type_names}
         node_types = np.zeros((celldata.shape[0], len(node_type_names)))
         node_type_idx = np.array(
             [
                 node_type_names.index(x) for x in celldata.obs[metadata["cluster_col_preprocessed"]].values
@@ -3982,43 +3978,43 @@
 
 class DataLoaderDestViLymphnode(DataLoader):
     """DataLoaderDestViLymphnode class. Inherits all functions from DataLoader."""
 
     def _register_celldata(self, n_top_genes: Optional[int] = None):
         """Load AnnData object of complete dataset."""
         metadata = {
-            "lateral_resolution": 1.,
+            "lateral_resolution": 1.0,
             "fn": "destVI_lymphnode.h5ad",
-            #"image_col": "in_tissue",
-            #"cluster_col": "cluster",
-            #"cluster_col_preprocessed": "cluster_preprocessed",
-            #"patient_col": "in_tissue",
-            "n_top_genes": n_top_genes
+            # "image_col": "in_tissue",
+            # "cluster_col": "cluster",
+            # "cluster_col_preprocessed": "cluster_preprocessed",
+            # "patient_col": "in_tissue",
+            "n_top_genes": n_top_genes,
         }
 
         celldata = read_h5ad(self.data_path + metadata["fn"]).copy()
         if n_top_genes:
             sc.pp.highly_variable_genes(celldata, n_top_genes=n_top_genes)
             celldata = celldata[:, celldata.var.highly_variable].copy()
 
-        #celldata.X = celldata.X.toarray()
+        # celldata.X = celldata.X.toarray()
         celldata.uns["metadata"] = metadata
 
         celldata.uns["img_to_patient_dict"] = {"1": "1"}
         self.img_to_patient_dict = {"1": "1"}
         print(celldata)
         self.celldata = celldata
 
     def _register_img_celldata(self):
         """Load dictionary of of image-wise celldata objects with {imgage key : anndata object of image}."""
-        #image_col = self.celldata.uns["metadata"]["image_col"]
-        #img_celldata = {}
-        #for k in self.celldata.uns["img_keys"]:
+        # image_col = self.celldata.uns["metadata"]["image_col"]
+        # img_celldata = {}
+        # for k in self.celldata.uns["img_keys"]:
         #    img_celldata[str(k)] = self.celldata[self.celldata.obs[image_col] == k].copy()
-        #self.img_celldata = img_celldata
+        # self.img_celldata = img_celldata
         self.img_celldata = {"1": self.celldata}
 
     def _register_graph_features(self, label_selection):
         """Load graph level covariates.
 
         Parameters
         ----------
@@ -4049,43 +4045,43 @@
 
 class DataLoaderDestViMousebrain(DataLoader):
     """DataLoaderDestViMousebrain class. Inherits all functions from DataLoader."""
 
     def _register_celldata(self, n_top_genes: Optional[int] = None):
         """Load AnnData object of complete dataset."""
         metadata = {
-            "lateral_resolution": 1.,
+            "lateral_resolution": 1.0,
             "fn": "destVI_mousebrain.h5ad",
-            #"image_col": "in_tissue",
-            #"cluster_col": "cluster",
-            #"cluster_col_preprocessed": "cluster_preprocessed",
-            #"patient_col": "in_tissue",
-            "n_top_genes": n_top_genes
+            # "image_col": "in_tissue",
+            # "cluster_col": "cluster",
+            # "cluster_col_preprocessed": "cluster_preprocessed",
+            # "patient_col": "in_tissue",
+            "n_top_genes": n_top_genes,
         }
 
         celldata = read_h5ad(self.data_path + metadata["fn"]).copy()
         if n_top_genes:
             sc.pp.highly_variable_genes(celldata, n_top_genes=n_top_genes)
             celldata = celldata[:, celldata.var.highly_variable].copy()
 
-        #celldata.X = celldata.X.toarray()
+        # celldata.X = celldata.X.toarray()
         celldata.uns["metadata"] = metadata
 
         celldata.uns["img_to_patient_dict"] = {"1": "1"}
         self.img_to_patient_dict = {"1": "1"}
         print(celldata)
         self.celldata = celldata
 
     def _register_img_celldata(self):
         """Load dictionary of of image-wise celldata objects with {imgage key : anndata object of image}."""
-        #image_col = self.celldata.uns["metadata"]["image_col"]
-        #img_celldata = {}
-        #for k in self.celldata.uns["img_keys"]:
+        # image_col = self.celldata.uns["metadata"]["image_col"]
+        # img_celldata = {}
+        # for k in self.celldata.uns["img_keys"]:
         #    img_celldata[str(k)] = self.celldata[self.celldata.obs[image_col] == k].copy()
-        #self.img_celldata = img_celldata
+        # self.img_celldata = img_celldata
         self.img_celldata = {"1": self.celldata}
 
     def _register_graph_features(self, label_selection):
         """Load graph level covariates.
 
         Parameters
         ----------
@@ -4116,43 +4112,43 @@
 
 class DataLoaderCell2locationLymphnode(DataLoader):
     """DataLoaderCell2locationLymphnode class. Inherits all functions from DataLoader."""
 
     def _register_celldata(self, n_top_genes: Optional[int] = None):
         """Load AnnData object of complete dataset."""
         metadata = {
-            "lateral_resolution": 1.,
+            "lateral_resolution": 1.0,
             "fn": "cell2location_lymphnode.h5ad",
-            #"image_col": "in_tissue",
-            #"cluster_col": "cluster",
-            #"cluster_col_preprocessed": "cluster_preprocessed",
-            #"patient_col": "in_tissue",
-            "n_top_genes": n_top_genes
+            # "image_col": "in_tissue",
+            # "cluster_col": "cluster",
+            # "cluster_col_preprocessed": "cluster_preprocessed",
+            # "patient_col": "in_tissue",
+            "n_top_genes": n_top_genes,
         }
 
         celldata = read_h5ad(self.data_path + metadata["fn"]).copy()
         if n_top_genes:
             sc.pp.highly_variable_genes(celldata, n_top_genes=n_top_genes)
             celldata = celldata[:, celldata.var.highly_variable].copy()
 
-        #celldata.X = celldata.X.toarray()
+        # celldata.X = celldata.X.toarray()
         celldata.uns["metadata"] = metadata
 
         celldata.uns["img_to_patient_dict"] = {"1": "1"}
         self.img_to_patient_dict = {"1": "1"}
         print(celldata)
         self.celldata = celldata
 
     def _register_img_celldata(self):
         """Load dictionary of of image-wise celldata objects with {imgage key : anndata object of image}."""
-        #image_col = self.celldata.uns["metadata"]["image_col"]
-        #img_celldata = {}
-        #for k in self.celldata.uns["img_keys"]:
+        # image_col = self.celldata.uns["metadata"]["image_col"]
+        # img_celldata = {}
+        # for k in self.celldata.uns["img_keys"]:
         #    img_celldata[str(k)] = self.celldata[self.celldata.obs[image_col] == k].copy()
-        #self.img_celldata = img_celldata
+        # self.img_celldata = img_celldata
         self.img_celldata = {"1": self.celldata}
 
     def _register_graph_features(self, label_selection):
         """Load graph level covariates.
 
         Parameters
         ----------
@@ -4216,15 +4212,15 @@
         "x_28_": "Megacaryocyte",
         "x_29_": "Mesenchymal",
     }
 
     def _register_celldata(self, n_top_genes: Optional[int] = None):
         """Load AnnData object of complete dataset."""
         metadata = {
-            "lateral_resolution": 1.,
+            "lateral_resolution": 1.0,
             "fn": "Cell_type/PCW13/S1T1_pciseq_mALL_pciseq_results_V02.csv",
             "cluster_col": "name",
             "cluster_col_preprocessed": "name_preprocessed",
             "pos_cols": ["X", "Y"],
         }
 
         celldata_df = read_csv(os.path.join(self.data_path, metadata["fn"]))
```

### Comparing `ncem-0.1.4/ncem/estimators/__init__.py` & `ncem-0.1.5/ncem/estimators/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Importing estimator classes."""
 from ncem.estimators.base_estimator import (Estimator, EstimatorGraph,
                                             EstimatorNoGraph)
 from ncem.estimators.base_estimator_neighbors import EstimatorNeighborhood
 from ncem.estimators.estimator_cvae import EstimatorCVAE
 from ncem.estimators.estimator_cvae_ncem import EstimatorCVAEncem
+from ncem.estimators.estimator_deconvolution import EstimatorDeconvolution
 from ncem.estimators.estimator_ed import EstimatorED
-from ncem.estimators.estimator_ed_ncem import EstimatorEDncem, EstimatorEdNcemNeighborhood
+from ncem.estimators.estimator_ed_ncem import (EstimatorEDncem,
+                                               EstimatorEdNcemNeighborhood)
 from ncem.estimators.estimator_interactions import EstimatorInteractions
 from ncem.estimators.estimator_linear import EstimatorLinear
-from ncem.estimators.estimator_deconvolution import EstimatorDeconvolution
```

### Comparing `ncem-0.1.4/ncem/estimators/base_estimator.py` & `ncem-0.1.5/ncem/estimators/base_estimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     def _load_data(
         self,
         data_origin: str,
         data_path: str,
         radius: Optional[int] = None,
         n_rings: int = 1,
         label_selection: Optional[List[str]] = None,
-        n_top_genes: Optional[int] = None
+        n_top_genes: Optional[int] = None,
     ):
         """Initialize a DataLoader object.
 
         Parameters
         ----------
         data_origin : str
             Data origin.
@@ -132,15 +132,15 @@
             N top genes for highly variable gene selection.
 
         Raises
         ------
         ValueError
             If `data_origin` not recognized.
         """
-        coord_type = 'generic'
+        coord_type = "generic"
         self.targeted_assay = True
         if data_origin.startswith("zhang"):
             from ncem.data import DataLoaderZhang as DataLoader
 
             self.undefined_node_types = ["other"]
         elif data_origin.startswith("jarosch"):
             from ncem.data import DataLoaderJarosch as DataLoader
@@ -159,74 +159,80 @@
 
             self.undefined_node_types = [
                 "dirt",
                 "undefined",
                 "tumor cells / immune cells",
                 "immune cells / vasculature",
             ]
-        elif data_origin.startswith('lohoff'):
+        elif data_origin.startswith("lohoff"):
             from ncem.data import DataLoaderLohoff as DataLoader
-            self.undefined_node_types = ['Low quality']
+
+            self.undefined_node_types = ["Low quality"]
         elif data_origin.startswith("luwt"):
             if data_origin == "luwt_imputation":
                 from ncem.data import DataLoaderLuWTimputed as DataLoader
             else:
                 from ncem.data import DataLoaderLuWT as DataLoader
 
-            self.undefined_node_types = ['Unknown']
+            self.undefined_node_types = ["Unknown"]
         elif data_origin.startswith("lutet2"):
             from ncem.data import DataLoaderLuTET2 as DataLoader
 
-            self.undefined_node_types = ['Unknown']
+            self.undefined_node_types = ["Unknown"]
         elif data_origin == "10xvisium":
             from ncem.data import DataLoader10xVisiumMouseBrain as DataLoader
 
             self.undefined_node_types = None
             if n_rings > 1:
-                coord_type = 'grid'
+                coord_type = "grid"
             else:
                 n_rings = 1
-                coord_type = 'generic'
+                coord_type = "generic"
                 radius = 0
         elif data_origin == "10xvisium_lymphnode":
             from ncem.data import DataLoader10xLymphnode as DataLoader
 
             self.undefined_node_types = None
             if n_rings > 1:
-                coord_type = 'grid'
+                coord_type = "grid"
             else:
                 n_rings = 1
-                coord_type = 'generic'
+                coord_type = "generic"
                 radius = 0
 
-        elif data_origin.startswith('destvi_lymphnode'):
+        elif data_origin.startswith("destvi_lymphnode"):
             self.targeted_assay = False
             from ncem.data import DataLoaderDestViLymphnode as DataLoader
 
             self.undefined_node_types = None
-        elif data_origin.startswith('destvi_mousebrain'):
+        elif data_origin.startswith("destvi_mousebrain"):
             self.targeted_assay = False
             from ncem.data import DataLoaderDestViMousebrain as DataLoader
 
             self.undefined_node_types = None
 
-        elif data_origin.startswith('cell2location_lymphnode'):
+        elif data_origin.startswith("cell2location_lymphnode"):
             self.targeted_assay = False
-            from ncem.data import DataLoaderCell2locationLymphnode as DataLoader
+            from ncem.data import \
+                DataLoaderCell2locationLymphnode as DataLoader
 
             self.undefined_node_types = None
 
         elif data_origin == "salasiss":
             from ncem.data import DataLoaderSalasIss as DataLoader
 
             self.undefined_node_types = None
 
         self.data = DataLoader(
-            data_path, radius=radius, coord_type=coord_type, n_rings=n_rings, label_selection=label_selection,
-            n_top_genes=n_top_genes
+            data_path,
+            radius=radius,
+            coord_type=coord_type,
+            n_rings=n_rings,
+            label_selection=label_selection,
+            n_top_genes=n_top_genes,
         )
 
     def get_data(
         self,
         data_origin: str,
         data_path: str,
         radius: Optional[int],
@@ -293,29 +299,31 @@
         labels_to_load = graph_covar_selection
         self._load_data(
             data_origin=data_origin,
             data_path=data_path,
             radius=radius,
             n_rings=n_rings,
             label_selection=labels_to_load,
-            n_top_genes=n_top_genes
+            n_top_genes=n_top_genes,
         )
         if robustness:
             np.random.seed(robustness_seed)
             n_images = np.int(len(self.data.img_celldata) * robustness)
             print(n_images)
-            image_keys = list(np.random.choice(
-                a=list(self.data.img_celldata.keys()),
-                size=n_images,
-                replace=False,
-            ))
+            image_keys = list(
+                np.random.choice(
+                    a=list(self.data.img_celldata.keys()),
+                    size=n_images,
+                    replace=False,
+                )
+            )
             self.data.img_celldata = {k: self.data.img_celldata[k] for k in image_keys}
             metadata = self.data.celldata.uns["metadata"]
 
-            self.data.celldata = self.data.celldata[self.data.celldata.obs[metadata['image_col']].isin(image_keys)]
+            self.data.celldata = self.data.celldata[self.data.celldata.obs[metadata["image_col"]].isin(image_keys)]
 
             print(
                 "\nAttention: Running robustness model with a fraction %f images, so [%i] images. \n"
                 "\nThis also adjusts celldata and img_celldata."
                 % (
                     robustness,
                     n_images,
@@ -325,113 +333,124 @@
             node_fraction = segmentation_robustness[0]
             overflow_fraction = segmentation_robustness[1]
             total_size = np.int(self.data.celldata.shape[0] * node_fraction)
 
             for key, ad in self.data.img_celldata.items():
                 size = np.int(ad.shape[0] * node_fraction)
                 random_indices = np.random.choice(ad.shape[0], size=size, replace=False)
-                a = ad.obsp['adjacency_matrix_connectivities'].toarray()
+                a = ad.obsp["adjacency_matrix_connectivities"].toarray()
                 err_ad = ad.copy()
                 for idx in random_indices:
                     adj = a[idx, :]
-                    neigh_idx = np.random.choice(np.where(adj == 1.)[0], size=1, replace=False)
+                    neigh_idx = np.random.choice(np.where(adj == 1.0)[0], size=1, replace=False)
                     err_ad.X[idx, :] = ad.X[idx, :] + overflow_fraction * ad.X[neigh_idx, :]
-                    err_ad.X[neigh_idx, :] = (1. - overflow_fraction) * ad.X[neigh_idx, :]
+                    err_ad.X[neigh_idx, :] = (1.0 - overflow_fraction) * ad.X[neigh_idx, :]
                 self.data.img_celldata[key] = err_ad
 
             print(
                 "\nAttention: Running segmentation robustness model on %f of all nodes, so [%i] nodes. \n"
                 "\nSignal overflow is set to %f . This adjusts img_celldata, celldata remains unchanged.\n"
-                % (
-                    node_fraction,
-                    total_size,
-                    overflow_fraction
-                )
+                % (node_fraction, total_size, overflow_fraction)
             )
         self.simulation = False
         if resimulate_nodes:
             self.simulation = True
             n_target_cell_types = 2 if resimulate_nodes_w_depdency else 1
             dependencies_per_type = 1
 
             # Create map from real cell types to simulated ones (can be coarser):
             found_all_types = False
             futile_counter = 0
             node_type_map_idx = None
             while not found_all_types:
-                node_type_map_idx = np.array([
-                    np.random.randint(low=0, high=n_target_cell_types)
-                    for _ in self.data.celldata.uns["node_type_names"].keys()
-                ])
+                node_type_map_idx = np.array(
+                    [
+                        np.random.randint(low=0, high=n_target_cell_types)
+                        for _ in self.data.celldata.uns["node_type_names"].keys()
+                    ]
+                )
                 futile_counter += 1
                 if np.all([x in node_type_map_idx for x in range(n_target_cell_types)]):
                     found_all_types = True
                 if futile_counter > 100:
                     raise ValueError("did not manage to sample all target cell types")
-            node_type_names = dict([
-                (x, "sim_" + str(y))
-                for x, y in zip(self.data.celldata.uns["node_type_names"].keys(), node_type_map_idx)
-            ])
+            node_type_names = dict(
+                [
+                    (x, "sim_" + str(y))
+                    for x, y in zip(self.data.celldata.uns["node_type_names"].keys(), node_type_map_idx)
+                ]
+            )
             self.data.celldata.uns["node_type_names"] = node_type_names
 
             nfeatures = self.data.img_celldata[list(self.data.img_celldata.keys())[0]].n_vars
             # Mean effect per simulated cell types:
-            effect_ct = np.random.uniform(low=0., high=10., size=(n_target_cell_types, nfeatures))
+            effect_ct = np.random.uniform(low=0.0, high=10.0, size=(n_target_cell_types, nfeatures))
             # Create dependency structure of cell types.
             # Base line dependency structure with all dependencies as 0.
             cov_ct = np.zeros((n_target_cell_types, n_target_cell_types))
             if resimulate_nodes_w_depdency:
                 # Add dependencies_per_type for each cell type:
                 for i in range(n_target_cell_types):
                     # Sample desired dependencies from non-self cell types:
-                    js = np.random.choice(a=[ii for ii in range(n_target_cell_types) if i != ii],
-                                          size=dependencies_per_type, replace=False)
-                    cov_ct[i, js] = 1.
+                    js = np.random.choice(
+                        a=[ii for ii in range(n_target_cell_types) if i != ii],
+                        size=dependencies_per_type,
+                        replace=False,
+                    )
+                    cov_ct[i, js] = 1.0
                 # Pairwise dependencies: Effect (self cell type, neighbor cell type, feature)
-                effect_neighbors = np.random.uniform(low=4., high=6.,
-                                                     size=(n_target_cell_types, n_target_cell_types, nfeatures))
+                effect_neighbors = np.random.uniform(
+                    low=4.0, high=6.0, size=(n_target_cell_types, n_target_cell_types, nfeatures)
+                )
                 # Simulate sparse effects:
                 sparsity_rate = resimulate_nodes_sparsity_rate  # fraction of zero effects
-                effect_neighbors[np.random.binomial(n=1, p=sparsity_rate, size=effect_neighbors.shape) == 1.] = 0.
+                effect_neighbors[np.random.binomial(n=1, p=sparsity_rate, size=effect_neighbors.shape) == 1.0] = 0.0
             else:
                 effect_neighbors = np.zeros((n_target_cell_types, n_target_cell_types, nfeatures))
-            sigma_sq = 1.
+            sigma_sq = 1.0
 
             self._simulation_parameters = {
                 "effect_ct": effect_ct,
                 "cov_ct": cov_ct,
                 "effect_neighbors": effect_neighbors,
                 "sigma_sq": sigma_sq,
-                "adatas": {}
+                "adatas": {},
             }
             for key, ad in self.data.img_celldata.items():
-                adj = ad.obsp['adjacency_matrix_connectivities'].toarray()
+                adj = ad.obsp["adjacency_matrix_connectivities"].toarray()
                 sim_ad = ad.copy()
                 nobs = sim_ad.n_obs
                 # Assign all cells from old cell type sets to corresponding new cell types, assumes one hot encoding.
-                sim_ad.obsm["node_types"] = np.concatenate([
-                    np.expand_dims(
-                        np.max(sim_ad.obsm["node_types"][:, np.where(node_type_map_idx == i)[0]], axis=1),
-                        axis=1
-                    )
-                    for i in range(n_target_cell_types)
-                ], axis=1)
-                assert np.all(sim_ad.obsm["node_types"].sum(axis=1) == 1.)
+                sim_ad.obsm["node_types"] = np.concatenate(
+                    [
+                        np.expand_dims(
+                            np.max(sim_ad.obsm["node_types"][:, np.where(node_type_map_idx == i)[0]], axis=1), axis=1
+                        )
+                        for i in range(n_target_cell_types)
+                    ],
+                    axis=1,
+                )
+                assert np.all(sim_ad.obsm["node_types"].sum(axis=1) == 1.0)
                 # Simulate count matrix:
                 dmat_ct = sim_ad.obsm["node_types"]
                 loc_neighbors = np.zeros((nobs, nfeatures))
                 for i in range(nobs):
-                    ct = np.where(dmat_ct[i, :] == 1.)[0]
+                    ct = np.where(dmat_ct[i, :] == 1.0)[0]
                     ct = ct[0]  # flatten list of length 1
-                    dmat_neighhors_i = np.zeros((1, n_target_cell_types,))
+                    dmat_neighhors_i = np.zeros(
+                        (
+                            1,
+                            n_target_cell_types,
+                        )
+                    )
                     if resimulate_nodes_w_depdency:
                         for j in np.where(np.asarray(adj[i, :]).flatten() > 0)[0]:
-                            ct_j = np.where(dmat_ct[j, :] == 1.)[0]
+                            ct_j = np.where(dmat_ct[j, :] == 1.0)[0]
                             ct_j = ct_j[0]  # flatten list of length 1
-                            dmat_neighhors_i[0, ct_j] = 1.
+                            dmat_neighhors_i[0, ct_j] = 1.0
                     loc_neighbors[i, :] = np.matmul(dmat_neighhors_i, effect_neighbors[ct])[0]
                 loc = np.matmul(dmat_ct, effect_ct) + loc_neighbors
                 sim_ad.X = np.random.normal(loc=loc, scale=sigma_sq)
                 self.data.img_celldata[key] = sim_ad
                 # Record simulation:
                 self._simulation_parameters["adatas"][key] = {
                     "adj": adj,
@@ -465,15 +484,15 @@
         self.a = {k: adata.obsp["adjacency_matrix_connectivities"] for k, adata in self.data.img_celldata.items()}
         if self.adj_type == "scaled":
             self.a = self.data._transform_all_a(self.a)
         if node_label_space_id == "standard":
             self.h_0 = {k: adata.X for k, adata in self.data.img_celldata.items()}
         elif node_label_space_id == "type":
             self.h_0 = {k: adata.obsm["node_types"] for k, adata in self.data.img_celldata.items()}
-        elif node_label_space_id == 'proportions':
+        elif node_label_space_id == "proportions":
             self.h_0 = {k: adata.obsm["proportions"] for k, adata in self.data.img_celldata.items()}
         else:
             raise ValueError("node_label_space_id %s not recognized" % node_label_space_id)
         if node_feature_space_id == "standard":
             self.h_1 = {k: adata.X for k, adata in self.data.img_celldata.items()}
         elif node_feature_space_id == "type":
             self.h_1 = {k: adata.obsm["node_types"] for k, adata in self.data.img_celldata.items()}
```

### Comparing `ncem-0.1.4/ncem/estimators/base_estimator_neighbors.py` & `ncem-0.1.5/ncem/estimators/base_estimator_neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,23 @@
             features = self.data.var_names.tolist()
             self.features = features
             self.target_feature_names = target_feature_names
             self.neighbor_feature_names = neighbor_feature_names
             self.idx_target_features = np.array([features.index(x) for x in target_feature_names])
             self.idx_neighbor_features = np.array([features.index(x) for x in neighbor_feature_names])
             assert len(self.idx_target_features) == len(self.idx_neighbor_features)
-            #assert len(set(self.idx_target_features.tolist()).intersection(set(self.idx_neighbor_features.tolist()))) == 0
+            # assert len(set(self.idx_target_features.tolist()).intersection(set(self.idx_neighbor_features.tolist()))) == 0
             self.n_features_in = len(self.idx_target_features)
 
     @property
     def n_neighbors_padded(self):
         if self._n_neighbors_padded is None:
-            self._n_neighbors_padded = int(np.max(np.asarray([
-                np.max(np.asarray(np.sum(a, axis=1)).flatten()) for a in self.a.values()
-            ])))
+            self._n_neighbors_padded = int(
+                np.max(np.asarray([np.max(np.asarray(np.sum(a, axis=1)).flatten()) for a in self.a.values()]))
+            )
         return self._n_neighbors_padded
 
     def _get_output_signature(self, resampled: bool = False):
         """Get output signatures.
 
         Parameters
         ----------
@@ -61,17 +61,15 @@
             Whether dataset is resampled or not.
 
         Returns
         -------
         output_signature
         """
         # target node features
-        h_targets = tf.TensorSpec(
-            shape=(self.n_eval_nodes_per_graph, self.n_features_in), dtype=tf.float32
-        )
+        h_targets = tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_in), dtype=tf.float32)
         # neighbor node features
         h_neighbors = tf.TensorSpec(
             shape=(self.n_eval_nodes_per_graph, self.n_neighbors_padded, self.n_features_in), dtype=tf.float32
         )
         sf = tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, 1), dtype=tf.float32)  # input node size factors
         # node-level covariates
         node_covar = tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_node_covariates), dtype=tf.float32)
@@ -89,27 +87,25 @@
                 output_signature = (
                     (h_targets, h_neighbors, sf, a, node_covar, domain),
                     (reconstruction, kl_dummy),
                     (h_targets, h_neighbors, sf, a, node_covar, domain),
                     (reconstruction, kl_dummy),
                 )
             else:
-                output_signature = ((h_targets, h_neighbors, sf, a, node_covar, domain),
-                                    (reconstruction, kl_dummy))
+                output_signature = ((h_targets, h_neighbors, sf, a, node_covar, domain), (reconstruction, kl_dummy))
         else:
             if resampled:
                 output_signature = (
                     (h_targets, h_neighbors, sf, a, node_covar, domain),
                     reconstruction,
                     (h_targets, h_neighbors, sf, a, node_covar, domain),
                     reconstruction,
                 )
             else:
-                output_signature = ((h_targets, h_neighbors, sf, a, node_covar, domain),
-                                    reconstruction)
+                output_signature = ((h_targets, h_neighbors, sf, a, node_covar, domain), reconstruction)
         # print(output_signature)
         return output_signature
 
     def _get_dataset(
         self,
         image_keys: List[str],
         nodes_idx: Dict[str, np.ndarray],
@@ -170,15 +166,15 @@
                             dtype=np.int32,
                         )
                     ]
                 else:
                     # dropping
                     index_list = [
                         np.asarray(
-                            nodes_idx[key][self.n_eval_nodes_per_graph * i: self.n_eval_nodes_per_graph * (i + 1)],
+                            nodes_idx[key][self.n_eval_nodes_per_graph * i : self.n_eval_nodes_per_graph * (i + 1)],
                             dtype=np.int32,
                         )
                         for i in range(len(nodes_idx[key]) // self.n_eval_nodes_per_graph)
                     ]
 
                 for indices in index_list:
                     h_out = self.h_1[key][idx_nodes[indices], :]
@@ -186,26 +182,26 @@
                         h_targets = self.h_0[key][idx_nodes[indices], :]
                     else:
                         h_targets = self.h_1[key][idx_nodes[indices], :][:, self.idx_target_features]
                     h_neighbors = []
                     a_neighborhood = np.zeros((self.n_eval_nodes_per_graph, self.n_neighbors_padded), "float32")
                     for i, j in enumerate(idx_nodes[indices]):
                         a_j = np.asarray(self.a[key][j, :].todense()).flatten()
-                        idx_neighbors = np.where(a_j > 0.)[0]
+                        idx_neighbors = np.where(a_j > 0.0)[0]
                         if self.h0_in:
                             h_neighbors_j = self.h_0[key][idx_neighbors, :]
                         else:
                             h_neighbors_j = self.h_1[key][idx_neighbors, :][:, self.idx_neighbor_features]
                         h_neighbors_j = np.expand_dims(h_neighbors_j, axis=0)
                         # Pad neighborhoods:
                         diff = self.n_neighbors_padded - h_neighbors_j.shape[1]
                         zeros = np.zeros((1, diff, h_neighbors_j.shape[2]), dtype="float32")
                         h_neighbors_j = np.concatenate([h_neighbors_j, zeros], axis=1)
                         h_neighbors.append(h_neighbors_j)
-                        a_neighborhood[i, :len(idx_neighbors)] = a_j[idx_neighbors]
+                        a_neighborhood[i, : len(idx_neighbors)] = a_j[idx_neighbors]
                     h_neighbors = np.concatenate(h_neighbors, axis=0)
                     if self.log_transform:
                         h_targets = np.log(h_targets + 1.0)
                         h_neighbors = np.log(h_neighbors + 1.0)
 
                     node_covar = self.node_covar[key][idx_nodes][indices, :]
                     sf = np.expand_dims(self.size_factors[key][idx_nodes][indices], axis=1)
```

### Comparing `ncem-0.1.4/ncem/estimators/estimator_cvae.py` & `ncem-0.1.5/ncem/estimators/estimator_cvae.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/estimators/estimator_cvae_ncem.py` & `ncem-0.1.5/ncem/estimators/estimator_cvae_ncem.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/estimators/estimator_deconvolution.py` & `ncem-0.1.5/ncem/estimators/estimator_deconvolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                             dtype=np.int32,
                         )
                     ]
                 else:
                     # dropping
                     index_list = [
                         np.asarray(
-                            nodes_idx[key][self.n_eval_nodes_per_graph * i: self.n_eval_nodes_per_graph * (i + 1)],
+                            nodes_idx[key][self.n_eval_nodes_per_graph * i : self.n_eval_nodes_per_graph * (i + 1)],
                             dtype=np.int32,
                         )
                         for i in range(len(nodes_idx[key]) // self.n_eval_nodes_per_graph)
                     ]
 
                 for indices in index_list:
                     h_0 = self.h_0[key][idx_nodes]
@@ -130,15 +130,15 @@
                     interactions = np.asarray(dmatrix("target:proportions-1", data))
 
                     interactions = coo_matrix(interactions)
                     coo = interactions.tocoo()
                     interactions_ind = np.asarray(np.mat([coo.row, coo.col]).transpose(), dtype="int64")
                     interactions_val = np.asarray(coo.data, dtype="float32")
                     interactions_shape = np.asarray(
-                        (self.n_eval_nodes_per_graph, self.n_features_0 ** 2), dtype="int64"
+                        (self.n_eval_nodes_per_graph, self.n_features_0**2), dtype="int64"
                     )
                     interactions = tf.SparseTensor(
                         indices=interactions_ind, values=interactions_val, dense_shape=interactions_shape
                     )
 
                     node_covar = self.node_covar[key][idx_nodes]
                     diff = self.max_nodes - node_covar.shape[0]
@@ -159,21 +159,21 @@
 
         print(self.n_features_0)
         dataset = tf.data.Dataset.from_generator(
             generator=generator,
             output_signature=(
                 (
                     tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_0), dtype=tf.float32),
-                    tf.SparseTensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_0 ** 2), dtype=tf.float32),
+                    tf.SparseTensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_0**2), dtype=tf.float32),
                     tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, 1), dtype=tf.float32),
                     tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_node_covariates), dtype=tf.float32),
                     tf.TensorSpec(shape=(self.n_domains,), dtype=tf.int32),
                 ),
                 tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_1), dtype=tf.float32),
-            )
+            ),
         )
         if train:
             if shuffle_buffer_size is not None:
                 dataset = dataset.shuffle(buffer_size=shuffle_buffer_size, seed=None, reshuffle_each_iteration=True)
             dataset = dataset.repeat()
         dataset = dataset.batch(batch_size)
         dataset = dataset.prefetch(prefetch)
@@ -245,15 +245,15 @@
             Arbitrary keyword arguments.
         """
         self.n_eval_nodes_per_graph = n_eval_nodes_per_graph
         self.model = ModelInteractions(
             input_shapes=(
                 self.n_features_0,  # target_dim
                 self.n_features_1,  # out_node_feature_dim
-                self.n_features_0 ** 2,  # interaction_dim
+                self.n_features_0**2,  # interaction_dim
                 self.n_eval_nodes_per_graph,  # in_node_dim
                 self.n_node_covariates,  # categ_condition_dim
                 self.n_domains,  # domain_dim
             ),
             l1_coef=l1_coef,
             l2_coef=l2_coef,
             use_interactions=use_interactions,
```

### Comparing `ncem-0.1.4/ncem/estimators/estimator_ed.py` & `ncem-0.1.5/ncem/estimators/estimator_ed.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/estimators/estimator_ed_ncem.py` & `ncem-0.1.5/ncem/estimators/estimator_ed_ncem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import abc
-import tensorflow as tf
 from typing import Tuple, Union
 
+import tensorflow as tf
+
 from ncem.estimators import Estimator, EstimatorGraph, EstimatorNeighborhood
 from ncem.estimators.base_estimator import transfer_layers
-from ncem.models import ModelEDncem, ModelEd2Ncem
+from ncem.models import ModelEd2Ncem, ModelEDncem
 from ncem.models.layers.output_layers import IDENTIFIER_OUTPUT_LAYER
 
 
 class EstimatorEDncemBase(Estimator, abc.ABC):
     model: Union[ModelEDncem, ModelEd2Ncem]
 
     def predict_embedding_any(self, img_keys, node_idx, batch_size: int = 1):
```

### Comparing `ncem-0.1.4/ncem/estimators/estimator_interactions.py` & `ncem-0.1.5/ncem/estimators/estimator_interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                     #    (self.n_eval_nodes_per_graph, self.n_features_0 ** 2), dtype="int64"
                     # )
                     interactions = coo_matrix(interactions)
                     coo = interactions.tocoo()
                     interactions_ind = np.asarray(np.mat([coo.row, coo.col]).transpose(), dtype="int64")
                     interactions_val = np.asarray(coo.data, dtype="float32")
                     interactions_shape = np.asarray(
-                        (self.n_eval_nodes_per_graph, self.n_features_0 ** 2), dtype="int64"
+                        (self.n_eval_nodes_per_graph, self.n_features_0**2), dtype="int64"
                     )
                     interactions = tf.SparseTensor(
                         indices=interactions_ind, values=interactions_val, dense_shape=interactions_shape
                     )
 
                     node_covar = self.node_covar[key][idx_nodes]
                     diff = self.max_nodes - node_covar.shape[0]
@@ -169,15 +169,15 @@
                     yield (target, interactions, sf, node_covar, g), h_1
 
         dataset = tf.data.Dataset.from_generator(
             generator=generator,
             output_signature=(
                 (
                     tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_0), dtype=tf.float32),
-                    tf.SparseTensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_0 ** 2), dtype=tf.float32),
+                    tf.SparseTensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_0**2), dtype=tf.float32),
                     tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, 1), dtype=tf.float32),
                     tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_node_covariates), dtype=tf.float32),
                     tf.TensorSpec(shape=(self.n_domains,), dtype=tf.int32),
                 ),
                 tf.TensorSpec(shape=(self.n_eval_nodes_per_graph, self.n_features_1), dtype=tf.float32),
             ),
         )
@@ -255,15 +255,15 @@
             Arbitrary keyword arguments.
         """
         self.n_eval_nodes_per_graph = n_eval_nodes_per_graph
         self.model = ModelInteractions(
             input_shapes=(
                 self.n_features_0,  # target_dim
                 self.n_features_1,  # out_node_feature_dim
-                self.n_features_0 ** 2,  # interaction_dim
+                self.n_features_0**2,  # interaction_dim
                 self.n_eval_nodes_per_graph,  # in_node_dim
                 self.n_node_covariates,  # categ_condition_dim
                 self.n_domains,  # domain_dim
             ),
             l1_coef=l1_coef,
             l2_coef=l2_coef,
             use_interactions=use_interactions,
```

### Comparing `ncem-0.1.4/ncem/estimators/estimator_linear.py` & `ncem-0.1.5/ncem/estimators/estimator_linear.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/interpretation/interpreter.py` & `ncem-0.1.5/ncem/interpretation/interpreter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import pickle
 from collections import OrderedDict
 from typing import Dict, List, Optional, Tuple, Union
 
 import matplotlib.colors as colors
 import matplotlib.pyplot as plt
+import networkx as nx
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import seaborn as sns
 import tensorflow as tf
 from anndata import AnnData
 from diffxpy.testing.correction import correct
+from patsy import dmatrix
 from scipy import sparse, stats
 from scipy.sparse import csr_matrix
 from tqdm import tqdm
-import networkx as nx
 
 import ncem.estimators as estimators
 import ncem.models as models
 import ncem.train as train
-from ncem.utils.wald_test import get_fim_inv, wald_test
 from ncem.utils.ols_fit import ols_fit
-from patsy import dmatrix
+from ncem.utils.wald_test import get_fim_inv, wald_test
 
 
 def _get_scanpy_colors():
     from typing import Mapping, Sequence
+
     from matplotlib import cm, colors
 
     # Colorblindness adjusted vega_10
     # See https://github.com/theislab/scanpy/issues/387
     vega_10 = list(map(colors.to_hex, cm.tab10.colors))
     vega_10_scanpy = vega_10.copy()
-    vega_10_scanpy[2] = '#279e68'  # green
-    vega_10_scanpy[4] = '#aa40fc'  # purple
-    vega_10_scanpy[8] = '#b5bd61'  # kakhi
+    vega_10_scanpy[2] = "#279e68"  # green
+    vega_10_scanpy[4] = "#aa40fc"  # purple
+    vega_10_scanpy[8] = "#b5bd61"  # kakhi
 
     # default matplotlib 2.0 palette
     # see 'category20' on https://github.com/vega/vega/wiki/Scales#scale-range-literals
     vega_20 = list(map(colors.to_hex, cm.tab20.colors))
 
     # reorderd, some removed, some added
     vega_20_scanpy = [
         # dark without grey:
         *vega_20[0:14:2],
         *vega_20[16::2],
         # light without grey:
         *vega_20[1:15:2],
         *vega_20[17::2],
         # manual additions:
-        '#ad494a',
-        '#8c6d31',
+        "#ad494a",
+        "#8c6d31",
     ]
     vega_20_scanpy[2] = vega_10_scanpy[2]
     vega_20_scanpy[4] = vega_10_scanpy[4]
     vega_20_scanpy[7] = vega_10_scanpy[8]  # kakhi shifted by missing grey
-    
+
     zeileis_28 = [
         "#023fa5",
         "#7d87b9",
         "#bec1d4",
         "#d6bcc0",
         "#bb7784",
         "#8e063b",
@@ -78,22 +79,22 @@
         "#0fcfc0",
         "#9cded6",
         "#d5eae7",
         "#f3e1eb",
         "#f6c4e1",
         "#f79cd4",
         # these last ones were added:
-        '#7f7f7f',
+        "#7f7f7f",
         "#c7c7c7",
         "#1CE6FF",
         "#336600",
     ]
 
     default_28 = zeileis_28
-    
+
     return vega_10_scanpy, vega_20_scanpy, default_28
 
 
 class InterpreterBase(estimators.Estimator):
     """InterpreterBase class."""
 
     data_path: str
@@ -215,28 +216,28 @@
             nodes_idx (dict): Dictionary of nodes per image in partition.
             batch_size (int): Batch size.
             seed (int): Random seed.
             prefetch (int): Prefetch.
         """
         pass
 
-    def get_data_again(self, data_path: str, data_origin: str, n_top_genes = None):
+    def get_data_again(self, data_path: str, data_origin: str, n_top_genes=None):
         """Loads data as previously done during model training.
 
         Args:
             data_path (str): Data path.
             data_origin (str): Data origin.
 
         Raises:
             ValueError: If `cond_type` is not recognized.
         """
         self.cond_type = self.gscontainer_runparams["cond_type"] if "cond_type" in self.gscontainer_runparams else None
         if self.cond_type == "gcn":
             self.adj_type = "scaled"
-        elif self.cond_type in ["max", 'lr_gat', None]:
+        elif self.cond_type in ["max", "lr_gat", None]:
             self.adj_type = "full"
         else:
             raise ValueError("cond_type %s not recognized" % self.cond_type)
         if "radius" in self.gscontainer_runparams.keys():
             radius = int(self.gscontainer_runparams["radius"])
         else:
             radius = int(self.gscontainer_runparams["max_dist"])
@@ -258,15 +259,15 @@
             graph_covar_selection=self.gscontainer_runparams["graph_covar_selection"],
             node_label_space_id=node_label_space_id,
             node_feature_space_id=node_feature_space_id,
             use_covar_node_position=self.gscontainer_runparams["use_covar_node_position"],
             use_covar_node_label=self.gscontainer_runparams["use_covar_node_label"],
             use_covar_graph_covar=self.gscontainer_runparams["use_covar_graph_covar"],
             domain_type=self.gscontainer_runparams["domain_type"],
-            n_top_genes=n_top_genes
+            n_top_genes=n_top_genes,
         )
         self.data_path = data_path
         self.n_eval_nodes_per_graph = self.gscontainer_runparams["n_eval_nodes_per_graph"]
         self.model_class = self.gscontainer_runparams["model_class"]
         self.data_set = self.gscontainer_runparams["data_set"]
         self.radius = radius
         self.cond_depth = (
@@ -309,16 +310,16 @@
             model = models.ModelED(**self._model_kwargs)
         elif self.model_class in ["ed_ncem", "clvmnp"]:
             model = models.ModelEDncem(**self._model_kwargs)
         elif self.model_class in ["linear", "linear_baseline"]:
             model = models.ModelLinear(**self._model_kwargs)
         elif self.model_class in ["interactions", "interactions_baseline"]:
             model = models.ModelInteractions(**self._model_kwargs)
-        elif self.model_class in ['ed_ncem2']:
-            model = models.ModelEd2Ncem(cond_type='lr_gat', **self._model_kwargs)
+        elif self.model_class in ["ed_ncem2"]:
+            model = models.ModelEd2Ncem(cond_type="lr_gat", **self._model_kwargs)
         elif self.model_class in ["deconvolution", "deconvolution_baseline"]:
             model = models.ModelInteractions(**self._model_kwargs)
         else:
             raise ValueError("model_class not recognized")
         self.model = model
 
         self.vi_model = False  # variational inference
@@ -489,19 +490,19 @@
         # Loop over sub-selected data set and sum gradients across all selected observations.
         target = []
         interactions = []
         sf = []
         node_covar = []
         g = []
         h_obs = []
-        
+
         count = 0
         for k, v in nodes_idx.items():
             count = count + len(v)
-        
+
         with tqdm(total=np.int(count / self.n_eval_nodes_per_graph)) as pbar:
             for _step, (x_batch, y_batch) in enumerate(ds):
                 target_batch, interaction_batch, sf_batch, node_covar_batch, g_batch = x_batch
                 target.append(target_batch.numpy().squeeze())
                 interactions.append(
                     csr_matrix(
                         (
@@ -512,22 +513,22 @@
                     ).todense()
                 )
                 sf.append(sf_batch.numpy().squeeze())
                 node_covar.append(node_covar_batch.numpy().squeeze())
                 g.append(g_batch.numpy().squeeze())
                 h_obs.append(y_batch[0].numpy().squeeze())
                 pbar.update(1)
-        
-        target = np.concatenate(target, axis=0)
-        interactions = np.concatenate(interactions, axis=0)
-        sf = np.concatenate(sf, axis=0)
-        node_covar = np.concatenate(node_covar, axis=0)
+
+        target = np.concatenate(np.expand_dims(target, axis=0), axis=0)
+        interactions = np.concatenate(np.expand_dims(interactions, axis=0), axis=0)
+        sf = np.concatenate(np.expand_dims(sf, axis=0), axis=0)
+        node_covar = np.concatenate(np.expand_dims(node_covar, axis=0), axis=0)
         g = np.array(g)
-        h_obs = np.concatenate(h_obs, axis=0)
-        
+        h_obs = np.concatenate(np.expand_dims(h_obs, axis=0), axis=0)
+
         return (target, interactions, sf, node_covar, g), h_obs
 
     def target_cell_relative_performance(
         self,
         image_key: str,
         baseline_model,
         target_cell_type: str,
@@ -894,504 +895,477 @@
         plt.tight_layout()
         if save is not None:
             plt.savefig(save + "_" + metric + suffix)
         if show:
             plt.show()
         plt.close(fig)
         plt.ion()
-    
-    def get_sender_receiver_effects(
-        self,
-        params_type: str = 'ols',
-        significance_threshold: float = 0.05
-    ):
+
+    def get_sender_receiver_effects(self, params_type: str = "ols", significance_threshold: float = 0.05):
         (target, interactions, _, _, _), y = self._get_np_data(
-            image_keys=self.img_keys_all, nodes_idx=self.nodes_idx_all)
+            image_keys=self.img_keys_all, nodes_idx=self.nodes_idx_all
+        )
 
-        print('using ols parameters.')
-        if params_type == 'ols':
-            x_design = np.concatenate([target, interactions], axis=1)
+        print("using ols parameters.")
+        if params_type == "ols":
+            print(target.shape)
+            print(interactions.shape)
+            x_design = np.concatenate([target, interactions.squeeze()], axis=1)
             ols = ols_fit(x_=x_design, y_=y)
             params = ols.squeeze()
         else:
-            params = (
-                self.model.training_model.weights[0]
-                .numpy()
-                .T
-            )
+            params = self.model.training_model.weights[0].numpy().T
 
         # get inverse fisher information matrix
-        print('calculating inv fim.')
+        print("calculating inv fim.")
         fim_inv = get_fim_inv(x_design, y)
 
+        interaction_shape = np.int(self.n_features_0**2)
+        params = params[:, self.n_features_0 : interaction_shape + self.n_features_0]
         is_sign, pvalues, qvalues = wald_test(
             params=params, fisher_inv=fim_inv, significance_threshold=significance_threshold
         )
-        interaction_shape = np.int(self.n_features_0**2)
-        # subset to interaction terms
-        is_sign = is_sign[self.n_features_0 : interaction_shape + self.n_features_0, :]
-        pvalues = pvalues[self.n_features_0 : interaction_shape + self.n_features_0, :]
-        qvalues = qvalues[self.n_features_0 : interaction_shape + self.n_features_0, :]
 
         self.pvalues = np.concatenate(
             np.expand_dims(np.split(pvalues, indices_or_sections=np.sqrt(pvalues.shape[0]), axis=0), axis=0),
             axis=0,
         )
         self.qvalues = np.concatenate(
             np.expand_dims(np.split(qvalues, indices_or_sections=np.sqrt(qvalues.shape[0]), axis=0), axis=0),
             axis=0,
         )
         self.is_sign = np.concatenate(
             np.expand_dims(np.split(is_sign, indices_or_sections=np.sqrt(is_sign.shape[0]), axis=0), axis=0),
             axis=0,
         )
 
-        interaction_params = params[:, self.n_features_0 : interaction_shape + self.n_features_0]
         self.fold_change = np.concatenate(
-            np.expand_dims(np.split(interaction_params.T, indices_or_sections=np.sqrt(interaction_params.T.shape[0]), axis=0), axis=0),
+            np.expand_dims(np.split(params.T, indices_or_sections=np.sqrt(params.T.shape[0]), axis=0), axis=0),
             axis=0,
         )
-        
+
     def type_coupling_analysis(
         self,
         undefined_types: Optional[List[str]] = None,
         fontsize: Optional[int] = None,
         figsize: Tuple[float, float] = (11.0, 10.0),
         save: Optional[str] = None,
         suffix: str = "_type_coupling_analysis.pdf",
         show: bool = True,
     ):
-        
+
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
-            plt.rcParams['axes.grid'] = False
-        sig_df = pd.DataFrame(
-            np.sum(self.is_sign, axis=-1), 
-            columns=self.cell_names,
-            index=self.cell_names
-        )
+            plt.rcParams["axes.grid"] = False
+        sig_df = pd.DataFrame(np.sum(self.is_sign, axis=-1), columns=self.cell_names, index=self.cell_names)
         if undefined_types:
             sig_df = sig_df.drop(columns=undefined_types, index=undefined_types)
         np.fill_diagonal(sig_df.values, 0)
-        plt.ioff()   
+        plt.ioff()
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
-        sns.heatmap(sig_df, cmap='Greys',)
-        plt.xlabel('sender')
-        plt.ylabel('receiver')
+        sns.heatmap(
+            sig_df,
+            cmap="Greys",
+        )
+        plt.xlabel("sender")
+        plt.ylabel("receiver")
         plt.tight_layout()
         if save is not None:
             plt.savefig(f"{save}_cv{str(self.cv_idx)}_{suffix}")
         if show:
             plt.show()
         plt.close(fig)
         plt.ion()
-        
+
     def type_coupling_analysis_circular(
         self,
         edge_attr: str,
-        edge_width_scale: float = 3.,
+        edge_width_scale: float = 3.0,
         fontsize: Optional[int] = None,
         figsize: Tuple[float, float] = (9, 8),
         de_genes_threshold: float = 0,
-        #magnitude_threshold: Optional[float] = None,
+        # magnitude_threshold: Optional[float] = None,
         save: Optional[str] = None,
         suffix: str = "_type_coupling_analysis_circular.pdf",
         show: bool = True,
         undefined_types: Optional[List[str]] = None,
-        text_space: float = 1.15
+        text_space: float = 1.15,
     ):
         coeff = self.fold_change * self.is_sign
-        coeff_df = pd.DataFrame(
-            np.sqrt(np.sum(coeff**2, axis=-1)), 
-            columns=self.cell_names,
-            index=self.cell_names
-        )
-        network_coeff_df = pd.DataFrame(coeff_df.unstack()).reset_index().rename(columns={'level_0': 'sender', 'level_1': 'receiver'})
-        network_coeff_df = network_coeff_df[network_coeff_df['receiver'] != network_coeff_df['sender']]
-        
-        sig_df = pd.DataFrame(
-            np.sum(self.is_sign, axis=-1), 
-            columns=self.cell_names,
-            index=self.cell_names
+        coeff_df = pd.DataFrame(np.sqrt(np.sum(coeff**2, axis=-1)), columns=self.cell_names, index=self.cell_names)
+        network_coeff_df = (
+            pd.DataFrame(coeff_df.unstack()).reset_index().rename(columns={"level_0": "sender", "level_1": "receiver"})
+        )
+        network_coeff_df = network_coeff_df[network_coeff_df["receiver"] != network_coeff_df["sender"]]
+
+        sig_df = pd.DataFrame(np.sum(self.is_sign, axis=-1), columns=self.cell_names, index=self.cell_names)
+        network_df = (
+            pd.DataFrame(sig_df.unstack()).reset_index().rename(columns={"level_0": "sender", "level_1": "receiver"})
         )
-        network_df = pd.DataFrame(sig_df.unstack()).reset_index().rename(columns={'level_0': 'sender', 'level_1': 'receiver'})
-        network_df = network_df[network_df['receiver'] != network_df['sender']]
+        network_df = network_df[network_df["receiver"] != network_df["sender"]]
         network_df["magnitude"] = network_coeff_df[0]
 
         network_df["de_genes"] = [
-            (np.abs(x) - np.min(np.abs(network_df[0].values))) / 
-            (np.max(np.abs(network_df[0].values)) - np.min(np.abs(network_df[0].values)))
-            for x in network_df[0].values]
+            (np.abs(x) - np.min(np.abs(network_df[0].values)))
+            / (np.max(np.abs(network_df[0].values)) - np.min(np.abs(network_df[0].values)))
+            for x in network_df[0].values
+        ]
         network_df["de_genes_abs"] = network_df[0]
 
         if undefined_types:
-            network_df = network_df[network_df['receiver'] != undefined_types]
-            network_df = network_df[network_df['sender'] != undefined_types]
+            network_df = network_df[network_df["receiver"] != undefined_types]
+            network_df = network_df[network_df["sender"] != undefined_types]
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
         vega_10_scanpy, vega_20_scanpy, default_28 = _get_scanpy_colors()
-        plt.ioff()   
+        plt.ioff()
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
-        ax.axis('off')
-        G=nx.from_pandas_edgelist(
-            network_df, source='sender', target='receiver', 
-            edge_attr=["magnitude", 'de_genes', 'de_genes_abs'], 
-            create_using=nx.DiGraph()
-        ) 
-        nodes = np.unique(network_df['receiver'])
-        pos=nx.circular_layout(G)
-        
+        ax.axis("off")
+        G = nx.from_pandas_edgelist(
+            network_df,
+            source="sender",
+            target="receiver",
+            edge_attr=["magnitude", "de_genes", "de_genes_abs"],
+            create_using=nx.DiGraph(),
+        )
+        nodes = np.unique(network_df["receiver"])
+        pos = nx.circular_layout(G)
+
         if len(nodes) <= 10:
-            nx.set_node_attributes(G, dict([(x,vega_10_scanpy[i]) for i, x in enumerate(nodes)]), "color")
+            nx.set_node_attributes(G, dict([(x, vega_10_scanpy[i]) for i, x in enumerate(nodes)]), "color")
         elif len(nodes) <= 20:
-            nx.set_node_attributes(G, dict([(x,vega_20_scanpy[i]) for i, x in enumerate(nodes)]), "color")
+            nx.set_node_attributes(G, dict([(x, vega_20_scanpy[i]) for i, x in enumerate(nodes)]), "color")
         else:
-            nx.set_node_attributes(G, dict([(x,default_28[i]) for i, x in enumerate(nodes)]), "color")
-            
-        node_color = nx.get_node_attributes(G, 'color')
+            nx.set_node_attributes(G, dict([(x, default_28[i]) for i, x in enumerate(nodes)]), "color")
+
+        node_color = nx.get_node_attributes(G, "color")
 
-        description = nx.draw_networkx_labels(G,pos, font_size=17)
+        description = nx.draw_networkx_labels(G, pos, font_size=17)
         n = len(self.cell_names)
         node_list = sorted(G.nodes())
         angle = []
         angle_dict = {}
-        for i, node in zip(range(n),node_list):
-            theta = 2.0*np.pi*i/n
-            angle.append((np.cos(theta),np.sin(theta)))
+        for i, node in zip(range(n), node_list):
+            theta = 2.0 * np.pi * i / n
+            angle.append((np.cos(theta), np.sin(theta)))
             angle_dict[node] = theta
         pos = {}
         for node_i, node in enumerate(node_list):
             pos[node] = angle[node_i]
 
         r = fig.canvas.get_renderer()
         trans = plt.gca().transData.inverted()
         for node, t in description.items():
             bb = t.get_window_extent(renderer=r)
             bbdata = bb.transformed(trans)
-            radius = text_space +bbdata.width/2.
-            position = (radius*np.cos(angle_dict[node]),radius* np.sin(angle_dict[node]))
+            radius = text_space + bbdata.width / 2.0
+            position = (radius * np.cos(angle_dict[node]), radius * np.sin(angle_dict[node]))
             t.set_position(position)
-            t.set_rotation(angle_dict[node]*360.0/(2.0*np.pi))
+            t.set_rotation(angle_dict[node] * 360.0 / (2.0 * np.pi))
             t.set_clip_on(False)
-            
-        selected_edges = [(u,v) for u,v,e in G.edges(data=True) if e['de_genes_abs'] > de_genes_threshold]
-        width = [e[edge_attr] * edge_width_scale for u,v,e in G.edges(data=True) if e['de_genes_abs'] > de_genes_threshold]
-        
+
+        selected_edges = [(u, v) for u, v, e in G.edges(data=True) if e["de_genes_abs"] > de_genes_threshold]
+        width = [
+            e[edge_attr] * edge_width_scale for u, v, e in G.edges(data=True) if e["de_genes_abs"] > de_genes_threshold
+        ]
+
         nx.draw_networkx(
-            G, pos, with_labels=False, node_size=500, edgelist=selected_edges,
-            width=width, edge_vmin=0., edge_vmax=1., edge_cmap=plt.cm.seismic, arrowstyle='-|>', 
-            vmin=0., vmax=1., cmap=plt.cm.binary, node_color=list(node_color.values()),
-            ax=ax, connectionstyle='arc3, rad = 0.1'
+            G,
+            pos,
+            with_labels=False,
+            node_size=500,
+            edgelist=selected_edges,
+            width=width,
+            edge_vmin=0.0,
+            edge_vmax=1.0,
+            edge_cmap=plt.cm.seismic,
+            arrowstyle="-|>",
+            vmin=0.0,
+            vmax=1.0,
+            cmap=plt.cm.binary,
+            node_color=list(node_color.values()),
+            ax=ax,
+            connectionstyle="arc3, rad = 0.1",
         )
         plt.tight_layout()
         if save is not None:
             plt.savefig(f"{save}_cv{str(self.cv_idx)}_{suffix}")
         if show:
             plt.show()
         plt.close(fig)
         plt.ion()
         return network_df
-        
+
     def sender_receiver_values(
         self,
         receiver: str,
         sender: str,
     ):
         receiver_idx = self.cell_names.index(receiver)
         sender_idx = self.cell_names.index(sender)
-        
-        fold_change = self.fold_change[receiver_idx,sender_idx,:]
-        pvals = self.pvalues[receiver_idx,sender_idx,:]
-        qvals = self.qvalues[receiver_idx,sender_idx,:]
-        h_0 = pd.DataFrame(
-            self.data.celldata.obsm['node_types'], columns=self.cell_names
-        )
+
+        fold_change = self.fold_change[receiver_idx, sender_idx, :]
+        pvals = self.pvalues[receiver_idx, sender_idx, :]
+        qvals = self.qvalues[receiver_idx, sender_idx, :]
+        h_0 = pd.DataFrame(self.data.celldata.obsm["node_types"], columns=self.cell_names)
         target_type = pd.DataFrame(np.array(h_0.idxmax(axis=1)), columns=["target_cell"]).reset_index()
         self.data.celldata.obs = target_type
-        means = self.data.celldata[self.data.celldata.obs['target_cell'] == receiver].X.mean(axis=0)
-        
+        means = self.data.celldata[self.data.celldata.obs["target_cell"] == receiver].X.mean(axis=0)
+
         df = pd.DataFrame(
             np.array([means, pvals, qvals, fold_change]).T,
-            index=self.data.celldata.var_names, columns=['mean expression', 'pvalue', 'qvalue', 'fold change']
+            index=self.data.celldata.var_names,
+            columns=["mean expression", "pvalue", "qvalue", "fold change"],
         )
-        df['-log 10 qvalue'] = -np.log10(df['qvalue'])
-        
+        df["-log 10 qvalue"] = -np.log10(df["qvalue"])
+
         return df
-    
+
     def sender_similarity_analysis(
         self,
         receiver: str,
         fontsize: Optional[int] = None,
         figsize: Tuple[float, float] = (8.0, 8.0),
         save: Optional[str] = None,
         suffix: str = "_sender_similarity_analysis.pdf",
         show: bool = True,
-        cbar_pos: Tuple[float, float, float, float] = (-0.3, .1, .4, .02)
+        cbar_pos: Tuple[float, float, float, float] = (-0.3, 0.1, 0.4, 0.02),
     ):
         receiver_idx = self.cell_names.index(receiver)
-        
-        corrcoef = np.corrcoef(self.fold_change[receiver_idx,:,:])
-        corrcoef = pd.DataFrame(
-            corrcoef,
-            columns=self.cell_names,
-            index=self.cell_names
-        )
+
+        corrcoef = np.corrcoef(self.fold_change[receiver_idx, :, :])
+        corrcoef = pd.DataFrame(corrcoef, columns=self.cell_names, index=self.cell_names)
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
-            plt.rcParams['axes.grid'] = False
-        plt.ioff()   
+            plt.rcParams["axes.grid"] = False
+        plt.ioff()
         clustermap = sns.clustermap(
-            corrcoef, cmap='Purples',  
-            figsize=figsize, 
-            row_cluster=True, 
-            cbar_kws={'label': "correlation", "orientation": "horizontal"},
-            cbar_pos=cbar_pos
+            corrcoef,
+            cmap="Purples",
+            figsize=figsize,
+            row_cluster=True,
+            cbar_kws={"label": "correlation", "orientation": "horizontal"},
+            cbar_pos=cbar_pos,
         )
-        
+
         if save is not None:
             clustermap.savefig()
         if show:
             plt.show()
         plt.ion()
-        
+
     def sender_receiver_effect_vulcanoplot(
         self,
         receiver: str,
         sender: str,
         significance_threshold: float = 0.05,
         fold_change_threshold: float = 0.021671495152134755,
         fontsize: Optional[int] = None,
         figsize: Tuple[float, float] = (4.5, 7.0),
         save: Optional[str] = None,
         suffix: str = "_sender_receiver_volcanoplot.pdf",
         show: bool = True,
     ):
         receiver_idx = self.cell_names.index(receiver)
         sender_idx = self.cell_names.index(sender)
-        
+
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
-            plt.rcParams['axes.grid'] = False
-        fig, ax = plt.subplots(1,1, figsize=figsize)
+            plt.rcParams["axes.grid"] = False
+        fig, ax = plt.subplots(1, 1, figsize=figsize)
         ax.grid(False)
-        # only significant ones 
-        qval_filter = np.where(self.qvalues[receiver_idx,sender_idx,:]>=significance_threshold)
-        vmax = np.max(np.abs(self.fold_change[receiver_idx,sender_idx,:]))
-        #print(vmax)
-        
+        # only significant ones
+        qval_filter = np.where(self.qvalues[receiver_idx, sender_idx, :] >= significance_threshold)
+        vmax = np.max(np.abs(self.fold_change[receiver_idx, sender_idx, :]))
+        # print(vmax)
+
         # overlaying significant ones with orange
         sns.scatterplot(
-            x=self.fold_change[receiver_idx,sender_idx,:][qval_filter], 
-            y=-np.log10(self.qvalues[receiver_idx,sender_idx,:])[qval_filter], 
-            color='white', edgecolor = 'black', s=100, ax=ax)
+            x=self.fold_change[receiver_idx, sender_idx, :][qval_filter],
+            y=-np.log10(self.qvalues[receiver_idx, sender_idx, :])[qval_filter],
+            color="white",
+            edgecolor="black",
+            s=100,
+            ax=ax,
+        )
 
-        qval_filter = np.where(self.qvalues[receiver_idx,sender_idx,:]<significance_threshold)
-        x = self.fold_change[receiver_idx,sender_idx,:][qval_filter]
+        qval_filter = np.where(self.qvalues[receiver_idx, sender_idx, :] < significance_threshold)
+        x = self.fold_change[receiver_idx, sender_idx, :][qval_filter]
         fc_filter = np.where(x < fold_change_threshold)
-        y = -np.nan_to_num(np.log10(self.qvalues[receiver_idx,sender_idx,:])[qval_filter])
-        sns.scatterplot(
-            x=x[fc_filter], 
-            y=y[fc_filter], 
-            color='darkgrey', edgecolor = 'black', s=100, ax=ax)
-
-        x = self.fold_change[receiver_idx,sender_idx,:][qval_filter]
-        fc_filter = np.where(x<= -fold_change_threshold)
-        y = -np.nan_to_num(np.log10(self.qvalues[receiver_idx,sender_idx,:])[qval_filter], neginf=-14.5)
-        sns.scatterplot(
-            x=x[fc_filter], 
-            y=y[fc_filter], 
-            color='blue', edgecolor = 'black', s=100, ax=ax)
-
-        x = self.fold_change[receiver_idx,sender_idx,:][qval_filter]
-        fc_filter = np.where(x>= fold_change_threshold)
-        y = -np.nan_to_num(np.log10(self.qvalues[receiver_idx,sender_idx,:])[qval_filter], neginf=-14.5)
-        sns.scatterplot(
-            x=x[fc_filter], 
-            y=y[fc_filter], 
-            color='red', edgecolor = 'black', s=100, ax=ax)
-
-        ax.set_xlim((-vmax*1.1, vmax*1.1))
-        #ax.set_ylim((-0.5, np.min([y[fc_filter], 15])))
-        ax.set_xlabel('$\log$ fold change')
-        ax.set_ylabel('$-\log_{10}$ FDR-corrected pvalues')
-        plt.axvline(-fold_change_threshold, color='black', linestyle='--', )
-        plt.axvline(fold_change_threshold, color='black', linestyle='--', )
-        plt.axhline(-np.log10(significance_threshold), linestyle='--', color='black')
-        
+        y = -np.nan_to_num(np.log10(self.qvalues[receiver_idx, sender_idx, :])[qval_filter])
+        sns.scatterplot(x=x[fc_filter], y=y[fc_filter], color="darkgrey", edgecolor="black", s=100, ax=ax)
+
+        x = self.fold_change[receiver_idx, sender_idx, :][qval_filter]
+        fc_filter = np.where(x <= -fold_change_threshold)
+        y = -np.nan_to_num(np.log10(self.qvalues[receiver_idx, sender_idx, :])[qval_filter], neginf=-14.5)
+        sns.scatterplot(x=x[fc_filter], y=y[fc_filter], color="blue", edgecolor="black", s=100, ax=ax)
+
+        x = self.fold_change[receiver_idx, sender_idx, :][qval_filter]
+        fc_filter = np.where(x >= fold_change_threshold)
+        y = -np.nan_to_num(np.log10(self.qvalues[receiver_idx, sender_idx, :])[qval_filter], neginf=-14.5)
+        sns.scatterplot(x=x[fc_filter], y=y[fc_filter], color="red", edgecolor="black", s=100, ax=ax)
+
+        ax.set_xlim((-vmax * 1.1, vmax * 1.1))
+        # ax.set_ylim((-0.5, np.min([y[fc_filter], 15])))
+        ax.set_xlabel("$\log$ fold change")
+        ax.set_ylabel("$-\log_{10}$ FDR-corrected pvalues")
+        plt.axvline(
+            -fold_change_threshold,
+            color="black",
+            linestyle="--",
+        )
+        plt.axvline(
+            fold_change_threshold,
+            color="black",
+            linestyle="--",
+        )
+        plt.axhline(-np.log10(significance_threshold), linestyle="--", color="black")
+
         plt.tight_layout()
         if save is not None:
             plt.savefig(f"{save}_cv{str(self.cv_idx)}_{suffix}")
         if show:
             plt.show()
         plt.close(fig)
         plt.ion()
-        
+
     def sender_receiver_gene_subset(
-        self,
-        receiver: str,
-        sender: str,
-        significance_threshold: float = 0.05,
-        fold_change_quantile: float = 0.2
+        self, receiver: str, sender: str, significance_threshold: float = 0.05, fold_change_quantile: float = 0.2
     ):
 
         receiver_idx = self.cell_names.index(receiver)
         sender_idx = self.cell_names.index(sender)
 
-        qvals = pd.DataFrame(
-            self.qvalues[receiver_idx, sender_idx, :], 
-            index=self.data.celldata.var_names
-        )
+        qvals = pd.DataFrame(self.qvalues[receiver_idx, sender_idx, :], index=self.data.celldata.var_names)
         fold_change = pd.DataFrame(
-            np.abs(self.fold_change[receiver_idx, sender_idx, :]), 
-            index=self.data.celldata.var_names
+            np.abs(self.fold_change[receiver_idx, sender_idx, :]), index=self.data.celldata.var_names
         )
         qvals = qvals.replace(0.0, 0.0000001)
         qvals = qvals[qvals <= significance_threshold]
         mask_rows = qvals.any(axis=1)
         qvals = qvals.loc[mask_rows]
         fold_change = fold_change.loc[mask_rows]
-        fold_change = fold_change[
-            fold_change >= np.max(np.array(fold_change))*fold_change_quantile
-        ]
+        fold_change = fold_change[fold_change >= np.max(np.array(fold_change)) * fold_change_quantile]
         mask_rows = fold_change.any(axis=1)
         fold_change = fold_change.loc[mask_rows]
         qvals = qvals.loc[mask_rows]
-        
+
         return list(qvals.index)
-    
+
     def sender_effect(
         self,
         receiver: str,
-        plot_mode: str = 'fold_change',
+        plot_mode: str = "fold_change",
         gene_subset: Optional[List[str]] = None,
         significance_threshold: float = 0.05,
         cut_pvals: float = -5,
         fontsize: Optional[int] = None,
         figsize: Tuple[float, float] = (6, 10),
         save: Optional[str] = None,
         suffix: str = "_sender_efect.pdf",
         show: bool = True,
     ):
         receiver_idx = self.cell_names.index(receiver)
-        
+
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
-        
-        if plot_mode == 'qvals':
+
+        if plot_mode == "qvals":
             arr = np.log(self.qvalues[receiver_idx, :, :].copy())
             arr[arr < cut_pvals] = cut_pvals
-            df = pd.DataFrame(
-                arr, 
-                index=self.cell_names,
-                columns=self.data.celldata.var_names
-            )
+            df = pd.DataFrame(arr, index=self.cell_names, columns=self.data.celldata.var_names)
             if gene_subset:
                 df = df.drop(index=receiver)[gene_subset]
 
             plt.ioff()
             fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
             sns.heatmap(
-                df.T,
-                cbar_kws={'label': "$\log_{10}$ FDR-corrected pvalues"},
-                cmap='Greys_r', vmin=-5, vmax=0.
+                df.T, cbar_kws={"label": "$\log_{10}$ FDR-corrected pvalues"}, cmap="Greys_r", vmin=-5, vmax=0.0
             )
-        elif plot_mode == 'fold_change':
+        elif plot_mode == "fold_change":
             arr = self.fold_change[receiver_idx, :, :].copy()
             arr[np.where(self.qvalues[receiver_idx, :, :] > significance_threshold)] = 0
-            df = pd.DataFrame(
-                arr, 
-                index=self.cell_names,
-                columns=self.data.celldata.var_names
-            )
+            df = pd.DataFrame(arr, index=self.cell_names, columns=self.data.celldata.var_names)
             plt.ioff()
             if gene_subset:
                 df = df.drop(index=receiver)[gene_subset]
             vmax = np.max(np.abs(df.values))
 
             fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
             sns.heatmap(
                 df.T,
-                cbar_kws={'label': "$\log$ fold change", 
-                           "location": "top"},
-                cmap="seismic", vmin=-vmax, vmax=vmax, 
+                cbar_kws={"label": "$\log$ fold change", "location": "top"},
+                cmap="seismic",
+                vmin=-vmax,
+                vmax=vmax,
             )
         plt.xlabel("sender cell type")
         plt.tight_layout()
         if save is not None:
             plt.savefig(f"{save}_cv{str(self.cv_idx)}_{receiver}_{suffix}")
         if show:
             plt.show()
         plt.close(fig)
         plt.ion()
-        
+
     def receiver_effect(
         self,
         sender: str,
-        plot_mode: str = 'fold_change',
+        plot_mode: str = "fold_change",
         gene_subset: Optional[List[str]] = None,
         significance_threshold: float = 0.05,
         cut_pvals: float = -5,
         fontsize: Optional[int] = None,
         figsize: Tuple[float, float] = (6, 10),
         save: Optional[str] = None,
         suffix: str = "_receiver_efect.pdf",
         show: bool = True,
     ):
         sender_idx = self.cell_names.index(sender)
-        
+
         if fontsize:
             sc.set_figure_params(scanpy=True, fontsize=fontsize)
-        
-        if plot_mode == 'qvals':
+
+        if plot_mode == "qvals":
             arr = np.log(self.qvalues[sender_idx, :, :].copy())
             arr[arr < cut_pvals] = cut_pvals
-            df = pd.DataFrame(
-                arr, 
-                index=self.cell_names,
-                columns=self.data.celldata.var_names
-            )
+            df = pd.DataFrame(arr, index=self.cell_names, columns=self.data.celldata.var_names)
             if gene_subset:
                 df = df.drop(index=sender)[gene_subset]
 
             plt.ioff()
             fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
             sns.heatmap(
-                df.T,
-                cbar_kws={'label': "$\log_{10}$ FDR-corrected pvalues"},
-                cmap='Greys_r', vmin=-5, vmax=0.
+                df.T, cbar_kws={"label": "$\log_{10}$ FDR-corrected pvalues"}, cmap="Greys_r", vmin=-5, vmax=0.0
             )
-        elif plot_mode == 'fold_change':
+        elif plot_mode == "fold_change":
             arr = self.fold_change[sender_idx, :, :].copy()
             arr[np.where(self.qvalues[:, sender_idx, :] > significance_threshold)] = 0
-            df = pd.DataFrame(
-                arr, 
-                index=self.cell_names,
-                columns=self.data.celldata.var_names
-            )
+            df = pd.DataFrame(arr, index=self.cell_names, columns=self.data.celldata.var_names)
             plt.ioff()
             if gene_subset:
                 df = df.drop(index=sender)[gene_subset]
             vmax = np.max(np.abs(df.values))
 
             fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
             sns.heatmap(
                 df.T,
-                cbar_kws={'label': "$\log$ fold change", 
-                           "location": "top"},
-                cmap="seismic", vmin=-vmax, vmax=vmax, 
+                cbar_kws={"label": "$\log$ fold change", "location": "top"},
+                cmap="seismic",
+                vmin=-vmax,
+                vmax=vmax,
             )
         plt.xlabel("receiver cell type")
         plt.tight_layout()
         if save is not None:
             plt.savefig(f"{save}_cv{str(self.cv_idx)}_{sender}_{suffix}")
         if show:
             plt.show()
         plt.close(fig)
         plt.ion()
-        
 
     def interaction_significance(
         self,
         image_keys,
         nodes_idx,
         significance_threshold: float = 0.01,
     ):
@@ -1920,44 +1894,33 @@
                 ).todense()
             )
             sf.append(sf_batch.numpy().squeeze())
             node_covar.append(node_covar_batch.numpy().squeeze())
             g.append(g_batch.numpy().squeeze())
             h_obs.append(y_batch[0].numpy().squeeze())
         return (target, interactions, sf, node_covar, g), h_obs
-    
-    def get_sender_receiver_effects(
-        self,
-        params_type: str = 'ols',
-        significance_threshold: float = 0.05
-    ):
-        data = {
-            "target": self.data.celldata.obsm['node_types'], 
-            "proportions": self.data.celldata.obsm['proportions']
-        }
+
+    def get_sender_receiver_effects(self, params_type: str = "ols", significance_threshold: float = 0.05):
+        data = {"target": self.data.celldata.obsm["node_types"], "proportions": self.data.celldata.obsm["proportions"]}
         target = np.asarray(dmatrix("target-1", data))
         interaction_shape = np.int(self.n_features_0**2)
         interactions = np.asarray(dmatrix("target:proportions-1", data))
 
         y = self.data.celldata.X
 
-        print('using ols parameters.')
-        if params_type == 'ols':
+        print("using ols parameters.")
+        if params_type == "ols":
             x_design = np.concatenate([target, interactions], axis=1)
             ols = ols_fit(x_=x_design, y_=y)
             params = ols.squeeze()
         else:
-            params = (
-                self.model.training_model.weights[0]
-                .numpy()
-                .T
-            )
+            params = self.model.training_model.weights[0].numpy().T
 
         # get inverse fisher information matrix
-        print('calculating inv fim.')
+        print("calculating inv fim.")
         fim_inv = get_fim_inv(x_design, y)
 
         is_sign, pvalues, qvalues = wald_test(
             params=params, fisher_inv=fim_inv, significance_threshold=significance_threshold
         )
         interaction_shape = np.int(self.n_features_0**2)
         # subset to interaction terms
@@ -1976,15 +1939,18 @@
         self.is_sign = np.concatenate(
             np.expand_dims(np.split(is_sign, indices_or_sections=np.sqrt(is_sign.shape[0]), axis=0), axis=0),
             axis=0,
         )
 
         interaction_params = params[:, self.n_features_0 : interaction_shape + self.n_features_0]
         self.fold_change = np.concatenate(
-            np.expand_dims(np.split(interaction_params.T, indices_or_sections=np.sqrt(interaction_params.T.shape[0]), axis=0), axis=0),
+            np.expand_dims(
+                np.split(interaction_params.T, indices_or_sections=np.sqrt(interaction_params.T.shape[0]), axis=0),
+                axis=0,
+            ),
             axis=0,
         )
 
     def interaction_significance(
         self,
         image_keys,
         nodes_idx,
```

### Comparing `ncem-0.1.4/ncem/models/custom_callbacks.py` & `ncem-0.1.5/ncem/models/custom_callbacks.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/models/layers/__init__.py` & `ncem-0.1.5/ncem/models/layers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,11 +5,11 @@
                                                  SamplingPrior)
 from ncem.models.layers.output_layers import (GaussianConstDispOutput,
                                               GaussianOutput,
                                               LinearConstDispOutput,
                                               LinearOutput,
                                               NegBinConstDispOutput,
                                               NegBinOutput,
-                                              NegBinSharedDispOutput,
-                                              get_out)
+                                              NegBinSharedDispOutput, get_out)
 from ncem.models.layers.preproc_input import DenseInteractions, PreprocInput
-from ncem.models.layers.single_gnn_layers import SingleLrGatLayer, SingleGatLayer
+from ncem.models.layers.single_gnn_layers import (SingleGatLayer,
+                                                  SingleLrGatLayer)
```

### Comparing `ncem-0.1.4/ncem/models/layers/gnn_layers.py` & `ncem-0.1.5/ncem/models/layers/gnn_layers.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/models/layers/layer_stacks_lvm.py` & `ncem-0.1.5/ncem/models/layers/layer_stacks_lvm.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/models/layers/output_layers.py` & `ncem-0.1.5/ncem/models/layers/output_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tensorflow as tf
 
 IDENTIFIER_OUTPUT_LAYER = "Output"
 
 
-def get_out(output_layer: str, out_feature_dim, scale_node_size, name: str = 'decoder'):
+def get_out(output_layer: str, out_feature_dim, scale_node_size, name: str = "decoder"):
     if output_layer == "gaussian":
         output_decoder_layer = GaussianOutput(
             original_dim=out_feature_dim,
             use_node_scale=scale_node_size,
             name=f"Gaussian{IDENTIFIER_OUTPUT_LAYER}_{name}",
         )
     elif output_layer == "nb":
```

### Comparing `ncem-0.1.4/ncem/models/layers/preproc_input.py` & `ncem-0.1.5/ncem/models/layers/preproc_input.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/models/layers/single_gnn_layers.py` & `ncem-0.1.5/ncem/models/layers/single_gnn_layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import tensorflow as tf
 
 
 class SingleMaxLayer(tf.keras.layers.Layer):
     """
     TODO MAX implementation here is not complete yet.
     """
+
     def call(self, inputs, **kwargs):
         x = inputs[0]
         a = inputs[1]
 
         a = tf.expand_dims(a, axis=-1)  # (batch, target nodes, padded neighbor nodes, 1)
         t = x * a
         t = tf.reduce_sum(t, axis=2)
@@ -17,14 +18,15 @@
         return y
 
 
 class SingleGcnLayer(tf.keras.layers.Layer):
     """
     TODO GCN implementation here is not complete yet.
     """
+
     def __init__(self, latent_dim, dropout_rate, activation, l2_reg, use_bias: bool = False, **kwargs):
         super().__init__(**kwargs)
         self.latent_dim = latent_dim
         self.dropout_rate = dropout_rate
         self.activation = tf.keras.activations.get(activation)
         self.l2_reg = l2_reg
         self.use_bias = use_bias
@@ -65,15 +67,14 @@
         if self.activation is not None:
             y = self.activation(y)
 
         return y
 
 
 class SingleLrGatLayer(tf.keras.layers.Layer):
-
     def __init__(self, lr_dim, dropout_rate, l2_reg, **kwargs):
         """Initialize GCNLayer.
 
         Parameters
         ----------
         dropout_rate
             Dropout rate.
@@ -92,31 +93,47 @@
         # Layer kernel
         self.kernel_l = self.add_weight(
             name="kernel_l",
             shape=(1, 1, self.lr_dim),
             initializer=tf.keras.initializers.glorot_uniform(),
             regularizer=tf.keras.regularizers.l2(self.l2_reg),
         )
-        self.bias_l = self.add_weight(name="bias_l", shape=(1, 1, self.lr_dim,))
+        self.bias_l = self.add_weight(
+            name="bias_l",
+            shape=(
+                1,
+                1,
+                self.lr_dim,
+            ),
+        )
         self.kernel_r = self.add_weight(
             name="kernel_r",
             shape=(1, 1, self.lr_dim),
             initializer=tf.keras.initializers.glorot_uniform(),
             regularizer=tf.keras.regularizers.l2(self.l2_reg),
         )
-        self.bias_r = self.add_weight(name="bias_r", shape=(1, 1, self.lr_dim,))
+        self.bias_r = self.add_weight(
+            name="bias_r",
+            shape=(
+                1,
+                1,
+                self.lr_dim,
+            ),
+        )
 
     def call(self, inputs, **kwargs):
         targets_receptor = inputs[0]  # (batch, target nodes, lr)
         # print('targets_receptor', targets_receptor.shape)
         neighbors_ligand = inputs[1]  # (batch, target nodes, padded neighbor nodes, lr)
         a = inputs[2]  # (batch, target nodes, padded neighbor nodes)
 
         targets_receptor = targets_receptor * self.kernel_r + self.bias_r  # (batch, target nodes, lr)
-        neighbors_ligand = neighbors_ligand * self.kernel_l + self.bias_l  # (batch, target nodes, padded neighbor nodes, lr)
+        neighbors_ligand = (
+            neighbors_ligand * self.kernel_l + self.bias_l
+        )  # (batch, target nodes, padded neighbor nodes, lr)
         targets_receptor = tf.expand_dims(targets_receptor, axis=-2)  # (batch, target nodes, 1, lr)
         weights = targets_receptor * neighbors_ligand
         # print('weights', weights.shape)
         # Mask embeddings to neighbors
         a = tf.expand_dims(a, axis=-1)  # (batch, target nodes, padded neighbor nodes, 1)
         weights = weights * a
         weights = tf.reduce_sum(weights, axis=2)  # (batch, target nodes, lr)
@@ -156,30 +173,47 @@
         # Layer kernel
         self.kernel_target = self.add_weight(
             name="kernel_l",
             shape=(1, 1, self.in_dim),
             initializer=tf.keras.initializers.glorot_uniform(),
             regularizer=tf.keras.regularizers.l2(self.l2_reg),
         )
-        self.bias_target = self.add_weight(name="bias_l", shape=(1, 1, self.in_dim,))
+        self.bias_target = self.add_weight(
+            name="bias_l",
+            shape=(
+                1,
+                1,
+                self.in_dim,
+            ),
+        )
         self.kernel_neighbor = self.add_weight(
             name="kernel_r",
             shape=(1, 1, self.in_dim),
             initializer=tf.keras.initializers.glorot_uniform(),
             regularizer=tf.keras.regularizers.l2(self.l2_reg),
         )
-        self.bias_neighbor = self.add_weight(name="bias_r", shape=(1, 1, 1, self.in_dim,))
+        self.bias_neighbor = self.add_weight(
+            name="bias_r",
+            shape=(
+                1,
+                1,
+                1,
+                self.in_dim,
+            ),
+        )
 
     def call(self, inputs, **kwargs):
         targets = inputs[0]  # (batch, target nodes, features)
         neighbors = inputs[1]  # (batch, target nodes, padded neighbor nodes, features)
         a = inputs[2]  # (batch, target nodes, padded neighbor nodes)
 
         targets = targets * self.kernel_neighbor + self.bias_neighbor  # (batch, target nodes, lr)
-        neighbors = neighbors * self.kernel_target + self.bias_target  # (batch, target nodes, padded neighbor nodes, lr)
+        neighbors = (
+            neighbors * self.kernel_target + self.bias_target
+        )  # (batch, target nodes, padded neighbor nodes, lr)
         targets = tf.expand_dims(targets, axis=-2)  # (batch, target nodes, 1, lr)
         weights = targets * neighbors
         # Mask embeddings to neighbors
         a = tf.expand_dims(a, axis=-1)  # (batch, target nodes, padded neighbor nodes, 1)
         weights = weights * a
         weights = tf.reduce_sum(weights, axis=2)  # (batch, target nodes, lr)
         y = tf.math.sigmoid(weights)
```

### Comparing `ncem-0.1.4/ncem/models/model_cvae.py` & `ncem-0.1.5/ncem/models/model_cvae.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import tensorflow as tf
 
-from ncem.models.layers import (Decoder, Encoder, get_out, PreprocInput, SamplingPrior)
+from ncem.models.layers import (Decoder, Encoder, PreprocInput, SamplingPrior,
+                                get_out)
 
 
 class ModelCVAE:
     """Model class for conditional variational autoencoder."""
 
     def __init__(
         self,
@@ -157,20 +158,24 @@
         sampling_decoder1 = self.decoder_model((latent_sampling_reshaped1, categ_condition))
         sampling_decoder2 = self.decoder_model((latent_sampling_reshaped2, categ_condition))
 
         output_decoder_layer = get_out(
             output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size
         )((output_decoder, input_node_size))
         output_sampling_decoder1 = get_out(
-            output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size,
-            name='sampling1'
+            output_layer=output_layer,
+            out_feature_dim=out_node_feature_dim,
+            scale_node_size=scale_node_size,
+            name="sampling1",
         )((sampling_decoder1, input_node_size))
         output_sampling_decoder2 = get_out(
-            output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size,
-            name='sampling2'
+            output_layer=output_layer,
+            out_feature_dim=out_node_feature_dim,
+            scale_node_size=scale_node_size,
+            name="sampling2",
         )((sampling_decoder2, input_node_size))
 
         output_decoder_concat = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_decoder_layer)
         output_sampling_concat1 = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_sampling_decoder1)
         output_sampling_concat2 = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_sampling_decoder2)
 
         self.encoder = tf.keras.Model(
```

### Comparing `ncem-0.1.4/ncem/models/model_cvae_ncem.py` & `ncem-0.1.5/ncem/models/model_cvae_ncem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union
 
 import numpy as np
 import tensorflow as tf
 
-from ncem.models.layers import (CondDecoder, CondEncoder, GCNLayer, MaxLayer, get_out, PreprocInput, SamplingPrior)
+from ncem.models.layers import (CondDecoder, CondEncoder, GCNLayer, MaxLayer,
+                                PreprocInput, SamplingPrior, get_out)
 
 
 class ModelCVAEncem:
     """Model class for NCEM conditional variational autoencoder with graph layer IND (MAX) or GCN."""
 
     def __init__(
         self,
@@ -239,20 +240,24 @@
         sampling_decoder1 = self.decoder_model((latent_sampling_reshaped1, x_neighbour_embedding, categ_condition))
         sampling_decoder2 = self.decoder_model((latent_sampling_reshaped2, x_neighbour_embedding, categ_condition))
 
         output_decoder_layer = get_out(
             output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size
         )((output_decoder, input_node_size))
         output_sampling_decoder1 = get_out(
-            output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size,
-            name='sampling1'
+            output_layer=output_layer,
+            out_feature_dim=out_node_feature_dim,
+            scale_node_size=scale_node_size,
+            name="sampling1",
         )((sampling_decoder1, input_node_size))
         output_sampling_decoder2 = get_out(
-            output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size,
-            name='sampling2'
+            output_layer=output_layer,
+            out_feature_dim=out_node_feature_dim,
+            scale_node_size=scale_node_size,
+            name="sampling2",
         )((sampling_decoder2, input_node_size))
 
         output_decoder_concat = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_decoder_layer)
         output_sampling_concat1 = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_sampling_decoder1)
         output_sampling_concat2 = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_sampling_decoder2)
 
         self.graph_condition_model = tf.keras.Model(
```

### Comparing `ncem-0.1.4/ncem/models/model_ed.py` & `ncem-0.1.5/ncem/models/model_ed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 
-from ncem.models.layers import (Decoder, Encoder, get_out)
+from ncem.models.layers import Decoder, Encoder, get_out
 
 
 class ModelED:
     """Model class for non-spatial encoder-decoder."""
 
     def __init__(
         self,
@@ -131,16 +131,18 @@
         output_decoder = self.decoder_model((z, categ_condition))
         sampling_decoder = self.decoder_model((latent_sampling_reshaped, categ_condition))
 
         output_decoder_layer = get_out(
             output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size
         )((output_decoder, input_node_size))
         output_sampling_decoder = get_out(
-            output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size,
-            name='sampling'
+            output_layer=output_layer,
+            out_feature_dim=out_node_feature_dim,
+            scale_node_size=scale_node_size,
+            name="sampling",
         )((sampling_decoder, input_node_size))
 
         output_decoder_concat = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_decoder_layer)
         output_sampling_concat = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_sampling_decoder)
 
         self.encoder = tf.keras.Model(
             inputs=[input_x, input_categ_condition, input_g], outputs=output_encoder, name="encoder"
```

### Comparing `ncem-0.1.4/ncem/models/model_ed_ncem.py` & `ncem-0.1.5/ncem/models/model_ed_ncem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 
 import tensorflow as tf
 
-from ncem.models.layers import (Decoder, Encoder, GCNLayer, MaxLayer, get_out)
+from ncem.models.layers import Decoder, Encoder, GCNLayer, MaxLayer, get_out
 
 
 class ModelEDncem:
     """Model class for NCEM encoder-decoder with graph layer IND (MAX) or GCN."""
 
     def __init__(
         self,
@@ -211,16 +211,18 @@
         output_decoder = self.decoder_model((z, categ_condition))
         sampling_decoder = self.decoder_model((latent_sampling_reshaped, categ_condition))
 
         output_decoder_layer = get_out(
             output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size
         )((output_decoder, input_node_size))
         output_sampling_decoder = get_out(
-            output_layer=output_layer, out_feature_dim=out_node_feature_dim, scale_node_size=scale_node_size,
-            name='sampling'
+            output_layer=output_layer,
+            out_feature_dim=out_node_feature_dim,
+            scale_node_size=scale_node_size,
+            name="sampling",
         )((sampling_decoder, input_node_size))
 
         output_decoder_concat = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_decoder_layer)
         output_sampling_concat = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_sampling_decoder)
 
         self.encoder = tf.keras.Model(
             inputs=[
```

### Comparing `ncem-0.1.4/ncem/models/model_ed_single_ncem.py` & `ncem-0.1.5/ncem/models/model_ed_single_ncem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import tensorflow as tf
 
-from ncem.models.layers import get_out, Decoder
-from ncem.models.layers.single_gnn_layers import SingleMaxLayer, SingleGcnLayer, SingleGatLayer, SingleLrGatLayer
+from ncem.models.layers import Decoder, get_out
+from ncem.models.layers.single_gnn_layers import (SingleGatLayer,
+                                                  SingleGcnLayer,
+                                                  SingleLrGatLayer,
+                                                  SingleMaxLayer)
 
 
 class ModelEd2Ncem:
     """Model class for NCEM encoder-decoder with graph layer IND (MAX) or GCN."""
 
     def __init__(
         self,
@@ -51,23 +54,25 @@
         neighbors_dim = input_shapes[3]
         categ_condition_dim = input_shapes[4]
         domain_dim = input_shapes[5]
 
         # node features - node representation of neighbors: Input Tensor - shape=(None, targets, F-in)
         input_x_targets = tf.keras.Input(shape=(num_targets_dim, in_lr_feature_dim), name="node_features_targets")
         # node features - node representation of neighbors: Input Tensor - shape=(None, neighbors, F-in)
-        input_x_neighbors = tf.keras.Input(shape=(num_targets_dim, neighbors_dim, in_lr_feature_dim),
-                                           name="node_features_neighbors")
+        input_x_neighbors = tf.keras.Input(
+            shape=(num_targets_dim, neighbors_dim, in_lr_feature_dim), name="node_features_neighbors"
+        )
         # node size - reconstruction: Input Tensor - shape=(None, targets, 1)
         input_node_size = tf.keras.Input(shape=(num_targets_dim, 1), name="node_size_reconstruct")
         # adj_matrices - A: Input Tensor - shape=(None, targets, neighbors)
         input_a = tf.keras.Input(shape=(num_targets_dim, neighbors_dim), name="adjacency_matrix")
         # Categorical predictors: Input Tensor - shape=(None, targets, P)
-        input_categ_condition = tf.keras.Input(shape=(num_targets_dim, categ_condition_dim),
-                                               name="categorical_predictor")
+        input_categ_condition = tf.keras.Input(
+            shape=(num_targets_dim, categ_condition_dim), name="categorical_predictor"
+        )
         # domain information of graph - shape=(None, 1)
         input_g = tf.keras.layers.Input(shape=(domain_dim,), name="input_da_group", dtype="int32")
 
         if use_domain:
             categ_condition = tf.concat(
                 [
                     input_categ_condition,
@@ -91,25 +96,23 @@
                 latent_dim=latent_dim,
                 dropout_rate=dropout_rate,
                 l2_reg=l2_coef,
                 name=f"lr_gat_layer",
             )([input_x_targets, input_x_neighbors, input_a])
         elif cond_type == "max":
             print("MAX")
-            x_encoder = SingleMaxLayer(
-                name=f"max_layer"
-            )([input_x_neighbors, input_a])
+            x_encoder = SingleMaxLayer(name=f"max_layer")([input_x_neighbors, input_a])
         elif cond_type == "gcn":
             x_encoder = SingleGcnLayer(
                 latent_dim=latent_dim,
                 dropout_rate=dropout_rate,
                 activation="relu",
                 l2_reg=l2_coef,
                 use_bias=True,
-                name=f"gcn_layer"
+                name=f"gcn_layer",
             )([input_x_targets, input_x_neighbors, input_a])
         elif cond_type == "none":
             x_encoder = input_x_targets
         else:
             raise ValueError("tried to access a non-supported conditional layer %s" % cond_type)
 
         # Decoder on neighborhood embeddings:
@@ -122,16 +125,17 @@
                 l2_coef=dec_l2_coef,
                 use_type_cond=use_type_cond,
                 use_batch_norm=dec_use_batch_norm,
             )((x_encoder, categ_condition))
         else:
             x = tf.concat([x_encoder, categ_condition], axis=-1)
 
-        output_decoder = get_out(output_layer=output_layer, out_feature_dim=out_feature_dim,
-                                 scale_node_size=scale_node_size)((x, input_node_size))
+        output_decoder = get_out(
+            output_layer=output_layer, out_feature_dim=out_feature_dim, scale_node_size=scale_node_size
+        )((x, input_node_size))
         output_decoder_concat = tf.keras.layers.Concatenate(axis=2, name="reconstruction")(output_decoder)
 
         self.encoder = tf.keras.Model(
             inputs=[
                 input_x_targets,
                 input_x_neighbors,
                 input_node_size,
```

### Comparing `ncem-0.1.4/ncem/models/model_interactions.py` & `ncem-0.1.5/ncem/models/model_interactions.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/models/model_linear.py` & `ncem-0.1.5/ncem/models/model_linear.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/train/summaries.py` & `ncem-0.1.5/ncem/train/summaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import seaborn as sns
-from tqdm import tqdm
 from matplotlib.ticker import FormatStrFormatter
+from tqdm import tqdm
 
 
 class GridSearchContainer:
     """GridSearchContainer class."""
 
     runparams: dict
     run_ids_clean: dict
@@ -112,17 +112,21 @@
                         [
                             "_".join(".".join(x.split(".")[:-1]).split("_")[:-1])
                             for x in os.listdir(indir)
                             if x.split("_")[-1].split(".")[0] == "time"
                         ]
                     )
                 )
-                cv_ids = np.sort(np.unique([x.split("_")[-1] for x in run_ids]))  # identifiers of cross-validation splits
+                cv_ids = np.sort(
+                    np.unique([x.split("_")[-1] for x in run_ids])
+                )  # identifiers of cross-validation splits
                 run_ids = np.sort(
-                    np.unique(["_".join(x.split("_")[:-1]) for x in run_ids])  # identifiers of hyper-parameters settings
+                    np.unique(
+                        ["_".join(x.split("_")[:-1]) for x in run_ids]
+                    )  # identifiers of hyper-parameters settings
                 )
                 run_ids_clean = []  # only IDs of completed runs (all files present)
                 for r in run_ids:
                     complete_run = True
                     for cv in cv_ids:
                         # Check pickled files:
                         for end in expected_pickle:
@@ -179,21 +183,25 @@
                         "data_set": [runparams[x]["data_set"] for x in run_ids_clean],
                         "model_class": [runparams[x]["model_class"] for x in run_ids_clean],
                         "cond_type": [runparams[x]["cond_type"] for x in run_ids_clean]
                         if "cond_type" in list(runparams[x].keys())
                         else "none",
                         "gs_id": [runparams[x]["gs_id"] for x in run_ids_clean],
                         "model_id": [runparams[x]["model_id"] for x in run_ids_clean],
-                        #"split_mode": [runparams[x]["split_mode"] for x in run_ids_clean],
-                        "radius": [runparams[x]["radius"] for x in run_ids_clean] if "radius" in list(runparams[x].keys()) else [runparams[x]["max_dist"] for x in run_ids_clean],
-                        "n_rings": [runparams[x]["n_rings"] for x in run_ids_clean] if "n_rings" in list(runparams[x].keys()) else "none",
+                        # "split_mode": [runparams[x]["split_mode"] for x in run_ids_clean],
+                        "radius": [runparams[x]["radius"] for x in run_ids_clean]
+                        if "radius" in list(runparams[x].keys())
+                        else [runparams[x]["max_dist"] for x in run_ids_clean],
+                        "n_rings": [runparams[x]["n_rings"] for x in run_ids_clean]
+                        if "n_rings" in list(runparams[x].keys())
+                        else "none",
                         "graph_covar_selection": [runparams[x]["graph_covar_selection"] for x in run_ids_clean],
-                        #"node_label_space_id": [runparams[x]["node_label_space_id"] for x in run_ids_clean],
-                        #"node_feature_space_id": [runparams[x]["node_feature_space_id"] for x in run_ids_clean],
-                        #"feature_transformation": [runparams[x]["feature_transformation"] for x in run_ids_clean],
+                        # "node_label_space_id": [runparams[x]["node_label_space_id"] for x in run_ids_clean],
+                        # "node_feature_space_id": [runparams[x]["node_feature_space_id"] for x in run_ids_clean],
+                        # "feature_transformation": [runparams[x]["feature_transformation"] for x in run_ids_clean],
                         "use_covar_node_position": [runparams[x]["use_covar_node_position"] for x in run_ids_clean],
                         "use_covar_node_label": [runparams[x]["use_covar_node_label"] for x in run_ids_clean],
                         "use_covar_graph_covar": [runparams[x]["use_covar_graph_covar"] for x in run_ids_clean],
                         "target_cell_type": [runparams[x]["target_cell_type"] for x in run_ids_clean]
                         if "target_cell_type" in list(runparams[x].keys())
                         else "none",
                         "optimizer": [runparams[x]["optimizer"] for x in run_ids_clean],
@@ -244,36 +252,46 @@
                         if "cond_l2_reg" in list(runparams[x].keys())
                         else "none",
                         "cond_use_bias": [str(runparams[x]["cond_use_bias"]) for x in run_ids_clean]
                         if "cond_bias" in list(runparams[x].keys())
                         else "none",
                         "use_domain": [runparams[x]["use_domain"] for x in run_ids_clean],
                         "domain_type": [runparams[x]["domain_type"] for x in run_ids_clean],
-                        "use_batch_norm": [runparams[x]["use_batch_norm"] for x in run_ids_clean] if "use_batch_norm" in list(runparams[x].keys())
+                        "use_batch_norm": [runparams[x]["use_batch_norm"] for x in run_ids_clean]
+                        if "use_batch_norm" in list(runparams[x].keys())
                         else "none",
                         "use_type_cond": [runparams[x]["use_type_cond"] for x in run_ids_clean]
                         if "use_type_cond" in list(runparams[x].keys())
                         else "none",
                         "scale_node_size": [runparams[x]["scale_node_size"] for x in run_ids_clean],
-                        "transform_input": [runparams[x]["transform_input"] for x in run_ids_clean] if "transform_input" in list(runparams[x].keys())
+                        "transform_input": [runparams[x]["transform_input"] for x in run_ids_clean]
+                        if "transform_input" in list(runparams[x].keys())
                         else "none",
                         "output_layer": [runparams[x]["output_layer"] for x in run_ids_clean],
                         "log_transform": [runparams[x]["log_transform"] for x in run_ids_clean]
                         if "log_transform" in list(runparams[x].keys())
                         else False,
-                        "segmentation_robustness_node_fraction": [runparams[x]["segmentation_robustness_node_fraction"] for x in run_ids_clean]
+                        "segmentation_robustness_node_fraction": [
+                            runparams[x]["segmentation_robustness_node_fraction"] for x in run_ids_clean
+                        ]
                         if "segmentation_robustness_node_fraction" in list(runparams[x].keys())
                         else False,
-                        "segmentation_robustness_overflow_fraction": [runparams[x]["segmentation_robustness_overflow_fraction"] for x in run_ids_clean]
+                        "segmentation_robustness_overflow_fraction": [
+                            runparams[x]["segmentation_robustness_overflow_fraction"] for x in run_ids_clean
+                        ]
                         if "segmentation_robustness_overflow_fraction" in list(runparams[x].keys())
                         else False,
-                        "resimulate_nodes_w_depdency": [runparams[x]["resimulate_nodes_w_depdency"] for x in run_ids_clean]
+                        "resimulate_nodes_w_depdency": [
+                            runparams[x]["resimulate_nodes_w_depdency"] for x in run_ids_clean
+                        ]
                         if "resimulate_nodes_w_depdency" in list(runparams[x].keys())
                         else False,
-                        "resimulate_nodes_sparsity_rate": [runparams[x]["resimulate_nodes_sparsity_rate"] for x in run_ids_clean]
+                        "resimulate_nodes_sparsity_rate": [
+                            runparams[x]["resimulate_nodes_sparsity_rate"] for x in run_ids_clean
+                        ]
                         if "resimulate_nodes_sparsity_rate" in list(runparams[x].keys())
                         else False,
                         "epochs": [runparams[x]["epochs"] for x in run_ids_clean],
                         "batch_size": [runparams[x]["batch_size"] for x in run_ids_clean],
                         "n_eval_nodes_per_graph": [runparams[x]["n_eval_nodes_per_graph"] for x in run_ids_clean],
                         "run_id_params": run_ids_clean,
                     }.items()
@@ -382,24 +400,27 @@
                                                             + m.replace("reconstruction_", "").replace("logp1_", ""),
                                                             [
                                                                 evals_posterior_sampling[x][cv]["train"][m]
                                                                 for x in run_ids_clean
                                                             ],
                                                         )
                                                         for m in list(
-                                                            evals_posterior_sampling[run_ids_clean[0]][cv]["train"].keys()
+                                                            evals_posterior_sampling[run_ids_clean[0]][cv][
+                                                                "train"
+                                                            ].keys()
                                                         )
                                                     ]
                                                 ).items()
                                             )
                                             + list(
                                                 dict(
                                                     [
                                                         (
-                                                            "val_" + m.replace("reconstruction_", "").replace("logp1_", ""),
+                                                            "val_"
+                                                            + m.replace("reconstruction_", "").replace("logp1_", ""),
                                                             [
                                                                 evals_posterior_sampling[x][cv]["val"][m]
                                                                 for x in run_ids_clean
                                                             ],
                                                         )
                                                         for m in list(
                                                             evals_posterior_sampling[run_ids_clean[0]][cv]["val"].keys()
@@ -415,24 +436,27 @@
                                                             + m.replace("reconstruction_", "").replace("logp1_", ""),
                                                             [
                                                                 evals_posterior_sampling[x][cv]["test"][m]
                                                                 for x in run_ids_clean
                                                             ],
                                                         )
                                                         for m in list(
-                                                            evals_posterior_sampling[run_ids_clean[0]][cv]["test"].keys()
+                                                            evals_posterior_sampling[run_ids_clean[0]][cv][
+                                                                "test"
+                                                            ].keys()
                                                         )
                                                     ]
                                                 ).items()
                                             )
                                             + list(
                                                 dict(
                                                     [
                                                         (
-                                                            "all_" + m.replace("reconstruction_", "").replace("logp1_", ""),
+                                                            "all_"
+                                                            + m.replace("reconstruction_", "").replace("logp1_", ""),
                                                             [
                                                                 evals_posterior_sampling[x][cv]["all"][m]
                                                                 for x in run_ids_clean
                                                             ],
                                                         )
                                                         for m in list(
                                                             evals_posterior_sampling[run_ids_clean[0]][cv]["all"].keys()
@@ -552,52 +576,56 @@
                                                     {
                                                         "model_class": [runparams[x]["model_class"]],
                                                         "cond_type": [runparams[x]["cond_type"]]
                                                         if "cond_type" in list(runparams[x].keys())
                                                         else "none",
                                                         "gs_id": [runparams[x]["gs_id"]],
                                                         "model_id": [runparams[x]["model_id"]],
-                                                        #"split_mode": [runparams[x]["split_mode"]],
-                                                        "radius": [runparams[x]["radius"]] if "radius" in list(runparams[x].keys()) else [runparams[x]["max_dist"]],
-                                                        "n_rings": [runparams[x]["n_rings"]] if "n_rings" in list(runparams[x].keys()) else "none",
+                                                        # "split_mode": [runparams[x]["split_mode"]],
+                                                        "radius": [runparams[x]["radius"]]
+                                                        if "radius" in list(runparams[x].keys())
+                                                        else [runparams[x]["max_dist"]],
+                                                        "n_rings": [runparams[x]["n_rings"]]
+                                                        if "n_rings" in list(runparams[x].keys())
+                                                        else "none",
                                                         "graph_covar_selection": [
                                                             runparams[x]["graph_covar_selection"]
                                                         ],
-                                                        #"node_label_space_id": [
+                                                        # "node_label_space_id": [
                                                         #    runparams[x]["node_label_space_id"]
-                                                        #],
-                                                        #"node_feature_space_id": [
+                                                        # ],
+                                                        # "node_feature_space_id": [
                                                         #    runparams[x]["node_feature_space_id"]
-                                                        #],
-                                                        #"feature_transformation": [
+                                                        # ],
+                                                        # "feature_transformation": [
                                                         #    runparams[x]["feature_transformation"]
-                                                        #],
+                                                        # ],
                                                         "use_covar_node_position": [
                                                             runparams[x]["use_covar_node_position"]
                                                         ],
                                                         "use_covar_node_label": [runparams[x]["use_covar_node_label"]],
                                                         "use_covar_graph_covar": [
                                                             runparams[x]["use_covar_graph_covar"]
                                                         ],
                                                         # "hold_out_covariate": [runparams[x]['hold_out_covariate']],
                                                         "optimizer": [runparams[x]["optimizer"]],
                                                         "learning_rate": [runparams[x]["learning_rate"]],
-                                                        #"intermediate_dim_enc": [runparams[x]["intermediate_dim_enc"]],
-                                                        #"intermediate_dim_dec": [runparams[x]["intermediate_dim_dec"]],
-                                                        #"latent_dim": [runparams[x]["latent_dim"]],
+                                                        # "intermediate_dim_enc": [runparams[x]["intermediate_dim_enc"]],
+                                                        # "intermediate_dim_dec": [runparams[x]["intermediate_dim_dec"]],
+                                                        # "latent_dim": [runparams[x]["latent_dim"]],
                                                         # "depth_enc": [runparams[x]['depth_enc']],
                                                         # "depth_dec": [runparams[x]['depth_dec']],
-                                                        #"dropout_rate": [runparams[x]["dropout_rate"]],
+                                                        # "dropout_rate": [runparams[x]["dropout_rate"]],
                                                         "l2_coef": [runparams[x]["l2_coef"]],
                                                         "l1_coef": [runparams[x]["l1_coef"]],
                                                         "use_domain": [runparams[x]["use_domain"]],
                                                         "domain_type": [runparams[x]["domain_type"]],
-                                                        #"use_batch_norm": [runparams[x]["use_batch_norm"]],
+                                                        # "use_batch_norm": [runparams[x]["use_batch_norm"]],
                                                         "scale_node_size": [runparams[x]["scale_node_size"]],
-                                                        #"transform_input": [runparams[x]["transform_input"]],
+                                                        # "transform_input": [runparams[x]["transform_input"]],
                                                         "output_layer": [runparams[x]["output_layer"]],
                                                         "log_transform": [runparams[x]["log_transform"]]
                                                         if "log_transform" in list(runparams[x].keys())
                                                         else False,
                                                         "epochs": [runparams[x]["epochs"]],
                                                         "batch_size": [runparams[x]["batch_size"]],
                                                         "run_id": x,
@@ -840,20 +868,20 @@
         self.info = info
 
     # Plotting functions:
     def plot_best_model_by_hyperparam(
         self,
         graph_model_class: str,
         baseline_model_class: str,
-        partition_show: str = 'test',
-        metric_show: str = 'r_squared_linreg',
-        partition_select: str = 'val',
-        metric_select: str = 'r_squared_linreg',
-        param_x: str = 'um_radius',
-        param_hue: str = 'model',
+        partition_show: str = "test",
+        metric_show: str = "r_squared_linreg",
+        partition_select: str = "val",
+        metric_select: str = "r_squared_linreg",
+        param_x: str = "um_radius",
+        param_hue: str = "model",
         rename_levels: Optional[List[Tuple[str, str]]] = None,
         subset_hyperparameters: Optional[List[Tuple[str, str]]] = None,
         cv_mode: str = "mean",
         yaxis_limit: Optional[Tuple[float, float]] = None,
         xticks: Optional[List[int]] = None,
         rotate_xticks: bool = True,
         figsize: Tuple[float, float] = (3.5, 4.0),
@@ -1005,15 +1033,15 @@
                 data=temp_graph,
                 hue=param_hue,
                 ax=ax,
                 markers=True,
             )
             ax.set_xscale("symlog", linthresh=10)
             if example_cellradius:
-                plt.axvline(example_cellradius, color='limegreen', linewidth=3.)
+                plt.axvline(example_cellradius, color="limegreen", linewidth=3.0)
         elif plot_mode == "mean_lineplot":
             temp_summary_table = summary_table[[param_hue, param_x, ycol]].groupby([param_hue, param_x]).mean()
             sns.lineplot(
                 x=param_x,
                 y=ycol,
                 palette=["grey"],
                 style=param_hue,
@@ -1037,16 +1065,16 @@
             ax.set_ylim(yaxis_limit)
         if xticks is not None:
             ax.set_xticks(xticks)
             ax.set_xticklabels(xticks)
         ax.yaxis.set_major_formatter(FormatStrFormatter("%0.3f"))
         if rotate_xticks:
             plt.xticks(rotation=90)
-        #ax.yaxis.tick_right()
-        #plt.yticks(rotation=180)
+        # ax.yaxis.tick_right()
+        # plt.yticks(rotation=180)
 
         # Save, show and return figure.
         # plt.tight_layout()
         if save is not None:
             plt.savefig(save + "_" + partition_show + suffix, bbox_extra_artists=(lgd,), bbox_inches="tight")
 
         if show:
```

### Comparing `ncem-0.1.4/ncem/train/train_model.py` & `ncem-0.1.5/ncem/train/train_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 import pickle
 from typing import Union
 
-from ncem.estimators import (EstimatorCVAE, EstimatorCVAEncem, EstimatorED,
-                             EstimatorEDncem, EstimatorEdNcemNeighborhood, EstimatorInteractions,
-                             EstimatorLinear, EstimatorDeconvolution)
+from ncem.estimators import (EstimatorCVAE, EstimatorCVAEncem,
+                             EstimatorDeconvolution, EstimatorED,
+                             EstimatorEDncem, EstimatorEdNcemNeighborhood,
+                             EstimatorInteractions, EstimatorLinear)
 
 
 class TrainModel:
     estimator: Union[
-        EstimatorLinear, EstimatorInteractions, EstimatorED, EstimatorEDncem, EstimatorCVAE, EstimatorCVAEncem,
-        EstimatorDeconvolution
+        EstimatorLinear,
+        EstimatorInteractions,
+        EstimatorED,
+        EstimatorEDncem,
+        EstimatorCVAE,
+        EstimatorCVAEncem,
+        EstimatorDeconvolution,
     ]
 
     @staticmethod
     def _try_save(fn: str, obj):
         with open(fn, "wb") as f:
             pickle.dump(obj=obj, file=f)
```

### Comparing `ncem-0.1.4/ncem/unit_test/directories.py` & `ncem-0.1.5/ncem/unit_test/directories.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/unit_test/test_dataloader_local.py` & `ncem-0.1.5/ncem/unit_test/test_dataloader_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
-from ncem.unit_test.directories import DATA_PATH_ZHANG, DATA_PATH_JAROSCH, DATA_PATH_HARTMANN, DATA_PATH_SCHUERCH, \
-    DATA_PATH_LU
+from ncem.unit_test.directories import (DATA_PATH_HARTMANN, DATA_PATH_JAROSCH,
+                                        DATA_PATH_LU, DATA_PATH_SCHUERCH,
+                                        DATA_PATH_ZHANG)
 
 
 class HelperTestDataLoader:
     data_origin: str
 
     def get_dataloader(self, data_origin: str):
         if data_origin == "zhang":
```

### Comparing `ncem-0.1.4/ncem/unit_test/test_estimator_local.py` & `ncem-0.1.5/ncem/unit_test/test_estimator_local.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-import pytest
 from typing import Union
 
+import pytest
+
 import ncem.api as ncem
 from ncem.estimators import Estimator
-
-from ncem.unit_test.directories import DATA_PATH_ZHANG, DATA_PATH_HARTMANN, DATA_PATH_LU, DATA_PATH_DESTVI
+from ncem.unit_test.directories import (DATA_PATH_DESTVI, DATA_PATH_HARTMANN,
+                                        DATA_PATH_LU, DATA_PATH_ZHANG)
 
 
 class HelperTestEstimator:
     est: Estimator
 
-    def get_estimator(
-        self,
-        model: str,
-        data_origin: str = "zhang",
-        **kwargs
-    ):
-        #node_label_space_id = "type"
+    def get_estimator(self, model: str, data_origin: str = "zhang", **kwargs):
+        # node_label_space_id = "type"
         node_label_space_id = "proportions"
         node_feature_space_id = "standard"
         if model in ["linear_baseline", "linear"]:
             self.est = ncem.train.EstimatorLinear()
         elif model in ["interactions_baseline", "interactions"]:
             self.est = ncem.train.EstimatorInteractions()
         elif model in ["linear_deconvolution"]:
@@ -74,22 +70,22 @@
             **kwargs
         )
 
     def test_train(self, model: str, data_origin: str = "zhang", **kwargs):
         self.get_estimator(model=model, data_origin=data_origin, **kwargs)
 
         kwargs_shared = {
-            'optimizer': "adam",
-            'latent_dim': 4,
-            'dropout_rate': 0.,
-            'l2_coef': 0.,
-            'l1_coef': 0.,
-            'n_eval_nodes_per_graph': 4,
-            'scale_node_size': False,
-            'output_layer': "gaussian"
+            "optimizer": "adam",
+            "latent_dim": 4,
+            "dropout_rate": 0.0,
+            "l2_coef": 0.0,
+            "l1_coef": 0.0,
+            "n_eval_nodes_per_graph": 4,
+            "scale_node_size": False,
+            "output_layer": "gaussian",
         }
 
         if model == "linear":
             kwargs = {"use_source_type": True, "use_domain": True, "learning_rate": 1e-2}
             train_kwargs = {}
         elif model == "linear_baseline":
             kwargs = {"use_source_type": False, "use_domain": True, "learning_rate": 1e-2}
@@ -143,37 +139,38 @@
                 "use_bias": True,
                 "learning_rate": 1e-2,
                 "beta": 0.1,
             }
             train_kwargs = {}
         elif model.startswith("ed_ncem2"):
             kwargs = kwargs_shared
-            kwargs.update({
-                "use_domain": True,
-                "use_bias": True,
-                "learning_rate": 1e-2,
-                "cond_type": self.est.cond_type,
-                "dec_intermediate_dim": 0,
-                "dec_n_hidden": 0,
-                "dec_dropout_rate": float,
-                "dec_l1_coef": 0.,
-                "dec_l2_coef": 0.,
-                "dec_use_batch_norm": False,
-            })
+            kwargs.update(
+                {
+                    "use_domain": True,
+                    "use_bias": True,
+                    "learning_rate": 1e-2,
+                    "cond_type": self.est.cond_type,
+                    "dec_intermediate_dim": 0,
+                    "dec_n_hidden": 0,
+                    "dec_dropout_rate": float,
+                    "dec_l1_coef": 0.0,
+                    "dec_l2_coef": 0.0,
+                    "dec_use_batch_norm": False,
+                }
+            )
             train_kwargs = {}
             self.est.set_input_features(
-                h0_in=False,
-                target_feature_names=["Abcb4", "Abcc3"],
-                neighbor_feature_names=["Adgre1", "Ammecr1"])
+                h0_in=False, target_feature_names=["Abcb4", "Abcc3"], neighbor_feature_names=["Adgre1", "Ammecr1"]
+            )
         else:
             assert False
         self._model_kwargs = kwargs
         self.est.init_model(**kwargs)
         self.est.split_data_node(validation_split=0.5, test_split=0.5)
-        #self.est.split_data_target_cell("B cells", validation_split=0.5, test_split=0.5)
+        # self.est.split_data_target_cell("B cells", validation_split=0.5, test_split=0.5)
 
         if data_origin == "hartmann":
             batch_size = None
         else:
             batch_size = 16
 
         if batch_size is None:
@@ -202,19 +199,22 @@
     def test_embedding(self):
         _ = self.est.predict_embedding_any(img_keys=self.est.img_keys_test, node_idx=self.est.nodes_idx_test)
 
     def test_decoding_weights(self):
         _ = self.est.get_decoding_weights()
 
 
-@pytest.mark.parametrize("transformation_kwargs", [
-    {"resimulate_nodes": True, "resimulate_nodes_w_depdency": True},
-    {"resimulate_nodes": True, "resimulate_nodes_w_depdency": False},
-    {"robustness": True},
-])
+@pytest.mark.parametrize(
+    "transformation_kwargs",
+    [
+        {"resimulate_nodes": True, "resimulate_nodes_w_depdency": True},
+        {"resimulate_nodes": True, "resimulate_nodes_w_depdency": False},
+        {"robustness": True},
+    ],
+)
 def test_data_transformations(transformation_kwargs: dict):
     estim = HelperTestEstimator()
     estim.test_train(model="interaction_baseline", data_origin="luwt", **transformation_kwargs)
 
 
 @pytest.mark.parametrize("dataset", ["luwt"])
 @pytest.mark.parametrize("model", ["interactions"])
@@ -234,23 +234,21 @@
 @pytest.mark.parametrize("model", ["cvae_ncem_max"])
 def test_cvae(dataset: str, model: str):
     estim = HelperTestEstimator()
     estim.test_train(model=model, data_origin=dataset)
 
 
 @pytest.mark.parametrize("dataset", ["luwt"])
-#@pytest.mark.parametrize("model", ["ed_ncem2_max", "ed_ncem2_gcn", "ed_ncem2_lr_gat", "ed_ncem2_gat"])
+# @pytest.mark.parametrize("model", ["ed_ncem2_max", "ed_ncem2_gcn", "ed_ncem2_lr_gat", "ed_ncem2_gat"])
 @pytest.mark.parametrize("model", ["ed_ncem2_none"])
 def test_ed2(dataset: str, model: str):
     estim = HelperTestEstimatorEd()
     estim.test_train(model=model, data_origin=dataset)
     estim.test_embedding()
     estim.test_decoding_weights()
 
 
 @pytest.mark.parametrize("dataset", ["destvi_lymphnode"])
 @pytest.mark.parametrize("model", ["linear_deconvolution"])
 def test_deconv(dataset: str, model: str):
     estim = HelperTestEstimator()
     estim.test_train(model=model, data_origin=dataset)
-
-
```

### Comparing `ncem-0.1.4/ncem/utils/losses.py` & `ncem-0.1.5/ncem/utils/losses.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/utils/metrics.py` & `ncem-0.1.5/ncem/utils/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     def f1():
         return tnp.ones(shape=(), dtype=tf.float32)
 
     def r():
         return ssxym / tnp.sqrt(xmym)  # formula for r
 
     def r2():
-        return r ** 2  # formula for r_squared
+        return r**2  # formula for r_squared
 
     # R-value
     # If the denominator was going to be 0, r = 0.0
     r = tf.cond(tnp.not_equal(xmym, tnp.zeros(shape=(), dtype=tf.float32)), r, f0)
     # Test for numerical error propagation (make sure -1 < r < 1)
     r_squared = tf.cond(tnp.greater(tnp.abs(r), tnp.ones(shape=(), dtype=tf.float32)), f1, r2)
     return r_squared
@@ -295,8 +295,8 @@
 
     ssxm = tnp.mean(tnp.square(x - xmean))
     ssym = tnp.mean(tnp.square(y - ymean))
     ssxym = tnp.mean((x - xmean) * (y - ymean))
 
     # R-value
     r = ssxym / tnp.sqrt(ssxm * ssym)
-    return r ** 2
+    return r**2
```

### Comparing `ncem-0.1.4/ncem/utils/sparse.py` & `ncem-0.1.5/ncem/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `ncem-0.1.4/ncem/utils/wald_test.py` & `ncem-0.1.5/ncem/utils/wald_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import numpy as np
+from scipy.sparse import issparse
 
 
 def get_fim_inv(x: np.array, y: np.array):
-    var = np.var(y, axis=0)
-    fim = np.expand_dims(np.matmul(x.T, x), axis=0) / np.expand_dims(var, axis=[1, 2])
-    
+    if issparse(y):
+        y = y.toarray()
+    var = np.var(y, axis=0, keepdims=True)
+    fim = np.expand_dims(np.matmul(np.array(x.T), np.array(x)), axis=0) / np.expand_dims(var, axis=[1]).T
     fim = np.nan_to_num(fim)
-    
-    fim_inv = np.array([
-        np.linalg.pinv(fim[i, :, :])
-        for i in range(fim.shape[0])
-    ])
+
+    fim_inv = np.array([np.linalg.pinv(fim[i, :, :]) for i in range(fim.shape[0])])
     return fim_inv
 
 
 def _get_p_value(a_var: np.array, fisher_inv: np.array, coef_loc_totest: int):
     """Return the p-value for differential expression for each gene.
 
     Parameters
@@ -56,21 +55,22 @@
         Significance threshold for corrected p-values.
 
     Returns
     -------
     bool_res, res
     """
     from diffxpy.testing.correction import correct
+
     significance = []
     qvalues = []
     pvalues = []
     for idx in range(params.T.shape[0]):
         pvals = _get_p_value(params.T, fisher_inv, idx)
         pvalues.append(pvals)
-        
+
     pvalues = np.concatenate(pvalues)
     qvalues = correct(pvalues)
-    pvalues = np.reshape(pvalues, (-1,params.T.shape[1])) 
-    qvalues = np.reshape(qvalues, (-1,params.T.shape[1]))  
+    pvalues = np.reshape(pvalues, (-1, params.T.shape[1]))
+    qvalues = np.reshape(qvalues, (-1, params.T.shape[1]))
     significance = qvalues < significance_threshold
 
     return significance, pvalues, qvalues
```

### Comparing `ncem-0.1.4/pyproject.toml` & `ncem-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 [tool.poetry]
 name = "ncem"
-version = "0.1.4"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.1.5"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "ncem. Learning cell communication from spatial graphs of cells."
 authors = ["Anna C. Schaar <anna.schaar@helmholtz-muenchen.de>"]
 license = "BSD"
 readme = "README.rst"
 homepage = "https://github.com/theislab/ncem"
 repository = "https://github.com/theislab/ncem"
 documentation = "https://ncem.readthedocs.io"
 packages = [
     { include = "ncem" },
 ]
 classifiers = [
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
 ]
 
-
 [tool.poetry.dependencies]
-python = ">=3.7,<3.9"
-click = "^7.1.2"
+python = ">=3.8,<=3.10"
+click = "^8.0.0"
 rich = "^10.1.0"
 PyYAML = "^5.4.1"
 Jinja2 = ">=2.11.3,<4.0.0"
-scanpy = "^1.7.2"
-tensorflow = "^2.5.0"
-squidpy = "^1.0.0"
+scanpy = "^1.9.3"
+squidpy = "^1.2.3"
 patsy = "^0.5.1"
-scipy = "^1.7.0"
-seaborn = "^0.11.1"
-matplotlib = "^3.4.2"
+scipy = "=1.9.1"
+seaborn = "^0.12.2"
+matplotlib = "^3.7.1"
 louvain = "^0.7.0"
 diffxpy = "^0.7.4"
 docrep = "^0.3.2"
+tensorflow = "^2.11.1"
+joblib = "^1.2.0"
+numpy = ">=1.22"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.3"
 coverage = {extras = ["toml"], version = "^5.3"}
-safety = "^1.9.0"
+safety = "^2.3.0"
 mypy = "^0.812"
 typeguard = "^2.12.0"
 xdoctest = {extras = ["colors"], version = "^0.15.0"}
 sphinx = "^3.5.4"
 sphinx-autobuild = "^2021.3.14"
-pre-commit = "^2.11.1"
-flake8 = "^3.9.2"
-black = "^20.8b1"
-flake8-bandit = "^2.1.2"
+pre-commit = "^2.21.0"
+flake8 = "=4.0.1"
+black = "=22.3.0"
+bandit="=1.7.2"
+flake8-bandit = ">=2.1.2"
 flake8-bugbear = "^21.4.3"
 flake8-docstrings = "^1.5.0"
 flake8-rst-docstrings = "^0.2.3"
-pep8-naming = "^0.11.1"
+pep8-naming = "^0.13.2"
 darglint = "^1.5.8"
 reorder-python-imports = "^2.5.0"
-pre-commit-hooks = "^3.3.0"
+pre-commit-hooks = "^4.4.0"
 sphinx-rtd-theme = "^0.5.0"
 sphinx-click = "^2.5.0"
 Pygments = "^2.11.2"
 
 [tool.poetry.scripts]
 ncem = "ncem.__main__:main"
```

### Comparing `ncem-0.1.4/PKG-INFO` & `ncem-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: ncem
-Version: 0.1.4
+Version: 0.1.5
 Summary: ncem. Learning cell communication from spatial graphs of cells.
 Home-page: https://github.com/theislab/ncem
 License: BSD
 Author: Anna C. Schaar
 Author-email: anna.schaar@helmholtz-muenchen.de
-Requires-Python: >=3.7,<3.9
+Requires-Python: >=3.8,<=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=2.11.3,<4.0.0)
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
-Requires-Dist: click (>=7.1.2,<8.0.0)
+Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: diffxpy (>=0.7.4,<0.8.0)
 Requires-Dist: docrep (>=0.3.2,<0.4.0)
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: louvain (>=0.7.0,<0.8.0)
-Requires-Dist: matplotlib (>=3.4.2,<4.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: numpy (>=1.22)
 Requires-Dist: patsy (>=0.5.1,<0.6.0)
 Requires-Dist: rich (>=10.1.0,<11.0.0)
-Requires-Dist: scanpy (>=1.7.2,<2.0.0)
-Requires-Dist: scipy (>=1.7.0,<2.0.0)
-Requires-Dist: seaborn (>=0.11.1,<0.12.0)
-Requires-Dist: squidpy (>=1.0.0,<2.0.0)
-Requires-Dist: tensorflow (>=2.5.0,<3.0.0)
+Requires-Dist: scanpy (>=1.9.3,<2.0.0)
+Requires-Dist: scipy (==1.9.1)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: squidpy (>=1.2.3,<2.0.0)
+Requires-Dist: tensorflow (>=2.11.1,<3.0.0)
 Project-URL: Documentation, https://ncem.readthedocs.io
 Project-URL: Repository, https://github.com/theislab/ncem
 Description-Content-Type: text/x-rst
 
 ncem
 ===========================
```

