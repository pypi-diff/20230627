# Comparing `tmp/necessary-0.4.2.tar.gz` & `tmp/necessary-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "necessary-0.4.2.tar", last modified: Mon Apr  3 05:16:32 2023, max compression
+gzip compressed data, was "necessary-0.4.3.tar", last modified: Tue Jun 27 18:17:30 2023, max compression
```

## Comparing `necessary-0.4.2.tar` & `necessary-0.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-03 05:16:32.213792 necessary-0.4.2/
--rw-r--r--   0 lucas      (502) staff       (20)    11357 2022-08-24 22:43:19.000000 necessary-0.4.2/LICENSE
--rw-r--r--   0 lucas      (502) staff       (20)     3031 2023-04-03 05:16:32.213601 necessary-0.4.2/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     2220 2023-02-01 06:04:36.000000 necessary-0.4.2/README.md
--rw-r--r--   0 lucas      (502) staff       (20)     2152 2023-04-03 05:12:49.000000 necessary-0.4.2/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       38 2023-04-03 05:16:32.213855 necessary-0.4.2/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-03 05:16:32.208359 necessary-0.4.2/src/
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-03 05:16:32.210795 necessary-0.4.2/src/necessary/
--rw-r--r--   0 lucas      (502) staff       (20)      400 2022-12-08 09:13:20.000000 necessary-0.4.2/src/necessary/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)       95 2022-10-26 01:31:48.000000 necessary-0.4.2/src/necessary/__init__.pyi
--rw-r--r--   0 lucas      (502) staff       (20)     6764 2023-04-03 05:15:52.000000 necessary-0.4.2/src/necessary/core.py
--rw-r--r--   0 lucas      (502) staff       (20)     1631 2022-10-26 01:31:48.000000 necessary-0.4.2/src/necessary/core.pyi
--rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-22 22:19:50.000000 necessary-0.4.2/src/necessary/py.typed
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-03 05:16:32.212037 necessary-0.4.2/src/necessary.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)     3031 2023-04-03 05:16:32.000000 necessary-0.4.2/src/necessary.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)      402 2023-04-03 05:16:32.000000 necessary-0.4.2/src/necessary.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2023-04-03 05:16:32.000000 necessary-0.4.2/src/necessary.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)      226 2023-04-03 05:16:32.000000 necessary-0.4.2/src/necessary.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)       10 2023-04-03 05:16:32.000000 necessary-0.4.2/src/necessary.egg-info/top_level.txt
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-03 05:16:32.213127 necessary-0.4.2/tests/
--rw-r--r--   0 lucas      (502) staff       (20)      890 2022-08-25 22:02:13.000000 necessary-0.4.2/tests/test_necessary.py
--rw-r--r--   0 lucas      (502) staff       (20)      469 2023-02-01 06:00:50.000000 necessary-0.4.2/tests/test_parsing.py
--rw-r--r--   0 lucas      (502) staff       (20)      502 2022-08-25 22:03:03.000000 necessary-0.4.2/tests/test_with.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-27 18:17:30.433828 necessary-0.4.3/
+-rw-r--r--   0 lucas      (502) staff       (20)    11357 2022-08-24 22:43:19.000000 necessary-0.4.3/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)     3031 2023-06-27 18:17:30.433694 necessary-0.4.3/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     2220 2023-02-01 06:04:36.000000 necessary-0.4.3/README.md
+-rw-r--r--   0 lucas      (502) staff       (20)     2152 2023-06-27 18:16:57.000000 necessary-0.4.3/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2023-06-27 18:17:30.433879 necessary-0.4.3/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-27 18:17:30.430055 necessary-0.4.3/src/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-27 18:17:30.431850 necessary-0.4.3/src/necessary/
+-rw-r--r--   0 lucas      (502) staff       (20)      400 2022-12-08 09:13:20.000000 necessary-0.4.3/src/necessary/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)       95 2022-10-26 01:31:48.000000 necessary-0.4.3/src/necessary/__init__.pyi
+-rw-r--r--   0 lucas      (502) staff       (20)     7198 2023-06-27 18:16:57.000000 necessary-0.4.3/src/necessary/core.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1679 2023-06-27 18:16:57.000000 necessary-0.4.3/src/necessary/core.pyi
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-22 22:19:50.000000 necessary-0.4.3/src/necessary/py.typed
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-27 18:17:30.432605 necessary-0.4.3/src/necessary.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     3031 2023-06-27 18:17:30.000000 necessary-0.4.3/src/necessary.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)      402 2023-06-27 18:17:30.000000 necessary-0.4.3/src/necessary.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2023-06-27 18:17:30.000000 necessary-0.4.3/src/necessary.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      226 2023-06-27 18:17:30.000000 necessary-0.4.3/src/necessary.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       10 2023-06-27 18:17:30.000000 necessary-0.4.3/src/necessary.egg-info/top_level.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-27 18:17:30.433335 necessary-0.4.3/tests/
+-rw-r--r--   0 lucas      (502) staff       (20)     1036 2023-06-27 18:16:57.000000 necessary-0.4.3/tests/test_necessary.py
+-rw-r--r--   0 lucas      (502) staff       (20)      469 2023-02-01 06:00:50.000000 necessary-0.4.3/tests/test_parsing.py
+-rw-r--r--   0 lucas      (502) staff       (20)      502 2022-08-25 22:03:03.000000 necessary-0.4.3/tests/test_with.py
```

### Comparing `necessary-0.4.2/LICENSE` & `necessary-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `necessary-0.4.2/PKG-INFO` & `necessary-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: necessary
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python package to enforce optional dependencies
 Author-email: Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/soldni/necessary
 Project-URL: Source, https://github.com/soldni/necessary
 Project-URL: Tracker, https://github.com/soldni/necessary/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `necessary-0.4.2/README.md` & `necessary-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `necessary-0.4.2/pyproject.toml` & `necessary-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "necessary"
-version = "0.4.2"
+version = "0.4.3"
 description = "Python package to enforce optional dependencies"
 authors = [
     {name = "Luca Soldaini", email = "luca@soldaini.net" }
 ]
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `necessary-0.4.2/src/necessary/core.py` & `necessary-0.4.3/src/necessary/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib.metadata
 import operator
 import warnings
 from functools import wraps
 from importlib import import_module
 from inspect import isclass
 from types import ModuleType
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Type, Union
 
 import requirements
 from packaging.version import Version, parse
 from requirements.requirement import Requirement
 
 PackageNameType = str
 PackageVersionType = Union[None, str, Version]
@@ -49,45 +49,49 @@
             message=f"Could not parse version of {module}. Error: {e}",
             category=UserWarning,
             stacklevel=2,
         )
         return None
 
 
-# class ModuleSpec(NamedTuple):
-#     module_name: PackageNameType
-#     module_version: PackageVersionType
+class NecessaryImportError(ImportError):
+    ...
 
 
 class necessary:
     """Check if a module is installed and optionally check its version."""
 
     def __init__(
         self,
         modules: FullSpecType,
         soft: bool = False,
         message: Optional[str] = None,
+        errors: Optional[Tuple[Type[Exception], ...]] = None,
     ):
         """
         Args:
             modules (FullSpecType): Either a module name, a tuple
                 consisting of (module name, version), or a list containing a
                 mix of the two.
             soft (bool): If True, the function will return False if the
                 module is not installed. If False, the function will raise an
                 ImportError.
             message (Optional[str]): If provided, the function will raise the
                 given message. If your message contains "{module_name}" and
                 "{module_version}", the function will replace them with the
                 their respective values.
+            errors (Optional[List[Type[Exception]]]): If provided, the tuple
+                of errors to be caught to determine if a module is not
+                installed. If not provided, default is [ModuleNotFoundError].
 
         Raises:
             ImportError: If the module is not installed and `soft` is False.
         """
         parsed_modules_spec = self.parse_modules_spec_input(modules)
+        self._errors = errors or (ModuleNotFoundError,)
         self._necessary = all(
             self.check_module_is_available(
                 req=module_spec, soft_check=soft, message=message
             )
             for module_spec in parsed_modules_spec
         )
 
@@ -116,15 +120,14 @@
             parsed_requirements.append(spec)
 
         return parsed_requirements
 
     def get_error(
         self, req: Requirement, message: Optional[str] = None
     ) -> ImportError:
-
         spec_message = (
             " with version requirements {module_version}" if req.specs else ""
         )
         message = message or (
             "Please install module {module_name}" + spec_message + "."
         )
 
@@ -139,26 +142,25 @@
 
     def check_module_is_available(
         self,
         req: Requirement,
         soft_check: bool = False,
         message: Optional[str] = None,
     ) -> bool:
-
         # this is the message to raise in case of failure and if no custom
         # message is provided by the user.
         if message is None:
             message = "'{module_name}' is required, please install it."
             if req.specs:
                 message = "version '{module_version}' of " + message
 
         # fist check is to see if we can import the module.
         try:
             module = import_module(str(req.name))
-        except ModuleNotFoundError:
+        except self._errors:
             if soft_check:
                 return False
             raise self.get_error(req=req, message=message)
 
         # then let's check if a minimum version is specified and if so,
         # check it.
         module_version = get_module_version(module)
@@ -189,24 +191,30 @@
         pass
 
 
 def Necessary(
     modules: FullSpecType,
     soft: bool = False,
     message: Optional[str] = None,
+    errors: Optional[Tuple[Type[Exception], ...]] = None,
 ):
     """A decorator that will raise an error when the decorated
     function or class is called and the module is not available."""
 
     def decorating_fn(decorated, modules=modules, soft=soft, message=message):
         to_decorate = decorated.__init__ if isclass(decorated) else decorated
 
         @wraps(to_decorate)
         def wrapper(*args, **kwargs):
-            with necessary(modules, soft=soft, message=message):
+            with necessary(
+                modules,
+                soft=soft,
+                message=message,
+                errors=errors,
+            ):
                 return to_decorate(*args, **kwargs)
 
         if isclass(decorated):
             decorated.__init__ = wrapper
             return decorated
         else:
             return wrapper
```

### Comparing `necessary-0.4.2/src/necessary/core.pyi` & `necessary-0.4.3/src/necessary/core.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from types import ModuleType
 from typing import (
     TYPE_CHECKING,
     Callable,
     List,
     Literal,
-    NamedTuple,
     Optional,
     Tuple,
+    Type,
     TypeVar,
     Union,
 )
 
-from packaging.version import LegacyVersion, Version
+from packaging.version import Version
+from requirements.requirement import Requirement
 from typing_extensions import TypeAlias
 
-PackageNameType: TypeAlias = str
-PackageVersionType: TypeAlias = Union[str, Version, LegacyVersion]
+PackageNameType = str
+PackageVersionType: TypeAlias = Union[None, str, Version]
 PackageNameAndVersionType: TypeAlias = Tuple[
     PackageNameType, PackageVersionType
 ]
 FullSpecType: TypeAlias = Union[
     PackageNameType,
     PackageNameAndVersionType,
     List[Union[PackageNameType, PackageNameAndVersionType]],
 ]
 
-class ModuleSpec(NamedTuple):
-    module_name: PackageNameType
-    module_version: PackageVersionType
+class NecessaryImportError(ImportError): ...
 
 def get_module_version(
     module: ModuleType,
-) -> Union[Version, LegacyVersion, None]: ...
+) -> Union[Version, None]: ...
 
 class necessary:
     def __init__(
         self,
         modules: FullSpecType,
         soft: bool = ...,
         message: Optional[str] = ...,
+        errors: Optional[Tuple[Type[Exception], ...]] = ...,
     ): ...
     def parse_modules_spec_input(
         self, modules_spec: FullSpecType
-    ) -> List[ModuleSpec]: ...
+    ) -> List[Requirement]: ...
     def check_module_is_available(
         self,
-        module_spec: ModuleSpec,
+        req: Requirement,
         soft_check: bool = ...,
         message: Optional[str] = ...,
     ) -> bool: ...
     def __enter__(self) -> "necessary": ...
     def __exit__(self, exc_type, exc_value, traceback) -> None: ...
 
     if TYPE_CHECKING:  # noqa: Y002
@@ -59,8 +59,9 @@
 
 _T = TypeVar("_T")
 
 def Necessary(
     modules: FullSpecType,
     soft: bool = ...,
     message: Optional[str] = ...,
+    errors: Optional[Tuple[Type[Exception], ...]] = ...,
 ) -> Callable[[_T], _T]: ...
```

### Comparing `necessary-0.4.2/src/necessary.egg-info/PKG-INFO` & `necessary-0.4.3/src/necessary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: necessary
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python package to enforce optional dependencies
 Author-email: Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/soldni/necessary
 Project-URL: Source, https://github.com/soldni/necessary
 Project-URL: Tracker, https://github.com/soldni/necessary/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `necessary-0.4.2/tests/test_necessary.py` & `necessary-0.4.3/tests/test_necessary.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,7 +26,11 @@
 
         self.assertFalse(necessary("2222", soft=True))
 
         with self.assertRaises(ImportError):
             necessary(("black", "303030303303"))
 
         self.assertFalse(necessary(("black", "303030303303"), soft=True))
+
+    def test_custom_error(self) -> None:
+        with self.assertRaises(ModuleNotFoundError):
+            necessary("foo", errors=(ValueError,))
```

