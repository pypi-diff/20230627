# Comparing `tmp/range_compression-0.2.5.tar.gz` & `tmp/range_compression-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "range_compression-0.2.5.tar", max compression
+gzip compressed data, was "range_compression-0.2.6.tar", max compression
```

## Comparing `range_compression-0.2.5.tar` & `range_compression-0.2.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      488 2023-05-19 02:23:35.360031 range_compression-0.2.5/README.md
--rw-r--r--   0        0        0      657 2023-06-27 06:22:11.964696 range_compression-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       90 2023-05-24 08:58:09.212988 range_compression-0.2.5/range_compression/__init__.py
--rw-r--r--   0        0        0     7045 2023-06-27 06:19:35.286998 range_compression-0.2.5/range_compression/range_compression.py
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 range_compression-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-05-19 02:23:35.360031 range_compression-0.2.6/README.md
+-rw-r--r--   0        0        0      657 2023-06-27 06:24:18.552189 range_compression-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-05-24 08:58:09.212988 range_compression-0.2.6/range_compression/__init__.py
+-rw-r--r--   0        0        0     7045 2023-06-27 06:19:35.286998 range_compression-0.2.6/range_compression/range_compression.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 range_compression-0.2.6/PKG-INFO
```

### Comparing `range_compression-0.2.5/pyproject.toml` & `range_compression-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "range-compression"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["myuan <zhengmy@ion.ac.cn>"]
 license = "LGPL"
 readme = "README.md"
 packages = [{include = "range_compression"}]
 repository = "https://github.com/myuanz/matrix-range-compression"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numba = "^0.57.1"
 numpy = "^1.24"
-polars = ">=0.17,<0.19"
+polars = ">=0.18,<0.19"
 importlib-metadata = { version = "^6.6.0", python = "^3.8" }
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 opencv-python-headless = "^4.7.0.72"
 tox = "^4.5.1"
```

### Comparing `range_compression-0.2.5/range_compression/range_compression.py` & `range_compression-0.2.6/range_compression/range_compression.py`

 * *Files identical despite different names*

### Comparing `range_compression-0.2.5/PKG-INFO` & `range_compression-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: range-compression
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Home-page: https://github.com/myuanz/matrix-range-compression
 License: LGPL
 Author: myuan
 Author-email: zhengmy@ion.ac.cn
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0) ; python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: numba (>=0.57.1,<0.58.0)
 Requires-Dist: numpy (>=1.24,<2.0)
-Requires-Dist: polars (>=0.17,<0.19)
+Requires-Dist: polars (>=0.18,<0.19)
 Project-URL: Repository, https://github.com/myuanz/matrix-range-compression
 Description-Content-Type: text/markdown
 
 # 矩阵区间压缩
 
 ## Quick start
```

