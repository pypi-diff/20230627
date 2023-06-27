# Comparing `tmp/eodc-2023.6.7.tar.gz` & `tmp/eodc-2023.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.7.tar", max compression
+gzip compressed data, was "eodc-2023.6.8.tar", max compression
```

## Comparing `eodc-2023.6.7.tar` & `eodc-2023.6.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-26 08:23:40.814599 eodc-2023.6.7/README.md
--rw-r--r--   0        0        0      213 2023-06-26 08:23:40.814599 eodc-2023.6.7/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-26 08:23:40.814599 eodc-2023.6.7/eodc/dask.py
--rw-r--r--   0        0        0    11579 2023-06-26 08:23:40.814599 eodc-2023.6.7/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-26 08:23:40.814599 eodc-2023.6.7/eodc/settings.py
--rw-r--r--   0        0        0     1204 2023-06-26 08:23:40.814599 eodc-2023.6.7/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 eodc-2023.6.7/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-27 12:34:34.781284 eodc-2023.6.8/README.md
+-rw-r--r--   0        0        0      213 2023-06-27 12:34:34.781284 eodc-2023.6.8/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-27 12:34:34.781284 eodc-2023.6.8/eodc/dask.py
+-rw-r--r--   0        0        0    11579 2023-06-27 12:34:34.781284 eodc-2023.6.8/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-27 12:34:34.781284 eodc-2023.6.8/eodc/settings.py
+-rw-r--r--   0        0        0     1207 2023-06-27 12:34:34.781284 eodc-2023.6.8/pyproject.toml
+-rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 eodc-2023.6.8/PKG-INFO
```

### Comparing `eodc-2023.6.7/README.md` & `eodc-2023.6.8/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.7/eodc/dask.py` & `eodc-2023.6.8/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.7/eodc/faas.py` & `eodc-2023.6.8/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.7/pyproject.toml` & `eodc-2023.6.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.7"
+version = "2023.6.8"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -21,17 +21,17 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 requests = "^2.28.2"
 pydantic = "^1.10.7"
 argo-workflows = "6.3.9"
 dask-gateway = "^2022.11.0"
-eodc-faas-force = "2023.6.2"
-eodc-faas-sen2like = "2023.6.2"
-eodc-faas-openeo = "2023.6.6"
+eodc-faas-force = "^2023.6.2"
+eodc-faas-sen2like = "^2023.6.2"
+eodc-faas-openeo = "^2023.6.8"
 pystac = "^1.7.3"
 eodc-faas-snap = "^2023.6.2"
 pyproj = "^3.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
```

### Comparing `eodc-2023.6.7/PKG-INFO` & `eodc-2023.6.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.7
+Version: 2023.6.8
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: argo-workflows (==6.3.9)
 Requires-Dist: dask-gateway (>=2022.11.0,<2023.0.0)
-Requires-Dist: eodc-faas-force (==2023.6.2)
-Requires-Dist: eodc-faas-openeo (==2023.6.6)
-Requires-Dist: eodc-faas-sen2like (==2023.6.2)
+Requires-Dist: eodc-faas-force (>=2023.6.2,<2024.0.0)
+Requires-Dist: eodc-faas-openeo (>=2023.6.8,<2024.0.0)
+Requires-Dist: eodc-faas-sen2like (>=2023.6.2,<2024.0.0)
 Requires-Dist: eodc-faas-snap (>=2023.6.2,<2024.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyproj (>=3.6.0,<4.0.0)
 Requires-Dist: pystac (>=1.7.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/eodcgmbh/eodc-sdk
 Description-Content-Type: text/markdown
```

