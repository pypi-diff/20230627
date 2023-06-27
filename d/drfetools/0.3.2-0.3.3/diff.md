# Comparing `tmp/drfetools-0.3.2.tar.gz` & `tmp/drfetools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drfetools-0.3.2.tar", max compression
+gzip compressed data, was "drfetools-0.3.3.tar", max compression
```

## Comparing `drfetools-0.3.2.tar` & `drfetools-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2021-09-02 20:40:08.000000 drfetools-0.3.2/LICENSE
--rw-r--r--   0        0        0    18709 2023-06-26 21:39:30.000000 drfetools-0.3.2/README.md
--rw-r--r--   0        0        0       25 2021-09-09 01:19:06.000000 drfetools-0.3.2/drfetools/__init__.py
--rwxr-xr-x   0        0        0     9851 2023-06-21 20:56:15.000000 drfetools-0.3.2/drfetools/dRFEtools.py
--rw-r--r--   0        0        0     8251 2023-06-21 20:40:36.000000 drfetools-0.3.2/drfetools/dev_scoring.py
--rw-r--r--   0        0        0     7643 2023-06-21 20:55:18.000000 drfetools-0.3.2/drfetools/lowess_redundant.py
--rw-r--r--   0        0        0     7306 2023-06-21 20:40:54.000000 drfetools-0.3.2/drfetools/random_forest.py
--rw-r--r--   0        0        0     1605 2021-09-30 19:29:32.000000 drfetools-0.3.2/drfetools/rank_function.py
--rw-r--r--   0        0        0      947 2023-06-27 12:15:44.000000 drfetools-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    19886 1970-01-01 00:00:00.000000 drfetools-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-09-02 20:40:08.000000 drfetools-0.3.3/LICENSE
+-rw-r--r--   0        0        0    18709 2023-06-26 21:39:30.000000 drfetools-0.3.3/README.md
+-rw-r--r--   0        0        0       48 2023-06-27 13:02:05.000000 drfetools-0.3.3/dRFEtools/__init__.py
+-rwxr-xr-x   0        0        0     9851 2023-06-27 12:59:16.000000 drfetools-0.3.3/dRFEtools/dRFEtools.py
+-rw-r--r--   0        0        0     8251 2023-06-21 20:40:36.000000 drfetools-0.3.3/dRFEtools/dev_scoring.py
+-rw-r--r--   0        0        0     7643 2023-06-21 20:55:18.000000 drfetools-0.3.3/dRFEtools/lowess_redundant.py
+-rw-r--r--   0        0        0     7306 2023-06-21 20:40:54.000000 drfetools-0.3.3/dRFEtools/random_forest.py
+-rw-r--r--   0        0        0     1605 2021-09-30 19:29:32.000000 drfetools-0.3.3/dRFEtools/rank_function.py
+-rw-r--r--   0        0        0     1035 2023-06-27 13:01:56.000000 drfetools-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    19886 1970-01-01 00:00:00.000000 drfetools-0.3.3/PKG-INFO
```

### Comparing `drfetools-0.3.2/LICENSE` & `drfetools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.2/README.md` & `drfetools-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.2/drfetools/dRFEtools.py` & `drfetools-0.3.3/dRFEtools/dRFEtools.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.2/drfetools/dev_scoring.py` & `drfetools-0.3.3/dRFEtools/dev_scoring.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.2/drfetools/lowess_redundant.py` & `drfetools-0.3.3/dRFEtools/lowess_redundant.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.2/drfetools/random_forest.py` & `drfetools-0.3.3/dRFEtools/random_forest.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.2/drfetools/rank_function.py` & `drfetools-0.3.3/dRFEtools/rank_function.py`

 * *Files identical despite different names*

### Comparing `drfetools-0.3.2/pyproject.toml` & `drfetools-0.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "dRFEtools"
 packages = [
-    {include = "drfetools"}
+    {include = "dRFEtools"}
 ]
-version = "0.3.2"
+version = "0.3.3"
 description = "A package for preforming dynamic recursive feature elimination with sklearn."
 authors = ["Kynon JM Benjamin <kj.benjamin90@gmail.com>", "Apuã Paquola <apua.paquola@libd.org>"]
 maintainers = ["Kynon JM Benjamin <kj.benjamin90@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/LieberInstitute/dRFEtools.git"
 repository = "https://github.com/LieberInstitute/dRFEtools.git"
@@ -23,10 +23,13 @@
 scipy = "^1.7"
 statsmodels = "^0.14.0"
 
 [tool.poetry.dev-dependencies]
 pandas-plink = "^2.2.9"
 gtfparse = "^1.2.1"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `drfetools-0.3.2/PKG-INFO` & `drfetools-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drfetools
-Version: 0.3.2
+Version: 0.3.3
 Summary: A package for preforming dynamic recursive feature elimination with sklearn.
 Home-page: https://github.com/LieberInstitute/dRFEtools.git
 License: GPL-3.0-only
 Keywords: recursive feature elimination,sklearn,feature ranking
 Author: Kynon JM Benjamin
 Author-email: kj.benjamin90@gmail.com
 Maintainer: Kynon JM Benjamin
```

