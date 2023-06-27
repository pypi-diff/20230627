# Comparing `tmp/pydiverse_transform-0.1.2.tar.gz` & `tmp/pydiverse_transform-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_transform-0.1.2.tar", max compression
+gzip compressed data, was "pydiverse_transform-0.1.3.tar", max compression
```

## Comparing `pydiverse_transform-0.1.2.tar` & `pydiverse_transform-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1517 2023-05-22 14:59:50.867488 pydiverse_transform-0.1.2/LICENSE
--rw-r--r--   0        0        0     2325 2023-06-01 15:40:30.967225 pydiverse_transform-0.1.2/docs/package/README.md
--rw-r--r--   0        0        0     1471 2023-06-01 15:44:26.899777 pydiverse_transform-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       13 2023-05-22 14:59:50.868554 pydiverse_transform-0.1.2/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      387 2023-05-22 14:59:50.868629 pydiverse_transform-0.1.2/src/pydiverse/transform/__init__.py
--rw-r--r--   0        0        0      108 2023-05-22 14:59:50.868774 pydiverse_transform-0.1.2/src/pydiverse/transform/core/__init__.py
--rw-r--r--   0        0        0     3470 2023-05-22 14:59:50.868845 pydiverse_transform-0.1.2/src/pydiverse/transform/core/alignment.py
--rw-r--r--   0        0        0     2797 2023-06-01 15:42:26.018480 pydiverse_transform-0.1.2/src/pydiverse/transform/core/column.py
--rw-r--r--   0        0        0     5082 2023-05-22 14:59:50.868981 pydiverse_transform-0.1.2/src/pydiverse/transform/core/dispatchers.py
--rw-r--r--   0        0        0      191 2023-05-22 14:59:50.869098 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/__init__.py
--rw-r--r--   0        0        0     1078 2023-05-22 14:59:50.869154 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/expressions.py
--rw-r--r--   0        0        0      682 2023-05-22 14:59:50.869206 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/lambda_getter.py
--rw-r--r--   0        0        0     4871 2023-05-22 14:59:50.869290 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/symbolic_expressions.py
--rw-r--r--   0        0        0     4881 2023-06-01 15:42:26.956127 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/translator.py
--rw-r--r--   0        0        0     1708 2023-06-01 15:42:55.420078 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/util.py
--rw-r--r--   0        0        0      530 2023-05-22 14:59:50.869466 pydiverse_transform-0.1.2/src/pydiverse/transform/core/functions.py
--rw-r--r--   0        0        0      135 2023-05-22 14:59:50.869536 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/__init__.py
--rw-r--r--   0        0        0      903 2023-05-22 14:59:50.869588 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/aggregate.py
--rw-r--r--   0        0        0     3590 2023-06-01 15:42:55.420238 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/core.py
--rw-r--r--   0        0        0     1694 2023-05-22 14:59:50.869690 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/logical.py
--rw-r--r--   0        0        0     2341 2023-05-22 14:59:50.869745 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/numeric.py
--rw-r--r--   0        0        0    17847 2023-06-01 15:42:55.420630 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/registry.py
--rw-r--r--   0        0        0      518 2023-05-22 14:59:50.869940 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/string.py
--rw-r--r--   0        0        0      334 2023-05-22 14:59:50.870004 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/window.py
--rw-r--r--   0        0        0     3833 2023-06-01 15:42:55.420907 pydiverse_transform-0.1.2/src/pydiverse/transform/core/table.py
--rw-r--r--   0        0        0    16536 2023-06-01 15:42:55.421102 pydiverse_transform-0.1.2/src/pydiverse/transform/core/table_impl.py
--rw-r--r--   0        0        0       84 2023-05-22 14:59:50.870262 pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/__init__.py
--rw-r--r--   0        0        0     2637 2023-06-01 15:42:55.421445 pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/bidict.py
--rw-r--r--   0        0        0     1161 2023-06-01 15:42:55.421699 pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/ordered_set.py
--rw-r--r--   0        0        0     1892 2023-05-22 14:59:50.870440 pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/util.py
--rw-r--r--   0        0        0    14653 2023-06-01 15:42:55.421911 pydiverse_transform-0.1.2/src/pydiverse/transform/core/verbs.py
--rw-r--r--   0        0        0       42 2023-05-22 14:59:50.870617 pydiverse_transform-0.1.2/src/pydiverse/transform/eager/__init__.py
--rw-r--r--   0        0        0      265 2023-05-22 14:59:50.870681 pydiverse_transform-0.1.2/src/pydiverse/transform/eager/eager_table.py
--rw-r--r--   0        0        0    21007 2023-06-01 15:42:55.422346 pydiverse_transform-0.1.2/src/pydiverse/transform/eager/pandas_table.py
--rw-r--r--   0        0        0       36 2023-05-22 14:59:50.870868 pydiverse_transform-0.1.2/src/pydiverse/transform/lazy/__init__.py
--rw-r--r--   0        0        0      454 2023-05-22 14:59:50.870935 pydiverse_transform-0.1.2/src/pydiverse/transform/lazy/lazy_table.py
--rw-r--r--   0        0        0    26997 2023-06-01 15:42:55.422749 pydiverse_transform-0.1.2/src/pydiverse/transform/lazy/sql_table.py
--rw-r--r--   0        0        0        0 2023-05-22 14:59:50.871139 pydiverse_transform-0.1.2/src/pydiverse/transform/util/__init__.py
--rw-r--r--   0        0        0      730 2023-06-01 15:32:07.608144 pydiverse_transform-0.1.2/src/pydiverse/transform/util/testing.py
--rw-r--r--   0        0        0     3154 1970-01-01 00:00:00.000000 pydiverse_transform-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2331 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/docs/package/README.md
+-rw-r--r--   0        0        0     1471 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      387 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/__init__.py
+-rw-r--r--   0        0        0     3470 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/alignment.py
+-rw-r--r--   0        0        0     2797 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/column.py
+-rw-r--r--   0        0        0     5082 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/dispatchers.py
+-rw-r--r--   0        0        0      191 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/expressions.py
+-rw-r--r--   0        0        0      682 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/lambda_getter.py
+-rw-r--r--   0        0        0     4871 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/symbolic_expressions.py
+-rw-r--r--   0        0        0     4881 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/translator.py
+-rw-r--r--   0        0        0     1708 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/util.py
+-rw-r--r--   0        0        0      530 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/functions.py
+-rw-r--r--   0        0        0      135 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/__init__.py
+-rw-r--r--   0        0        0      903 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/aggregate.py
+-rw-r--r--   0        0        0     3590 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/core.py
+-rw-r--r--   0        0        0     1694 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/logical.py
+-rw-r--r--   0        0        0     2341 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/numeric.py
+-rw-r--r--   0        0        0    17847 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/registry.py
+-rw-r--r--   0        0        0      518 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/string.py
+-rw-r--r--   0        0        0      334 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/window.py
+-rw-r--r--   0        0        0     3833 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/table.py
+-rw-r--r--   0        0        0    16536 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/table_impl.py
+-rw-r--r--   0        0        0       84 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/__init__.py
+-rw-r--r--   0        0        0     2637 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/bidict.py
+-rw-r--r--   0        0        0     1161 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/ordered_set.py
+-rw-r--r--   0        0        0     1892 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/util.py
+-rw-r--r--   0        0        0    14653 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/verbs.py
+-rw-r--r--   0        0        0       42 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/eager/__init__.py
+-rw-r--r--   0        0        0      265 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/eager/eager_table.py
+-rw-r--r--   0        0        0    21015 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/eager/pandas_table.py
+-rw-r--r--   0        0        0       36 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/lazy/__init__.py
+-rw-r--r--   0        0        0      454 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/lazy/lazy_table.py
+-rw-r--r--   0        0        0    26850 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/lazy/sql_table.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/util/__init__.py
+-rw-r--r--   0        0        0      730 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/util/testing.py
+-rw-r--r--   0        0        0     3160 1970-01-01 00:00:00.000000 pydiverse_transform-0.1.3/PKG-INFO
```

### Comparing `pydiverse_transform-0.1.2/LICENSE` & `pydiverse_transform-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/docs/package/README.md` & `pydiverse_transform-0.1.3/docs/package/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pydiverse.transform
 
-[![CI](https://github.com/pydiverse/pydiverse.transform/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.transform/actions/workflows/ci.yml)
+[![CI](https://github.com/pydiverse/pydiverse.transform/actions/workflows/tests.yml/badge.svg)](https://github.com/pydiverse/pydiverse.transform/actions/workflows/tests.yml)
 
 Pipe based dataframe manipulation library that can also transform data on SQL databases
 
 This is an early stage version 0.x which lacks documentation. Please contact
 https://github.com/orgs/pydiverse/teams/code-owners if you like to become an early adopter
 or to contribute early stage usage examples.
```

### Comparing `pydiverse_transform-0.1.2/pyproject.toml` & `pydiverse_transform-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-transform"
-version = "0.1.2"
+version = "0.1.3"
 description = "Pipe based dataframe manipulation library that can also transform data on SQL databases"
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
```

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/alignment.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/alignment.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/column.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/column.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/dispatchers.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/dispatchers.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/expressions.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/lambda_getter.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/lambda_getter.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/symbolic_expressions.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/symbolic_expressions.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/translator.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/translator.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/util.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/util.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/functions.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/functions.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/aggregate.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/aggregate.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/core.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/logical.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/logical.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/numeric.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/numeric.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/registry.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/registry.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/string.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/string.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/table.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/table.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/table_impl.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/table_impl.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/bidict.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/bidict.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/ordered_set.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/util.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/util.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/core/verbs.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/core/verbs.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/eager/pandas_table.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/eager/pandas_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import functools
 import itertools
 import operator
 import warnings
-from typing import Callable
+from typing import Callable, Any
 
 import numpy as np
 import pandas as pd
 import pandas.core.dtypes.cast
 import pandas.core.dtypes.dtypes
 
 from pydiverse.transform.core import ops
@@ -53,23 +53,22 @@
             columns={
                 name: self.df_name_mapping[col.uuid] for name, col in columns.items()
             }
         )
 
         super().__init__(name=name, columns=columns)
 
-    def _convert_dtype(self, dtype: np.dtype) -> str:
-        type = dtype.type
-        if issubclass(type, np.integer):
+    def _convert_dtype(self, dtype: Any) -> str:
+        if pd.api.types.is_integer_dtype(dtype):
             return "int"
-        if issubclass(type, np.floating):
+        if pd.api.types.is_float_dtype(dtype):
             return "float"
-        if issubclass(type, np.bool_):
+        if pd.api.types.is_bool_dtype(dtype):
             return "bool"
-        if issubclass(type, str):
+        if pd.api.types.is_string_dtype(dtype):
             return "str"
 
         raise NotImplementedError(f"Invalid type {dtype}.")
 
     def is_aligned_with(self, col) -> bool:
         len_self = len(self.df.index)
```

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/lazy/sql_table.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/lazy/sql_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,19 +243,16 @@
         # Convert self.selects to SQLAlchemy Expressions
         s = []
         for name, uuid in self.selected_cols():
             sql_col = self.cols[uuid].compiled(self.sql_columns)
             if not isinstance(sql_col, sql.ColumnElement):
                 sql_col = sql.literal(sql_col)
             s.append(sql_col.label(name))
-        try:
-            select = select.with_only_columns(s)
-        except sqlalchemy.exc.ArgumentError:
-            # since sqlalchemy 2.0.0
-            select = select.with_only_columns(*s)
+
+        select = select.with_only_columns(*s)
 
         # ORDER BY
         if self.order_bys:
             o = []
             for o_by in self.order_bys:
                 compiled, _ = self.compiler.translate(o_by.order)
                 col = compiled(self.sql_columns)
```

### Comparing `pydiverse_transform-0.1.2/src/pydiverse/transform/util/testing.py` & `pydiverse_transform-0.1.3/src/pydiverse/transform/util/testing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.2/PKG-INFO` & `pydiverse_transform-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-transform
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pipe based dataframe manipulation library that can also transform data on SQL databases
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -18,15 +18,15 @@
 Requires-Dist: SQLAlchemy (>=1.4.27)
 Requires-Dist: numpy (>=1.23.1)
 Requires-Dist: pandas (>=1.4.3)
 Description-Content-Type: text/markdown
 
 # pydiverse.transform
 
-[![CI](https://github.com/pydiverse/pydiverse.transform/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.transform/actions/workflows/ci.yml)
+[![CI](https://github.com/pydiverse/pydiverse.transform/actions/workflows/tests.yml/badge.svg)](https://github.com/pydiverse/pydiverse.transform/actions/workflows/tests.yml)
 
 Pipe based dataframe manipulation library that can also transform data on SQL databases
 
 This is an early stage version 0.x which lacks documentation. Please contact
 https://github.com/orgs/pydiverse/teams/code-owners if you like to become an early adopter
 or to contribute early stage usage examples.
```

