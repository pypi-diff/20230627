# Comparing `tmp/python_simpleconf-0.5.9.tar.gz` & `tmp/python_simpleconf-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_simpleconf-0.5.9.tar", max compression
+gzip compressed data, was "python_simpleconf-0.6.0.tar", max compression
```

## Comparing `python_simpleconf-0.5.9.tar` & `python_simpleconf-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1056 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/LICENSE
--rw-r--r--   0        0        0     5173 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/README.md
--rw-r--r--   0        0        0     1220 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/simpleconf/__init__.py
--rw-r--r--   0        0        0     2319 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/simpleconf/caster.py
--rw-r--r--   0        0        0     7642 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/simpleconf/config.py
--rw-r--r--   0        0        0      172 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/simpleconf/exceptions.py
--rw-r--r--   0        0        0     1164 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/__init__.py
--rw-r--r--   0        0        0      258 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/dict.py
--rw-r--r--   0        0        0     1525 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/env.py
--rw-r--r--   0        0        0     1991 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/ini.py
--rw-r--r--   0        0        0      401 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/json.py
--rw-r--r--   0        0        0     1602 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/osenv.py
--rw-r--r--   0        0        0      593 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/toml.py
--rw-r--r--   0        0        0      490 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/yaml.py
--rw-r--r--   0        0        0     1750 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/utils.py
--rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 python_simpleconf-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5173 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/README.md
+-rw-r--r--   0        0        0     1428 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/__init__.py
+-rw-r--r--   0        0        0     2337 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/caster.py
+-rw-r--r--   0        0        0     7642 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/config.py
+-rw-r--r--   0        0        0      172 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/exceptions.py
+-rw-r--r--   0        0        0     1164 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/loaders/__init__.py
+-rw-r--r--   0        0        0      258 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/loaders/dict.py
+-rw-r--r--   0        0        0     1525 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/loaders/env.py
+-rw-r--r--   0        0        0     1991 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/loaders/ini.py
+-rw-r--r--   0        0        0      401 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/loaders/json.py
+-rw-r--r--   0        0        0     1602 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/loaders/osenv.py
+-rw-r--r--   0        0        0      769 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/loaders/toml.py
+-rw-r--r--   0        0        0      490 2023-06-27 00:35:19.229447 python_simpleconf-0.6.0/simpleconf/loaders/yaml.py
+-rw-r--r--   0        0        0     2183 2023-06-27 00:35:19.233446 python_simpleconf-0.6.0/simpleconf/utils.py
+-rw-r--r--   0        0        0     6497 1970-01-01 00:00:00.000000 python_simpleconf-0.6.0/PKG-INFO
```

### Comparing `python_simpleconf-0.5.9/LICENSE` & `python_simpleconf-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.9/README.md` & `python_simpleconf-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.9/pyproject.toml` & `python_simpleconf-0.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "python-simpleconf"
-version = "0.5.9"
+version = "0.6.0"
 description = "Simple configuration management with python."
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/simpleconf"
 repository = "https://github.com/pwwang/simpleconf"
 packages = [
@@ -16,23 +16,25 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 diot = "^0.2.1"
 python-dotenv = { version="^0.21", optional = true}
 pyyaml = { version="^6", optional = true}
-rtoml = {version = "^0.8", optional = true}
+# Use rtoml only when the wheel is available (linux)
+rtoml = {version = "^0.8", optional = true, python = "<3.11", platform = "linux"}
+tomli = {version = "^2.0", optional = true, python = "<3.11", markers = 'sys_platform != "linux"'}
 iniconfig = {version = "^2.0", optional = true}
 
 [tool.poetry.extras]
 ini = [ "iniconfig" ]
 env = [ "python-dotenv"]
 yaml = [ "pyyaml"]
-toml = [ "rtoml"]
-all = [ "iniconfig", "python-dotenv", "pyyaml", "rtoml"]
+toml = [ "rtoml", "tomli"]
+all = [ "iniconfig", "python-dotenv", "pyyaml", "rtoml", "tomli"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
 
 [tool.pytest.ini_options]
 addopts = "-vv -p no:asyncio --cov=simpleconf --cov-report xml:cov.xml --cov-report term-missing"
```

### Comparing `python_simpleconf-0.5.9/simpleconf/caster.py` & `python_simpleconf-0.6.0/simpleconf/caster.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     if value.lower() == "false":
         return False
     raise ValueError(f"Expect `@bool:true` or `@bool:false`, got `{value}`")
 
 
 def _cast_toml(value: str) -> Any:
     """Cast toml string"""
-    rtoml = require_package("rtoml")
-    return rtoml.loads(value)
+    toml = require_package("rtoml", "tomllib", "tomli")
+    return toml.loads(value)
 
 
 int_caster = type_caster("@int:", lambda x: int(float(x)))
 float_caster = type_caster("@float:", float)
 bool_caster = type_caster("@bool:", _cast_bool)
 none_caster = type_caster("@none", _cast_none)
 null_caster = type_caster("null", _cast_none)
```

### Comparing `python_simpleconf-0.5.9/simpleconf/config.py` & `python_simpleconf-0.6.0/simpleconf/config.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.9/simpleconf/loaders/__init__.py` & `python_simpleconf-0.6.0/simpleconf/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.9/simpleconf/loaders/env.py` & `python_simpleconf-0.6.0/simpleconf/loaders/env.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.9/simpleconf/loaders/ini.py` & `python_simpleconf-0.6.0/simpleconf/loaders/ini.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.9/simpleconf/loaders/osenv.py` & `python_simpleconf-0.6.0/simpleconf/loaders/osenv.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.9/simpleconf/loaders/toml.py` & `python_simpleconf-0.6.0/simpleconf/loaders/toml.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..caster import (
     none_caster,
     null_caster,
 )
 from . import Loader
 
-rtoml = require_package("rtoml")
+toml = require_package("rtoml", "tomllib", "tomli")
 
 
 class TomlLoader(Loader):
     """Toml file loader"""
 
     CASTERS = [
         none_caster,
@@ -20,9 +20,13 @@
     ]
 
     def loading(self, conf: Any, ignore_nonexist: bool) -> Diot:
         """Load the configuration from a toml file"""
         if not self._exists(conf, ignore_nonexist):
             return Diot()
 
-        with open(conf) as f:
-            return Diot(rtoml.load(f))
+        if toml.__name__ in ("tomli", "tomllib"):  # pragma: no cover
+            with open(conf, "rb") as f:
+                return Diot(toml.load(f))
+
+        with open(conf, "r") as f:
+            return Diot(toml.load(f))
```

### Comparing `python_simpleconf-0.5.9/simpleconf/utils.py` & `python_simpleconf-0.6.0/simpleconf/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 
+from __future__ import annotations
+
 from pathlib import Path
 from importlib import import_module
 from types import ModuleType
 from typing import TYPE_CHECKING, Any
 
 from .exceptions import FormatNotSupported
 
@@ -28,15 +30,15 @@
 
     if out == "yml":
         return "yaml"
 
     return out
 
 
-def get_loader(ext: str) -> "Loader":
+def get_loader(ext: str) -> Loader:
     """Get the loader for the extension"""
     if ext == "dict":
         from .loaders.dict import DictLoader
         return DictLoader()
     if ext == "env":
         from .loaders.env import EnvLoader
         return EnvLoader()
@@ -55,13 +57,25 @@
     if ext == "yaml":
         from .loaders.yaml import YamlLoader
         return YamlLoader()
 
     raise FormatNotSupported(f"{ext} is not supported.")
 
 
-def require_package(package: str) -> "ModuleType":
+def require_package(package: str, *fallbacks: str) -> ModuleType:
     """Require the package and return the module"""
     try:
         return import_module(package)
     except ModuleNotFoundError:
-        raise ImportError(f"{package} is not installed.")
+        for fallback in fallbacks:
+            try:
+                return import_module(fallback)
+            except ModuleNotFoundError:
+                pass
+
+        if fallbacks:
+            raise ImportError(
+                f"Neither '{package}' nor its fallbacks "
+                f"`{', '.join(fallbacks)}` is installed."
+            ) from None
+        else:
+            raise ImportError(f"'{package}' is not installed.") from None
```

### Comparing `python_simpleconf-0.5.9/PKG-INFO` & `python_simpleconf-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-simpleconf
-Version: 0.5.9
+Version: 0.6.0
 Summary: Simple configuration management with python.
 Home-page: https://github.com/pwwang/simpleconf
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,16 @@
 Provides-Extra: ini
 Provides-Extra: toml
 Provides-Extra: yaml
 Requires-Dist: diot (>=0.2.1,<0.3.0)
 Requires-Dist: iniconfig (>=2.0,<3.0) ; extra == "ini" or extra == "all"
 Requires-Dist: python-dotenv (>=0.21,<0.22) ; extra == "env" or extra == "all"
 Requires-Dist: pyyaml (>=6,<7) ; extra == "yaml" or extra == "all"
-Requires-Dist: rtoml (>=0.8,<0.9) ; extra == "toml" or extra == "all"
+Requires-Dist: rtoml (>=0.8,<0.9) ; (python_version < "3.11" and sys_platform == "linux") and (extra == "toml" or extra == "all")
+Requires-Dist: tomli (>=2.0,<3.0) ; (sys_platform != "linux" and python_version < "3.11") and (extra == "toml" or extra == "all")
 Project-URL: Repository, https://github.com/pwwang/simpleconf
 Description-Content-Type: text/markdown
 
 # simpleconf
 
 Simple configuration management for python
```

