# Comparing `tmp/arlas-tagger_api-24.0.1.tar.gz` & `tmp/arlas-tagger_api-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arlas-tagger_api-24.0.1.tar", last modified: Tue Apr 25 07:07:19 2023, max compression
+gzip compressed data, was "dist/arlas-tagger_api-24.0.2.tar", last modified: Tue Jun 27 09:44:40 2023, max compression
```

## Comparing `arlas-tagger_api-24.0.1.tar` & `arlas-tagger_api-24.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/
--rw-r--r--   0 container  (1000) container  (1000)      335 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/PKG-INFO
--rw-r--r--   0 container  (1000) container  (1000)     3196 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/README.md
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/arlas_tagger_api.egg-info/
--rw-r--r--   0 container  (1000) container  (1000)      335 2023-04-25 07:07:18.000000 arlas-tagger_api-24.0.1/arlas_tagger_api.egg-info/PKG-INFO
--rw-r--r--   0 container  (1000) container  (1000)     1448 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/arlas_tagger_api.egg-info/SOURCES.txt
--rw-r--r--   0 container  (1000) container  (1000)        1 2023-04-25 07:07:18.000000 arlas-tagger_api-24.0.1/arlas_tagger_api.egg-info/dependency_links.txt
--rw-r--r--   0 container  (1000) container  (1000)       48 2023-04-25 07:07:18.000000 arlas-tagger_api-24.0.1/arlas_tagger_api.egg-info/requires.txt
--rw-r--r--   0 container  (1000) container  (1000)       29 2023-04-25 07:07:18.000000 arlas-tagger_api-24.0.1/arlas_tagger_api.egg-info/top_level.txt
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/
--rw-r--r--   0 container  (1000) container  (1000)     1030 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)    24174 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/api_client.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/apis/
--rw-r--r--   0 container  (1000) container  (1000)      137 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/apis/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)    10732 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/apis/status_api.py
--rw-r--r--   0 container  (1000) container  (1000)    15559 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/apis/write_api.py
--rw-r--r--   0 container  (1000) container  (1000)     6815 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/configuration.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/
--rw-r--r--   0 container  (1000) container  (1000)      704 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)     3989 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/error.py
--rw-r--r--   0 container  (1000) container  (1000)     4271 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/expression.py
--rw-r--r--   0 container  (1000) container  (1000)     3919 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/failure.py
--rw-r--r--   0 container  (1000) container  (1000)     4605 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/filter.py
--rw-r--r--   0 container  (1000) container  (1000)     3383 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/form.py
--rw-r--r--   0 container  (1000) container  (1000)     4967 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/page.py
--rw-r--r--   0 container  (1000) container  (1000)     3563 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/projection.py
--rw-r--r--   0 container  (1000) container  (1000)     3483 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/propagation.py
--rw-r--r--   0 container  (1000) container  (1000)     5430 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/search.py
--rw-r--r--   0 container  (1000) container  (1000)     3355 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/tag.py
--rw-r--r--   0 container  (1000) container  (1000)    10742 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/tag_ref_request.py
--rw-r--r--   0 container  (1000) container  (1000)     5832 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/tag_request.py
--rw-r--r--   0 container  (1000) container  (1000)    10308 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/update_response.py
--rw-r--r--   0 container  (1000) container  (1000)    12814 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/arlas_tagger_api_python/rest.py
--rw-r--r--   0 container  (1000) container  (1000)       38 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/setup.cfg
--rw-r--r--   0 container  (1000) container  (1000)      963 2023-04-25 07:07:17.000000 arlas-tagger_api-24.0.1/setup.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-04-25 07:07:19.000000 arlas-tagger_api-24.0.1/test/
--rw-r--r--   0 container  (1000) container  (1000)        0 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/test/__init__.py
--rw-r--r--   0 container  (1000) container  (1000)      860 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/test/test_error.py
--rw-r--r--   0 container  (1000) container  (1000)      900 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/test/test_expression.py
--rw-r--r--   0 container  (1000) container  (1000)      876 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/test/test_failure.py
--rw-r--r--   0 container  (1000) container  (1000)      868 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/test/test_filter.py
--rw-r--r--   0 container  (1000) container  (1000)      852 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/test/test_form.py
--rw-r--r--   0 container  (1000) container  (1000)      852 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/test/test_page.py
--rw-r--r--   0 container  (1000) container  (1000)      900 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/test/test_projection.py
--rw-r--r--   0 container  (1000) container  (1000)      908 2023-04-25 07:07:08.000000 arlas-tagger_api-24.0.1/test/test_propagation.py
--rw-r--r--   0 container  (1000) container  (1000)      868 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/test/test_search.py
--rw-r--r--   0 container  (1000) container  (1000)      963 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/test/test_status_api.py
--rw-r--r--   0 container  (1000) container  (1000)      844 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/test/test_tag.py
--rw-r--r--   0 container  (1000) container  (1000)      928 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/test/test_tag_ref_request.py
--rw-r--r--   0 container  (1000) container  (1000)      902 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/test/test_tag_request.py
--rw-r--r--   0 container  (1000) container  (1000)      934 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/test/test_update_response.py
--rw-r--r--   0 container  (1000) container  (1000)     1052 2023-04-25 07:07:09.000000 arlas-tagger_api-24.0.1/test/test_write_api.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/
+-rw-r--r--   0 container  (1000) container  (1000)      335 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/PKG-INFO
+-rw-r--r--   0 container  (1000) container  (1000)     3196 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/README.md
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api.egg-info/
+-rw-r--r--   0 container  (1000) container  (1000)      335 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api.egg-info/PKG-INFO
+-rw-r--r--   0 container  (1000) container  (1000)     1448 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api.egg-info/SOURCES.txt
+-rw-r--r--   0 container  (1000) container  (1000)        1 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api.egg-info/dependency_links.txt
+-rw-r--r--   0 container  (1000) container  (1000)       48 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api.egg-info/requires.txt
+-rw-r--r--   0 container  (1000) container  (1000)       29 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api.egg-info/top_level.txt
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/
+-rw-r--r--   0 container  (1000) container  (1000)     1030 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)    24174 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/api_client.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/apis/
+-rw-r--r--   0 container  (1000) container  (1000)      137 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/apis/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)    10732 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/apis/status_api.py
+-rw-r--r--   0 container  (1000) container  (1000)    15559 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/apis/write_api.py
+-rw-r--r--   0 container  (1000) container  (1000)     6815 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/configuration.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/
+-rw-r--r--   0 container  (1000) container  (1000)      704 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)     3989 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/error.py
+-rw-r--r--   0 container  (1000) container  (1000)     4271 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/expression.py
+-rw-r--r--   0 container  (1000) container  (1000)     3919 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/failure.py
+-rw-r--r--   0 container  (1000) container  (1000)     4605 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/filter.py
+-rw-r--r--   0 container  (1000) container  (1000)     3383 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/form.py
+-rw-r--r--   0 container  (1000) container  (1000)     4967 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/page.py
+-rw-r--r--   0 container  (1000) container  (1000)     3563 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/projection.py
+-rw-r--r--   0 container  (1000) container  (1000)     3483 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/propagation.py
+-rw-r--r--   0 container  (1000) container  (1000)     5430 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/search.py
+-rw-r--r--   0 container  (1000) container  (1000)     3355 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/tag.py
+-rw-r--r--   0 container  (1000) container  (1000)    10742 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/tag_ref_request.py
+-rw-r--r--   0 container  (1000) container  (1000)     5832 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/tag_request.py
+-rw-r--r--   0 container  (1000) container  (1000)    10308 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/update_response.py
+-rw-r--r--   0 container  (1000) container  (1000)    12814 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/arlas_tagger_api_python/rest.py
+-rw-r--r--   0 container  (1000) container  (1000)       38 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/setup.cfg
+-rw-r--r--   0 container  (1000) container  (1000)      963 2023-06-27 09:44:39.000000 arlas-tagger_api-24.0.2/setup.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2023-06-27 09:44:40.000000 arlas-tagger_api-24.0.2/test/
+-rw-r--r--   0 container  (1000) container  (1000)        0 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/__init__.py
+-rw-r--r--   0 container  (1000) container  (1000)      860 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_error.py
+-rw-r--r--   0 container  (1000) container  (1000)      900 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_expression.py
+-rw-r--r--   0 container  (1000) container  (1000)      876 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_failure.py
+-rw-r--r--   0 container  (1000) container  (1000)      868 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_filter.py
+-rw-r--r--   0 container  (1000) container  (1000)      852 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_form.py
+-rw-r--r--   0 container  (1000) container  (1000)      852 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_page.py
+-rw-r--r--   0 container  (1000) container  (1000)      900 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_projection.py
+-rw-r--r--   0 container  (1000) container  (1000)      908 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_propagation.py
+-rw-r--r--   0 container  (1000) container  (1000)      868 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_search.py
+-rw-r--r--   0 container  (1000) container  (1000)      963 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_status_api.py
+-rw-r--r--   0 container  (1000) container  (1000)      844 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_tag.py
+-rw-r--r--   0 container  (1000) container  (1000)      928 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_tag_ref_request.py
+-rw-r--r--   0 container  (1000) container  (1000)      902 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_tag_request.py
+-rw-r--r--   0 container  (1000) container  (1000)      934 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_update_response.py
+-rw-r--r--   0 container  (1000) container  (1000)     1052 2023-06-27 09:44:25.000000 arlas-tagger_api-24.0.2/test/test_write_api.py
```

### Comparing `arlas-tagger_api-24.0.1/README.md` & `arlas-tagger_api-24.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # arlas-tagger-api-python
 (Un)Tag fields of ARLAS collections
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 24.0.1
+- API version: 24.0.2
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [http://www.gisaia.com/](http://www.gisaia.com/)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api.egg-info/SOURCES.txt` & `arlas-tagger_api-24.0.2/arlas_tagger_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/__init__.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/api_client.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import os
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/apis/status_api.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/apis/status_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/apis/write_api.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/apis/write_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/configuration.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -215,10 +215,10 @@
         Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 24.0.1\n"\
+               "Version of the API: 24.0.2\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/__init__.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/error.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/expression.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/failure.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/failure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/filter.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/form.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/page.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/projection.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/propagation.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/propagation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/search.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/tag.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/tag_ref_request.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/tag_ref_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/tag_request.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/tag_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/models/update_response.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/models/update_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-tagger_api-24.0.1/arlas_tagger_api_python/rest.py` & `arlas-tagger_api-24.0.2/arlas_tagger_api_python/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/setup.py` & `arlas-tagger_api-24.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "arlas-tagger_api"
-VERSION = "24.0.1"
+VERSION = "24.0.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `arlas-tagger_api-24.0.1/test/test_error.py` & `arlas-tagger_api-24.0.2/test/test_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_expression.py` & `arlas-tagger_api-24.0.2/test/test_expression.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_failure.py` & `arlas-tagger_api-24.0.2/test/test_failure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_filter.py` & `arlas-tagger_api-24.0.2/test/test_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_form.py` & `arlas-tagger_api-24.0.2/test/test_form.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_page.py` & `arlas-tagger_api-24.0.2/test/test_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_projection.py` & `arlas-tagger_api-24.0.2/test/test_projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_propagation.py` & `arlas-tagger_api-24.0.2/test/test_propagation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_search.py` & `arlas-tagger_api-24.0.2/test/test_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_status_api.py` & `arlas-tagger_api-24.0.2/test/test_status_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_tag.py` & `arlas-tagger_api-24.0.2/test/test_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_tag_ref_request.py` & `arlas-tagger_api-24.0.2/test/test_tag_ref_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_tag_request.py` & `arlas-tagger_api-24.0.2/test/test_tag_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_update_response.py` & `arlas-tagger_api-24.0.2/test/test_update_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-tagger_api-24.0.1/test/test_write_api.py` & `arlas-tagger_api-24.0.2/test/test_write_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Tagger API
 
     (Un)Tag fields of ARLAS collections
 
-    OpenAPI spec version: 24.0.1
+    OpenAPI spec version: 24.0.2
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

