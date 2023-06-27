# Comparing `tmp/pysj-1.0.1.tar.gz` & `tmp/pysj-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysj-1.0.1.tar", last modified: Tue May  9 11:01:50 2023, max compression
+gzip compressed data, was "pysj-1.0.2.tar", last modified: Tue Jun 27 20:10:38 2023, max compression
```

## Comparing `pysj-1.0.1.tar` & `pysj-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     2779 2022-04-02 07:00:57.140323 pysj-1.0.1/.gitignore
--rw-r--r--   0        0        0      559 2022-01-16 18:00:32.029533 pysj-1.0.1/.vscode/launch.json
--rw-r--r--   0        0        0      191 2022-01-16 18:00:32.029533 pysj-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      863 2022-01-16 18:00:32.029533 pysj-1.0.1/.vscode/tasks.json
--rw-r--r--   0        0        0     1086 2022-04-01 06:05:35.328085 pysj-1.0.1/LICENSE
--rw-r--r--   0        0        0     3311 2023-01-14 19:27:20.016232 pysj-1.0.1/README.md
--rw-r--r--   0        0        0      681 2022-11-24 12:22:55.458603 pysj-1.0.1/dodo.py
--rw-r--r--   0        0        0      815 2022-07-28 10:45:58.822848 pysj-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      443 2023-05-09 11:01:48.355733 pysj-1.0.1/pysj/__init__.py
--rw-r--r--   0        0        0     1975 2023-01-14 17:39:57.802289 pysj-1.0.1/pysj/crypto.py
--rw-r--r--   0        0        0     1524 2022-03-01 18:57:00.446349 pysj-1.0.1/pysj/formats.py
--rw-r--r--   0        0        0     8772 2023-05-09 11:01:48.355733 pysj-1.0.1/pysj/main.py
--rw-r--r--   0        0        0     5150 2023-05-09 10:58:36.371421 pysj-1.0.1/pysj/overengineer.py
--rw-r--r--   0        0        0     1015 2022-04-01 10:10:26.613031 pysj-1.0.1/tests/test_Crypto.py
--rw-r--r--   0        0        0     1305 2023-05-09 10:58:36.247421 pysj-1.0.1/tests/test_ExtendedJSONTranscoding.py
--rw-r--r--   0        0        0      466 2023-05-09 10:58:36.227421 pysj-1.0.1/tests/test_Flatten.py
--rw-r--r--   0        0        0      312 2022-03-13 11:30:51.360579 pysj-1.0.1/tests/test_Paginate.py
--rw-r--r--   0        0        0      920 2021-12-30 13:26:02.657349 pysj-1.0.1/tests/test_Seconds.py
--rw-r--r--   0        0        0      854 2023-05-09 10:58:36.247421 pysj-1.0.1/tests/test_Timer.py
--rw-r--r--   0        0        0      752 2023-01-14 11:43:55.663699 pysj-1.0.1/tests/test_chunk.py
--rw-r--r--   0        0        0      176 2023-01-14 11:55:22.601104 pysj-1.0.1/tests/test_first.py
--rw-r--r--   0        0        0      655 2023-05-09 10:58:36.227421 pysj-1.0.1/tests/test_formats.py
--rw-r--r--   0        0        0      158 2023-05-09 10:58:36.219421 pysj-1.0.1/tests/test_iso.py
--rw-r--r--   0        0        0      642 2023-05-09 10:58:05.551469 pysj-1.0.1/tests/test_months_in_interval.py
--rw-r--r--   0        0        0      368 2023-01-14 17:41:15.342353 pysj-1.0.1/tests/test_moving_average.py
--rw-r--r--   0        0        0      831 2023-05-09 10:58:36.263421 pysj-1.0.1/tests/test_n_wise.py
--rw-r--r--   0        0        0      204 2023-01-14 11:55:22.601104 pysj-1.0.1/tests/test_take.py
--rw-r--r--   0        0        0      336 2023-05-09 10:58:36.259421 pysj-1.0.1/tests/test_transpose.py
--rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 pysj-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2779 2022-04-02 07:00:57.140323 pysj-1.0.2/.gitignore
+-rw-r--r--   0        0        0      559 2022-01-16 18:00:32.029533 pysj-1.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0      191 2022-01-16 18:00:32.029533 pysj-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      863 2022-01-16 18:00:32.029533 pysj-1.0.2/.vscode/tasks.json
+-rw-r--r--   0        0        0     1086 2023-05-09 11:02:34.635985 pysj-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3311 2023-01-14 19:27:20.016232 pysj-1.0.2/README.md
+-rw-r--r--   0        0        0      681 2022-11-24 12:22:55.458603 pysj-1.0.2/dodo.py
+-rw-r--r--   0        0        0      819 2023-06-26 21:53:18.005108 pysj-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      488 2023-06-27 20:10:36.450129 pysj-1.0.2/pysj/__init__.py
+-rw-r--r--   0        0        0     1975 2023-01-14 17:39:57.802289 pysj-1.0.2/pysj/crypto.py
+-rw-r--r--   0        0        0     1524 2022-03-01 18:57:00.446349 pysj-1.0.2/pysj/formats.py
+-rw-r--r--   0        0        0    11221 2023-06-27 20:10:36.446129 pysj-1.0.2/pysj/main.py
+-rw-r--r--   0        0        0     5150 2023-05-09 10:58:36.371421 pysj-1.0.2/pysj/overengineer.py
+-rw-r--r--   0        0        0     1015 2022-04-01 10:10:26.613031 pysj-1.0.2/tests/test_Crypto.py
+-rw-r--r--   0        0        0     1305 2023-05-09 10:58:36.247421 pysj-1.0.2/tests/test_ExtendedJSONTranscoding.py
+-rw-r--r--   0        0        0      466 2023-05-09 10:58:36.227421 pysj-1.0.2/tests/test_Flatten.py
+-rw-r--r--   0        0        0      312 2022-03-13 11:30:51.360579 pysj-1.0.2/tests/test_Paginate.py
+-rw-r--r--   0        0        0      901 2023-06-27 06:56:57.778454 pysj-1.0.2/tests/test_Point.py
+-rw-r--r--   0        0        0      505 2023-06-27 20:08:10.815851 pysj-1.0.2/tests/test_PythonVersion.py
+-rw-r--r--   0        0        0      920 2021-12-30 13:26:02.657349 pysj-1.0.2/tests/test_Seconds.py
+-rw-r--r--   0        0        0      854 2023-05-09 10:58:36.247421 pysj-1.0.2/tests/test_Timer.py
+-rw-r--r--   0        0        0      752 2023-01-14 11:43:55.663699 pysj-1.0.2/tests/test_chunk.py
+-rw-r--r--   0        0        0      176 2023-01-14 11:55:22.601104 pysj-1.0.2/tests/test_first.py
+-rw-r--r--   0        0        0      655 2023-05-09 10:58:36.227421 pysj-1.0.2/tests/test_formats.py
+-rw-r--r--   0        0        0      158 2023-05-09 10:58:36.219421 pysj-1.0.2/tests/test_iso.py
+-rw-r--r--   0        0        0      852 2023-05-09 17:55:03.921803 pysj-1.0.2/tests/test_months_in_interval.py
+-rw-r--r--   0        0        0      368 2023-01-14 17:41:15.342353 pysj-1.0.2/tests/test_moving_average.py
+-rw-r--r--   0        0        0      831 2023-05-09 10:58:36.263421 pysj-1.0.2/tests/test_n_wise.py
+-rw-r--r--   0        0        0      204 2023-01-14 11:55:22.601104 pysj-1.0.2/tests/test_take.py
+-rw-r--r--   0        0        0      336 2023-05-09 10:58:36.259421 pysj-1.0.2/tests/test_transpose.py
+-rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 pysj-1.0.2/PKG-INFO
```

### Comparing `pysj-1.0.1/.gitignore` & `pysj-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/.vscode/launch.json` & `pysj-1.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/.vscode/tasks.json` & `pysj-1.0.2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/LICENSE` & `pysj-1.0.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 Sondre S. Ødegård
+Copyright (c) 2023 Sondre S. Ødegård
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pysj-1.0.1/README.md` & `pysj-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/dodo.py` & `pysj-1.0.2/dodo.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/pyproject.toml` & `pysj-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 flit = {}
 doit = {}
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py{36,37,38,39,310}
+envlist = py{36,37,38,39,310,311}
 
 [testenv]
 deps = 
     pytest
     numpy
     black
     isort
```

### Comparing `pysj-1.0.1/pysj/crypto.py` & `pysj-1.0.2/pysj/crypto.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/pysj/formats.py` & `pysj-1.0.2/pysj/formats.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/pysj/main.py` & `pysj-1.0.2/pysj/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,70 @@
 import dataclasses
 import json
+import math
+import sys
 import time
 from datetime import date, datetime, timedelta
 from fractions import Fraction
 from itertools import islice, tee, zip_longest
 from typing import (Any, Callable, Iterable, List, Literal, Optional, Tuple,
                     Union)
 
 NUMPY_SUPPORT_FLAG = True
 try:
     import numpy as np
 except ImportError:
     NUMPY_SUPPORT_FLAG = False
 
 
+class PythonVersion:
+    def __init__(self, value=None):
+        if not value:
+            self.version = sys.version_info[:2]
+        else:
+            if isinstance(value, str):
+                self.version = tuple(map(int, value.split(".")))
+            elif isinstance(value, int):
+                self.version = tuple(map(int, (str(value)[0], str(value)[1:])))
+        self.version_string = ".".join(map(str, self.version))
+
+    def __str__(self):
+        return self.version_string
+
+    def __repr__(self):
+        return f"{type(self)} {self.version_string}"
+
+    def __eq__(self, other):
+        return self.version == PythonVersion(other).version
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __ge__(self, other):
+        return self._convert_version_to_int(self) >= self._convert_version_to_int(other)
+
+    def __gt__(self, other):
+        return self._convert_version_to_int(self) > self._convert_version_to_int(other)
+
+    def __le__(self, other):
+        return self._convert_version_to_int(self) <= self._convert_version_to_int(other)
+
+    def __lt__(self, other):
+        return self._convert_version_to_int(self) < self._convert_version_to_int(other)
+
+    @staticmethod
+    def _convert_version_to_int(value):
+        if not isinstance(value, PythonVersion):
+            value = PythonVersion(value)
+        return value.version[0] * 100 + value.version[1]
+
+
+py = PythonVersion()
+
+
 class Timer:
     """Simple class working like a stopwatch."""
 
     def __init__(self) -> None:
         self.time = None
         self.start_time = time.perf_counter()
 
@@ -312,7 +359,44 @@
     return next(iterable_)
 
 
 def chunk(n, iterable: Iterable, fillvalue=None):
     """Yields chunks of size *n* from *iterable*. Last chunk are filled with *fillvalue* if size of *iterable* is not a multiple of *n*."""
     args = [iter(iterable)] * n
     return zip_longest(*args, fillvalue=fillvalue)
+
+
+if sys.version_info <= (3, 9):  # Point requires Python 3.10 or higher.
+
+    class Point:
+        def __init__(
+            self,
+            x: int | float | None = None,
+            y: int | float | None = None,
+            z: int | float | None = None,
+        ):
+            self.x = x
+            self.y = y
+            self.z = z
+
+            self.vector = tuple(s for s in [x, y, z] if s is not None)
+            self.dimensions = self.axis = len(self.vector)
+
+        def __str__(self):
+            return f"Point({', '.join(map(str, self.vector))})"
+
+        def __repr__(self):
+            return self.__str__()
+
+        def __abs__(self):
+            return math.dist(tuple(0 for s in self.vector), self.vector)
+
+        def __hash__(self):
+            return hash(str(list(map(float, self.vector))))
+
+else:
+
+    class Point:
+        def __init__(self, *_):
+            raise NotImplementedError(
+                "The Point type is only implemented for Python >= 3.10."
+            )
```

### Comparing `pysj-1.0.1/pysj/overengineer.py` & `pysj-1.0.2/pysj/overengineer.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/tests/test_Crypto.py` & `pysj-1.0.2/tests/test_Crypto.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/tests/test_ExtendedJSONTranscoding.py` & `pysj-1.0.2/tests/test_ExtendedJSONTranscoding.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/tests/test_Seconds.py` & `pysj-1.0.2/tests/test_Seconds.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/tests/test_Timer.py` & `pysj-1.0.2/tests/test_Timer.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/tests/test_chunk.py` & `pysj-1.0.2/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/tests/test_formats.py` & `pysj-1.0.2/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/tests/test_n_wise.py` & `pysj-1.0.2/tests/test_n_wise.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0.1/PKG-INFO` & `pysj-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysj
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pysj makes Python development more comfortable, with utils, classes and helper
 Author: Sondre S. Ødegård
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Project-URL: Documentation, https://github.com/sondreod/pysj
```

