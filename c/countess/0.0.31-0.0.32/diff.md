# Comparing `tmp/countess-0.0.31.tar.gz` & `tmp/countess-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.31.tar", last modified: Wed Jun 14 10:54:51 2023, max compression
+gzip compressed data, was "countess-0.0.32.tar", last modified: Tue Jun 27 02:52:54 2023, max compression
```

## Comparing `countess-0.0.31.tar` & `countess-0.0.32.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 10:54:51.116999 countess-0.0.31/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.31/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-05-25 01:44:18.000000 countess-0.0.31/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-06-14 10:54:51.116999 countess-0.0.31/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-06-14 10:53:02.000000 countess-0.0.31/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 10:54:51.112999 countess-0.0.31/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-06-14 10:53:09.000000 countess-0.0.31/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 10:54:51.112999 countess-0.0.31/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.31/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      415 2023-05-25 01:44:18.000000 countess-0.0.31/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4157 2023-05-25 01:44:18.000000 countess-0.0.31/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-05-25 01:44:18.000000 countess-0.0.31/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    16574 2023-06-14 10:48:54.000000 countess-0.0.31/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7480 2023-06-14 04:42:03.000000 countess-0.0.31/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13676 2023-06-14 05:39:47.000000 countess-0.0.31/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 10:54:51.112999 countess-0.0.31/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.31/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18816 2023-06-14 04:38:55.000000 countess-0.0.31/countess/gui/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-05-25 01:44:18.000000 countess-0.0.31/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    15051 2023-06-14 04:42:03.000000 countess-0.0.31/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14244 2023-06-14 04:42:03.000000 countess-0.0.31/countess/gui/tabular.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    20013 2023-06-14 04:42:03.000000 countess-0.0.31/countess/gui/tree.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 10:54:51.116999 countess-0.0.31/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.31/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5851 2023-06-14 05:42:19.000000 countess-0.0.31/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-06-14 04:38:55.000000 countess-0.0.31/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1642 2023-06-14 04:42:03.000000 countess-0.0.31/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2160 2023-06-01 00:52:52.000000 countess-0.0.31/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4722 2023-06-14 05:37:27.000000 countess-0.0.31/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-05-25 01:44:18.000000 countess-0.0.31/countess/plugins/hdf5.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3287 2023-06-14 04:42:03.000000 countess-0.0.31/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-05-25 01:44:18.000000 countess-0.0.31/countess/plugins/log_score.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2562 2023-05-25 01:44:18.000000 countess-0.0.31/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4165 2023-06-14 04:42:03.000000 countess-0.0.31/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1560 2023-05-31 03:55:05.000000 countess-0.0.31/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6552 2023-06-14 05:20:24.000000 countess-0.0.31/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2194 2023-06-14 04:38:55.000000 countess-0.0.31/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2238 2023-06-14 04:38:55.000000 countess-0.0.31/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.31/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 10:54:51.116999 countess-0.0.31/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.31/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    12859 2023-05-25 01:44:18.000000 countess-0.0.31/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 10:54:51.112999 countess-0.0.31/countess.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-06-14 10:54:51.000000 countess-0.0.31/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1089 2023-06-14 10:54:51.000000 countess-0.0.31/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-06-14 10:54:51.000000 countess-0.0.31/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      997 2023-06-14 10:54:51.000000 countess-0.0.31/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      201 2023-06-14 10:54:51.000000 countess-0.0.31/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-06-14 10:54:51.000000 countess-0.0.31/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2809 2023-05-26 06:01:26.000000 countess-0.0.31/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-06-14 10:54:51.116999 countess-0.0.31/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.31/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-14 10:54:51.116999 countess-0.0.31/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      480 2023-05-25 01:44:18.000000 countess-0.0.31/tests/test_gui.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-27 02:52:54.622594 countess-0.0.32/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.32/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-05-25 01:44:18.000000 countess-0.0.32/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3476 2023-06-27 02:52:54.622594 countess-0.0.32/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-06-27 02:52:04.000000 countess-0.0.32/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-27 02:52:54.618594 countess-0.0.32/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-06-27 02:52:09.000000 countess-0.0.32/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-27 02:52:54.618594 countess-0.0.32/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.32/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      415 2023-05-25 01:44:18.000000 countess-0.0.32/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4157 2023-05-25 01:44:18.000000 countess-0.0.32/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2032 2023-06-26 03:46:06.000000 countess-0.0.32/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    16739 2023-06-26 03:46:06.000000 countess-0.0.32/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7481 2023-06-26 04:37:01.000000 countess-0.0.32/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13984 2023-06-27 00:42:13.000000 countess-0.0.32/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-27 02:52:54.618594 countess-0.0.32/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.32/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18816 2023-06-27 00:42:13.000000 countess-0.0.32/countess/gui/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-05-25 01:44:18.000000 countess-0.0.32/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    15108 2023-06-27 00:42:13.000000 countess-0.0.32/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14241 2023-06-22 05:40:05.000000 countess-0.0.32/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20013 2023-06-14 04:42:03.000000 countess-0.0.32/countess/gui/tree.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-27 02:52:54.622594 countess-0.0.32/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.32/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6181 2023-06-27 01:16:32.000000 countess-0.0.32/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-06-27 00:42:13.000000 countess-0.0.32/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1889 2023-06-27 00:42:13.000000 countess-0.0.32/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2160 2023-06-01 00:52:52.000000 countess-0.0.32/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4722 2023-06-27 00:42:13.000000 countess-0.0.32/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-05-25 01:44:18.000000 countess-0.0.32/countess/plugins/hdf5.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3300 2023-06-27 00:42:13.000000 countess-0.0.32/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-05-25 01:44:18.000000 countess-0.0.32/countess/plugins/log_score.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2562 2023-05-25 01:44:18.000000 countess-0.0.32/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4165 2023-06-27 00:42:28.000000 countess-0.0.32/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1591 2023-06-22 10:07:37.000000 countess-0.0.32/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6572 2023-06-27 00:43:08.000000 countess-0.0.32/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2194 2023-06-27 00:42:13.000000 countess-0.0.32/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2869 2023-06-27 00:42:13.000000 countess-0.0.32/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.32/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-27 02:52:54.622594 countess-0.0.32/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.32/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12859 2023-06-22 04:09:14.000000 countess-0.0.32/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-27 02:52:54.618594 countess-0.0.32/countess.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3476 2023-06-27 02:52:54.000000 countess-0.0.32/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1089 2023-06-27 02:52:54.000000 countess-0.0.32/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-06-27 02:52:54.000000 countess-0.0.32/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      997 2023-06-27 02:52:54.000000 countess-0.0.32/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      201 2023-06-27 02:52:54.000000 countess-0.0.32/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-06-27 02:52:54.000000 countess-0.0.32/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2808 2023-06-26 03:46:06.000000 countess-0.0.32/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-06-27 02:52:54.622594 countess-0.0.32/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.32/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-27 02:52:54.622594 countess-0.0.32/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      480 2023-05-25 01:44:18.000000 countess-0.0.32/tests/test_gui.py
```

### Comparing `countess-0.0.31/LICENSE.txt` & `countess-0.0.32/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/PKG-INFO` & `countess-0.0.32/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.31
+Version: 0.0.32
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.31
+# CountESS 0.0.32
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.31/README.md` & `countess-0.0.32/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.31
+# CountESS 0.0.32
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.31/countess/core/config.py` & `countess-0.0.32/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/core/logger.py` & `countess-0.0.32/countess/core/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,17 @@
         self.log("warning", message, detail)
 
     def error(self, message: str, detail: Optional[str] = None):
         """Log a message at level error"""
         self.log("error", message, detail)
 
     def exception(self, exception: Exception):
-        self.error(str(exception), detail="".join(traceback.format_exception(exception)))
+        # Slightly odd calling to maintain compatibility with 3.9 and 3.10
+        message = traceback.format_exception(None, value=exception, tb=None)
+        self.error(str(exception), detail="".join(message))
 
     def clear(self):
         """Clear logs (if possible)"""
         return None
 
 
 class ConsoleLogger(Logger):
```

### Comparing `countess-0.0.31/countess/core/parameters.py` & `countess-0.0.32/countess/core/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import hashlib
 import os.path
 import re
-from typing import Any, Iterable, Mapping, Optional, Type
+from typing import Any, Iterable, Mapping, Optional, Type, Union
 
 PARAM_DIGEST_HASH = "sha256"
 
 
 class BaseParam:
     """Represents the parameters which can be set on a plugin."""
 
@@ -210,15 +210,15 @@
     file_types = [("Any", "*")]
 
     def __init__(self, label: str, value=None, read_only: bool = False, file_types=None):
         super().__init__(label, value, read_only)
         if file_types is not None:
             self.file_types = file_types
 
-    def clean_value(self, value: str | tuple | list, file_types=None):
+    def clean_value(self, value: Union[str, tuple, list], file_types=None):
         try:
             return os.path.relpath(str(value))
         except ValueError:
             return value
 
 
 class ChoiceParam(BaseParam):
@@ -343,14 +343,20 @@
 
     def set_choices(self, choices: Iterable[str]):
         super().set_choices([self.NONE_VALUE] + list(choices))
 
     def is_none(self):
         return self.value == self.NONE_VALUE
 
+    def get_column(self, df):
+        if self.value == self.NONE_VALUE:
+            return None
+        else:
+            return super().get_column(df)
+
 
 class MultipleChoiceParam(ChoiceParam):
     pass
 
 
 class ArrayParam(BaseParam):
     """An ArrayParam contains zero or more copies of `param`, which can be a
```

### Comparing `countess-0.0.31/countess/core/pipeline.py` & `countess-0.0.32/countess/core/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field
 from typing import Any, Optional
 
 from countess.core.logger import Logger
 from countess.core.plugins import BasePlugin, get_plugin_classes
 
-PRERUN_ROW_LIMIT = 10000
+PRERUN_ROW_LIMIT = 100000
 
 
 @dataclass
 class PipelineNode:
     name: str
     plugin: Optional[BasePlugin] = None
     position: Optional[tuple[float, float]] = None
```

### Comparing `countess-0.0.31/countess/core/plugins.py` & `countess-0.0.32/countess/core/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import hashlib
 import importlib
 import importlib.metadata
 import logging
 import os.path
 import sys
 from collections.abc import Mapping, MutableMapping
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from countess.core.logger import Logger
 from countess.core.parameters import (
     ArrayParam,
@@ -39,15 +39,22 @@
 )
 
 PRERUN_ROW_LIMIT = 100
 
 
 def get_plugin_classes():
     plugin_classes = set()
-    for ep in importlib.metadata.entry_points(group="countess_plugins"):
+    try:
+        # Python >= 3.10
+        entry_points = importlib.metadata.entry_points().select(group="countess_plugins")
+    except AttributeError:
+        # Python < 3.10
+        entry_points = importlib.metadata.entry_points()["countess_plugins"]
+
+    for ep in entry_points:
         try:
             plugin_class = ep.load()
         except (ModuleNotFoundError, ImportError, NotImplementedError) as exc:
             logging.warning("%s could not be loaded: %s", ep, exc)
             continue
 
         if issubclass(plugin_class, BasePlugin):
@@ -68,14 +75,15 @@
 class BasePlugin:
     """Base class for all plugins.  Plugins exist as entrypoints, but also
     PluginManager checks that plugins subclass this class before accepting them
     as plugins."""
 
     name: str = ""
     description: str = ""
+    additional: str = ""
     link: Optional[str] = None
 
     parameters: MutableMapping[str, BaseParam] = {}
 
     @property
     def version(self) -> str:
         return sys.modules[self.__module__].VERSION
@@ -125,20 +133,20 @@
         pipeline is running."""
         raise NotImplementedError(f"{self.__class__}.run()")
 
     def add_parameter(self, name: str, param: BaseParam):
         self.parameters[name] = param.copy()
         return self.parameters[name]
 
-    def set_parameter(self, key: str, value: bool | int | float | str, base_dir: str = "."):
+    def set_parameter(self, key: str, value: Union[bool, int, float, str], base_dir: str = "."):
         param = self.parameters
         for k in key.split("."):
             # XXX types are a mess here
             param = param[k]  # type: ignore
-        if isinstance(param, (FileParam, FileSaveParam)):
+        if isinstance(param, (FileParam, FileSaveParam)) and value is not None:
             assert isinstance(value, str)
             param.value = os.path.join(base_dir, value)
         else:
             param.value = value  # type: ignore
 
     def get_parameters(self, base_dir="."):
         for key, parameter in self.parameters.items():
@@ -212,43 +220,45 @@
     input_columns: list[str] = []
     input_dtypes: list[str] = []
 
     def prepare_df(self, df: pd.DataFrame, logger: Logger):
         assert isinstance(df, pd.DataFrame)
         if hasattr(df.index, "dtypes"):
             self.input_columns = [n for n in df.index.names if n] + list(df.columns)
-            self.input_dtypes = [d for d, n in zip(df.index.dtypes, df.index.names) if n] + list(df.dtypes)
+            self.input_dtypes = [d for d, n in zip(df.index.dtypes, df.index.names) if n] + list(
+                df.dtypes
+            )
         elif df.index.name:
             self.input_columns = [df.index.name] + list(df.columns)
             self.input_dtypes = [df.index.dtype] + list(df.dtypes)
         else:
             self.input_columns = list(df.columns)
             self.input_dtypes = list(df.dtypes)
 
         for p in self.parameters.values():
             p.set_column_choices(self.input_columns)
 
     # XXX prepare and run handle multiple inputs differntly?
 
     def prepare(
         self,
-        data: pd.DataFrame | Mapping[str, pd.DataFrame],
+        data: Union[pd.DataFrame, Mapping[str, pd.DataFrame]],
         logger: Logger,
     ) -> bool:
         if isinstance(data, Mapping):
             data = pd.concat(data.values())
 
         return self.prepare_df(data, logger)
 
     def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
         raise NotImplementedError(f"Implement {self.__class__.__name__}.run_df()")
 
     def run(
         self,
-        data: pd.DataFrame | Mapping[str, pd.DataFrame],
+        data: Union[pd.DataFrame, Mapping[str, pd.DataFrame]],
         logger: Logger,
         row_limit: Optional[int] = None,
     ) -> pd.DataFrame:
         assert isinstance(logger, Logger)
         assert row_limit is None or isinstance(row_limit, int)
 
         logger.progress("Starting", 0)
```

### Comparing `countess-0.0.31/countess/gui/config.py` & `countess-0.0.32/countess/gui/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/gui/logger.py` & `countess-0.0.32/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/gui/main.py` & `countess-0.0.32/countess/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         self.columnconfigure(0, weight=1)
 
         label_frame = tk.LabelFrame(self, text=title, padx=10, pady=10)
         label_frame.grid(row=1, column=0, sticky=tk.EW, padx=10, pady=10)
 
         for n, plugin_class in enumerate(plugin_classes):
-            label_text = plugin_class.description.split(". ")[0].strip()
+            label_text = plugin_class.description
             tk.Button(
                 label_frame,
                 text=plugin_class.name,
                 command=lambda plugin_class=plugin_class: callback(plugin_class),
             ).grid(row=n + 1, column=0, sticky=tk.EW)
             tk.Label(label_frame, text=label_text).grid(row=n + 1, column=1, sticky=tk.W, padx=10)
 
@@ -100,14 +100,16 @@
             else:
                 self.notes_widget = tk.Button(
                     self.frame, text="add notes", command=self.on_add_notes
                 )
                 self.notes_widget.grid(row=2, columnspan=2, padx=10, pady=5)
 
             descr = re.sub(r"\s+", " ", self.node.plugin.description)
+            if self.node.plugin.additional:
+                descr += "\n" + re.sub(r"\s+", " ", self.node.plugin.additional)
 
             self.label["text"] = "%s %s — %s" % (
                 self.node.plugin.name,
                 self.node.plugin.version,
                 descr,
             )
             if self.node.plugin.link:
@@ -200,16 +202,15 @@
         self.config_change_task = self.frame.after(500, self.config_change_task_callback)
 
     def config_change_task_callback(self):
         self.config_change_task = None
         self.logger.clear()
         self.logger_subframe.grid(row=3, sticky=tk.NSEW)
         self.node.prerun(self.logger)
-        if self.node.result is not None:
-            self.show_preview_subframe()
+        self.show_preview_subframe()
         self.configurator.update()
         self.logger_subframe.after(5000, self.config_change_task_callback_2)
         self.change_callback(self.node)
 
     def config_change_task_callback_2(self):
         if self.logger.count == 0:
             self.logger_subframe.grid_forget()
```

### Comparing `countess-0.0.31/countess/gui/tabular.py` & `countess-0.0.32/countess/gui/tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,33 +317,33 @@
 
         for cw in self.columns:
             cw.tag_delete("xsel")
 
         if r1 != r2:
             self.select_rows = (r1, r2)
             for cw in self.columns:
-                cw.tag_add("xsel", f"{r1}.0", f"{r2}.end")
+                cw.tag_add("xsel", f"{r1}.0", f"{r2+1}.0")
                 cw.tag_config("xsel", background="lightgrey")
         else:
             self.select_rows = None
 
     def __column_copy(self, event):
         # If this was a multi-row selection, then replace
         # the copy buffer with a copy of those whole rows.
         if not self.select_rows:
             return  # not multi-row, keep it.
 
         r1, r2 = self.select_rows
         df = self.dataframe.iloc[self.offset + r1 - 1 : self.offset + r2]
         buf = io.StringIO()
-        df.to_csv(buf, sep="\t", newline="\n")
+        df.to_csv(buf, sep="\t")
 
         # XXX very cheesy, but self.clipboard_append() etc didn't
         # seem to work, so this is a terrible workaround ... dump the
         # TSV into a new tk.Text, select the whole thing and copy it
         # into the clipboard.
         top = tk.Toplevel()
         text = tk.Text(top)
-        text.insert(tk.END, buf)
+        text.insert(tk.END, buf.getvalue())
         text.tag_add("sel", "1.0", tk.END)
         text.event_generate("<<Copy>>")
         top.destroy()
```

### Comparing `countess-0.0.31/countess/gui/tree.py` & `countess-0.0.32/countess/gui/tree.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/plugins/csv.py` & `countess-0.0.32/countess/plugins/csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,19 @@
     """Load CSV files"""
 
     name = "CSV Load"
     description = "Loads data from CSV or similar delimited text files and assigns types to columns"
     link = "https://countess-project.github.io/CountESS/plugins/#csv-reader"
     version = VERSION
 
-    file_types = [("CSV", "*.csv"), ("TSV", "*.tsv"), ("TXT", "*.txt")]
+    file_types = [
+        ("CSV", "*.csv *.csv.gz *.csv.bz2"),
+        ("TSV", "*.tsv *.tsv.gz *.tsv.bz2"),
+        ("TXT", "*.txt *.txt.gz *.txt.bz2"),
+    ]
 
     parameters = {
         "delimiter": ChoiceParam("Delimiter", ",", choices=[",", ";", "TAB", "|", "WHITESPACE"]),
         "quoting": ChoiceParam(
             "Quoting", "None", choices=["None", "Double-Quote", "Quote with Escape"]
         ),
         "comment": ChoiceParam("Comment", "None", choices=["None", "#", ";"]),
@@ -165,15 +169,21 @@
         filename = self.parameters["filename"].value
         sep = self.parameters["delimiter"].value
         if sep == "TAB":
             sep = "\t"
         elif sep == "SPACE":
             sep = " "
 
+        has_named_index = (data.index.name is not None) or (
+            hasattr(data.index, "names") and data.index.names[0] is not None
+        )
+
         options = {
+            "header": self.parameters["header"].value,
+            "index": has_named_index,
             "sep": sep,
             "quoting": csv.QUOTE_NONNUMERIC
             if self.parameters["quoting"].value
             else csv.QUOTE_MINIMAL,
         }
 
         if row_limit is None:
```

### Comparing `countess-0.0.31/countess/plugins/data_table.py` & `countess-0.0.32/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/plugins/fastq.py` & `countess-0.0.32/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/plugins/group_by.py` & `countess-0.0.32/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/plugins/hdf5.py` & `countess-0.0.32/countess/plugins/hdf5.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/plugins/join.py` & `countess-0.0.32/countess/plugins/join.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Mapping, MutableMapping
-from typing import Optional
+from typing import Optional, Union
 
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
 from countess.core.parameters import ArrayParam, BooleanParam, ChoiceParam, MultiParam
 from countess.core.plugins import PandasBasePlugin
@@ -76,15 +76,15 @@
         elif ip1.required.value:
             join_how = "left"
         elif ip2.required.value:
             join_how = "right"
         else:
             join_how = "outer"
 
-        join_params: MutableMapping[str, str | bool] = {
+        join_params: MutableMapping[str, Union[str, bool]] = {
             "how": join_how,
         }
 
         dfs = list(data.values())
 
         if not ip1.join_on.value or ip1.join_on.value == INDEX:
             join_params["left_index"] = True
```

### Comparing `countess-0.0.31/countess/plugins/mutagenize.py` & `countess-0.0.32/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/plugins/pivot.py` & `countess-0.0.32/countess/plugins/pivot.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/plugins/python.py` & `countess-0.0.32/countess/plugins/python.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 # (eg: classes, methods, functions) won't.
 
 SIMPLE_TYPES = set((bool, int, float, str, tuple, list))
 
 
 class PythonPlugin(PandasTransformPlugin):
     name = "Python Code"
-    description = """
-        Apply python code to each row.
+    description = "Apply python code to each row."
+    additional = """
         Columns are mapped to local variables and back.
-        "__index" is set to the index value.
         If you assign to a variable called "__filter",
         only rows where that value is true will be kept.
     """
 
     version = VERSION
 
     parameters = {"code": TextParam("Python Code")}
@@ -34,14 +33,15 @@
         code_object = compile(self.parameters["code"].value, "<PythonPlugin>", mode="exec")
 
         def _process(row):
             row_dict = dict(row)
             exec(code_object, {}, row_dict)  # pylint: disable=exec-used
             return dict((k, v) for k, v in row_dict.items() if type(v) in SIMPLE_TYPES)
 
-        dfo = df.assign(__index=df.index)
+        # XXX It'd be nice to do this without resetting the index
+        dfo = df.reset_index(drop=False)
         dfo = dfo.apply(_process, axis=1, result_type="expand")
 
         if "__filter" in dfo.columns:
             dfo = dfo.query("__filter").drop(columns="__filter")
 
         return dfo
```

### Comparing `countess-0.0.31/countess/plugins/regex.py` & `countess-0.0.32/countess/plugins/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,18 @@
             df = df.set_index(index_names)
 
         return df
 
 
 class RegexReaderPlugin(PandasInputPlugin):
     name = "Regex Reader"
-    description = """Loads arbitrary data from line-delimited files, applying a regular expression
-      to each line to extract fields.  If you're trying to read generic CSV or TSV files, use the CSV
-      plugin instead as it handles escaping correctly."""
+    description = "Loads arbitrary data from line-delimited files"
+    additional = """Applies a regular expression to each line to extract fields.
+        If you're trying to read generic CSV or TSV files, use the CSV plugin
+        instead as it handles escaping correctly."""
     link = "https://countess-project.github.io/CountESS/plugins/#regex-reader"
     version = VERSION
 
     file_types = [("CSV", "*.csv"), ("TXT", "*.txt")]
 
     parameters = {
         "regex": StringParam("Regular Expression", "(.*)"),
```

### Comparing `countess-0.0.31/countess/plugins/sequence.py` & `countess-0.0.32/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess/plugins/variant.py` & `countess-0.0.32/countess/plugins/variant.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,80 @@
-from typing import Optional
-
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
-from countess.core.parameters import BooleanParam, ColumnChoiceParam, IntegerParam, StringParam
+from countess.core.parameters import (
+    BooleanParam,
+    ColumnChoiceParam,
+    ColumnOrNoneChoiceParam,
+    IntegerParam,
+    StringParam,
+)
 from countess.core.plugins import PandasTransformPlugin
 from countess.utils.variant import find_variant_string
 
 
-def process_row(var_seq: str, ref_seq: str, max_mutations: int, logger: Logger) -> Optional[str]:
-    try:
-        return find_variant_string("g.", ref_seq, var_seq, max_mutations)
-    except ValueError as exc:
-        logger.warning(str(exc))
-        return None
-
-
 class VariantPlugin(PandasTransformPlugin):
     """Turns a DNA sequence into a HGVS variant code"""
 
     name = "Variant Translator"
     description = "Turns a DNA sequence into a HGVS variant code"
     version = VERSION
     link = "https://countess-project.github.io/CountESS/plugins/#variant"
 
     parameters = {
         "column": ColumnChoiceParam("Input Column", "sequence"),
-        "sequence": StringParam("Reference Sequence"),
+        "reference": ColumnOrNoneChoiceParam("Reference Column"),
+        "sequence": StringParam("*OR* Reference Sequence"),
         "auto": BooleanParam("Automatic Reference Sequence?", False),
         "output": StringParam("Output Column", "variant"),
         "max_mutations": IntegerParam("Max Mutations", 10),
         "drop": BooleanParam("Drop unidentified variants", False),
     }
 
     def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
         assert isinstance(self.parameters["column"], ColumnChoiceParam)
+        assert isinstance(self.parameters["reference"], ColumnChoiceParam)
         assert isinstance(self.parameters["sequence"], StringParam)
         assert isinstance(self.parameters["output"], StringParam)
         assert isinstance(self.parameters["max_mutations"], IntegerParam)
 
         dfo = df.copy()
 
         column = self.parameters["column"].get_column(df)
+        reference = self.parameters["reference"].get_column(df)
         output = self.parameters["output"].value
 
         if self.parameters["auto"].value:
             value = pd.Series.mode(column)[0]
             self.parameters["sequence"].value = value
 
-        sequence = self.parameters["sequence"].value
         max_mutations = self.parameters["max_mutations"].value
 
-        dfo[output] = column.apply(process_row, args=(sequence, max_mutations, logger))
+        if reference is not None:
+
+            def func(ref_var):
+                try:
+                    return find_variant_string("g.", ref_var[0], ref_var[1], max_mutations)
+                except ValueError as exc:
+                    logger.warning(str(exc))
+                    return None
+
+            dfo[output] = pd.DataFrame([column, reference]).apply(
+                func, raw=True, result_type="reduce"
+            )
+        else:
+            ref_str = self.parameters["sequence"].value
+
+            def func(var_str):
+                try:
+                    return find_variant_string("g.", ref_str, var_str, max_mutations)
+                except ValueError as exc:
+                    logger.warning(str(exc))
+                    return None
+
+            dfo[output] = column.apply(func)
 
         if self.parameters["drop"].value:
             dfo = dfo.query("variant.notnull()")
 
         return dfo
```

### Comparing `countess-0.0.31/countess/utils/variant.py` & `countess-0.0.32/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess.egg-info/PKG-INFO` & `countess-0.0.32/countess.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.31
+Version: 0.0.32
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.31
+# CountESS 0.0.32
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.31/countess.egg-info/SOURCES.txt` & `countess-0.0.32/countess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/countess.egg-info/entry_points.txt` & `countess-0.0.32/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.31/pyproject.toml` & `countess-0.0.32/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     { name = "Nick Moore", email="nick@zoic.org" },
     { name = "Alan Rubin", email="alan@rubin.id.au" },
 ]
 maintainers = [
     { name = "Nick Moore", email="nick@zoic.org" },
 ]
 description = "CountESS"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 license = { text = "BSD-3-Clause" }
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
```

