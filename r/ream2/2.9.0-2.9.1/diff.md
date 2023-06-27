# Comparing `tmp/ream2-2.9.0.tar.gz` & `tmp/ream2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-2.9.0.tar", max compression
+gzip compressed data, was "ream2-2.9.1.tar", max compression
```

## Comparing `ream2-2.9.0.tar` & `ream2-2.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-06-20 22:05:30.913429 ream2-2.9.0/LICENSE
--rw-r--r--   0        0        0     5267 2023-06-20 22:05:30.913429 ream2-2.9.0/README.md
--rw-r--r--   0        0        0      763 2023-06-20 22:05:30.913429 ream2-2.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/__init__.py
--rw-r--r--   0        0        0    14886 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/actor_graph.py
--rw-r--r--   0        0        0     2197 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/actor_version.py
--rw-r--r--   0        0        0        0 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/actors/__init__.py
--rw-r--r--   0        0        0     4115 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/actors/base.py
--rw-r--r--   0        0        0     1155 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/actors/dsid.py
--rw-r--r--   0        0        0     1332 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/actors/enum.py
--rw-r--r--   0        0        0      363 2023-06-20 22:05:30.913429 ream2-2.9.0/ream/actors/interface.py
--rw-r--r--   0        0        0    37817 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/cache_helper.py
--rw-r--r--   0        0        0     3393 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/cli_helper.py
--rw-r--r--   0        0        0    34210 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/data_model_helper.py
--rw-r--r--   0        0        0    14434 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/dataset_helper.py
--rw-r--r--   0        0        0     9838 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/fs.py
--rw-r--r--   0        0        0     6636 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/helper.py
--rw-r--r--   0        0        0     5684 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/params_helper.py
--rw-r--r--   0        0        0     1119 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/prelude.py
--rw-r--r--   0        0        0     2248 2023-06-20 22:05:30.917430 ream2-2.9.0/ream/workspace.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 17:42:00.464939 ream2-2.9.1/LICENSE
+-rw-r--r--   0        0        0     5267 2023-06-24 17:42:00.464939 ream2-2.9.1/README.md
+-rw-r--r--   0        0        0      763 2023-06-24 17:42:00.464939 ream2-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/__init__.py
+-rw-r--r--   0        0        0    14886 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/actor_graph.py
+-rw-r--r--   0        0        0     2197 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/actors/__init__.py
+-rw-r--r--   0        0        0     4115 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/actors/base.py
+-rw-r--r--   0        0        0     1155 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/actors/dsid.py
+-rw-r--r--   0        0        0     1332 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/actors/enum.py
+-rw-r--r--   0        0        0      363 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/actors/interface.py
+-rw-r--r--   0        0        0    39212 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/cli_helper.py
+-rw-r--r--   0        0        0    34210 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/data_model_helper.py
+-rw-r--r--   0        0        0    14434 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/dataset_helper.py
+-rw-r--r--   0        0        0     9838 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/fs.py
+-rw-r--r--   0        0        0     6636 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/helper.py
+-rw-r--r--   0        0        0     6182 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/params_helper.py
+-rw-r--r--   0        0        0     1119 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/prelude.py
+-rw-r--r--   0        0        0     2248 2023-06-24 17:42:00.464939 ream2-2.9.1/ream/workspace.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.9.1/PKG-INFO
```

### Comparing `ream2-2.9.0/LICENSE` & `ream2-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/README.md` & `ream2-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/pyproject.toml` & `ream2-2.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ream2"
-version = "2.9.0"
+version = "2.9.1"
 description = "An actor architecture for research software"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/ream"
 repository = "https://github.com/binh-vu/ream"
 packages = [
```

### Comparing `ream2-2.9.0/ream/actor_graph.py` & `ream2-2.9.1/ream/actor_graph.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/actor_state.py` & `ream2-2.9.1/ream/actor_state.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/actor_version.py` & `ream2-2.9.1/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/actors/base.py` & `ream2-2.9.1/ream/actors/base.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/actors/dsid.py` & `ream2-2.9.1/ream/actors/dsid.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/actors/enum.py` & `ream2-2.9.1/ream/actors/enum.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/cache_helper.py` & `ream2-2.9.1/ream/cache_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 from __future__ import annotations
 
 import bz2
 import functools
 import gzip
 import pickle
+from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from contextlib import contextmanager
 from inspect import Parameter, signature
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    Generic,
     Iterable,
     Literal,
     Optional,
     Protocol,
     Sequence,
     Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
     get_type_hints,
 )
 
+import orjson
 import serde.prelude as serde
 from hugedict.misc import Chain2, identity
 from hugedict.sqlitedict import SqliteDict, SqliteDictFieldType
 from loguru import logger
-from ream.fs import FS
-from ream.helper import orjson_dumps
 from serde.helper import AVAILABLE_COMPRESSIONS, JsonSerde
 from timer import Timer
 from typing_extensions import Self
 
+from ream.fs import FS
+from ream.helper import orjson_dumps
+
 try:
     import lz4.frame as lz4_frame  # type: ignore
 except ImportError:
     lz4_frame = None
 
 NoneType = type(None)
 # arguments are (self, *args, **kwargs)
@@ -278,18 +282,21 @@
 class Cache:
     jl = JLSerdeCache
     pickle = PickleSerdeCache
     cls = ClsSerdeCache
 
     @staticmethod
     @contextmanager
-    def autoclear_mem_cache(obj: object, cache_attr: str = "_cache"):
+    def autoclear_mem_cache(
+        objs: Union[object, list[object]], cache_attr: str = "_cache"
+    ):
         yield None
-        if hasattr(obj, cache_attr):
-            getattr(obj, cache_attr).clear()
+        for obj in objs if isinstance(objs, list) else [objs]:
+            if hasattr(obj, cache_attr):
+                getattr(obj, cache_attr).clear()
 
     @staticmethod
     def mem(
         cache_args: Optional[list[str]] = None,
         cache_self_args: Optional[Callable[..., dict]] = None,
         cache_key: Optional[CacheKeyFn | Callable[..., tuple]] = None,
         cache_attr: str = "_cache",
@@ -885,14 +892,51 @@
 
         self.disable = disable
 
     def get_working_fs(self) -> FS:
         return self.workdir
 
 
+class CacheableFn(ABC, Cacheable):
+    """This utility provides a way to break a giantic function into smaller pieces that can be cached individually."""
+
+    def __init__(
+        self, use_args: list[str], workdir: Union[FS, Path], disable: bool = False
+    ):
+        super().__init__(workdir, disable)
+        self.use_args = use_args
+
+    @staticmethod
+    def get_cache_key(slf: CacheableFn, args: F) -> bytes:
+        return orjson.dumps(
+            {attr: getattr(args, attr) for attr in slf.get_use_args()},
+            option=orjson.OPT_SORT_KEYS | orjson.OPT_SERIALIZE_DATACLASS,
+        )
+
+    @functools.lru_cache()
+    def get_use_args(self) -> set[str]:
+        cache_args = set()
+        for fn in self.get_dependable_fns():
+            cache_args.update(fn.get_use_args())
+        return cache_args
+
+    @functools.lru_cache()
+    def get_dependable_fns(self) -> list[CacheableFn]:
+        fns = []
+        for obj in self.__dict__.values():
+            if isinstance(obj, CacheableFn):
+                fns.append(obj)
+        return fns
+
+    @abstractmethod
+    def __call__(self, args):
+        """This is where to put the function body. To cache it, wraps it with @Cache.<X> decorators"""
+        ...
+
+
 class SaveLoadProtocol(Protocol):
     def save(self, file: Path) -> None:
         ...
 
     @classmethod
     def load(cls, file: Path) -> Self:
         ...
```

### Comparing `ream2-2.9.0/ream/cli_helper.py` & `ream2-2.9.1/ream/cli_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/data_model_helper.py` & `ream2-2.9.1/ream/data_model_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/dataset_helper.py` & `ream2-2.9.1/ream/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/fs.py` & `ream2-2.9.1/ream/fs.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/helper.py` & `ream2-2.9.1/ream/helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/params_helper.py` & `ream2-2.9.1/ream/params_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from copy import deepcopy
+from functools import partial
 from dataclasses import Field, asdict, dataclass, fields, is_dataclass, replace
 from typing import Any, Dict, List, Type, Union
 
 DataClassInstance = Any
 
 
 @dataclass
@@ -53,14 +54,25 @@
             setattr(other, getattr(self, field.name), None)
         return other
 
     def get_method_class(self, method_field: Field) -> Type:
         method = getattr(self, method_field.name)
         return method_field.metadata["variants"][method]
 
+    def get_method_constructor(self, method_field: Field, **kwargs):
+        method = getattr(self, method_field.name)
+        if (
+            "variant_constructors" in method_field.metadata
+            and method in method_field.metadata["variant_constructors"]
+        ):
+            return partial(
+                method_field.metadata["variant_constructors"][method], **kwargs
+            )
+        return partial(self.get_method_class(method_field), **kwargs)
+
     def get_method_params(self, method_field: Field) -> DataClassInstance:
         method = getattr(self, method_field.name)
         return getattr(self, method)
 
     def get_method_fields(self) -> list[Field]:
         if not hasattr(self, "__method_fields"):
             method_fields = []
```

### Comparing `ream2-2.9.0/ream/prelude.py` & `ream2-2.9.1/ream/prelude.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/ream/workspace.py` & `ream2-2.9.1/ream/workspace.py`

 * *Files identical despite different names*

### Comparing `ream2-2.9.0/PKG-INFO` & `ream2-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ream2
-Version: 2.9.0
+Version: 2.9.1
 Summary: An actor architecture for research software
 Home-page: https://github.com/binh-vu/ream
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

