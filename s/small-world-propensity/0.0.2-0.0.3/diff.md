# Comparing `tmp/small_world_propensity-0.0.2.tar.gz` & `tmp/small_world_propensity-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "small_world_propensity-0.0.2.tar", max compression
+gzip compressed data, was "small_world_propensity-0.0.3.tar", max compression
```

## Comparing `small_world_propensity-0.0.2.tar` & `small_world_propensity-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2344 2023-06-15 13:13:34.958452 small_world_propensity-0.0.2/README.md
--rw-r--r--   0        0        0     1710 2023-06-15 13:13:51.418575 small_world_propensity-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      284 2023-06-15 13:13:34.974452 small_world_propensity-0.0.2/small_world_propensity/__init__.py
--rw-r--r--   0        0        0     7058 2023-06-15 13:13:34.974452 small_world_propensity-0.0.2/small_world_propensity/small_world_propensity.py
--rw-r--r--   0        0        0     3117 1970-01-01 00:00:00.000000 small_world_propensity-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3069 2023-06-27 09:59:36.443259 small_world_propensity-0.0.3/README.md
+-rw-r--r--   0        0        0     1773 2023-06-27 09:59:54.279970 small_world_propensity-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      284 2023-06-27 09:59:36.483260 small_world_propensity-0.0.3/small_world_propensity/__init__.py
+-rw-r--r--   0        0        0     7058 2023-06-27 09:59:36.483260 small_world_propensity-0.0.3/small_world_propensity/small_world_propensity.py
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 small_world_propensity-0.0.3/PKG-INFO
```

### Comparing `small_world_propensity-0.0.2/README.md` & `small_world_propensity-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Small World Propensity
 
+[![GitHub release](https://img.shields.io/github/v/release/rkdan/small_world_propensity?include_prereleases)](https://GitHub.com/rkdan/small_world_propensity/releases)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/small-world-propensity.svg)](https://pypi.python.org/pypi/small-world-propensity/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
 This python package was adapted from the MATLAB package as first presented in [Small-World Propensity and Weighted Brain Networks](https://www.nature.com/articles/srep22057) (2016) by Sarah Feldt Muldoon, Eric W. Bridgeford & Danielle S. Bassett. Their original MATLAB implementation can be found [here](https://kk1995.github.io/BauerLab/BauerLab/MATLAB/lib/+mouse/+graph/smallWorldPropensity.html).
 
 ## Use
 The small-world propensity package can be installed using pip
 ```
 python -m pip install small-world-propensity
 ```
@@ -27,14 +32,18 @@
 ```
 Finally we produce the randomized cat matrix:
 ```
 cat_rand = swp.randomize_matrix(cat_symm)
 ```
 ![Cat matrices](https://github.com/rkdan/small_world_propensity/blob/main/img/cat.png?raw=True)
 
+The graphs visualized in a circular layout look as follows:
+
+![Cat graphs](https://github.com/rkdan/small_world_propensity/blob/main/img/cat_graphs.png?raw=True)
+
 ## Comparison of $\phi$ in real networks
 We can take the networks used in _Muldoon et al_ and plot $\phi$, $\Delta_L$, $\Delta_C$, and $\delta$. Note that these networks are not the exact same as the ones used in _Muldoon et al_, and due to differences in how Numpy performs permutations, and the use of NetworkX and iGraph libraries, the results are not identical, but still match closely.
 
 The adjacency matrices:
 ![Adjacency matrices](https://github.com/rkdan/small_world_propensity/blob/main/img/matrices.png?raw=True)
 
 And the results:
```

### Comparing `small_world_propensity-0.0.2/pyproject.toml` & `small_world_propensity-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "small-world-propensity"
-version = "0.0.2"
+version = "0.0.3"
 description = "A package designed to calculate the small-world propensity of a weighted, undirected network. Translated from the MATLAB version featured in Muldoon et al."
 authors = ["Ryan Daniels"]
+repository = "https://github.com/rkdan/small_world_propensity"
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "small_world_propensity"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.24.3"
```

### Comparing `small_world_propensity-0.0.2/small_world_propensity/small_world_propensity.py` & `small_world_propensity-0.0.3/small_world_propensity/small_world_propensity.py`

 * *Files identical despite different names*

### Comparing `small_world_propensity-0.0.2/PKG-INFO` & `small_world_propensity-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: small-world-propensity
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package designed to calculate the small-world propensity of a weighted, undirected network. Translated from the MATLAB version featured in Muldoon et al.
+Home-page: https://github.com/rkdan/small_world_propensity
 License: GPL-3.0-only
 Author: Ryan Daniels
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: python-igraph (>=0.10.4,<0.11.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Repository, https://github.com/rkdan/small_world_propensity
 Description-Content-Type: text/markdown
 
 # Small World Propensity
 
+[![GitHub release](https://img.shields.io/github/v/release/rkdan/small_world_propensity?include_prereleases)](https://GitHub.com/rkdan/small_world_propensity/releases)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/small-world-propensity.svg)](https://pypi.python.org/pypi/small-world-propensity/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
 This python package was adapted from the MATLAB package as first presented in [Small-World Propensity and Weighted Brain Networks](https://www.nature.com/articles/srep22057) (2016) by Sarah Feldt Muldoon, Eric W. Bridgeford & Danielle S. Bassett. Their original MATLAB implementation can be found [here](https://kk1995.github.io/BauerLab/BauerLab/MATLAB/lib/+mouse/+graph/smallWorldPropensity.html).
 
 ## Use
 The small-world propensity package can be installed using pip
 ```
 python -m pip install small-world-propensity
 ```
@@ -45,14 +52,18 @@
 ```
 Finally we produce the randomized cat matrix:
 ```
 cat_rand = swp.randomize_matrix(cat_symm)
 ```
 ![Cat matrices](https://github.com/rkdan/small_world_propensity/blob/main/img/cat.png?raw=True)
 
+The graphs visualized in a circular layout look as follows:
+
+![Cat graphs](https://github.com/rkdan/small_world_propensity/blob/main/img/cat_graphs.png?raw=True)
+
 ## Comparison of $\phi$ in real networks
 We can take the networks used in _Muldoon et al_ and plot $\phi$, $\Delta_L$, $\Delta_C$, and $\delta$. Note that these networks are not the exact same as the ones used in _Muldoon et al_, and due to differences in how Numpy performs permutations, and the use of NetworkX and iGraph libraries, the results are not identical, but still match closely.
 
 The adjacency matrices:
 ![Adjacency matrices](https://github.com/rkdan/small_world_propensity/blob/main/img/matrices.png?raw=True)
 
 And the results:
```

