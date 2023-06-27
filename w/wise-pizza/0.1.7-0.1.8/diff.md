# Comparing `tmp/wise-pizza-0.1.7.tar.gz` & `tmp/wise-pizza-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.1.7.tar", last modified: Wed Jun 21 19:18:10 2023, max compression
+gzip compressed data, was "wise-pizza-0.1.8.tar", last modified: Tue Jun 27 13:35:02 2023, max compression
```

## Comparing `wise-pizza-0.1.7.tar` & `wise-pizza-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-21 19:18:10.260544 wise-pizza-0.1.7/
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-21 19:18:10.260021 wise-pizza-0.1.7/PKG-INFO
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/README.md
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-06-21 19:18:10.260655 wise-pizza-0.1.7/setup.cfg
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-06-21 19:17:15.000000 wise-pizza-0.1.7/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-21 19:18:10.255498 wise-pizza-0.1.7/wise_pizza/
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      118 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/__init__.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    11407 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/explain.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/find_alpha.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3917 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/make_matrix.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     9197 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/plotting.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      518 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/segment_data.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/slicer.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/solver.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-21 19:18:10.259169 wise-pizza-0.1.7/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:35:02.643746 wise-pizza-0.1.8/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-27 13:35:02.643522 wise-pizza-0.1.8/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/README.md
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-06-27 13:35:02.643807 wise-pizza-0.1.8/setup.cfg
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1185 2023-06-27 13:33:55.000000 wise-pizza-0.1.8/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:35:02.634882 wise-pizza-0.1.8/wise_pizza/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      118 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/__init__.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11407 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/explain.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/find_alpha.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4745 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/make_matrix.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9197 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/plotting.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      518 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/segment_data.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/slicer.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/solver.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:35:02.643173 wise-pizza-0.1.8/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.1.7/LICENSE` & `wise-pizza-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/PKG-INFO` & `wise-pizza-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wise-pizza-0.1.7/README.md` & `wise-pizza-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/setup.py` & `wise-pizza-0.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 from setuptools import find_packages, setup
 
+
+def _read_requirements_file(path: str):
+    with open(path) as f:
+        return list(map(
+            lambda req: req.strip(),
+            f.readlines(),
+        ))
+
+
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.1.7",
+    version="0.1.8",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    install_requires=[
-        "ipython",
-        "kaleido",
-        "numpy",
-        "pandas",
-        "pytest",
-        "plotly",
-        "scikit_learn",
-        "scipy>=1.8.0",
-        "tqdm",
-        "cloudpickle",
-        "pivottablejs"
-    ],
+    install_requires=_read_requirements_file('requirements.txt'),
     extras_require={
-        "test": [
-            "flake8",
-            "pytest",
-            "pytest-cov"
-        ],
+        "test": _read_requirements_file('requirements-dev.txt'),
     },
     packages=find_packages(
         include=[
             'wise_pizza',
             'wise_pizza.*'
         ],
         exclude=['tests*'],
```

### Comparing `wise-pizza-0.1.7/wise_pizza/explain.py` & `wise-pizza-0.1.8/wise_pizza/explain.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/wise_pizza/find_alpha.py` & `wise-pizza-0.1.8/wise_pizza/find_alpha.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/wise_pizza/make_matrix.py` & `wise-pizza-0.1.8/wise_pizza/make_matrix.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 import itertools
-from typing import Optional
+from typing import Optional, List, Dict
 
 import numpy as np
+import scipy
 from tqdm import tqdm
 import pandas as pd
 from scipy.sparse import csc_matrix, hstack
 
 
-def join_to_sparse(dim_df: pd.DataFrame, this_df: pd.DataFrame, verbose=0):
-    col_names = []
+def join_to_sparse(dim_df: pd.DataFrame, dim_name: str, verbose=0):
+    values = sorted(dim_df[dim_name].unique())
+
+    # create an "eye" dataframe
+    ext_df = pd.DataFrame(data=np.eye(len(values)), columns=values)
+    ext_df[dim_name] = values
+
+    join_df = pd.merge(dim_df, ext_df, on=[dim_name])
+    join_df = join_df.sort_values(list(dim_df.columns))
+    vals = csc_matrix(join_df[values].values)
+    if verbose > 0:
+        print(values, vals.shape)
+    return vals, values
+
+
+def segment_defs(dim_df: pd.DataFrame, used_dims, verbose=0) -> List[Dict[str, str]]:
     col_defs = []
-    ext_df = this_df.copy()
-    mat = np.eye(len(this_df))
-    these_dims = list(this_df.columns)
+    this_df = dim_df[used_dims].drop_duplicates().reset_index(drop=True)
     # create an "eye" dataframe on the unique reduced dimensions
     for i, vals in enumerate(this_df.itertuples(index=False)):
-        col_name = "_".join(map(str, vals))
-        col_names.append(col_name)
-        col_defs.append(dict(zip(these_dims, vals)))
-        ext_df[col_name] = mat[i]
-    dim_df_columns = list(dim_df.columns)
-    join_df = pd.merge(dim_df, ext_df, on=these_dims)
-    join_df = join_df.sort_values(dim_df_columns)
-    vals = csc_matrix(join_df[col_names].values)
+        col_defs.append(dict(zip(used_dims, vals)))
+
     if verbose > 0:
-        print(these_dims, vals.shape)
-    return vals, col_defs
+        print(used_dims, len(col_defs))
+    return col_defs
+
+
+def construct_dummies(
+    segment_defs: List[Dict[str, str]], cache: Dict[str, Dict[str, np.ndarray]]
+) -> scipy.sparse.csc_matrix:
+    dummies = []
+    for sgdf in segment_defs:
+        tmp = None
+        for k, v in sgdf.items():
+            if tmp is None:
+                tmp = cache[k][v]
+            else:
+                tmp = tmp.multiply(cache[k][v])
+        dummies.append(tmp)
+    return hstack(dummies)
 
 
 # This approach was way slower than the join one; keeping it here for reference :)
 # def join_to_sparse(dim_df, this_df, chunk_size=100, verbose=0):
 #     mats = []
 #     tuples = []
 #     col_defs = []
@@ -84,28 +106,36 @@
     if force_dim is None:
         dims = list(dim_df.columns)
     else:
         assert force_dim in dim_df.columns
         dims = [c for c in dim_df.columns if c != force_dim]
 
     # drop dimensions with only one value, for clarity
-    dims = [d for d in dims  if len(dim_df[d].unique()) > 1]
+    dims = [d for d in dims if len(dim_df[d].unique()) > 1]
 
     defs = []
     mats = []
     dims_range_min = min(len(dims), max(1, min_depth))
     dims_range_max = min(len(dims) + 1, max_depth + 1)
     dims_range = range(dims_range_min, dims_range_max)
+
+    # first pass: generate single-dim dummies
+    dummy_cache = {}
+    for d in dim_df.columns:
+        this_mat, these_defs = join_to_sparse(dim_df, d, verbose=verbose)
+        dummy_cache[d] = {this_def: this_mat[:, i : i + 1] for i, this_def in enumerate(these_defs)}
+
     for num_dims in tqdm(dims_range) if verbose else dims_range:
         for these_dims in itertools.combinations(dims, num_dims):
             if num_dims == 1 and these_dims[0] == "Change from":
                 continue
             if force_dim is None:
                 used_dims = list(these_dims)
             else:
                 used_dims = [force_dim] + list(these_dims)
-            this_df = dim_df[used_dims].drop_duplicates().reset_index(drop=True)
-            this_mat, these_defs = join_to_sparse(dim_df, this_df, verbose=verbose)
+
+            these_defs = segment_defs(dim_df, used_dims, verbose=verbose)
+            this_mat = construct_dummies(these_defs, dummy_cache)
             mats.append(this_mat)
             defs += these_defs
     mat = hstack(mats)
     return mat, defs
```

### Comparing `wise-pizza-0.1.7/wise_pizza/plotting.py` & `wise-pizza-0.1.8/wise_pizza/plotting.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/wise_pizza/segment_data.py` & `wise-pizza-0.1.8/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/wise_pizza/slicer.py` & `wise-pizza-0.1.8/wise_pizza/slicer.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/wise_pizza/solver.py` & `wise-pizza-0.1.8/wise_pizza/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/wise_pizza/utils.py` & `wise-pizza-0.1.8/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.7/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.1.8/wise_pizza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

