# Comparing `tmp/named-env-2.1.0.tar.gz` & `tmp/named_env-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "named-env-2.1.0.tar", max compression
+gzip compressed data, was "named_env-2.2.0.tar", max compression
```

## Comparing `named-env-2.1.0.tar` & `named_env-2.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1057 2022-11-23 08:54:36.365852 named-env-2.1.0/LICENSE
--rw-r--r--   0        0        0      525 2022-11-23 08:54:36.366074 named-env-2.1.0/README.md
--rw-r--r--   0        0        0      777 2022-11-23 14:37:51.480273 named-env-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      408 2022-11-23 09:03:10.235847 named-env-2.1.0/src/named_env/__init__.py
--rw-r--r--   0        0        0      561 2022-11-23 08:54:36.367699 named-env-2.1.0/src/named_env/exceptions.py
--rw-r--r--   0        0        0      436 2022-11-23 13:27:14.743482 named-env-2.1.0/src/named_env/namespace.py
--rw-r--r--   0        0        0        0 2022-11-23 08:54:36.368117 named-env-2.1.0/src/named_env/py.typed
--rw-r--r--   0        0        0     4353 2022-11-23 13:56:35.190588 named-env-2.1.0/src/named_env/variables.py
--rw-r--r--   0        0        0      328 2022-11-23 08:54:36.368700 named-env-2.1.0/src/named_env/version.py
--rw-r--r--   0        0        0     1194 2022-11-23 14:39:42.822283 named-env-2.1.0/setup.py
--rw-r--r--   0        0        0     1165 2022-11-23 14:39:42.822464 named-env-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-06-27 15:25:43.958896 named_env-2.2.0/LICENSE
+-rw-r--r--   0        0        0      525 2023-06-27 15:25:43.958958 named_env-2.2.0/README.md
+-rw-r--r--   0        0        0     3738 2023-06-27 16:25:32.015924 named_env-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      439 2023-06-27 16:12:37.375261 named_env-2.2.0/src/named_env/__init__.py
+-rw-r--r--   0        0        0      674 2023-06-27 16:12:37.372785 named_env-2.2.0/src/named_env/exceptions.py
+-rw-r--r--   0        0        0      436 2023-06-27 15:25:43.959639 named_env-2.2.0/src/named_env/namespace.py
+-rw-r--r--   0        0        0        0 2023-06-27 15:25:43.959664 named_env-2.2.0/src/named_env/py.typed
+-rw-r--r--   0        0        0     5229 2023-06-27 16:24:27.612250 named_env-2.2.0/src/named_env/variables.py
+-rw-r--r--   0        0        0      328 2023-06-27 15:25:43.959804 named_env-2.2.0/src/named_env/version.py
+-rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 named_env-2.2.0/setup.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 named_env-2.2.0/PKG-INFO
```

### Comparing `named-env-2.1.0/LICENSE` & `named_env-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `named-env-2.1.0/README.md` & `named_env-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `named-env-2.1.0/src/named_env/variables.py` & `named_env-2.2.0/src/named_env/variables.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Variables definition"""
 
 import os
 import typing as t
 
-from .exceptions import MissingVariableError
+from .exceptions import (
+    MissingVariableError,
+    ChoiceValueError,
+)
 from .namespace import EnvironmentNamespace
 
 __all__ = [
     "BaseVariableMixin",
     "RequiredVariableMixin",
     "OptionalVariableMixin",
     "RequiredString",
@@ -24,66 +27,81 @@
 
 sentinel = object()
 
 
 class BaseVariableMixin:
     """Common ancestor for all variables classes"""
 
+    _choice: t.Optional[t.Sequence] = None
+
     def __set_name__(self, owner, name):
         self._name = name
 
     def __get__(self, obj, objtype=None):
         if self._value is sentinel:
             env = (
                 obj.environ
                 if isinstance(obj, EnvironmentNamespace)
                 else objtype.environ
                 if issubclass(objtype, EnvironmentNamespace)
                 else os.environ
             )
             if self._name in env:
-                self._value = self.cast(env[self._name])
+                self._set_value(env[self._name])
             elif isinstance(self, OptionalVariableMixin):
-                # Cast defaults also
-                self._value = self.cast(self.default)
+                self._set_value(self.default)
             elif isinstance(self, RequiredVariableMixin):
                 raise MissingVariableError(variable=self._name, description=self.description)
         return self._value
 
+    def _set_value(self, value: t.Any) -> None:
+        """Cast-check-set"""
+        cast_value: t.Any = self.cast(value)
+        self._validate_cast_value(cast_value)
+        self._value = cast_value
+
+    def _validate_cast_value(self, cast_value: t.Any) -> None:
+        if self._choice is not None and cast_value not in self._choice:
+            raise ChoiceValueError(f"{self._name} variable has an unexpected value")
+
     @classmethod
     def _get_base_class(cls) -> type:
         """Find first non-BaseVariableMixin superclass"""
         for klass in cls.mro():
             if not issubclass(klass, BaseVariableMixin):
                 return klass
         raise TypeError(f"Non-BaseVariableMixin superclass not found for {cls}")
 
     def __new__(cls, *args, **kwargs) -> t.Any:
+        choice: t.Optional[t.Sequence] = kwargs.pop("choice", None)
         obj = cls._get_base_class().__new__(cls, *args, **kwargs)  # noqa
+        obj._choice = choice
         obj._name = None
         obj._value = sentinel
         return obj
 
     @classmethod
     def cast(cls, value):
         """Transform environment string value into desired type"""
         return cls._get_base_class()(value)
 
 
 class RequiredVariableMixin(BaseVariableMixin):
     """Required variables with optional description to inform on failed obtaining"""
 
-    def __init__(self, *, description: t.Optional[str] = None) -> None:
+    # pylint: disable=unused-argument
+    def __init__(self, *, description: t.Optional[str] = None, choice: t.Optional[t.Sequence] = None) -> None:
         self.description = description
 
 
 class OptionalVariableMixin(BaseVariableMixin):
     """Optional variables with required default value"""
 
-    def __init__(self, default: t.Any) -> None:
+    # pylint: disable=unused-argument
+    def __init__(self, default: t.Any, choice: t.Optional[t.Sequence] = None) -> None:
         self.default = default
 
 
 class Boolean(BaseVariableMixin):
     """Bool-like class to interpret string values"""
 
     _POSITIVE_VALUES: t.Set[str] = {"y", "yes", "true", "1"}
@@ -101,14 +119,18 @@
 class List(BaseVariableMixin, list):
     """Comma-separated lists reading"""
 
     @classmethod
     def cast(cls, value: t.Union[t.List[str], str]) -> t.List[str]:
         return [item.strip() for item in value.split(",") if item] if isinstance(value, str) else value
 
+    def _validate_cast_value(self, cast_value: t.Any) -> None:
+        for cast_value_item in cast_value:  # type: t.Any
+            super()._validate_cast_value(cast_value_item)
+
 
 class RequiredString(RequiredVariableMixin, str):
     """String-like required variable class"""
 
 
 class RequiredFloat(RequiredVariableMixin, float):
     """Float-like required variable class"""
```

### Comparing `named-env-2.1.0/setup.py` & `named_env-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 ['named_env']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'named-env',
-    'version': '2.1.0',
+    'version': '2.2.0',
     'description': 'Class-based environment variables typed specification',
     'long_description': '# named-env\n\nClass-based environment variables typed specification.\n\n## Installation\n\n```shell\npip install named-env\n```\n\n## Usage example\n\n```python\nfrom named_env import EnvironmentNamespace, RequiredInteger\nimport os\n\n\nclass WebApplicationEnvironmentNamespace(EnvironmentNamespace):\n    WEB_SERVER_PORT = RequiredInteger()\n\n\nenv = WebApplicationEnvironmentNamespace()\n\nif __name__ == "__main__":\n    os.environ["WEB_SERVER_PORT"] = "80"\n    print(env.WEB_SERVER_PORT)  # 80\n    print(type(env.WEB_SERVER_PORT))  # int\n```\n',
     'author': 'Artem Novikov',
     'author_email': 'artnew@list.ru',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/reartnew/named-env',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `named-env-2.1.0/PKG-INFO` & `named_env-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: named-env
-Version: 2.1.0
+Version: 2.2.0
 Summary: Class-based environment variables typed specification
 Home-page: https://github.com/reartnew/named-env
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/reartnew/named-env
 Description-Content-Type: text/markdown
 
 # named-env
 
 Class-based environment variables typed specification.
```

