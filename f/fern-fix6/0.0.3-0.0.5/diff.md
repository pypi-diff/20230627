# Comparing `tmp/fern_fix6-0.0.3.tar.gz` & `tmp/fern_fix6-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_fix6-0.0.3.tar", max compression
+gzip compressed data, was "fern_fix6-0.0.5.tar", max compression
```

## Comparing `fern_fix6-0.0.3.tar` & `fern_fix6-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2479 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/README.md
--rw-r--r--   0        0        0      368 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      956 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/__init__.py
--rw-r--r--   0        0        0     2185 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/client.py
--rw-r--r--   0        0        0      348 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      289 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/errors/__init__.py
--rw-r--r--   0        0        0      271 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/errors/conflict_error.py
--rw-r--r--   0        0        0      271 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/errors/not_found_error.py
--rw-r--r--   0        0        0      313 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/py.typed
--rw-r--r--   0        0        0      270 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/admin/__init__.py
--rw-r--r--   0        0        0     2453 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/admin/client.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/atmospheric/__init__.py
--rw-r--r--   0        0        0     3670 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/atmospheric/client.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/ghg/__init__.py
--rw-r--r--   0        0        0     8748 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/ghg/client.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/healthcheck/__init__.py
--rw-r--r--   0        0        0     1582 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/healthcheck/client.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/masks/__init__.py
--rw-r--r--   0        0        0     3508 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/masks/client.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/projects/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/projects/client.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/satellite/__init__.py
--rw-r--r--   0        0        0     3193 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/satellite/client.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/soil/__init__.py
--rw-r--r--   0        0        0     2169 2023-06-27 15:42:47.495107 fern_fix6-0.0.3/src/fix6/resources/soil/client.py
--rw-r--r--   0        0        0       65 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/resources/weather/__init__.py
--rw-r--r--   0        0        0     3358 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/resources/weather/client.py
--rw-r--r--   0        0        0      815 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/__init__.py
--rw-r--r--   0        0        0      968 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/climate_data.py
--rw-r--r--   0        0        0      848 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/climate_returner.py
--rw-r--r--   0        0        0      745 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/http_error.py
--rw-r--r--   0        0        0      843 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/http_validation_error.py
--rw-r--r--   0        0        0      894 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/index_metadata.py
--rw-r--r--   0        0        0      791 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/project_area.py
--rw-r--r--   0        0        0     1337 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/project_supabase.py
--rw-r--r--   0        0        0      869 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      950 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/weather_data.py
--rw-r--r--   0        0        0      848 2023-06-27 15:42:47.499107 fern_fix6-0.0.3/src/fix6/types/weather_returner.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 fern_fix6-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-06-27 16:13:24.719705 fern_fix6-0.0.5/README.md
+-rw-r--r--   0        0        0      368 2023-06-27 16:13:24.719705 fern_fix6-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      956 2023-06-27 16:13:24.719705 fern_fix6-0.0.5/src/fix6/__init__.py
+-rw-r--r--   0        0        0     2185 2023-06-27 16:13:24.719705 fern_fix6-0.0.5/src/fix6/client.py
+-rw-r--r--   0        0        0      348 2023-06-27 16:13:24.719705 fern_fix6-0.0.5/src/fix6/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-27 16:13:24.719705 fern_fix6-0.0.5/src/fix6/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-27 16:13:24.719705 fern_fix6-0.0.5/src/fix6/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-27 16:13:24.719705 fern_fix6-0.0.5/src/fix6/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      289 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/errors/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/errors/conflict_error.py
+-rw-r--r--   0        0        0      271 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/errors/not_found_error.py
+-rw-r--r--   0        0        0      313 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/py.typed
+-rw-r--r--   0        0        0      270 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/admin/__init__.py
+-rw-r--r--   0        0        0     2453 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/admin/client.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/atmospheric/__init__.py
+-rw-r--r--   0        0        0     3670 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/atmospheric/client.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/ghg/__init__.py
+-rw-r--r--   0        0        0     8748 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/ghg/client.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/healthcheck/__init__.py
+-rw-r--r--   0        0        0     1582 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/healthcheck/client.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/masks/__init__.py
+-rw-r--r--   0        0        0     3508 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/masks/client.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/projects/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/projects/client.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/satellite/__init__.py
+-rw-r--r--   0        0        0     3193 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/satellite/client.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/soil/__init__.py
+-rw-r--r--   0        0        0     2169 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/soil/client.py
+-rw-r--r--   0        0        0       65 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/weather/__init__.py
+-rw-r--r--   0        0        0     3358 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/resources/weather/client.py
+-rw-r--r--   0        0        0      815 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/__init__.py
+-rw-r--r--   0        0        0      968 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/climate_data.py
+-rw-r--r--   0        0        0      848 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/climate_returner.py
+-rw-r--r--   0        0        0      745 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/http_error.py
+-rw-r--r--   0        0        0      843 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/http_validation_error.py
+-rw-r--r--   0        0        0      894 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/index_metadata.py
+-rw-r--r--   0        0        0      791 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/project_area.py
+-rw-r--r--   0        0        0     1337 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/project_supabase.py
+-rw-r--r--   0        0        0      869 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      950 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/weather_data.py
+-rw-r--r--   0        0        0      848 2023-06-27 16:13:24.723705 fern_fix6-0.0.5/src/fix6/types/weather_returner.py
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 fern_fix6-0.0.5/PKG-INFO
```

### Comparing `fern_fix6-0.0.3/README.md` & `fern_fix6-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/__init__.py` & `fern_fix6-0.0.5/src/fix6/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/client.py` & `fern_fix6-0.0.5/src/fix6/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/core/datetime_utils.py` & `fern_fix6-0.0.5/src/fix6/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/core/jsonable_encoder.py` & `fern_fix6-0.0.5/src/fix6/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/admin/client.py` & `fern_fix6-0.0.5/src/fix6/resources/admin/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/atmospheric/client.py` & `fern_fix6-0.0.5/src/fix6/resources/atmospheric/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/ghg/client.py` & `fern_fix6-0.0.5/src/fix6/resources/ghg/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/healthcheck/client.py` & `fern_fix6-0.0.5/src/fix6/resources/healthcheck/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/masks/client.py` & `fern_fix6-0.0.5/src/fix6/resources/masks/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/projects/client.py` & `fern_fix6-0.0.5/src/fix6/resources/projects/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/satellite/client.py` & `fern_fix6-0.0.5/src/fix6/resources/satellite/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/soil/client.py` & `fern_fix6-0.0.5/src/fix6/resources/soil/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/resources/weather/client.py` & `fern_fix6-0.0.5/src/fix6/resources/weather/client.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/__init__.py` & `fern_fix6-0.0.5/src/fix6/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/climate_data.py` & `fern_fix6-0.0.5/src/fix6/types/climate_data.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/climate_returner.py` & `fern_fix6-0.0.5/src/fix6/types/climate_returner.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/http_error.py` & `fern_fix6-0.0.5/src/fix6/types/http_error.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/http_validation_error.py` & `fern_fix6-0.0.5/src/fix6/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/index_metadata.py` & `fern_fix6-0.0.5/src/fix6/types/index_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/project_area.py` & `fern_fix6-0.0.5/src/fix6/types/project_area.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/project_supabase.py` & `fern_fix6-0.0.5/src/fix6/types/project_supabase.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/validation_error.py` & `fern_fix6-0.0.5/src/fix6/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/weather_data.py` & `fern_fix6-0.0.5/src/fix6/types/weather_data.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/src/fix6/types/weather_returner.py` & `fern_fix6-0.0.5/src/fix6/types/weather_returner.py`

 * *Files identical despite different names*

### Comparing `fern_fix6-0.0.3/PKG-INFO` & `fern_fix6-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-fix6
-Version: 0.0.3
+Version: 0.0.5
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

