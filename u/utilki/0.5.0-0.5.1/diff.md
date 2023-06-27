# Comparing `tmp/utilki-0.5.0.tar.gz` & `tmp/utilki-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.5.0.tar", max compression
+gzip compressed data, was "utilki-0.5.1.tar", max compression
```

## Comparing `utilki-0.5.0.tar` & `utilki-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-27 13:59:08.321137 utilki-0.5.0/README.md
--rw-r--r--   0        0        0      525 2023-06-27 13:59:08.321137 utilki-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      269 2023-06-27 13:59:08.321137 utilki-0.5.0/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-06-27 13:59:08.321137 utilki-0.5.0/utilki/cli.py
--rw-r--r--   0        0        0     5273 2023-06-27 13:59:08.321137 utilki-0.5.0/utilki/log_utils.py
--rw-r--r--   0        0        0     6939 2023-06-27 13:59:08.321137 utilki-0.5.0/utilki/task_mixin.py
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-27 14:34:10.017912 utilki-0.5.1/README.md
+-rw-r--r--   0        0        0      525 2023-06-27 14:34:10.017912 utilki-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-06-27 14:34:10.017912 utilki-0.5.1/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-06-27 14:34:10.017912 utilki-0.5.1/utilki/cli.py
+-rw-r--r--   0        0        0     5273 2023-06-27 14:34:10.017912 utilki-0.5.1/utilki/log_utils.py
+-rw-r--r--   0        0        0     7325 2023-06-27 14:34:10.017912 utilki-0.5.1/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.5.1/PKG-INFO
```

### Comparing `utilki-0.5.0/README.md` & `utilki-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.5.0/pyproject.toml` & `utilki-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.5.0"
+version = "0.5.1"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.5.0/utilki/cli.py` & `utilki-0.5.1/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.5.0/utilki/log_utils.py` & `utilki-0.5.1/utilki/log_utils.py`

 * *Files identical despite different names*

### Comparing `utilki-0.5.0/utilki/task_mixin.py` & `utilki-0.5.1/utilki/task_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from datetime import datetime
+from datetime import datetime, date
 from dataclasses import Field
 from pydantic.fields import ModelField
 from typing import (
     Any,
     ClassVar,
     Dict,
     Iterable,
@@ -24,28 +24,60 @@
     List[int],
     List[float],
     List[str],
 ]
 
 
 singles = [int, float, str, bool, datetime]
-lists = [List[int], List[float], List[str], List[bool], List[List[str]]]
+lists = [
+    List[int],
+    List[float],
+    List[str],
+    List[bool],
+    List[datetime],
+    List[List[int]],
+    List[List[float]],
+    List[List[str]],
+    List[List[bool]],
+]
 options = [
     Union[int, None],
     Union[float, None],
     Union[str, None],
     Union[bool, None],
+    Union[datetime, None],
+    Union[List[int], None],
+    Union[List[float], None],
+    Union[List[str], None],
+    Union[List[bool], None],
+    Union[List[datetime], None],
 ]
 
 dicts = [Dict[str, Any], Dict[str, str], Dict[str, int], Dict[str, float]] + [
-    Dict[str, Dict[str, Any]]
+    Dict[str, Dict[str, Any]],
+    Dict[str, Dict[str, str]],
+    Dict[str, Dict[str, int]],
+    Dict[str, Dict[str, float]],
 ]
 
 types_we_support = singles + lists + options + dicts
 
+
+defaults = Union[
+    int,
+    float,
+    str,
+    bool,
+    datetime,
+    List[int],
+    List[float],
+    List[str],
+    List[bool],
+]
+
 IsDefault = bool
 
 
 class TaskMixin:
     __dataclass_fields__: ClassVar[Dict[str, Any]]
     __fields__: ClassVar[Dict[str, Any]]
 
@@ -157,24 +189,28 @@
     elif len(n) == 6:
         return datetime(n[0], n[1], n[2], n[3], n[4], n[5])
     else:
         raise ValueError("Invalid datetime format")
 
 
 def parse_variations(type_, value, name_):
-    if type_ == List[int]:
+    if type_ == bool:
+        return parse_bool(value)
+    elif type_ == int:
+        return int(value)
+    elif type_ == float:
+        return float(value)
+    elif type_ == List[int]:
         return parse_list(value, int, name_)
     elif type_ == List[str]:
         return parse_list(value, str, name_)
     elif type_ == List[float]:
         return parse_list(value, float, name_)
     elif type_ == List[bool]:
         return parse_list(value, parse_bool, name_)
-    elif type_ == List[List[str]]:
-        return json.loads(value)
     elif type_ == Union[int, None]:
         return parse_options(value, int)
     elif type_ == Union[str, None]:
         return parse_options(value, str)
     elif type_ == Union[float, None]:
         return parse_options(value, float)
     elif type_ == Union[bool, None]:
@@ -183,32 +219,24 @@
         return json.loads(value)
     elif type_ == Dict[str, Any]:
         return json.loads(value)
     elif type_ == Dict[float, Any]:
         return json.loads(value)
     elif type_ == Dict[bool, Any]:
         return json.loads(value)
-    elif type_ == Dict[str, Dict[str, Any]]:
-        return json.loads(value)
-    elif type_ == bool:
-        return parse_bool(value)
-    elif type_ == int:
-        return int(value)
-    elif type_ == float:
-        return float(value)
     elif type_ == str:
         try:
             res = json.loads(value)
             if type(res) == int:
                 return str(res)
             else:
                 return res
         except Exception:
             return str(value)
-    elif type_ == datetime:
+    elif type_ in [datetime, date]:
         # FIXME actually like use proper parsing lmao
         if value.startswith('"') and value.endswith('"'):
             value = value[1:-1]
         has_t_or_colon = ":" in value or "T" in value
         num_parts = len(value.split("-"))
         if has_t_or_colon:
             value = value.replace(" ", "-")
```

### Comparing `utilki-0.5.0/PKG-INFO` & `utilki-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.5.0
+Version: 0.5.1
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

