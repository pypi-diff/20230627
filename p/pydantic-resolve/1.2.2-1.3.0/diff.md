# Comparing `tmp/pydantic_resolve-1.2.2.tar.gz` & `tmp/pydantic_resolve-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.2.2.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.3.0.tar", max compression
```

## Comparing `pydantic_resolve-1.2.2.tar` & `pydantic_resolve-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.2.2/LICENSE
--rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.2.2/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.2.2/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2271 2023-06-21 14:55:58.477090 pydantic_resolve-1.2.2/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.2.2/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     4927 2023-06-21 15:02:54.668646 pydantic_resolve-1.2.2/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     3916 2023-06-20 06:16:54.008785 pydantic_resolve-1.2.2/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-06-21 15:05:32.966535 pydantic_resolve-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.2.2/README.md
--rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.3.0/LICENSE
+-rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.3.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.3.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2271 2023-06-21 14:55:58.477090 pydantic_resolve-1.3.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.3.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     6117 2023-06-27 16:04:17.836316 pydantic_resolve-1.3.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     3916 2023-06-20 06:16:54.008785 pydantic_resolve-1.3.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-06-27 16:03:58.731975 pydantic_resolve-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.3.0/README.md
+-rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.3.0/PKG-INFO
```

### Comparing `pydantic_resolve-1.2.2/LICENSE` & `pydantic_resolve-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.2/pydantic_resolve/__init__.py` & `pydantic_resolve-1.3.0/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.2/pydantic_resolve/core.py` & `pydantic_resolve-1.3.0/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.2/pydantic_resolve/resolver.py` & `pydantic_resolve-1.3.0/pydantic_resolve/resolver.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,36 +26,60 @@
 
 T = TypeVar("T")
 
 class Resolver:
     """
     Entrypoint of a resolve action
     """
-    def __init__(self, loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None, ensure_type=False):
+    def __init__(
+            self, 
+            loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None, 
+            loader_instances: Optional[Dict[Any, Any]] = None,
+            ensure_type=False):
         self.ctx = contextvars.ContextVar('pydantic_resolve_internal_context', default={})
+
+        # for dataloader which has class attributes, you can assign the value at here
         self.loader_filters_ctx = contextvars.ContextVar('pydantic_resolve_internal_filter', default=loader_filters or {})
+
+        # now you can pass your loader instance, Resolver will check isinstance
+        if loader_instances and self.validate_instance(loader_instances):
+            self.loader_instances = loader_instances
+        else:
+            self.loader_instances = None
+
         self.ensure_type = ensure_type
     
+    def validate_instance(self, loader_instances: Dict[Any, Any]):
+        for cls, loader in loader_instances.items():
+            if not issubclass(cls, DataLoader):
+                raise AttributeError(f'{cls.__name__} must be subclass of DataLoader')
+            if not isinstance(loader, cls):
+                raise AttributeError(f'{loader.__name__} is not instance of {cls.__name__}')
+        return True
 
     def exec_method(self, method):
         signature = inspect.signature(method)
         params = {}
 
         # manage the creation of loader instances
         for k, v in signature.parameters.items():
             if isinstance(v.default, Depends):
                 # Base: DataLoader or batch_load_fn
                 Base = v.default.dependency
 
+                # check loader_instance first, if has predefined loader instance, just use it.
+                if self.loader_instances and self.loader_instances.get(Base):
+                    loader = self.loader_instances.get(Base)
+                    params[k] = loader
+                    continue
+
                 # module.kls to avoid same kls name from different module
                 cache_key = f'{v.default.dependency.__module__}.{v.default.dependency.__name__}'
-
                 cache_provider = self.ctx.get()
                 hit = cache_provider.get(cache_key, None)
-
                 if hit:
                     loader = hit
                 else:
                     # create loader instance 
                     if isclass(Base):
                         # if extra transform provides
                         loader = Base()
```

### Comparing `pydantic_resolve-1.2.2/pydantic_resolve/util.py` & `pydantic_resolve-1.3.0/pydantic_resolve/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.2/pyproject.toml` & `pydantic_resolve-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.2.2"
+version = "1.3.0"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.2.2/README.md` & `pydantic_resolve-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.2/PKG-INFO` & `pydantic_resolve-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.2.2
+Version: 1.3.0
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
```

