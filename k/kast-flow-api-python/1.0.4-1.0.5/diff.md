# Comparing `tmp/kast_flow_api_python-1.0.4.tar.gz` & `tmp/kast_flow_api_python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kast_flow_api_python-1.0.4.tar", max compression
+gzip compressed data, was "kast_flow_api_python-1.0.5.tar", max compression
```

## Comparing `kast_flow_api_python-1.0.4.tar` & `kast_flow_api_python-1.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-17 13:00:30.531251 kast_flow_api_python-1.0.4/kast_flow_api/__init__.py
--rw-r--r--   0        0        0     8058 2023-06-17 13:00:30.504251 kast_flow_api_python-1.0.4/kast_flow_api/v1.py
--rw-r--r--   0        0        0      528 2023-06-17 13:00:50.763301 kast_flow_api_python-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-27 08:59:44.985066 kast_flow_api_python-1.0.5/kast_flow_api/__init__.py
+-rw-r--r--   0        0        0     8970 2023-06-27 08:59:44.960066 kast_flow_api_python-1.0.5/kast_flow_api/v1.py
+-rw-r--r--   0        0        0      528 2023-06-27 09:00:05.108127 kast_flow_api_python-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.5/PKG-INFO
```

### Comparing `kast_flow_api_python-1.0.4/kast_flow_api/v1.py` & `kast_flow_api_python-1.0.5/kast_flow_api/v1.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 from enum import StrEnum
 from functools import wraps
 from typing import Any, Callable, Protocol, Self, Tuple, Type, TypeVar, cast
 
 from dacite import Config, from_dict
 
 
+class KastSchemaFileName:
+    @staticmethod
+    def batch(schemaRegistry_path: str, topics: str) -> str:
+        return f"{schemaRegistry_path}/{topics}.avsc"
+
+    @staticmethod
+    def stream(schemaRegistry_path: str, topics: str) -> str:
+        return f"{schemaRegistry_path}_{topics}.avsc"
+
+
 class KastFormat(StrEnum):
     AVRO = "avro"
     JSON = "json"
     CSV = "csv"
     PARQUET = "parquet"
 
     @staticmethod
@@ -45,14 +55,43 @@
     def id(self: Self) -> str:
         ...
 
     @property
     def schema(self: Self) -> Any:
         ...
 
+    @property
+    def engine(self: Self) -> Any:
+        ...
+
+    @classmethod
+    def read(
+        cls: Type[Self], id: str, format: str, path: str, schema: str, **kwargs: Any
+    ) -> "KastDataFrame":
+        ...
+
+    @classmethod
+    def fromDataFrame(
+        cls: Type[Self], df: Any, id: str, parents: list[str] = []
+    ) -> "KastDataFrame":
+        ...
+
+    @classmethod
+    def createDataFrame(
+        cls: Type[Self], df: Any, id: str, schema: str
+    ) -> "KastDataFrame":
+        ...
+
+    def write(self: Self, format: str, topics: str, mode: str, **kwargs: Any) -> None:
+        ...
+
+    @classmethod
+    def emptyDataFrame(cls: Type[Self], id: str) -> "KastDataFrame":
+        ...
+
     def createOrReplaceTempView(self: Self, name: str = "") -> "KastDataFrame":
         ...
 
     def map(self: Self, fn: Any, schema: str | dict[str, Any]) -> "KastDataFrame":
         ...
 
     def show(
@@ -62,21 +101,14 @@
 
     def sql(self: Self, query: str) -> "KastDataFrame":
         ...
 
     def table_sql(self: Self, query: str) -> None:
         ...
 
-    def to_df(self: Self) -> Any:
-        ...
-
-    @property
-    def table_engine(self: Self) -> Any:
-        ...
-
 
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class SideOutValue:
     out: str
     schema: str
 
 
@@ -111,14 +143,15 @@
     def emptyKastDataFrame(self: Self) -> KastDataFrame:
         ...
 
 
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class KastFunction(Protocol):
     id: str
+    registerSchema: bool = False
     outs: KastOuts = field(default_factory=make_outs)
 
     def compute(
         self: Self,
         tool: KastTool,
         tables: list[KastDataFrame],
     ) -> KastDataFrame:
```

### Comparing `kast_flow_api_python-1.0.4/pyproject.toml` & `kast_flow_api_python-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kast-flow-api-python"
-version = "1.0.4"
+version = "1.0.5"
 description = "kast python api unified processing engine"
 authors = ["kast"]
 packages = [
     { include = "kast_flow_api" }
 ]
 
 [tool.poetry.dependencies]
```

