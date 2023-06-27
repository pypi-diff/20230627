# Comparing `tmp/bqemulatormanager-0.2.0.tar.gz` & `tmp/bqemulatormanager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqemulatormanager-0.2.0.tar", max compression
+gzip compressed data, was "bqemulatormanager-0.2.1.tar", max compression
```

## Comparing `bqemulatormanager-0.2.0.tar` & `bqemulatormanager-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1321 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/README.md
--rw-r--r--   0        0        0      145 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/bqemulatormanager/__init__.py
--rw-r--r--   0        0        0     1456 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/bqemulatormanager/emulator.py
--rw-r--r--   0        0        0     3484 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/bqemulatormanager/manager.py
--rw-r--r--   0        0        0     2878 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/bqemulatormanager/schema.py
--rw-r--r--   0        0        0     1178 2023-06-19 07:58:37.576342 bqemulatormanager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 bqemulatormanager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1327 2023-06-27 04:04:46.961096 bqemulatormanager-0.2.1/README.md
+-rw-r--r--   0        0        0      145 2023-06-27 04:04:46.961096 bqemulatormanager-0.2.1/bqemulatormanager/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-27 04:04:46.961096 bqemulatormanager-0.2.1/bqemulatormanager/emulator.py
+-rw-r--r--   0        0        0     3489 2023-06-27 04:04:46.961096 bqemulatormanager-0.2.1/bqemulatormanager/manager.py
+-rw-r--r--   0        0        0     2878 2023-06-27 04:04:46.961096 bqemulatormanager-0.2.1/bqemulatormanager/schema.py
+-rw-r--r--   0        0        0     1178 2023-06-27 04:05:05.533276 bqemulatormanager-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 bqemulatormanager-0.2.1/PKG-INFO
```

### Comparing `bqemulatormanager-0.2.0/README.md` & `bqemulatormanager-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     df = manager.query(sql)
 print(df)
 ```
 
 unit test example is [here](https://github.com/gyuta/bqemulatormanager/blob/main/examples/testing.py).
 
 ### automatically detect schema
-When called `Manager.load`, `SchemaManager` search correspond table schema from `schema_path` (default is `master_schema.yaml`).
+When called `Manager.load`, `SchemaManager` search correspond table schema from `schema_path` (default is `bqem_master_schema.yaml`).
 
-If schema definition canot be found, `SchemaManager` request it from BigQuery in production environmant and update master schema file.
+If schema definition cannot be found, `SchemaManager` request it from BigQuery in production environment and update master schema file.
```

### Comparing `bqemulatormanager-0.2.0/bqemulatormanager/emulator.py` & `bqemulatormanager-0.2.1/bqemulatormanager/emulator.py`

 * *Files identical despite different names*

### Comparing `bqemulatormanager-0.2.0/bqemulatormanager/manager.py` & `bqemulatormanager-0.2.1/bqemulatormanager/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class Manager:
     def __init__(
         self,
         project: str = "test",
         port: int = 9050,
         grpc_port: int = 9060,
-        schema_path: str = "master_schema.yaml",
+        schema_path: str = "bqem_master_schema.yaml",
         launch_emulator: bool = True,
         debug_mode: bool = False,
         max_pool: int = 20,
     ):
         original_port = port
         grpc_original_port = grpc_port
         for i in range(max_pool):
```

### Comparing `bqemulatormanager-0.2.0/bqemulatormanager/schema.py` & `bqemulatormanager-0.2.1/bqemulatormanager/schema.py`

 * *Files identical despite different names*

### Comparing `bqemulatormanager-0.2.0/pyproject.toml` & `bqemulatormanager-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bqemulatormanager"
-version = "0.2.0"  # using poetry-dynamic-versioning
+version = "0.2.1"  # using poetry-dynamic-versioning
 description = "bqemulatormanager is a wrapper of bigquery-emulator which provides us BigQuery mock working in local machine."
 authors = ["gyuta <kuroshiba0408@gmail.com>", "M3, Inc."]
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
```

### Comparing `bqemulatormanager-0.2.0/PKG-INFO` & `bqemulatormanager-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqemulatormanager
-Version: 0.2.0
+Version: 0.2.1
 Summary: bqemulatormanager is a wrapper of bigquery-emulator which provides us BigQuery mock working in local machine.
 Author: gyuta
 Author-email: kuroshiba0408@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -55,10 +55,10 @@
     df = manager.query(sql)
 print(df)
 ```
 
 unit test example is [here](https://github.com/gyuta/bqemulatormanager/blob/main/examples/testing.py).
 
 ### automatically detect schema
-When called `Manager.load`, `SchemaManager` search correspond table schema from `schema_path` (default is `master_schema.yaml`).
+When called `Manager.load`, `SchemaManager` search correspond table schema from `schema_path` (default is `bqem_master_schema.yaml`).
 
-If schema definition canot be found, `SchemaManager` request it from BigQuery in production environmant and update master schema file.
+If schema definition cannot be found, `SchemaManager` request it from BigQuery in production environment and update master schema file.
```

