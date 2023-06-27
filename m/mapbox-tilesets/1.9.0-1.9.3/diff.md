# Comparing `tmp/mapbox-tilesets-1.9.0.tar.gz` & `tmp/mapbox-tilesets-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mapbox-tilesets-1.9.0.tar", last modified: Wed Jun 21 21:26:50 2023, max compression
+gzip compressed data, was "dist/mapbox-tilesets-1.9.3.tar", last modified: Tue Jun 27 18:20:51 2023, max compression
```

## Comparing `mapbox-tilesets-1.9.0.tar` & `mapbox-tilesets-1.9.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    15395 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15036 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      767 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/scripts/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    29264 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/scripts/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6046 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15395 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      924 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      261 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1594 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3045 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_activity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5265 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_create.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2809 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_delete.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6170 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_estimate_area.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4178 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_jobs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8142 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2052 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_publish.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11664 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_sources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2350 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3568 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_tilejson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2245 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_update.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2506 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_update_recipe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_validate_recipe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_view_recipe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      826 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_file_validator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      212 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_version_documentation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15395 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15036 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       53 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/mapbox_tilesets/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      805 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/mapbox_tilesets/errors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/mapbox_tilesets/scripts/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    29264 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/mapbox_tilesets/scripts/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6174 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/mapbox_tilesets/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15395 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      924 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      261 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1594 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-27 18:20:51.000000 mapbox-tilesets-1.9.3/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3045 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_activity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5265 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_create.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2757 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_delete.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6257 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_estimate_area.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4178 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_jobs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8142 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2052 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_publish.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11751 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_sources.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2346 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3550 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_tilejson.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2245 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_update.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2506 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_update_recipe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_validate_recipe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1923 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_cli_view_recipe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      826 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_file_validator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      212 2023-06-27 18:19:21.000000 mapbox-tilesets-1.9.3/tests/test_version_documentation.py
```

### Comparing `mapbox-tilesets-1.9.0/LICENSE.md` & `mapbox-tilesets-1.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/PKG-INFO` & `mapbox-tilesets-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapbox-tilesets
-Version: 1.9.0
+Version: 1.9.3
 Summary: CLI for interacting with and preparing data for the Tilesets API
 Home-page: https://github.com/mapbox/tilesets-cli
 Author: Mapbox
 Author-email: sam@mapbox.com
 License: BSD-2
 Description-Content-Type: text/markdown
 Provides-Extra: estimate-area
```

### Comparing `mapbox-tilesets-1.9.0/README.md` & `mapbox-tilesets-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/mapbox_tilesets/errors.py` & `mapbox-tilesets-1.9.3/mapbox_tilesets/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Error handling for the tilesets CLI"""
+from click import ClickException
 
 
-class TilesetsError(Exception):
+class TilesetsError(ClickException):
     """Base Tilesets error
     Deriving errors from this base isolates module development
     problems from Python usage problems.
     """
 
     exit_code = 1
```

### Comparing `mapbox-tilesets-1.9.0/mapbox_tilesets/scripts/cli.py` & `mapbox-tilesets-1.9.3/mapbox_tilesets/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/mapbox_tilesets/utils.py` & `mapbox-tilesets-1.9.3/mapbox_tilesets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import importlib
 import os
 import re
 
 import numpy as np
 
-from jsonschema import validate
+from click import ClickException
+from jsonschema import validate, ValidationError
 from requests import Session
 
 import mapbox_tilesets
 import geojson
 import json
 
 
@@ -122,15 +123,18 @@
             "properties": {
                 "$id": "#/properties/properties",
                 "type": "object",
                 "title": "The Properties Schema",
             },
         },
     }
-    validate(instance=feature, schema=schema)
+    try:
+        validate(instance=feature, schema=schema)
+    except ValidationError as e:
+        raise ClickException(e)
     geojson_validate(index, feature)
 
 
 def _convert_precision_to_zoom(precision):
     """Converts precision to zoom level based on the minimum zoom
 
     Parameters
```

### Comparing `mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/PKG-INFO` & `mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapbox-tilesets
-Version: 1.9.0
+Version: 1.9.3
 Summary: CLI for interacting with and preparing data for the Tilesets API
 Home-page: https://github.com/mapbox/tilesets-cli
 Author: Mapbox
 Author-email: sam@mapbox.com
 License: BSD-2
 Description-Content-Type: text/markdown
 Provides-Extra: estimate-area
```

### Comparing `mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/SOURCES.txt` & `mapbox-tilesets-1.9.3/mapbox_tilesets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/setup.py` & `mapbox-tilesets-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_activity.py` & `mapbox-tilesets-1.9.3/tests/test_cli_activity.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_create.py` & `mapbox-tilesets-1.9.3/tests/test_cli_create.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_delete.py` & `mapbox-tilesets-1.9.3/tests/test_cli_delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import pytest
 
 from click.testing import CliRunner
 from unittest import mock
 
 from mapbox_tilesets.scripts.cli import delete
-from mapbox_tilesets.errors import TilesetsError
 
 
 class MockResponse:
     def __init__(self, mock_json, status_code):
         self.text = json.dumps(mock_json)
         print(self.text)
         self._json = mock_json
@@ -78,8 +77,8 @@
         {"message": "uh oh"}, status_code=422
     )
     result = runner.invoke(delete, ["test.id", "--force"])
     mock_request_delete.assert_called_with(
         "https://api.mapbox.com/tilesets/v1/test.id?access_token=pk.eyJ1IjoidGVzdC11c2VyIn0K"
     )
     assert result.exit_code == 1
-    assert isinstance(result.exception, TilesetsError)
+    assert isinstance(result.exception, SystemExit)
```

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_estimate_area.py` & `mapbox-tilesets-1.9.3/tests/test_cli_estimate_area.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from click.testing import CliRunner
 
 from mapbox_tilesets.scripts.cli import estimate_area
+from utils import clean_runner_output
 
 
 # rainy day scenarios
 def test_cli_estimate_area_features_from_invalid_stdin_geojson():
     message = "Error with feature parsing. Ensure that feature inputs are valid and formatted correctly. Try 'tilesets estimate-area --help' for help."
     runner = CliRunner()
     invalidated_result = runner.invoke(
         estimate_area, ["--precision", "10m"], input="invalidGeoJson input"
     )
     assert invalidated_result.exit_code == 1
-    assert str(invalidated_result.exception) == message
+    assert clean_runner_output(invalidated_result.output) == message
 
 
 def test_cli_estimate_area_features_from_invalid_geojson_content():
     message = "'properties' is a required property"
     runner = CliRunner()
     invalidated_result = runner.invoke(
         estimate_area,
         ["tests/fixtures/invalid-geojson.ldgeojson", "--precision", "1m"],
     )
-    assert message in str(invalidated_result.exception)
+    assert message in str(invalidated_result.output)
     assert invalidated_result.exit_code == 1
 
 
 def test_cli_estimate_area_features_from_nonexistent_geojson_file():
     message = "Error with feature parsing. Ensure that feature inputs are valid and formatted correctly. Try 'tilesets estimate-area --help' for help."
     runner = CliRunner()
     invalidated_result = runner.invoke(
         estimate_area,
         ["tests/fixtures/nonexistent-geojson.ldgeojson", "--precision", "1m"],
     )
-    assert str(invalidated_result.exception) == message
+    assert clean_runner_output(invalidated_result.output) == message
     assert invalidated_result.exit_code == 1
 
 
 def test_cli_estimate_area_no_precision():
     runner = CliRunner()
     invalidated_result = runner.invoke(
         estimate_area,
@@ -60,26 +61,26 @@
     message = "The --force-1cm flag must be present to enable 1cm precision area calculation and may take longer for large feature inputs or data with global extents. 1cm precision for tileset processing is only available upon request after contacting Mapbox support."
     runner = CliRunner()
     invalidated_result = runner.invoke(
         estimate_area,
         ["tests/fixtures/valid.ldgeojson", "-p", "1cm"],
     )
     assert invalidated_result.exit_code == 1
-    assert str(invalidated_result.exception) == message
+    assert clean_runner_output(invalidated_result.output) == message
 
 
 def test_cli_estimate_area_invalid_1cm_precision_flag():
     message = "The --force-1cm flag is enabled but the precision is not 1cm."
     runner = CliRunner()
     invalidated_result = runner.invoke(
         estimate_area,
         ["tests/fixtures/valid.ldgeojson", "-p", "1m", "--force-1cm"],
     )
     assert invalidated_result.exit_code == 1
-    assert str(invalidated_result.exception) == message
+    assert clean_runner_output(invalidated_result.output) == message
 
 
 # sunny day scenarios
 def test_cli_estimate_area_valid_features_files_and_precision():
     output = '{"km2": "382565", "precision": "10m", "pricing_docs": "For more information, visit https://www.mapbox.com/pricing/#tilesets"}\n'
     runner = CliRunner()
     validated_result = runner.invoke(
```

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_jobs.py` & `mapbox-tilesets-1.9.3/tests/test_cli_jobs.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_list.py` & `mapbox-tilesets-1.9.3/tests/test_cli_list.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_publish.py` & `mapbox-tilesets-1.9.3/tests/test_cli_publish.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_sources.py` & `mapbox-tilesets-1.9.3/tests/test_cli_sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     add_source,
     upload_source,
     view_source,
     delete_source,
     validate_source,
     list_sources,
 )
+from utils import clean_runner_output
 
 
 @pytest.mark.usefixtures("token_environ")
 @mock.patch("mapbox_tilesets.scripts.cli.MultipartEncoder")
 @mock.patch("mapbox_tilesets.scripts.cli.MultipartEncoderMonitor")
 @mock.patch("requests.Session.post")
 def test_cli_add_source(
@@ -69,15 +70,15 @@
     runner = CliRunner()
     validated_result = runner.invoke(
         add_source, ["test-user-wrong", "hello-world", "tests/fixtures/valid.ldgeojson"]
     )
     assert validated_result.exit_code == 1
 
     assert (
-        str(validated_result.exception)
+        clean_runner_output(validated_result.output)
         == "Token username wrong-user does not match username test-user-wrong"
     )
 
 
 def test_cli_add_source_no_token():
     if "MAPBOX_ACCESS_TOKEN" in os.environ:
         del os.environ["MAPBOX_ACCESS_TOKEN"]
@@ -87,15 +88,15 @@
     runner = CliRunner()
     unauthenticated_result = runner.invoke(
         add_source, ["test-user", "hello-world", "tests/fixtures/valid.ldgeojson"]
     )
     assert unauthenticated_result.exit_code == 1
 
     assert (
-        str(unauthenticated_result.exception)
+        clean_runner_output(unauthenticated_result.output)
         == """No access token provided. Please set the MAPBOX_ACCESS_TOKEN environment variable or use the --token flag."""
     )
 
 
 @pytest.mark.usefixtures("token_environ")
 @mock.patch("requests.Session.post")
 def test_cli_add_source_no_validation(mock_request_post, MockResponse):
@@ -112,15 +113,15 @@
             "tests/fixtures/invalid.ldgeojson",
             "--no-validation",
         ],
     )
     assert no_validation_result.exit_code == 1
 
     assert (
-        no_validation_result.exception.message
+        clean_runner_output(no_validation_result.output)
         == '{"message": "Invalid file format. Only GeoJSON features are allowed."}'
     )
 
 
 @pytest.mark.usefixtures("token_environ")
 @mock.patch("mapbox_tilesets.scripts.cli.MultipartEncoder")
 @mock.patch("mapbox_tilesets.scripts.cli.MultipartEncoderMonitor")
@@ -250,15 +251,15 @@
             "populated-places-source",
             "tests/fixtures/invalid-polygon.ldgeojson",
         ],
     )
     assert validated_result.exit_code == 1
 
     assert (
-        str(validated_result.exception)
+        clean_runner_output(validated_result.output)
         == "Error in feature number 0: Each linear ring must end where it started"
     )
 
 
 @pytest.mark.usefixtures("token_environ")
 def validate_source_id(self):
     self.assertRaises(
```

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_status.py` & `mapbox-tilesets-1.9.3/tests/test_cli_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import pytest
 
 from click.testing import CliRunner
 from unittest import mock
 
 from mapbox_tilesets.scripts.cli import status
-from mapbox_tilesets.errors import TilesetsError
+from utils import clean_runner_output
 
 
 @pytest.mark.usefixtures("token_environ")
 @mock.patch("requests.Session.get")
 def test_cli_status(mock_request_get, MockResponse):
     runner = CliRunner()
 
@@ -59,9 +59,9 @@
     message = {"message": "test.id has no jobs."}
     mock_request_get.return_value = MockResponse(message, 404)
     result = runner.invoke(status, ["test.id"])
     mock_request_get.assert_called_with(
         "https://api.mapbox.com/tilesets/v1/test.id/jobs?limit=1&access_token=pk.eyJ1IjoidGVzdC11c2VyIn0K"
     )
     assert result.exit_code == 1
-    assert isinstance(result.exception, TilesetsError)
-    assert result.exception.message == '{"message": "test.id has no jobs."}'
+    assert isinstance(result.exception, SystemExit)
+    assert clean_runner_output(result.output) == '{"message": "test.id has no jobs."}'
```

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_tilejson.py` & `mapbox-tilesets-1.9.3/tests/test_cli_tilejson.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import pytest
 from unittest import mock
 from click.testing import CliRunner
 from mapbox_tilesets.scripts.cli import tilejson
-from mapbox_tilesets.errors import TilesetsError, TilesetNameError
+from utils import clean_runner_output
 
 
 class MockResponse:
     def __init__(self, mock_json, status_code):
         self.text = json.dumps(mock_json)
         self._json = mock_json
         self.status_code = status_code
@@ -90,19 +90,19 @@
     # sends expected request
     mock_request_get.return_value = MockResponse({"message": "uh oh"}, 422)
     result = runner.invoke(tilejson, ["test.id,test.another"])
     mock_request_get.assert_called_with(
         "https://api.mapbox.com/v4/test.id,test.another.json?access_token=pk.eyJ1IjoidGVzdC11c2VyIn0K"
     )
     assert result.exit_code == 1
-    assert isinstance(result.exception, TilesetsError)
+    assert isinstance(result.exception, SystemExit)
 
 
 @pytest.mark.usefixtures("token_environ")
 def test_cli_tilejson_invalid_tileset_id():
     runner = CliRunner()
 
     # sends expected request
     result = runner.invoke(tilejson, ["invalid@@id"])
     assert result.exit_code == 1
-    assert isinstance(result.exception, TilesetNameError)
-    assert "invalid@@id" in str(result.exception)
+    assert isinstance(result.exception, SystemExit)
+    assert clean_runner_output(result.output) == "Invalid Tileset ID"
```

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_update.py` & `mapbox-tilesets-1.9.3/tests/test_cli_update.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_update_recipe.py` & `mapbox-tilesets-1.9.3/tests/test_cli_update_recipe.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_validate_recipe.py` & `mapbox-tilesets-1.9.3/tests/test_cli_validate_recipe.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_cli_view_recipe.py` & `mapbox-tilesets-1.9.3/tests/test_cli_view_recipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import pytest
 
 from click.testing import CliRunner
 from unittest import mock
 
 from mapbox_tilesets.scripts.cli import view_recipe
+from utils import clean_runner_output
 
 
 @pytest.mark.usefixtures("token_environ")
 @mock.patch("requests.Session.get")
 def test_cli_view_recipe(mock_request_get, MockResponse):
     runner = CliRunner()
 
@@ -46,9 +47,8 @@
     # sends expected request
     mock_request_get.return_value = MockResponse("not found", status_code=404)
     result = runner.invoke(view_recipe, ["test.id"])
     mock_request_get.assert_called_with(
         "https://api.mapbox.com/tilesets/v1/test.id/recipe?access_token=pk.eyJ1IjoidGVzdC11c2VyIn0K"
     )
     assert result.exit_code == 1
-
-    assert result.exception.message == '"not found"'
+    assert clean_runner_output(result.output) == '"not found"'
```

### Comparing `mapbox-tilesets-1.9.0/tests/test_file_validator.py` & `mapbox-tilesets-1.9.3/tests/test_file_validator.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.9.0/tests/test_utils.py` & `mapbox-tilesets-1.9.3/tests/test_utils.py`

 * *Files identical despite different names*

