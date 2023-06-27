# Comparing `tmp/jsonablr-1.0.0.tar.gz` & `tmp/jsonablr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonablr-1.0.0.tar", max compression
+gzip compressed data, was "jsonablr-1.1.0.tar", max compression
```

## Comparing `jsonablr-1.0.0.tar` & `jsonablr-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-06-26 17:24:04.431422 jsonablr-1.0.0/LICENSE
--rw-r--r--   0        0        0     1870 2023-06-26 21:39:00.368116 jsonablr-1.0.0/README.md
--rw-r--r--   0        0        0       86 2023-06-27 11:04:34.940297 jsonablr-1.0.0/jsonablr/__init__.py
--rw-r--r--   0        0        0     6404 2023-06-27 11:02:14.362196 jsonablr-1.0.0/jsonablr/main.py
--rw-r--r--   0        0        0      561 2023-06-27 11:07:57.039066 jsonablr-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 jsonablr-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-26 17:24:04.431422 jsonablr-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1870 2023-06-26 21:39:00.368116 jsonablr-1.1.0/README.md
+-rw-r--r--   0        0        0      118 2023-06-27 16:27:20.064626 jsonablr-1.1.0/jsonablr/__init__.py
+-rw-r--r--   0        0        0     6822 2023-06-27 16:28:38.207825 jsonablr-1.1.0/jsonablr/main.py
+-rw-r--r--   0        0        0      561 2023-06-27 16:32:21.155708 jsonablr-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 jsonablr-1.1.0/PKG-INFO
```

### Comparing `jsonablr-1.0.0/LICENSE` & `jsonablr-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonablr-1.0.0/README.md` & `jsonablr-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonablr-1.0.0/jsonablr/main.py` & `jsonablr-1.1.0/jsonablr/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Encoders
 """
+from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 from datetime import datetime, date, timezone
 import dataclasses
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from pydantic import BaseModel
@@ -36,22 +37,37 @@
     exclude_unset: bool = False
     exclude_none: bool = False
     exclude_defaults: bool = False
     sqlalchemy_safe: bool = True
     preserve_set: bool = False
 
 
-def encode(data: Any, **kwargs) -> dict:
+def encode(data: Any, **options) -> dict:
     encoder = JsonAblr(
-        encoders=kwargs.pop('encoders', {}),
-        **Options.parse_obj(kwargs).dict()
+        encoders=options.pop('encoders', {}),
+        **Options.parse_obj(options).dict()
     )
     return encoder(data)
 
 
+def encode_output(func=None, **options):
+    encoder = JsonAblr(
+        encoders=options.pop('encoders', {}),
+        **Options.parse_obj(options).dict()
+    )
+
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            return encoder.encode(func(*args, **kwargs))
+        return wrapper
+
+    return decorator if func is None else decorator(func)
+
+
 encoder_map:  Dict[Callable[[Any], Any], Tuple[Any, ...]] = {}
 for type_, encoder in ENCODERS_BY_TYPE.items():
     encoder_map.setdefault(encoder, tuple())
     encoder_map[encoder] += (type_,)
 
 
 class JsonAblr:
```

### Comparing `jsonablr-1.0.0/pyproject.toml` & `jsonablr-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Bernard van Niekerk <bernard.van.niekerk@icloud.com>"]
 description = "Serialize Pydantic models and non-JSONable types into a JSONable variable."
 name = "jsonablr"
 readme = "README.md"
 repository = "https://github.com/frizzy/jsonablr.git"
-version = "1.0.0"
+version = "1.1.0"
 
 [tool.poetry.dependencies]
 pydantic = "^1.10"
 python = "^3.9"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `jsonablr-1.0.0/PKG-INFO` & `jsonablr-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonablr
-Version: 1.0.0
+Version: 1.1.0
 Summary: Serialize Pydantic models and non-JSONable types into a JSONable variable.
 Home-page: https://github.com/frizzy/jsonablr.git
 Author: Bernard van Niekerk
 Author-email: bernard.van.niekerk@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

