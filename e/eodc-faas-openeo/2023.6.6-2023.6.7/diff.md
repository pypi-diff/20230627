# Comparing `tmp/eodc_faas_openeo-2023.6.6.tar.gz` & `tmp/eodc_faas_openeo-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_openeo-2023.6.6.tar", max compression
+gzip compressed data, was "eodc_faas_openeo-2023.6.7.tar", max compression
```

## Comparing `eodc_faas_openeo-2023.6.6.tar` & `eodc_faas_openeo-2023.6.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       11 2023-06-22 06:40:14.428000 eodc_faas_openeo-2023.6.6/README.md
--rw-r--r--   0        0        0      102 2023-06-22 06:40:14.428000 eodc_faas_openeo-2023.6.6/openeo_executor_bindings/__init__.py
--rw-r--r--   0        0        0      901 2023-06-22 06:40:14.428000 eodc_faas_openeo-2023.6.6/openeo_executor_bindings/model.py
--rw-r--r--   0        0        0      612 2023-06-22 06:40:14.428000 eodc_faas_openeo-2023.6.6/pyproject.toml
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 eodc_faas_openeo-2023.6.6/PKG-INFO
+-rw-r--r--   0        0        0       11 2023-06-27 11:53:43.468000 eodc_faas_openeo-2023.6.7/README.md
+-rw-r--r--   0        0        0      102 2023-06-27 11:53:43.468000 eodc_faas_openeo-2023.6.7/openeo_executor_bindings/__init__.py
+-rw-r--r--   0        0        0      901 2023-06-27 11:53:43.468000 eodc_faas_openeo-2023.6.7/openeo_executor_bindings/model.py
+-rw-r--r--   0        0        0      612 2023-06-27 11:53:43.468000 eodc_faas_openeo-2023.6.7/pyproject.toml
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 eodc_faas_openeo-2023.6.7/PKG-INFO
```

### Comparing `eodc_faas_openeo-2023.6.6/openeo_executor_bindings/model.py` & `eodc_faas_openeo-2023.6.7/openeo_executor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_openeo-2023.6.6/pyproject.toml` & `eodc_faas_openeo-2023.6.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-openeo"
-version = "2023.6.6"
+version = "2023.6.7"
 description = "Bindings for the OpenEO processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "openeo_executor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_openeo-2023.6.6/PKG-INFO` & `eodc_faas_openeo-2023.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-openeo
-Version: 2023.6.6
+Version: 2023.6.7
 Summary: Bindings for the OpenEO processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

