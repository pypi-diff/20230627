# Comparing `tmp/glue_helper_lib-0.4.0.tar.gz` & `tmp/glue_helper_lib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_helper_lib-0.4.0.tar", max compression
+gzip compressed data, was "glue_helper_lib-0.5.0.tar", max compression
```

## Comparing `glue_helper_lib-0.4.0.tar` & `glue_helper_lib-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.4.0/LICENSE
--rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.4.0/glue_helper_lib/__init__.py
--rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.4.0/glue_helper_lib/arguments.py
--rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.4.0/glue_helper_lib/hudi/__init__.py
--rw-r--r--   0        0        0     8811 2023-04-30 14:55:32.831653 glue_helper_lib-0.4.0/glue_helper_lib/hudi/config.py
--rw-r--r--   0        0        0     1148 2023-05-02 12:40:59.679248 glue_helper_lib-0.4.0/glue_helper_lib/hudi/session.py
--rw-r--r--   0        0        0     2005 2023-06-08 15:16:47.875481 glue_helper_lib-0.4.0/glue_helper_lib/hudi/table.py
--rw-r--r--   0        0        0     1163 2023-05-03 09:40:20.828320 glue_helper_lib-0.4.0/glue_helper_lib/logging.py
--rw-r--r--   0        0        0      700 2023-05-02 12:38:54.926123 glue_helper_lib-0.4.0/glue_helper_lib/session.py
--rw-r--r--   0        0        0     1562 2023-05-02 15:07:44.250302 glue_helper_lib-0.4.0/glue_helper_lib/table.py
--rw-r--r--   0        0        0      711 2023-06-08 15:51:53.095481 glue_helper_lib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.5.0/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.5.0/glue_helper_lib/__init__.py
+-rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.5.0/glue_helper_lib/arguments.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.5.0/glue_helper_lib/hudi/__init__.py
+-rw-r--r--   0        0        0     9098 2023-06-27 07:55:34.303614 glue_helper_lib-0.5.0/glue_helper_lib/hudi/config.py
+-rw-r--r--   0        0        0     1148 2023-05-02 12:40:59.679248 glue_helper_lib-0.5.0/glue_helper_lib/hudi/session.py
+-rw-r--r--   0        0        0     2005 2023-06-08 15:16:47.875481 glue_helper_lib-0.5.0/glue_helper_lib/hudi/table.py
+-rw-r--r--   0        0        0     1163 2023-05-03 09:40:20.828320 glue_helper_lib-0.5.0/glue_helper_lib/logging.py
+-rw-r--r--   0        0        0      714 2023-06-17 15:39:16.309191 glue_helper_lib-0.5.0/glue_helper_lib/session.py
+-rw-r--r--   0        0        0     1562 2023-06-27 07:40:10.813610 glue_helper_lib-0.5.0/glue_helper_lib/table.py
+-rw-r--r--   0        0        0      711 2023-06-27 07:56:01.843614 glue_helper_lib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.5.0/PKG-INFO
```

### Comparing `glue_helper_lib-0.4.0/LICENSE` & `glue_helper_lib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.4.0/glue_helper_lib/arguments.py` & `glue_helper_lib-0.5.0/glue_helper_lib/arguments.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.4.0/glue_helper_lib/hudi/config.py` & `glue_helper_lib-0.5.0/glue_helper_lib/hudi/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import enum
 import typing
+from dataclasses import dataclass
 
 
 class TableType(enum.Enum):
     COPY_ON_WRITE = "COPY_ON_WRITE"
     MERGE_ON_READ = "MERGE_ON_READ"
 
 
@@ -79,32 +80,37 @@
             "partitioning:",
             partitioning,
             "partitioned on datetime:",
             partitioned_on_datetime,
         )
 
 
-OUTPUT_DATE_FORMAT = "yyyyMMdd"
-ISO_INPUT_FORMAT = "yyyy-MM-dd'T'HH:mm:ss.SSSZ"
-
-
 def get_keygenerator_class_name(key_generator: KeyGenerator):
     return f"org.apache.hudi.keygen.{key_generator.value}"
 
 
-def get_additional_options_for_datetime_keygen(partitioned_on_datetime: bool):
+@dataclass
+class DatetimePartitioning:
+    input_date_format: str = "yyyy-MM-dd'T'HH:mm:ss.SSSZ"
+    timezone: str = "UTC"
+    output_date_format: str = "yyyyMMdd"
+
+
+def get_additional_options_for_datetime_keygen(
+    datetime_partitioning: typing.Optional[DatetimePartitioning],
+):
     # https://hudi.apache.org/blog/2021/02/13/hudi-key-generators/#timestampbasedkeygenerator
-    if partitioned_on_datetime:
+    if datetime_partitioning:
         return {
             "hoodie.deltastreamer.keygen.timebased.timestamp.type": "DATE_STRING",
-            "hoodie.deltastreamer.keygen.timebased.input.dateformat": ISO_INPUT_FORMAT,
+            "hoodie.deltastreamer.keygen.timebased.input.dateformat": datetime_partitioning.input_date_format,
             "hoodie.deltastreamer.keygen.timebased.input.dateformat.list.delimiter.regex": "",  # noqa: E501
             "hoodie.deltastreamer.keygen.timebased.input.timezone": "",
-            "hoodie.deltastreamer.keygen.timebased.output.dateformat": OUTPUT_DATE_FORMAT,  # noqa: E501
-            "hoodie.deltastreamer.keygen.timebased.timezone": "UTC",
+            "hoodie.deltastreamer.keygen.timebased.output.dateformat": datetime_partitioning.output_date_format,  # noqa: E501
+            "hoodie.deltastreamer.keygen.timebased.timezone": datetime_partitioning.timezone,
         }
     else:
         return {}
 
 
 def parse_record_key_columns(columns: typing.List[str]):
     if not columns:
@@ -214,27 +220,27 @@
 }
 
 
 def get_hudi_options(
     database_name: str,
     table_name: str,
     table_type: TableType,
-    partitioned_on_datetime: bool,
+    datetime_partitioning: typing.Optional[DatetimePartitioning],
     index_type: IndexType,
     record_key_columns: typing.List[str],
     precombine_column_name: str,
     partition_key_column_name: typing.Optional[str],
     hudi_table_path: str,
 ):
     if not partition_key_column_name:
         partition_key_column_name = ""
     key_generator_class = get_keygenerator_class(
         len(record_key_columns),
         True if partition_key_column_name else False,
-        partitioned_on_datetime,
+        True if datetime_partitioning else False,
     )
     options: typing.Dict[str, str] = {
         **fixed_hudi_options,
         "hoodie.table.name": table_name,
         "hoodie.datasource.write.table_type_opt_key": get_table_type_opt_key_value(
             table_type
         ),
@@ -248,14 +254,14 @@
         "hoodie.datasource.hive_sync.enable": "true",
         "hoodie.datasource.hive_sync.database": database_name,
         "hoodie.datasource.hive_sync.table": table_name,
         "path": hudi_table_path,
         **get_index_type_option(index_type),
         **get_partitioning_options(
             partition_key_column_name,
-            partitioned_on_datetime,
+            True if datetime_partitioning else False,
             key_generator_class,
         ),
-        **get_additional_options_for_datetime_keygen(partitioned_on_datetime),
+        **get_additional_options_for_datetime_keygen(datetime_partitioning),
     }
 
     return options
```

### Comparing `glue_helper_lib-0.4.0/glue_helper_lib/hudi/session.py` & `glue_helper_lib-0.5.0/glue_helper_lib/hudi/session.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.4.0/glue_helper_lib/hudi/table.py` & `glue_helper_lib-0.5.0/glue_helper_lib/hudi/table.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.4.0/glue_helper_lib/logging.py` & `glue_helper_lib-0.5.0/glue_helper_lib/logging.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.4.0/glue_helper_lib/session.py` & `glue_helper_lib-0.5.0/glue_helper_lib/session.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,14 @@
         ...
 
 
 class SparkGlueSession:
     def __init__(self) -> None:
         self._spark_context = SparkContext()
         self._glue_context = GlueContext(self._spark_context)
-        self._spark_session = self._glue_context.spark_session
+        self._spark_session: SparkSession = self._glue_context.spark_session
 
     def get_spark_session(self):
         return self._spark_session
 
     def get_glue_context(self):
         return self._glue_context
```

### Comparing `glue_helper_lib-0.4.0/glue_helper_lib/table.py` & `glue_helper_lib-0.5.0/glue_helper_lib/table.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.4.0/pyproject.toml` & `glue_helper_lib-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-helper-lib"
-version = "0.4.0"
+version = "0.5.0"
 description = "A library containing multiple helper and utility functionalities for AWS Glue"
 authors = ["Martijn Sturm <martijn.sturm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "glue_helper_lib" }]
 
 [tool.poetry.dependencies]
```

### Comparing `glue_helper_lib-0.4.0/PKG-INFO` & `glue_helper_lib-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-helper-lib
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library containing multiple helper and utility functionalities for AWS Glue
 License: MIT
 Author: Martijn Sturm
 Author-email: martijn.sturm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

