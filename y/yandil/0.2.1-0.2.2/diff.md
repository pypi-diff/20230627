# Comparing `tmp/yandil-0.2.1.tar.gz` & `tmp/yandil-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.2.1.tar", max compression
+gzip compressed data, was "yandil-0.2.2.tar", max compression
```

## Comparing `yandil-0.2.1.tar` & `yandil-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11594 2023-06-26 20:49:21.618091 yandil-0.2.1/README.md
--rw-r--r--   0        0        0      817 2023-06-26 20:50:27.278769 yandil-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0    10681 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/dependency.py
--rw-r--r--   0        0        0     1020 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3192 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      257 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      301 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     3548 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    11925 1970-01-01 00:00:00.000000 yandil-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11594 2023-06-26 22:29:57.082696 yandil-0.2.2/README.md
+-rw-r--r--   0        0        0      817 2023-06-26 22:30:51.626426 yandil-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0    10681 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1217 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      257 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      301 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     3548 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-06-26 22:29:57.082696 yandil-0.2.2/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    11925 1970-01-01 00:00:00.000000 yandil-0.2.2/PKG-INFO
```

### Comparing `yandil-0.2.1/README.md` & `yandil-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/pyproject.toml` & `yandil-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.2.1"
+version = "0.2.2"
 description = "Yet ANother Dependency Injection Library"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 
@@ -30,15 +30,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.1"
+version = "0.2.2"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.2.1/src/yandil/configuration/configuration_container.py` & `yandil-0.2.2/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/src/yandil/container.py` & `yandil-0.2.2/src/yandil/container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/src/yandil/declarative/decorators.py` & `yandil-0.2.2/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/src/yandil/dependency.py` & `yandil-0.2.2/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/src/yandil/dependency_filler.py` & `yandil-0.2.2/src/yandil/dependency_filler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from typing import Any, Dict, Optional, Type, get_type_hints
 
 from yandil.container import Container, default_container
+from yandil.errors.dependency_not_found_error import DependencyNotFoundError
 
 
 class DependencyFiller:
     def __init__(self, container: Optional[Container] = None):
         if container is None:
             container = default_container
         self.__dependencies_container = container
 
     def fill(self, target_class: Type) -> None:
         target_class_base_init = target_class.__init__
         dependencies = self.__get_target_class_dependencies(target_class)
 
-        def init_with_dependencies(target_self) -> None:
-            target_class_base_init(target_self, **dependencies)
+        def init_with_dependencies(target_self, *args, **kwargs) -> None:
+            target_class_base_init(target_self, *args, **kwargs, **dependencies)
 
         target_class.__init__ = init_with_dependencies
 
     def __get_target_class_dependencies(self, target_class: Type) -> Dict[str, Any]:
         dependencies_dict = {}
         for argument_name, argument_type in get_type_hints(target_class.__init__).items():
-            dependencies_dict[argument_name] = self.__dependencies_container[argument_type]
+            try:
+                dependencies_dict[argument_name] = self.__dependencies_container[argument_type]
+            except DependencyNotFoundError:
+                pass
         return dependencies_dict
```

### Comparing `yandil-0.2.1/src/yandil/discovery/class_discovery.py` & `yandil-0.2.2/src/yandil/discovery/class_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/src/yandil/discovery/module_discovery.py` & `yandil-0.2.2/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.2.2/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/src/yandil/loaders/self_discover_dependency_loader.py` & `yandil-0.2.2/src/yandil/loaders/self_discover_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/src/yandil/typing_tools.py` & `yandil-0.2.2/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.1/PKG-INFO` & `yandil-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.2.1
+Version: 0.2.2
 Summary: Yet ANother Dependency Injection Library
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

