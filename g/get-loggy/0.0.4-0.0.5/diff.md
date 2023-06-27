# Comparing `tmp/get-loggy-0.0.4.tar.gz` & `tmp/get-loggy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-loggy-0.0.4.tar", last modified: Fri Jul 15 04:16:16 2022, max compression
+gzip compressed data, was "get-loggy-0.0.5.tar", last modified: Tue Jun 27 05:49:52 2023, max compression
```

## Comparing `get-loggy-0.0.4.tar` & `get-loggy-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 04:16:16.229972 get-loggy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-07-15 04:16:08.000000 get-loggy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-07-15 04:16:16.229972 get-loggy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2994 2022-07-15 04:16:08.000000 get-loggy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 04:16:16.229972 get-loggy-0.0.4/get_loggy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-07-15 04:16:16.000000 get-loggy-0.0.4/get_loggy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-07-15 04:16:16.000000 get-loggy-0.0.4/get_loggy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 04:16:16.000000 get-loggy-0.0.4/get_loggy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-15 04:16:16.000000 get-loggy-0.0.4/get_loggy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 04:16:16.229972 get-loggy-0.0.4/loggy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 04:16:08.000000 get-loggy-0.0.4/loggy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-07-15 04:16:08.000000 get-loggy-0.0.4/loggy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6633 2022-07-15 04:16:08.000000 get-loggy-0.0.4/loggy/loggy.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-07-15 04:16:08.000000 get-loggy-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-15 04:16:16.229972 get-loggy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-07-15 04:16:08.000000 get-loggy-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 04:16:16.229972 get-loggy-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-07-15 04:16:08.000000 get-loggy-0.0.4/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-07-15 04:16:08.000000 get-loggy-0.0.4/test/test_loggy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:49:52.060299 get-loggy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 05:49:43.000000 get-loggy-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-27 05:49:52.060299 get-loggy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-27 05:49:43.000000 get-loggy-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:49:52.060299 get-loggy-0.0.5/get_loggy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-27 05:49:52.000000 get-loggy-0.0.5/get_loggy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 05:49:52.000000 get-loggy-0.0.5/get_loggy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:49:52.000000 get-loggy-0.0.5/get_loggy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 05:49:52.000000 get-loggy-0.0.5/get_loggy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:49:52.060299 get-loggy-0.0.5/loggy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:49:43.000000 get-loggy-0.0.5/loggy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-27 05:49:43.000000 get-loggy-0.0.5/loggy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-27 05:49:43.000000 get-loggy-0.0.5/loggy/loggy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 05:49:43.000000 get-loggy-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:49:52.060299 get-loggy-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-27 05:49:43.000000 get-loggy-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:49:52.060299 get-loggy-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-27 05:49:43.000000 get-loggy-0.0.5/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-27 05:49:43.000000 get-loggy-0.0.5/test/test_loggy.py
```

### Comparing `get-loggy-0.0.4/LICENSE` & `get-loggy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `get-loggy-0.0.4/PKG-INFO` & `get-loggy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-loggy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple logging utility.
 Home-page: https://github.com/mattdood/loggy
 Author: Matthew Wimberly
 Author-email: matthew.wimb@gmail.com
 Project-URL: Bug Tracker, https://github.com/mattdood/loggy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `get-loggy-0.0.4/README.md` & `get-loggy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `get-loggy-0.0.4/get_loggy.egg-info/PKG-INFO` & `get-loggy-0.0.5/get_loggy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-loggy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple logging utility.
 Home-page: https://github.com/mattdood/loggy
 Author: Matthew Wimberly
 Author-email: matthew.wimb@gmail.com
 Project-URL: Bug Tracker, https://github.com/mattdood/loggy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `get-loggy-0.0.4/loggy/exceptions.py` & `get-loggy-0.0.5/loggy/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import functools
-from typing import List
+from typing import Any, List
 
 
 class MutuallyExclusiveArgumentsError(Exception):
     """Arguments that are mutually exclusive."""
     def __init__(self, kwarg_names) -> None:
         err = f"These groups or arguments are mutually exclusive: {', '.join(kw for kw in kwarg_names)}"
         super().__init__(err)
 
 
-def exclusive_args(kwarg_names: List[str]):
+def exclusive_args(kwarg_names: List[str]) -> Any:
     """Mutually exclusive argument wrapper.
 
     Takes a list of arguments then compares them to
     what was passed in.
 
     Functions can be wrapped multiple times with different
     combinations of mutually exclusive arguments.
```

### Comparing `get-loggy-0.0.4/loggy/loggy.py` & `get-loggy-0.0.5/loggy/loggy.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,19 @@
             Example: `{"filename": "sample.log", "mode": "a"}`
 
     Returns:
         logger (Logger): A log class with access to `critical`, `debug`, `error`,
             `info`, and `warning` level logging.
     """
     logger = logging.getLogger(__package__)
+
+    # Remove any existing handlers
+    for handler in logger.handlers:
+        logger.removeHandler(handler)
+
     logger.setLevel(log_level.upper())
 
     # Use an append-only file handler if filename supplied
     if log_file:
         handler = logging.FileHandler(**log_file if log_file else dict())
         handler.setFormatter(LogFormatter(*log_format if log_format else LOG_FORMAT))
 
@@ -176,9 +181,10 @@
             LogFormatter(
                 *log_format if log_format else LOG_FORMAT,
                 use_color=use_color
             )
         )
 
     logger.addHandler(handler)
+
     return logger
```

### Comparing `get-loggy-0.0.4/setup.py` & `get-loggy-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="get-loggy",
-    version="0.0.4",
+    version="0.0.5",
     author="Matthew Wimberly",
     author_email="matthew.wimb@gmail.com",
     description="A simple logging utility.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattdood/loggy",
     project_urls={
```

### Comparing `get-loggy-0.0.4/test/test_exceptions.py` & `get-loggy-0.0.5/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `get-loggy-0.0.4/test/test_loggy.py` & `get-loggy-0.0.5/test/test_loggy.py`

 * *Files identical despite different names*

