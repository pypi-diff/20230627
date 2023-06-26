# Comparing `tmp/vegafusion-1.3.0rc4.tar.gz` & `tmp/vegafusion-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.3.0rc4.tar", last modified: Tue May 30 22:42:34 2023, max compression
+gzip compressed data, was "vegafusion-1.4.0rc1.tar", last modified: Mon Jun 26 19:10:12 2023, max compression
```

## Comparing `vegafusion-1.3.0rc4.tar` & `vegafusion-1.4.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.369663 vegafusion-1.3.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)    13990 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.369663 vegafusion-1.3.0rc4/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-26 19:10:12.569885 vegafusion-1.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/connection/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/local_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.3.0rc4/LICENSE.txt` & `vegafusion-1.4.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/PKG-INFO` & `vegafusion-1.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.3.0rc4
+Version: 1.4.0rc1
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.3.0rc4/README.md` & `vegafusion-1.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/setup.cfg` & `vegafusion-1.4.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.3.0-rc4
+version = 1.4.0-rc1
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -30,14 +30,14 @@
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.3.0-rc4
+	vegafusion-python-embed==1.4.0-rc1
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.3.0rc4/tests/test_conext_manager.py` & `vegafusion-1.4.0rc1/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/tests/test_input_utc.py` & `vegafusion-1.4.0rc1/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/tests/test_pretransform.py` & `vegafusion-1.4.0rc1/tests/test_pretransform.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/tests/test_pretransform_specs.py` & `vegafusion-1.4.0rc1/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/tests/test_row_limit.py` & `vegafusion-1.4.0rc1/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/tests/test_save.py` & `vegafusion-1.4.0rc1/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/tests/test_transformed_data.py` & `vegafusion-1.4.0rc1/tests/test_transformed_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         ("line/step_chart", 68, ["symbol", "date", "price"]),
         ("line/with_cumsum", 52, ["year", "wheat", "cumulative_wheat"]),
         ("line/with_generator", 256, ["x", "sin", "cos", "key", "value"]),
         ("line/with_logarithmic_scale", 15, ["year", "sum_people"]),
         ("line/with_points", 100, ["x", "f(x)"]),
         ("other/beckers_barley_wrapped_facet", 120, ["variety", "site", "median_yield"]),
         ("other/binned_heatmap", 378, ["__count", "bin_maxbins_60_IMDB_Rating_end"]),
+        ("other/boxplot", 19, ["age", "mid_box_people"]),
         ("other/comet_chart", 120, ["variety", "1932", "delta"]),
         ("other/gantt_chart", 3, ["task", "start", "end"]),
         ("other/hexbins", 84, ["month_date", "xFeaturePos", "mean_temp_max"]),
         ("other/isotype_grid", 100, ["id", "row", "col"]),
         ("other/multiple_marks", 560, ["symbol", "date", "price"]),
         ("other/stem_and_leaf", 100, ["samples", "stem", "leaf", "position"]),
         ("other/wilkinson_dot_plot", 21, ["data", "id"]),
```

### Comparing `vegafusion-1.3.0rc4/tests/test_transformer.py` & `vegafusion-1.4.0rc1/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/__init__.py` & `vegafusion-1.4.0rc1/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/compilers.py` & `vegafusion-1.4.0rc1/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/connection/__init__.py` & `vegafusion-1.4.0rc1/vegafusion/connection/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     """
     has_header: bool
     delimeter: str
     file_extension: str
     schema: Optional[pa.Schema]
 
 
+class RegistrationNotSupportedError(RuntimeError):
+    pass
+
+
 class SqlConnection(ABC):
     """
     Python interface for SQL connections
     """
     @classmethod
     def dialect(cls) -> str:
         """
@@ -78,72 +82,72 @@
         Register the provided pandas DataFrame as a table with the provided name
 
         :param name: Table name
         :param df: pandas DataFrame
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
-        raise ValueError("Connection does not support registration of pandas datasets")
+        raise RegistrationNotSupportedError("Connection does not support registration of pandas datasets")
 
     def register_arrow(self, name: str, table: pa.Table, temporary: bool = False):
         """
         Register the provided pyarrow Table as a table with the provided name
         :param name: Table name
         :param table: pyarrow Table
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
-        raise ValueError("Connection does not support registration of arrow datasets")
+        raise RegistrationNotSupportedError("Connection does not support registration of arrow datasets")
 
     def register_json(self, name: str, path: str, temporary: bool = False):
         """
         Register the JSON file at the provided path as a table with the provided name
         :param name: Table name
         :param path: Path to JSON file
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
-        raise ValueError("Connection does not support registration of json datasets")
+        raise RegistrationNotSupportedError("Connection does not support registration of json datasets")
 
     def register_csv(self, name: str, path: str, options: CsvReadOptions, temporary: bool = False):
         """
         Register the CSV file at the provided path as a table with the provided name
         :param name: Table name
         :param path: Path to CSV file
         :param options: CSV options
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
-        raise ValueError("Connection does not support registration of csv datasets")
+        raise RegistrationNotSupportedError("Connection does not support registration of csv datasets")
 
     def register_parquet(self, name: str, path: str, temporary: bool = False):
         """
         Register the Parquet file at the provided path as a table with the provided name
         :param name: Table name
         :param path: Path to parquet file
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
-        raise ValueError("Connection does not support registration of parquet datasets")
+        raise RegistrationNotSupportedError("Connection does not support registration of parquet datasets")
 
     def register_arrow_file(self, name: str, path: str, temporary: bool = False):
         """
         Register the Arrow file at the provided path as a table with the provided name
         :param name: Table name
         :param path: Path to arrow file (aka feather file)
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
-        raise ValueError("Connection does not support registration of arrow file datasets")
+        raise RegistrationNotSupportedError("Connection does not support registration of arrow file datasets")
 
     def unregister(self, name: str):
         """
         Unregister a table (temporary or otherwise) by name
         :param name: Table name
         """
-        raise ValueError("Connection does not support unregistration")
+        raise RegistrationNotSupportedError("Connection does not support unregistration")
 
     def unregister_temporary_tables(self):
         """
         Unregister all dynamically registered tables
         """
-        raise ValueError("Connection does not support unregistering temporary tables")
+        raise RegistrationNotSupportedError("Connection does not support unregistering temporary tables")
```

### Comparing `vegafusion-1.3.0rc4/vegafusion/connection/duckdb.py` & `vegafusion-1.4.0rc1/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/evaluation.py` & `vegafusion-1.4.0rc1/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/local_tz.py` & `vegafusion-1.4.0rc1/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/renderer.py` & `vegafusion-1.4.0rc1/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/runtime.py` & `vegafusion-1.4.0rc1/vegafusion/runtime.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/save.py` & `vegafusion-1.4.0rc1/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/transformer.py` & `vegafusion-1.4.0rc1/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion/utils.py` & `vegafusion-1.4.0rc1/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc4/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.4.0rc1/vegafusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.3.0rc4
+Version: 1.4.0rc1
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.3.0rc4/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.4.0rc1/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

