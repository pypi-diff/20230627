# Comparing `tmp/featurepy-0.2.4.tar.gz` & `tmp/featurepy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurepy-0.2.4.tar", max compression
+gzip compressed data, was "featurepy-0.2.5.tar", max compression
```

## Comparing `featurepy-0.2.4.tar` & `featurepy-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.2.4/LICENSE
--rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.2.4/README.md
--rw-r--r--   0        0        0      823 2023-06-26 22:08:53.427377 featurepy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-11 09:55:40.361310 featurepy-0.2.4/src/featurepy/__init__.py
--rw-r--r--   0        0        0     1529 2023-06-14 00:06:33.902940 featurepy-0.2.4/src/featurepy/feature_class.py
--rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.2.4/src/featurepy/flask/__init__.py
--rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.2.4/src/featurepy/flask/views.py
--rw-r--r--   0        0        0     3467 2023-06-21 09:40:58.948087 featurepy-0.2.4/src/featurepy/model_constraints.py
--rw-r--r--   0        0        0     1773 2023-06-18 14:41:26.107466 featurepy-0.2.4/src/featurepy/parametric_features.py
--rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.2.4/src/featurepy/scripts/__init__.py
--rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.2.4/src/featurepy/scripts/features.py
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 featurepy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.2.5/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.2.5/README.md
+-rw-r--r--   0        0        0      823 2023-06-26 22:35:39.875393 featurepy-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-11 09:55:40.361310 featurepy-0.2.5/src/featurepy/__init__.py
+-rw-r--r--   0        0        0     1428 2023-06-26 22:34:56.292604 featurepy-0.2.5/src/featurepy/feature_class.py
+-rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.2.5/src/featurepy/flask/__init__.py
+-rw-r--r--   0        0        0      230 2023-05-18 14:59:44.476705 featurepy-0.2.5/src/featurepy/flask/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1901 2023-05-18 14:59:44.477827 featurepy-0.2.5/src/featurepy/flask/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.2.5/src/featurepy/flask/views.py
+-rw-r--r--   0        0        0     3467 2023-06-21 09:40:58.948087 featurepy-0.2.5/src/featurepy/model_constraints.py
+-rw-r--r--   0        0        0     1773 2023-06-18 14:41:26.107466 featurepy-0.2.5/src/featurepy/parametric_features.py
+-rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.2.5/src/featurepy/scripts/__init__.py
+-rw-r--r--   0        0        0      202 2023-06-03 17:07:40.240249 featurepy-0.2.5/src/featurepy/scripts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1328 2023-06-03 17:07:40.240691 featurepy-0.2.5/src/featurepy/scripts/__pycache__/features.cpython-311.pyc
+-rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.2.5/src/featurepy/scripts/features.py
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 featurepy-0.2.5/PKG-INFO
```

### Comparing `featurepy-0.2.4/LICENSE` & `featurepy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.4/pyproject.toml` & `featurepy-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "featurepy"
-version = "0.2.4"
+version = "0.2.5"
 description = "Framework for building software product lines using feature-oriented programming (FOP) and aspect-oriented programming (AOP) in Python."
 authors = ["Adrian Wong <adrianwong227@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aspectlib = "^2.0.0"
```

### Comparing `featurepy-0.2.4/src/featurepy/feature_class.py` & `featurepy-0.2.5/src/featurepy/feature_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,51 +3,46 @@
 from functools import wraps
 from types import FunctionType
 
 import inspect
 
 
 def feature_method(func):
-    wraps(func)
-
+    @wraps(func)
     def wrapper(self, *args, **kwargs):
 
         cutpoint_aspects = self.aspects[func.__name__] if func.__name__ in self.aspects else {
         }
         result_func = func
         for cutpoint, aspects in cutpoint_aspects.items():
             base_func = result_func
-            # if isinstance(cutpoint, str):
-            #     cutpoint = eval(cutpoint)
 
             def weaved_func(self, *args, **kwargs):
                 with weave(cutpoint, aspects):
                     return base_func(self, *args, **kwargs)
 
             result_func = weaved_func
 
         return result_func(self, *args, **kwargs)
 
     return wrapper
 
 
 # TODO: weave aspects on methods
 def feature(cls):
-    wraps(cls)
-
     class Wrapper(cls):
         aspects = {}
 
         @classmethod
-        def register_aspect(clss, method, cutpoint, aspect, **kwargs):  # Missing options
+        def register_aspect(clss, method, cutpoint, *aspects, **kwargs):  # Missing options
             if method not in clss.aspects:
                 clss.aspects[method] = {}
             if cutpoint not in clss.aspects[method]:
                 clss.aspects[method][cutpoint] = []
-            clss.aspects[method][cutpoint].append(aspect)
+            clss.aspects[method][cutpoint].extend(aspects)
 
         def __init__(self, *args, **kwargs):
 
             super().__init__(*args, **kwargs)
 
     for name, function in inspect.getmembers(Wrapper, inspect.isfunction):
         setattr(Wrapper, name, feature_method(function))
```

### Comparing `featurepy-0.2.4/src/featurepy/flask/views.py` & `featurepy-0.2.5/src/featurepy/flask/views.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.4/src/featurepy/model_constraints.py` & `featurepy-0.2.5/src/featurepy/model_constraints.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.4/src/featurepy/parametric_features.py` & `featurepy-0.2.5/src/featurepy/parametric_features.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.4/PKG-INFO` & `featurepy-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurepy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Framework for building software product lines using feature-oriented programming (FOP) and aspect-oriented programming (AOP) in Python.
 Author: Adrian Wong
 Author-email: adrianwong227@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aspectlib (>=2.0.0,<3.0.0)
```

