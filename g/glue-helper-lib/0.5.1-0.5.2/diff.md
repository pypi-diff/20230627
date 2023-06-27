# Comparing `tmp/glue_helper_lib-0.5.1.tar.gz` & `tmp/glue_helper_lib-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_helper_lib-0.5.1.tar", max compression
+gzip compressed data, was "glue_helper_lib-0.5.2.tar", max compression
```

## Comparing `glue_helper_lib-0.5.1.tar` & `glue_helper_lib-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.5.1/LICENSE
--rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.5.1/glue_helper_lib/__init__.py
--rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.5.1/glue_helper_lib/arguments.py
--rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.5.1/glue_helper_lib/hudi/__init__.py
--rw-r--r--   0        0        0     9098 2023-06-27 07:55:34.303614 glue_helper_lib-0.5.1/glue_helper_lib/hudi/config.py
--rw-r--r--   0        0        0     1148 2023-05-02 12:40:59.679248 glue_helper_lib-0.5.1/glue_helper_lib/hudi/session.py
--rw-r--r--   0        0        0     2037 2023-06-27 08:07:48.823617 glue_helper_lib-0.5.1/glue_helper_lib/hudi/table.py
--rw-r--r--   0        0        0     1163 2023-05-03 09:40:20.828320 glue_helper_lib-0.5.1/glue_helper_lib/logging.py
--rw-r--r--   0        0        0      714 2023-06-17 15:39:16.309191 glue_helper_lib-0.5.1/glue_helper_lib/session.py
--rw-r--r--   0        0        0     1562 2023-06-27 07:40:10.813610 glue_helper_lib-0.5.1/glue_helper_lib/table.py
--rw-r--r--   0        0        0      711 2023-06-27 08:09:51.553618 glue_helper_lib-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.5.2/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.5.2/glue_helper_lib/__init__.py
+-rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.5.2/glue_helper_lib/arguments.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.5.2/glue_helper_lib/hudi/__init__.py
+-rw-r--r--   0        0        0     9098 2023-06-27 07:55:34.303614 glue_helper_lib-0.5.2/glue_helper_lib/hudi/config.py
+-rw-r--r--   0        0        0     1148 2023-05-02 12:40:59.679248 glue_helper_lib-0.5.2/glue_helper_lib/hudi/session.py
+-rw-r--r--   0        0        0     2334 2023-06-27 11:54:34.233678 glue_helper_lib-0.5.2/glue_helper_lib/hudi/table.py
+-rw-r--r--   0        0        0     1163 2023-05-03 09:40:20.828320 glue_helper_lib-0.5.2/glue_helper_lib/logging.py
+-rw-r--r--   0        0        0      714 2023-06-17 15:39:16.309191 glue_helper_lib-0.5.2/glue_helper_lib/session.py
+-rw-r--r--   0        0        0     1562 2023-06-27 07:40:10.813610 glue_helper_lib-0.5.2/glue_helper_lib/table.py
+-rw-r--r--   0        0        0      711 2023-06-27 11:55:55.963679 glue_helper_lib-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.5.2/PKG-INFO
```

### Comparing `glue_helper_lib-0.5.1/LICENSE` & `glue_helper_lib-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.1/glue_helper_lib/arguments.py` & `glue_helper_lib-0.5.2/glue_helper_lib/arguments.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.1/glue_helper_lib/hudi/config.py` & `glue_helper_lib-0.5.2/glue_helper_lib/hudi/config.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.1/glue_helper_lib/hudi/session.py` & `glue_helper_lib-0.5.2/glue_helper_lib/hudi/session.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.1/glue_helper_lib/hudi/table.py` & `glue_helper_lib-0.5.2/glue_helper_lib/hudi/table.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 import pyspark.sql
 import enum
 
 
 @dataclasses.dataclass
 class Partitioning:
-    partition_column: typing.Optional[str]
+    partition_column: str
     datetime: typing.Optional[config.DatetimePartitioning]
 
 
 class WriteMode(enum.Enum):
     OVERWRITE = "overwrite"
     UPSERT = "upsert"
 
@@ -20,38 +20,47 @@
 @dataclasses.dataclass
 class WriteHudiTableArguments:
     catalog: table.GlueCatalogArguments
     index_type: config.IndexType
     table_type: config.TableType
     record_key_colums: typing.List[str]
     precombine_column: str
-    partitioning: Partitioning
+    partitioning: typing.Optional[Partitioning]
     write_mode: WriteMode
 
 
 class HudiGlueTable:
     _write_mode_to_mode_string = {
         WriteMode.OVERWRITE: "overwrite",
         WriteMode.UPSERT: "append",
     }
 
     def __init__(self, storage_location: table.StorageLocation) -> None:
         self._storage_location = storage_location
 
     def _get_hudi_config(self, write_args: WriteHudiTableArguments):
+        if not write_args.partitioning:
+            datetime_partitioning = None
+            partition_key_column_name = None
+        else:
+            datetime_partitioning = write_args.partitioning.datetime
+            partition_key_column_name = (
+                write_args.partitioning.partition_column
+            )
+
         return config.get_hudi_options(
             database_name=write_args.catalog.database,
             table_name=write_args.catalog.table,
             hudi_table_path=str(self._storage_location),
             table_type=write_args.table_type,
-            datetime_partitioning=write_args.partitioning.datetime,
+            datetime_partitioning=datetime_partitioning,
             index_type=write_args.index_type,
             record_key_columns=write_args.record_key_colums,
             precombine_column_name=write_args.precombine_column,
-            partition_key_column_name=write_args.partitioning.partition_column,
+            partition_key_column_name=partition_key_column_name,
         )
 
     def write(
         self, df: pyspark.sql.DataFrame, write_args: WriteHudiTableArguments
     ):
         df.write.format("hudi").options(
             **self._get_hudi_config(write_args)
```

### Comparing `glue_helper_lib-0.5.1/glue_helper_lib/logging.py` & `glue_helper_lib-0.5.2/glue_helper_lib/logging.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.1/glue_helper_lib/session.py` & `glue_helper_lib-0.5.2/glue_helper_lib/session.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.1/glue_helper_lib/table.py` & `glue_helper_lib-0.5.2/glue_helper_lib/table.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.1/pyproject.toml` & `glue_helper_lib-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-helper-lib"
-version = "0.5.1"
+version = "0.5.2"
 description = "A library containing multiple helper and utility functionalities for AWS Glue"
 authors = ["Martijn Sturm <martijn.sturm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "glue_helper_lib" }]
 
 [tool.poetry.dependencies]
```

### Comparing `glue_helper_lib-0.5.1/PKG-INFO` & `glue_helper_lib-0.5.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-helper-lib
-Version: 0.5.1
+Version: 0.5.2
 Summary: A library containing multiple helper and utility functionalities for AWS Glue
 License: MIT
 Author: Martijn Sturm
 Author-email: martijn.sturm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

