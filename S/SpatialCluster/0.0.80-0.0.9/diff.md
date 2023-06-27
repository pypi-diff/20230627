# Comparing `tmp/SpatialCluster-0.0.80.tar.gz` & `tmp/SpatialCluster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpatialCluster-0.0.80.tar", last modified: Tue Jun 27 10:14:21 2023, max compression
+gzip compressed data, was "SpatialCluster-0.0.9.tar", last modified: Wed Nov 24 21:12:00 2021, max compression
```

## Comparing `SpatialCluster-0.0.80.tar` & `SpatialCluster-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,18 @@
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.573209 SpatialCluster-0.0.80/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1103 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/LICENSE
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      873 2023-06-27 10:14:21.572212 SpatialCluster-0.0.80/PKG-INFO
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      277 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/README.md
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.269695 SpatialCluster-0.0.80/SpatialCluster/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      236 2023-06-27 08:01:06.000000 SpatialCluster-0.0.80/SpatialCluster/__init__.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      372 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/constants.py
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.372392 SpatialCluster-0.0.80/SpatialCluster/data/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)  7846116 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/data/reduced_data_MinMaxScaler_PCA_manzana_224.csv
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      209 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/datasets.py
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.506924 SpatialCluster-0.0.80/SpatialCluster/methods/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     3501 2023-06-26 00:11:13.000000 SpatialCluster-0.0.80/SpatialCluster/methods/DMoN.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)    16495 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/methods/DMoN_core.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1128 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/methods/GMM.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     2773 2023-06-27 08:06:37.000000 SpatialCluster-0.0.80/SpatialCluster/methods/KNN.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      881 2023-06-27 08:00:17.000000 SpatialCluster-0.0.80/SpatialCluster/methods/SOM.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1775 2023-06-14 04:50:39.000000 SpatialCluster-0.0.80/SpatialCluster/methods/TDI.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/methods/__init__.py
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.523867 SpatialCluster-0.0.80/SpatialCluster/metrics/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1698 2023-06-27 10:11:33.000000 SpatialCluster-0.0.80/SpatialCluster/metrics/AMI.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1668 2023-06-27 10:11:30.000000 SpatialCluster-0.0.80/SpatialCluster/metrics/ARI.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/metrics/__init__.py
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.541807 SpatialCluster-0.0.80/SpatialCluster/preprocess/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)       64 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/preprocess/__init__.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     2478 2023-06-14 11:13:25.000000 SpatialCluster-0.0.80/SpatialCluster/preprocess/adjacency.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      843 2023-06-25 07:13:20.000000 SpatialCluster-0.0.80/SpatialCluster/preprocess/data_format.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     4536 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/preprocess/rings.py
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.558750 SpatialCluster-0.0.80/SpatialCluster/utils/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/utils/__init__.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      708 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/utils/data_format.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1357 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/utils/data_structures.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      342 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/utils/get_areas.py
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.566724 SpatialCluster-0.0.80/SpatialCluster/visualization/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/SpatialCluster/visualization/__init__.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     2330 2023-06-22 10:06:12.000000 SpatialCluster-0.0.80/SpatialCluster/visualization/plotters.py
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2023-06-27 10:14:21.275283 SpatialCluster-0.0.80/SpatialCluster.egg-info/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      873 2023-06-27 10:14:21.000000 SpatialCluster-0.0.80/SpatialCluster.egg-info/PKG-INFO
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1073 2023-06-27 10:14:21.000000 SpatialCluster-0.0.80/SpatialCluster.egg-info/SOURCES.txt
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)        1 2023-06-27 10:14:21.000000 SpatialCluster-0.0.80/SpatialCluster.egg-info/dependency_links.txt
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)       91 2023-06-27 10:14:21.000000 SpatialCluster-0.0.80/SpatialCluster.egg-info/requires.txt
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)       15 2023-06-27 10:14:21.000000 SpatialCluster-0.0.80/SpatialCluster.egg-info/top_level.txt
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      108 2023-06-09 22:41:54.000000 SpatialCluster-0.0.80/pyproject.toml
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)       38 2023-06-27 10:14:21.573209 SpatialCluster-0.0.80/setup.cfg
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1258 2023-06-27 08:01:02.000000 SpatialCluster-0.0.80/setup.py
+drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 21:12:00.113873 SpatialCluster-0.0.9/
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1103 2021-11-23 22:55:25.000000 SpatialCluster-0.0.9/LICENSE
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      836 2021-11-24 21:12:00.111904 SpatialCluster-0.0.9/PKG-INFO
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      220 2021-11-23 23:51:12.000000 SpatialCluster-0.0.9/README.md
+drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 21:12:00.093952 SpatialCluster-0.0.9/SpatialCluster/
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)    17728 2021-11-24 20:17:22.000000 SpatialCluster-0.0.9/SpatialCluster/DMoN.py
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      208 2021-11-24 21:02:09.000000 SpatialCluster-0.0.9/SpatialCluster/__init__.py
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      198 2021-11-24 19:45:31.000000 SpatialCluster-0.0.9/SpatialCluster/constants.py
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)     5462 2021-11-24 20:35:20.000000 SpatialCluster-0.0.9/SpatialCluster/core.py
+drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 21:12:00.109874 SpatialCluster-0.0.9/SpatialCluster.egg-info/
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      836 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/PKG-INFO
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      331 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)        1 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)       41 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/requires.txt
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)       15 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/top_level.txt
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      108 2021-11-23 23:33:31.000000 SpatialCluster-0.0.9/pyproject.toml
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)       38 2021-11-24 21:12:00.113873 SpatialCluster-0.0.9/setup.cfg
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1124 2021-11-24 21:02:53.000000 SpatialCluster-0.0.9/setup.py
```

### Comparing `SpatialCluster-0.0.80/LICENSE` & `SpatialCluster-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SpatialCluster-0.0.80/PKG-INFO` & `SpatialCluster-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: SpatialCluster
-Version: 0.0.80
+Version: 0.0.9
 Summary: Spatial cluster package
 Home-page: https://github.com/AxlKings/SpatialCluster
 Author: AxelReyesO (Axel Reyes O)
 Author-email: <axel.reyes@sansano.usm.cl>
 License: MIT
 Keywords: python spatial urban cluster
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -30,10 +31,9 @@
 
 Install using `pip`!
 
 ```sh
 $ pip install SpatialCluster
 ```
 
-## Documentation
+## To do...
 
-https://spatialcluster.readthedocs.io/en/latest/
```

### Comparing `SpatialCluster-0.0.80/SpatialCluster/methods/DMoN_core.py` & `SpatialCluster-0.0.9/SpatialCluster/DMoN.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from sklearn.metrics import cluster
 import tensorflow.compat.v2 as tf
-import scipy as sp
-import numpy as np
 import array
+import scipy.sparse as sp
+import numpy as np
+from scipy import spatial
 
 
 class DMoN(tf.keras.layers.Layer):
     """Implementation of Deep Modularity Network (DMoN) layer.
     Deep Modularity Network (DMoN) layer implementation as presented in
     "Graph Clustering with Graph Neural Networks" in a form of TF 2.0 Keras layer.
     DMoN optimizes modularity clustering objective in a fully unsupervised mode,
@@ -135,19 +135,19 @@
             self.activation = tf.keras.layers.Lambda(lambda x: x)
         else:
             raise ValueError('GCN activation of unknown type')
 
     def build(self, input_shape):
         """Builds the Keras model according to the input shape."""
         self.n_features = input_shape[0][-1]
-        self.kernel = self.add_weight(
+        self.kernel = self.add_variable(
             'kernel', shape=(self.n_features, self.n_channels))
-        self.bias = self.add_weight('bias', shape=(self.n_channels,))
+        self.bias = self.add_variable('bias', shape=(self.n_channels,))
         if self.skip_connection:
-            self.skip_weight = self.add_weight(
+            self.skip_weight = self.add_variable(
                 'skip_weight', shape=(self.n_channels,))
         else:
             self.skip_weight = 0
         super().build(input_shape)
 
     def call(self, inputs):
         """Computes GCN representations according to input features and input graph.
@@ -291,27 +291,27 @@
         use the unnormalized Laplacian construction.
         add_self_loops: If True, adds a one-diagonal corresponding to self-loops in
         the graph.
     Returns:
         A scipy sparse matrix containing the normalized version of the input graph.
     """
     if add_self_loops:
-        graph = graph + sp.sparse.identity(graph.shape[0])
+        graph = graph + sp.identity(graph.shape[0])
     degree = np.squeeze(np.asarray(graph.sum(axis=1)))
     if normalized:
         with np.errstate(divide='ignore'):
             inverse_sqrt_degree = 1. / np.sqrt(degree)
         inverse_sqrt_degree[inverse_sqrt_degree == np.inf] = 0
-        inverse_sqrt_degree = sp.sparse.diags(inverse_sqrt_degree)
+        inverse_sqrt_degree = sp.diags(inverse_sqrt_degree)
         return inverse_sqrt_degree @ graph @ inverse_sqrt_degree
     else:
         with np.errstate(divide='ignore'):
             inverse_degree = 1. / degree
         inverse_degree[inverse_degree == np.inf] = 0
-        inverse_degree = sp.sparse.diags(inverse_degree)
+        inverse_degree = sp.diags(inverse_degree)
         return inverse_degree @ graph
 
 # -----------------------------------------------------------------------------
 
 def load_npz(
     filename
 ):
@@ -321,19 +321,19 @@
     Returns:
         A tuple (graph, features, labels, label_indices) with the sparse adjacency
         matrix of a graph, sparse feature matrix, dense label array, and dense label
         index array (indices of nodes that have the labels in the label array).
     """
     with np.load(open(filename, 'rb'), allow_pickle=True) as loader:
         loader = dict(loader)
-        adjacency = sp.sparse.csr_matrix(
+        adjacency = sp.csr_matrix(
             (loader['adj_data'], loader['adj_indices'], loader['adj_indptr']),
             shape=loader['adj_shape'])
 
-        features = sp.sparse.csr_matrix(
+        features = sp.csr_matrix(
             (loader['feature_data'], loader['feature_indices'],
             loader['feature_indptr']),
             shape=loader['feature_shape'])
 
         label_indices = loader['label_indices']
         labels = loader['labels']
     assert adjacency.shape[0] == features.shape[
@@ -378,8 +378,57 @@
     for n_channels in [64]: # architecture
         output = GCN(n_channels)([output, input_graph])
     pool, pool_assignment = DMoN(n_clusters, collapse_regularization=reg, dropout_rate=dropout)([output, input_adjacency])
     return tf.keras.Model(
         inputs=[input_features, input_graph, input_adjacency],
         outputs=[pool, pool_assignment])
 
-# -----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
+
+
+class IncrementalCOOMatrix(object):
+
+    def __init__(self, shape, dtype):
+        if dtype is np.int32:
+            type_flag = 'i'
+        elif dtype is np.int64:
+            type_flag = 'l'
+        elif dtype is np.float32:
+            type_flag = 'f'
+        elif dtype is np.float64:
+            type_flag = 'd'
+        else:
+            raise Exception('Dtype not supported.')
+
+        self.dtype = dtype
+        self.shape = shape
+
+        self.rows = array.array('i')
+        self.cols = array.array('i')
+        self.data = array.array(type_flag)
+
+    def append(self, i, j, v):
+        m, n = self.shape
+        if (i >= m or j >= n):
+            raise Exception('Index out of bounds')
+
+        self.rows.append(i)
+        self.cols.append(j)
+        self.data.append(v)
+
+    def tocoo(self):
+        rows = np.frombuffer(self.rows, dtype=np.int32)
+        cols = np.frombuffer(self.cols, dtype=np.int32)
+        data = np.frombuffer(self.data, dtype=self.dtype)
+
+        return sp.coo_matrix((data, (rows, cols)),
+                             shape=self.shape)
+
+    def __len__(self):
+
+        return len(self.data)
+
+# -----------------------------------------------------------------------------
+
+
+
+
```

### Comparing `SpatialCluster-0.0.80/SpatialCluster.egg-info/PKG-INFO` & `SpatialCluster-0.0.9/SpatialCluster.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: SpatialCluster
-Version: 0.0.80
+Version: 0.0.9
 Summary: Spatial cluster package
 Home-page: https://github.com/AxlKings/SpatialCluster
 Author: AxelReyesO (Axel Reyes O)
 Author-email: <axel.reyes@sansano.usm.cl>
 License: MIT
 Keywords: python spatial urban cluster
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -30,10 +31,9 @@
 
 Install using `pip`!
 
 ```sh
 $ pip install SpatialCluster
 ```
 
-## Documentation
+## To do...
 
-https://spatialcluster.readthedocs.io/en/latest/
```

### Comparing `SpatialCluster-0.0.80/setup.py` & `SpatialCluster-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 import os
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.80'
+VERSION = '0.0.9'
 DESCRIPTION = 'Spatial cluster package'
 
 # Setting up
 setup(
     name="SpatialCluster",
     version=VERSION,
     author="AxelReyesO (Axel Reyes O)",
     author_email="<axel.reyes@sansano.usm.cl>",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    install_requires=['scikit-learn','tensorflow','scipy','numpy','matplotlib','folium','minisom','seaborn','geopandas','contextily'],
+    install_requires=['tensorflow','scipy','numpy','matplotlib','folium'],
     url="https://github.com/AxlKings/SpatialCluster",
     keywords='python spatial urban cluster',
     license='MIT',
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ],
-    include_package_data=True,
-    package_data={'': ['data/*.csv']},
+    ]
 )
```

