# Comparing `tmp/drfetools-0.3.1.tar.gz` & `tmp/drfetools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drfetools-0.3.1.tar", max compression
+gzip compressed data, was "drfetools-0.3.2.tar", max compression
```

## Comparing `drfetools-0.3.1.tar` & `drfetools-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2021-09-02 20:40:08.000000 drfetools-0.3.1/LICENSE
--rw-r--r--   0        0        0    18709 2023-06-26 21:39:30.000000 drfetools-0.3.1/README.md
--rw-r--r--   0        0        0       25 2021-09-09 01:19:06.000000 drfetools-0.3.1/dRFEtools/__init__.py
--rwxr-xr-x   0        0        0     9851 2023-06-21 20:56:15.000000 drfetools-0.3.1/dRFEtools/dRFEtools.py
--rw-r--r--   0        0        0     8251 2023-06-21 20:40:36.000000 drfetools-0.3.1/dRFEtools/dev_scoring.py
--rw-r--r--   0        0        0     7643 2023-06-21 20:55:18.000000 drfetools-0.3.1/dRFEtools/lowess_redundant.py
--rw-r--r--   0        0        0     7306 2023-06-21 20:40:54.000000 drfetools-0.3.1/dRFEtools/random_forest.py
--rw-r--r--   0        0        0     1605 2021-09-30 19:29:32.000000 drfetools-0.3.1/dRFEtools/rank_function.py
--rw-r--r--   0        0        0      947 2023-06-26 21:38:42.000000 drfetools-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    19886 1970-01-01 00:00:00.000000 drfetools-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-09-02 20:40:08.000000 drfetools-0.3.2/LICENSE
+-rw-r--r--   0        0        0    18709 2023-06-26 21:39:30.000000 drfetools-0.3.2/README.md
+-rw-r--r--   0        0        0       25 2021-09-09 01:19:06.000000 drfetools-0.3.2/drfetools/__init__.py
+-rwxr-xr-x   0        0        0     9851 2023-06-21 20:56:15.000000 drfetools-0.3.2/drfetools/dRFEtools.py
+-rw-r--r--   0        0        0     8251 2023-06-21 20:40:36.000000 drfetools-0.3.2/drfetools/dev_scoring.py
+-rw-r--r--   0        0        0     7643 2023-06-21 20:55:18.000000 drfetools-0.3.2/drfetools/lowess_redundant.py
+-rw-r--r--   0        0        0     7306 2023-06-21 20:40:54.000000 drfetools-0.3.2/drfetools/random_forest.py
+-rw-r--r--   0        0        0     1605 2021-09-30 19:29:32.000000 drfetools-0.3.2/drfetools/rank_function.py
+-rw-r--r--   0        0        0      947 2023-06-27 12:15:44.000000 drfetools-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    19886 1970-01-01 00:00:00.000000 drfetools-0.3.2/PKG-INFO
```

### Comparing `drfetools-0.3.1/LICENSE` & `drfetools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.1/README.md` & `drfetools-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.1/dRFEtools/dRFEtools.py` & `drfetools-0.3.2/drfetools/dRFEtools.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.1/dRFEtools/dev_scoring.py` & `drfetools-0.3.2/drfetools/dev_scoring.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.1/dRFEtools/lowess_redundant.py` & `drfetools-0.3.2/drfetools/lowess_redundant.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.1/dRFEtools/random_forest.py` & `drfetools-0.3.2/drfetools/random_forest.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.1/dRFEtools/rank_function.py` & `drfetools-0.3.2/drfetools/rank_function.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.1/pyproject.toml` & `drfetools-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "dRFEtools"
 packages = [
-    {include = "dRFEtools"}
+    {include = "drfetools"}
 ]
-version = "0.3.1"
+version = "0.3.2"
 description = "A package for preforming dynamic recursive feature elimination with sklearn."
 authors = ["Kynon JM Benjamin <kj.benjamin90@gmail.com>", "Apuã Paquola <apua.paquola@libd.org>"]
 maintainers = ["Kynon JM Benjamin <kj.benjamin90@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/LieberInstitute/dRFEtools.git"
 repository = "https://github.com/LieberInstitute/dRFEtools.git"
 keywords = ['recursive feature elimination', 'sklearn', 'feature ranking']
 
 [tool.poetry.dependencies]
 python = "^3.8"
-numpy = "^1.24.0"
+numpy = "^1.20.0"
 pandas = "^2.0.2"
 matplotlib = "^3.7.0"
 plotnine = "^0.12.1"
 scikit-learn = "^1.2"
 scipy = "^1.7"
 statsmodels = "^0.14.0"
```

### Comparing `drfetools-0.3.1/PKG-INFO` & `drfetools-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drfetools
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package for preforming dynamic recursive feature elimination with sklearn.
 Home-page: https://github.com/LieberInstitute/dRFEtools.git
 License: GPL-3.0-only
 Keywords: recursive feature elimination,sklearn,feature ranking
 Author: Kynon JM Benjamin
 Author-email: kj.benjamin90@gmail.com
 Maintainer: Kynon JM Benjamin
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: plotnine (>=0.12.1,<0.13.0)
 Requires-Dist: scikit-learn (>=1.2,<2.0)
 Requires-Dist: scipy (>=1.7,<2.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Project-URL: Repository, https://github.com/LieberInstitute/dRFEtools.git
 Description-Content-Type: text/markdown
```

