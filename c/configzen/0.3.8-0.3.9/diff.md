# Comparing `tmp/configzen-0.3.8.tar.gz` & `tmp/configzen-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.3.8.tar", max compression
+gzip compressed data, was "configzen-0.3.9.tar", max compression
```

## Comparing `configzen-0.3.8.tar` & `configzen-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.8/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.8/configzen/__main__.py
--rw-r--r--   0        0        0    69360 2023-06-21 19:39:30.254748 configzen-0.3.8/configzen/config.py
--rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.8/configzen/decorators.py
--rw-r--r--   0        0        0     3635 2023-06-21 19:36:00.617371 configzen-0.3.8/configzen/errors.py
--rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.8/configzen/field.py
--rw-r--r--   0        0        0    26257 2023-06-21 19:40:28.209184 configzen-0.3.8/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.8/configzen/py.typed
--rw-r--r--   0        0        0     4686 2023-06-21 19:36:00.610371 configzen-0.3.8/configzen/route.py
--rw-r--r--   0        0        0     1124 2023-06-21 19:40:00.222571 configzen-0.3.8/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.8/LICENSE
--rw-r--r--   0        0        0     1255 2023-06-21 19:42:27.934760 configzen-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.8/README.md
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.9/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.9/configzen/__main__.py
+-rw-r--r--   0        0        0    69581 2023-06-21 19:46:41.922698 configzen-0.3.9/configzen/config.py
+-rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.9/configzen/decorators.py
+-rw-r--r--   0        0        0     3635 2023-06-21 19:36:00.617371 configzen-0.3.9/configzen/errors.py
+-rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.9/configzen/field.py
+-rw-r--r--   0        0        0    26257 2023-06-21 19:40:28.209184 configzen-0.3.9/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.9/configzen/py.typed
+-rw-r--r--   0        0        0     4686 2023-06-21 19:36:00.610371 configzen-0.3.9/configzen/route.py
+-rw-r--r--   0        0        0     1124 2023-06-21 19:40:00.222571 configzen-0.3.9/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1255 2023-06-21 19:46:55.134889 configzen-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.9/README.md
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.9/PKG-INFO
```

### Comparing `configzen-0.3.8/configzen/__init__.py` & `configzen-0.3.9/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/configzen/__main__.py` & `configzen-0.3.9/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/configzen/config.py` & `configzen-0.3.9/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1886,14 +1886,20 @@
             If None, the whole configuration is returned.
 
         Returns
         -------
         The configuration accessor.
         """
         if route is None:
+            context = get_context_or_none(self)
+            self_at = None
+            if context is not None:
+                self_at = context.at
+            if self_at is not None:
+                return self_at
             return self
         return ConfigAt(self, None, route)
 
     @overload
     def get(
         self: ConfigModelT,
         route: None = None,
```

### Comparing `configzen-0.3.8/configzen/decorators.py` & `configzen-0.3.9/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/configzen/errors.py` & `configzen-0.3.9/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/configzen/field.py` & `configzen-0.3.9/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/configzen/processor.py` & `configzen-0.3.9/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/configzen/route.py` & `configzen-0.3.9/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/configzen/typedefs.py` & `configzen-0.3.9/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/LICENSE` & `configzen-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/pyproject.toml` & `configzen-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.3.8"
+version = "0.3.9"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.3.8/README.md` & `configzen-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.3.8/PKG-INFO` & `configzen-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.3.8
+Version: 0.3.9
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

