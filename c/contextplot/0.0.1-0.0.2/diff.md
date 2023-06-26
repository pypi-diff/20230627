# Comparing `tmp/contextplot-0.0.1.tar.gz` & `tmp/contextplot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contextplot-0.0.1.tar", last modified: Mon Jun 26 23:19:54 2023, max compression
+gzip compressed data, was "contextplot-0.0.2.tar", last modified: Mon Jun 26 23:44:30 2023, max compression
```

## Comparing `contextplot-0.0.1.tar` & `contextplot-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:19:54.040459 contextplot-0.0.1/
--rw-r--r--   0 josh       (502) staff       (20)     1071 2023-06-26 23:19:09.000000 contextplot-0.0.1/LICENSE
--rw-r--r--   0 josh       (502) staff       (20)      811 2023-06-26 23:19:54.040318 contextplot-0.0.1/PKG-INFO
--rw-r--r--   0 josh       (502) staff       (20)      280 2023-06-26 20:39:14.000000 contextplot-0.0.1/README.md
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:19:54.039377 contextplot-0.0.1/contextplot/
--rw-r--r--   0 josh       (502) staff       (20)     7013 2023-06-26 23:11:02.000000 contextplot-0.0.1/contextplot/__init__.py
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:19:54.040066 contextplot-0.0.1/contextplot.egg-info/
--rw-r--r--   0 josh       (502) staff       (20)      811 2023-06-26 23:19:54.000000 contextplot-0.0.1/contextplot.egg-info/PKG-INFO
--rw-r--r--   0 josh       (502) staff       (20)      239 2023-06-26 23:19:54.000000 contextplot-0.0.1/contextplot.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (502) staff       (20)        1 2023-06-26 23:19:54.000000 contextplot-0.0.1/contextplot.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (502) staff       (20)       25 2023-06-26 23:19:54.000000 contextplot-0.0.1/contextplot.egg-info/requires.txt
--rw-r--r--   0 josh       (502) staff       (20)       12 2023-06-26 23:19:54.000000 contextplot-0.0.1/contextplot.egg-info/top_level.txt
--rw-r--r--   0 josh       (502) staff       (20)      598 2023-06-26 23:17:50.000000 contextplot-0.0.1/pyproject.toml
--rw-r--r--   0 josh       (502) staff       (20)       38 2023-06-26 23:19:54.040503 contextplot-0.0.1/setup.cfg
--rw-r--r--   0 josh       (502) staff       (20)      334 2023-06-26 20:42:26.000000 contextplot-0.0.1/setup.py
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:44:30.482838 contextplot-0.0.2/
+-rw-r--r--   0 josh       (502) staff       (20)     1071 2023-06-26 23:19:09.000000 contextplot-0.0.2/LICENSE
+-rw-r--r--   0 josh       (502) staff       (20)      811 2023-06-26 23:44:30.482726 contextplot-0.0.2/PKG-INFO
+-rw-r--r--   0 josh       (502) staff       (20)      280 2023-06-26 20:39:14.000000 contextplot-0.0.2/README.md
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:44:30.481997 contextplot-0.0.2/contextplot/
+-rw-r--r--   0 josh       (502) staff       (20)     6834 2023-06-26 23:40:29.000000 contextplot-0.0.2/contextplot/__init__.py
+drwxr-xr-x   0 josh       (502) staff       (20)        0 2023-06-26 23:44:30.482568 contextplot-0.0.2/contextplot.egg-info/
+-rw-r--r--   0 josh       (502) staff       (20)      811 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (502) staff       (20)      239 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (502) staff       (20)        1 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (502) staff       (20)       25 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/requires.txt
+-rw-r--r--   0 josh       (502) staff       (20)       12 2023-06-26 23:44:30.000000 contextplot-0.0.2/contextplot.egg-info/top_level.txt
+-rw-r--r--   0 josh       (502) staff       (20)      598 2023-06-26 23:43:12.000000 contextplot-0.0.2/pyproject.toml
+-rw-r--r--   0 josh       (502) staff       (20)       38 2023-06-26 23:44:30.482875 contextplot-0.0.2/setup.cfg
+-rw-r--r--   0 josh       (502) staff       (20)      339 2023-06-26 23:43:17.000000 contextplot-0.0.2/setup.py
```

### Comparing `contextplot-0.0.1/LICENSE` & `contextplot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `contextplot-0.0.1/PKG-INFO` & `contextplot-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contextplot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Make Matplotlib plots in Jupyter notebooks using a context manager API
 Author: Josh Burkart
 Project-URL: Bug Tracker, https://gitlab.com/joshburkart/joshpyutil/-/issues
 Project-URL: Homepage, https://gitlab.com/joshburkart/joshpyutil
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contextplot-0.0.1/contextplot/__init__.py` & `contextplot-0.0.2/contextplot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,27 +30,26 @@
 ]
 
 
 @dataclasses.dataclass
 class _AxesWrapper:
 
     _ax: plt.Axes
-    _swallow_returns: bool = True
 
     def __getattr__(self, name: str) -> Any:
         method = getattr(self._ax, name)
 
-        @functools.wraps(method)
-        def wrapped_method(*args, **kwargs):
-            return_value = method(*args, **kwargs)
-            if not self._swallow_returns:
-                return return_value
-            return None
+        if callable(method):
 
-        return wrapped_method
+            @functools.wraps(method)
+            def wrapped_method(*args, **kwargs):
+                method(*args, **kwargs)
+
+            return wrapped_method
+        return method
 
 
 @dataclasses.dataclass
 class _ContextPlot:
     figure: plt.Figure
     axes: np.ndarray[plt.Axes]
     _active_flat_index: int = 0
@@ -74,18 +73,17 @@
         
         Automatically swallows anything returned by a method. For use with 
         `InteractiveShell.ast_node_interactivity = "all"`.
         """
         return _AxesWrapper(_ax=self.axes.flat[self._active_flat_index])
 
     @property
-    def ax_no_swallow(self):
-        """Use this to access (a wrapper around) the underlying `plt.Axes` object"""
-        return _AxesWrapper(_ax=self.axes.flat[self._active_flat_index],
-                            _swallow_returns=False)
+    def ax_raw(self):
+        """Use this to access the underlying `plt.Axes` object"""
+        return self.axes.flat[self._active_flat_index]
 
 
 @contextlib.contextmanager
 def context_plot(*args, size_inches=None, dpi=400, **kwargs):
     """A context manager-based API for making Matplotlib plots in Jupyter notebooks"""
     figure, axes = plt.subplots(*args,
                                 squeeze=False,
```

### Comparing `contextplot-0.0.1/contextplot.egg-info/PKG-INFO` & `contextplot-0.0.2/contextplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contextplot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Make Matplotlib plots in Jupyter notebooks using a context manager API
 Author: Josh Burkart
 Project-URL: Bug Tracker, https://gitlab.com/joshburkart/joshpyutil/-/issues
 Project-URL: Homepage, https://gitlab.com/joshburkart/joshpyutil
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contextplot-0.0.1/pyproject.toml` & `contextplot-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "Make Matplotlib plots in Jupyter notebooks using a context manager API"
 name = "contextplot"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.0.1"
+version = "0.0.2"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/joshburkart/joshpyutil/-/issues"
 "Homepage" = "https://gitlab.com/joshburkart/joshpyutil"
 
 [build-system]
 build-backend = "setuptools.build_meta"
```

