# Comparing `tmp/scinumtools-1.4.0.tar.gz` & `tmp/scinumtools-1.4.1.tar.gz`

## Comparing `scinumtools-1.4.0.tar` & `scinumtools-1.4.1.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.4.0/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.4.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.4.0/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/README.md
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/cached_data.npy
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/pyproject.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/requirements.txt
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/test_data.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/test_math.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/test_stats.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/test_struct.py
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/test_units.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.4.0/tests/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.4.0/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.4.0/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.4.1/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.4.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/phys/units/DimensionsClass.py
+-rw-r--r--   0        0        0    10765 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/phys/units/UnitClass.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.4.1/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/cached_data.npy
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/pyproject.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/requirements.txt
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/test_stats.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/test_struct.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/test_units.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.4.1/tests/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.4.1/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.4.1/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.4.1/PKG-INFO
```

### Comparing `scinumtools-1.4.0/.github/workflows/python-publish.yml` & `scinumtools-1.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/data/ImageClass.py` & `scinumtools-1.4.1/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.4.1/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.4.1/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.4.1/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.4.1/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.4.1/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.4.1/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.4.1/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.4.1/tests/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.4.1/tests/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.4.1/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.4.1/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/pyproject.toml` & `scinumtools-1.4.1/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/test_data.py` & `scinumtools-1.4.1/tests/test_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,49 @@
 sys.path.insert(0, 'src')
 
 from scinumtools.data import *
 
 def test_caching():
 
     file_cache = "tests/cached_data.npy"
-
+    
     if os.path.isfile(file_cache):
         os.remove(file_cache)
     assert not os.path.isfile(file_cache)
     
     @CachedFunction(file_cache)
     def read_data(a, b):
         return dict(a=a, b=b)
 
-    data = read_data('foo','bar')
-    
+    data = read_data('foo','bar')    
     assert data == dict(a='foo', b='bar')
-    assert os.path.isfile(file_cache)
-    
-    data = read_data('foo2','bar2')
 
+    data = read_data('foo2','bar2')
+    assert os.path.isfile(file_cache)
     assert data == dict(a='foo', b='bar')
+    
+    if os.path.isfile(file_cache):
+        os.remove(file_cache)
+    assert not os.path.isfile(file_cache)
 
+    @CachedFunction(file_cache)
+    def read_data():
+        return {
+            'array': np.linspace(1,100,100),
+            'scalar': 34,
+            'string': 'foo',
+        }
+    
+    data = read_data()
+    np.testing.assert_equal(data, dict(
+        array=np.linspace(1,100,100),
+        scalar=34,
+        string='foo',
+    ))
+    
 def test_normalizing():
 
     xlen = 10
     ylen = 20
     data = np.linspace(1,xlen*ylen,xlen*ylen).reshape(xlen,ylen) - 10
 
     # Test only data
```

### Comparing `scinumtools-1.4.0/tests/test_math.py` & `scinumtools-1.4.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/test_stats.py` & `scinumtools-1.4.1/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/test_struct.py` & `scinumtools-1.4.1/tests/test_struct.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from textwrap import dedent
 import sys
 sys.path.insert(0, 'src')
 
 from scinumtools.structs import *
 
 def test_row_collector_list():
+    
     columns = ['col1','col2','col3']
     with ListCollector(columns) as lc:
         lc.append([1,2,3])
         lc.append([4,5,6])
         lc.append([7,8,9])
         assert lc.col1 == [1,4,7]
         assert lc.col2 == [2,5,8]
@@ -24,22 +25,25 @@
             lc.to_dataframe(),
             pd.DataFrame(dict(
                 col1 = [1,4,7],
                 col2 = [2,5,8],
                 col3 = [3,6,9],
             ))
         )
-        assert lc.to_text() == dedent("""\
+        result = dedent("""\
                col1  col2  col3
             0     1     2     3
             1     4     5     6
             2     7     8     9
         """.rstrip())
-
+        assert lc.to_text() == result
+        assert str(lc) == result
+        
 def test_row_collector_array():
+    
     with ArrayCollector(['col1','col2','col3']) as ac:
         ac.append([1,2,3])
         ac.append([4,5,6])
         ac.append([7,8,0])
         np.testing.assert_equal(ac.col1, [1,4,7])
         np.testing.assert_equal(ac.col2, [2,5,8])
         np.testing.assert_equal(ac.col3, [3,6,0])
@@ -52,20 +56,23 @@
             ac.to_dataframe(),
             pd.DataFrame(dict(
                 col1 = [1.,4.,7.],
                 col2 = [2.,5.,8.],
                 col3 = [3.,6.,0.],
             ))
         )
-        assert ac.to_text() == dedent("""\
+        result = dedent("""\
                col1  col2  col3
             0   1.0   2.0   3.0
             1   4.0   5.0   6.0
             2   7.0   8.0   0.0
         """.rstrip())
+        assert ac.to_text() == result
+        assert str(ac) == result
+        
     columns = {'col1':dict(dtype=str),'col2':dict(dtype=float),'col3':dict(dtype=bool)}
     with ArrayCollector(columns) as ac:
         ac.append([1,2,3])
         ac.append([4,5,6])
         ac.append([7,8,0])
         np.testing.assert_equal(ac.col1, ['1','4','7'])
         np.testing.assert_equal(ac.col2, [2,5,8])
@@ -79,20 +86,22 @@
             ac.to_dataframe(),
             pd.DataFrame(dict(
                 col1 = ['1','4','7'],
                 col2 = [2.,5.,8.],
                 col3 = [True,True,False],
             ))
         )
-        assert ac.to_text() == dedent("""\
+        result = dedent("""\
               col1  col2   col3
             0    1   2.0   True
             1    4   5.0   True
             2    7   8.0  False
         """.rstrip())
+        assert ac.to_text() == result
+        assert str(ac) == result
 
 def test_parameter_list():
     def test(params):
         assert params[0].a == 1
         assert params[1]['a'] == 4
         for param in params:
             assert param['a'] in [1,4]
```

### Comparing `scinumtools-1.4.0/tests/test_units.py` & `scinumtools-1.4.1/tests/test_units.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 from scinumtools.phys.units.UnitList import UnitStandard, UnitPrefixes
 from scinumtools.phys.units import *
 
 def test_definitions():
     
     unitlist = ParameterDict(['magnitude','dimensions','definition','name'], UnitStandard)
     for symbol, unit in unitlist.items():
-        if unit['definition'] is None:
+        if not isinstance(unit['definition'],str):
             continue
         q = Quantity(1, unit['definition'])
         assert isclose(q.magnitude,  unit['magnitude'], rel_tol=1e-07)
         assert q.dimensions == unit['dimensions']
     prefixes = ParameterDict(['magnitude','dimensions','definition','name'], UnitPrefixes)
 
 def test_temperatures():
     
     # Temperature conversions
-    assert str(Quantity(23,'K').to('Cel'))          == "Quantity(-2.501e+02 Cel)"
-    assert str(Quantity(23,'K').to('[degF]'))       == "Quantity(-4.183e+02 [degF])"
-    assert str(Quantity(23,'K').to('[degR]'))       == "Quantity(4.140e+01 [degR])"
-    assert str(Quantity(23,'Cel').to('K'))          == "Quantity(2.961e+02 K)"
-    assert str(Quantity(23,'Cel').to('[degF]'))     == "Quantity(7.340e+01 [degF])"
-    assert str(Quantity(23,'Cel').to('[degR]'))     == "Quantity(5.331e+02 [degR])"
-    assert str(Quantity(23,'[degF]').to('K'))       == "Quantity(2.681e+02 K)"
-    assert str(Quantity(23,'[degF]').to('Cel'))     == "Quantity(-5.000e+00 Cel)"
-    assert str(Quantity(23,'[degF]').to('[degR]'))  == "Quantity(4.827e+02 [degR])"
-    assert str(Quantity(23,'[degR]').to('K'))       == "Quantity(1.278e+01 K)"
-    assert str(Quantity(23,'[degR]').to('Cel'))     == "Quantity(-2.604e+02 Cel)"
-    assert str(Quantity(23,'[degR]').to('[degF]'))  == "Quantity(-4.367e+02 [degF])"
-    assert str(Quantity(2300,'Cel').to('kK'))       == "Quantity(2.573e+00 kK)"
+    assert str(Quantity(23,'K').to('Cel'))        == "Quantity(-2.501e+02 Cel)"
+    assert str(Quantity(23,'K').to('degF'))       == "Quantity(-4.183e+02 degF)"
+    assert str(Quantity(23,'K').to('degR'))       == "Quantity(4.140e+01 degR)"
+    assert str(Quantity(23,'Cel').to('K'))        == "Quantity(2.961e+02 K)"
+    assert str(Quantity(23,'Cel').to('degF'))     == "Quantity(7.340e+01 degF)"
+    assert str(Quantity(23,'Cel').to('degR'))     == "Quantity(5.331e+02 degR)"
+    assert str(Quantity(23,'degF').to('K'))       == "Quantity(2.681e+02 K)"
+    assert str(Quantity(23,'degF').to('Cel'))     == "Quantity(-5.000e+00 Cel)"
+    assert str(Quantity(23,'degF').to('degR'))    == "Quantity(4.827e+02 degR)"
+    assert str(Quantity(23,'degR').to('K'))       == "Quantity(1.278e+01 K)"
+    assert str(Quantity(23,'degR').to('Cel'))     == "Quantity(-2.604e+02 Cel)"
+    assert str(Quantity(23,'degR').to('degF'))    == "Quantity(-4.367e+02 degF)"
+    assert str(Quantity(2300,'Cel').to('kK'))     == "Quantity(2.573e+00 kK)"
     
 def test_inversion():
 
     assert str(Quantity(23, 'Hz').to('s'))     == "Quantity(4.348e-02 s)"
     assert str(Quantity(34, 'Ohm').to('S'))    == "Quantity(2.941e-02 S)"
     assert str(Quantity(102, 'J').to('erg-1')) == "Quantity(9.804e-10 erg-1)"
 
@@ -97,9 +97,65 @@
     assert str(q) == "Quantity([2. 3. 4.] m)"
     q = q ** 10
     assert str(q) == "Quantity([1.024e+03 5.905e+04 1.049e+06] m10)"
 
     # Test unit conversion on arrays
     assert str(Quantity([1,2,3], 'm').to('km')) == "Quantity([0.001 0.002 0.003] km)"
 
+def test_numpy():
+    
     # Test numpy functions
-    assert str(np.sqrt(Quantity([4, 9, 16], 'm'))) == "Quantity([2. 3. 4.] m)"
+    assert str(np.sqrt(Quantity([4, 9, 16], 'm2'))) == "Quantity([2. 3. 4.] m2)"
+
+def test_operation_sides():
+    
+    p = Quantity([2,3,4], 'm')
+    q = Quantity([5,6,7], 'm')
+    assert p+q == q+p
+    assert p-q == -(q-p)
+    assert q*2 == 2*q
+    assert p/2 == 1/(2/p)
+
+def test_units():
+
+    assert str(Unit('m'))         == "Quantity(1.000e+00 m)"
+    assert str(Unit('kg*m2*s-2')) == "Quantity(1.000e+00 kg*m2*s-2)"
+    
+    unit = Unit()
+    assert str(unit.m)      == "Quantity(1.000e+00 m)"
+    assert str(2*unit.kJ)   == "Quantity(2.000e+00 kJ)"
+    assert str(unit.kg*unit.m**2/unit.s**2) == "Quantity(1.000e+00 kg*m2*s-2)"
+    assert str(unit.J.to('erg')) == "Quantity(1.000e+07 erg)"
+
+def test_constants():
+
+    assert str(Constant('c')) == "Quantity(1.000e+00 [c])"
+
+    const = Constant()
+    assert str(const.c)   == "Quantity(1.000e+00 [c])"
+    assert str(const.m_e) == "Quantity(1.000e+00 [m_e])"
+    
+def test_unique_names():
+
+    units = list(UnitStandard.keys())
+    for unit in UnitStandard.keys():
+        for prefix in UnitPrefixes.keys():
+            units.append(f"{prefix}{unit}")
+    units.sort()
+    seen = set()
+    dupes = [x for x in units if x in seen or seen.add(x)]    
+    assert len(dupes)==0
+
+def test_dimensions():
+    
+    dims = Dimensions(m=(5,-2), g=3, s=1, cd=(-0,3), K=(34,1), rad=(18,12))
+    assert str(dims) == "Dimensions(m=Ratio(-5,2), g=3, s=1, K=34, rad=Ratio(3,2))"
+
+    dims1 = Dimensions(m=3, g=(3,2))
+    dims2 = Dimensions(m=2, g=(4,7))
+    assert not dims1==dims2
+    assert str(dims1+dims1) == "Dimensions(m=3, g=Ratio(3,2))"
+    assert str(dims2-dims2) == "Dimensions(m=2, g=Ratio(4,7))"
+    assert str(dims1*dims2) == "Dimensions(m=5, g=Ratio(29,14))"
+    assert str(dims1/dims2) == "Dimensions(m=1, g=Ratio(13,14))"
+    assert str(dims1**2)    == "Dimensions(m=6, g=3)"
+    assert str(dims2**0.5)  == "Dimensions(m=1, g=Ratio(2,7))"
```

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/data/ImageClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.4.1/src/scinumtools/phys/units/QuantityClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import List
 import numpy as np
 import re
-from math import isclose
 from typing import Union
-from dataclasses import dataclass
 
 from ...structs.ParameterClass import ParameterDict
 from ...math.solver import ExpressionSolver, AtomBase, OperatorPar, OperatorMul, OperatorTruediv
 from .UnitList import *
-from .UnitConverters import TemperatureConverter
+from .UnitConverters import *
+#from .DimensionsClass import *
 
 class Quantity:
     prefixes: dict            # list of prefixes 
     unitlist: dict            # list of units
     
     magnitude: float          # quantity magnitude
     dimensions: List[int]     # quantity dimensions
@@ -54,63 +53,98 @@
                 self.baseunits = {UnitBase[d]:dim for d,dim in enumerate(self.dimensions) if dim!=0}
         else:
             raise Exception("Insufficient quantity definition", magnitude, dimensions, baseunits)
         # Remove zero base units
         for unit in list(self.baseunits.keys()):
             if self.baseunits[unit]==0:
                 del self.baseunits[unit]
-        
+
+    def _add(self, left, right):
+        if not isinstance(left, Quantity):
+            left = Quantity(left)
+        if not isinstance(right, Quantity):
+            right = Quantity(right)
+        if not left.dimensions==right.dimensions:
+            raise Exception('Addition of two units with different dimensions:', self, right)
+        magnitude = left.magnitude + right.magnitude
+        dimensions = list(left.dimensions)
+        baseunits = dict(left.baseunits)
+        return Quantity(magnitude, dimensions, baseunits)
+
     def __add__(self, other):
-        if not isinstance(other, Quantity):
-            other = Quantity(other)
-        if not self.dimensions==other.dimensions:
-            raise Exception('Addition of two units with different dimensions:', self, other)
-        magnitude = self.magnitude + other.magnitude
-        dimensions = list(self.dimensions)
-        baseunits = dict(self.baseunits)
+        return self._add(self, other)
+    
+    def __radd__(self, other):
+        return self._add(other, self)
+
+    def _sub(self, left, right):
+        if not isinstance(left, Quantity):
+            left = Quantity(left)
+        if not isinstance(right, Quantity):
+            right = Quantity(right)
+        if not left.dimensions==right.dimensions:
+            raise Exception('Substraction of two units with different dimensions:', self, right)
+        magnitude = left.magnitude - right.magnitude
+        dimensions = list(left.dimensions)
+        baseunits = dict(left.baseunits)
         return Quantity(magnitude, dimensions, baseunits)
 
     def __sub__(self, other):
-        if not isinstance(other, Quantity):
-            other = Quantity(other)
-        if not self.dimensions==other.dimensions:
-            raise Exception('Substraction of two units with different dimensions:', self, other)
-        magnitude = self.magnitude - other.magnitude
-        dimensions = list(self.dimensions)
-        baseunits = dict(self.baseunits)
-        return Quantity(magnitude, dimensions, baseunits)
+        return self._sub(self, other)
+
+    def __rsub__(self, other):
+        return self._sub(other, self)
     
-    def __mul__(self, other):
-        if not isinstance(other, Quantity):
-            other = Quantity(other)
-        magnitude = self.magnitude * other.magnitude
-        dimensions = [self.dimensions[i]+other.dimensions[i] for i in range(len(UnitBase))]
-        baseunits = dict(self.baseunits)
-        for unit,exp in other.baseunits.items():
+    def _mul(self, left, right):
+        if not isinstance(left, Quantity):
+            left = Quantity(left)
+        if not isinstance(right, Quantity):
+            right = Quantity(right)
+        magnitude = left.magnitude * right.magnitude
+        dimensions = [left.dimensions[i]+right.dimensions[i] for i in range(len(UnitBase))]
+        baseunits = dict(left.baseunits)
+        for unit,exp in right.baseunits.items():
             baseunits[unit] = baseunits[unit]+exp if unit in baseunits else exp
         return Quantity(magnitude, dimensions, baseunits)
 
-    def __truediv__(self, other):
-        if not isinstance(other, Quantity):
-            other = Quantity(other)
-        magnitude = self.magnitude / other.magnitude
-        dimensions = [self.dimensions[i]-other.dimensions[i] for i in range(len(UnitBase))]
-        baseunits = dict(self.baseunits)
-        for unit,exp in other.baseunits.items():
+    def __mul__(self, other):
+        return self._mul(self, other)
+
+    def __rmul__(self, other):
+        return self._mul(other, self)
+    
+    def _truediv(self, left, right):
+        if not isinstance(left, Quantity):
+            left = Quantity(left)
+        if not isinstance(right, Quantity):
+            right = Quantity(right)
+        magnitude = left.magnitude / right.magnitude
+        dimensions = [left.dimensions[i]-right.dimensions[i] for i in range(len(UnitBase))]
+        baseunits = dict(left.baseunits)
+        for unit,exp in right.baseunits.items():
             baseunits[unit] = baseunits[unit]-exp if unit in baseunits else -exp
         return Quantity(magnitude, dimensions, baseunits)
 
+    def __truediv__(self, other):
+        return self._truediv(self, other)
+    
+    def __rtruediv__(self, other):
+        return self._truediv(other, self)
+    
     def __pow__(self, power):
         magnitude = self.magnitude**power
         dimensions = [self.dimensions[i]*power for i in range(len(UnitBase))]
         baseunits = {unit:exp*power for unit,exp in self.baseunits.items()}
         return Quantity(magnitude, dimensions, baseunits)
 
+    def __neg__(self):
+        return Quantity(-self.magnitude, self.dimensions, self.baseunits)
+    
     def __eq__(self, other):
-        if not isclose(self.magnitude, other.magnitude, rel_tol=self.precision):
+        if not np.allclose(self.magnitude, other.magnitude, rtol=self.precision):
             return False
         if self.dimensions!=other.dimensions:
             return False
         return True
     
     def __str__(self):
         magnitude = self.value()
@@ -136,14 +170,27 @@
         else:
             return f"Quantity({magnitude:s})"
 
     def __array__(self):
         return self.magnitude
 
     def __array_wrap__(self, out_arr, context=None):
+        """
+        if context[0]==np.sqrt:
+            dimensions = []
+            for d in range(len(UnitBase)):
+                dimensions.append( self.dimensions[d] )
+                if dimensions[d]==0:
+                    continue
+                elif isinstance(dimensions[d], int):
+                    dimensions[d] = Ratio(dimensions[d], 2)
+                elif isinstance(dimensions[d], Ratio):
+                    dimensions[d] = Ratio(dimensions[d][0], dimensions[d][1]+2)
+            print(dimensions)
+        """
         return Quantity(out_arr, self.dimensions, self.baseunits)
     
     def _atom_parser(self, string=None):
         # parse number
         m = re.match(r'^[-]?([0-9.]+)(e([0-9+-]+)|)$', str(string))
         if m:
             magnitude = float(string)
@@ -217,12 +264,13 @@
                 if np.all([-unit1.dimensions[d]==unit2.dimensions[d] for d in range(len(UnitBase))]):
                     unit1 = Quantity(1)/self
                 else:
                     raise Exception("Converting units with different dimensions:",
                                     unit1.dimensions, unit2.dimensions)
             with TemperatureConverter(unit1.baseunits, unit2.baseunits) as tc:
                 if tc.convertable:
-                    return Quantity(tc.convert(unit1.magnitude, unit2.magnitude), units)
+                    unit2.magnitude = unit1.magnitude/tc.convert(unit1.magnitude, unit2.magnitude)
+                    #return Quantity(tc.convert(unit1.magnitude, unit2.magnitude), units)
             unit = unit1/unit2
             return Quantity(unit.magnitude, units)
         else:
             raise Exception("Invalid units format:", units)
```

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.4.1/src/scinumtools/phys/units/UnitConverters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,63 @@
-class TemperatureConverter:
+class Converter:
+
     convertable: bool = False
     unit1: dict = None
     unit2: dict = None
     
     def __enter__(self):
         return self
     
     def __exit__(self, type, value, traceback):
         pass
         
     def __init__(self, baseunits1, baseunits2):
-        convertable = ['Cel','[degF]']
         for unitid, exponent in baseunits1.items():
-            if unitid.split(':')[-1] in convertable:
+            if unitid.split(':')[-1] in self.process:
                 self.convertable = True
         for unitid, exponent in baseunits2.items():
-            if unitid.split(':')[-1] in convertable:
+            if unitid.split(':')[-1] in self.process:
                 self.convertable = True
         if self.convertable:
             if len(baseunits1)!=1 or len(baseunits2)!=1:
-                raise Exception("Only direct temperatures can be converted between each other:", baseunits1, baseunits2)
+                raise Exception("Only simple units can be converted between each other:", baseunits1, baseunits2)
             else:
                 self.unit1 = list(baseunits1.keys())[0].split(':')[-1]
                 self.unit2 = list(baseunits2.keys())[0].split(':')[-1]
+
+class TemperatureConverter(Converter):
                 
+    process: list = ['Cel','degF']
+    
     def convert(self, magnitude1, magnitude2):
         if self.unit1=='K' and self.unit2=='Cel':
             return (magnitude1-273.15)/magnitude2
-        elif self.unit1=='K' and self.unit2=='[degF]':
+        elif self.unit1=='K' and self.unit2=='degF':
             return ((magnitude1-273.15)*9/5+32)/magnitude2
-        elif self.unit1=='[degR]' and self.unit2=='[degF]':
+        elif self.unit1=='degR' and self.unit2=='degF':
             return (magnitude1*9/5-459.67)/magnitude2
-        elif self.unit1=='[degR]' and self.unit2=='Cel':
+        elif self.unit1=='degR' and self.unit2=='Cel':
             return ((magnitude1*9/5-491.67)*5/9)/magnitude2
         elif self.unit1=='Cel' and self.unit2=='K':
             return (magnitude1+273.15)/magnitude2
-        elif self.unit1=='Cel' and self.unit2=='[degF]':
+        elif self.unit1=='Cel' and self.unit2=='degF':
             return ((magnitude1*9/5)+32)/magnitude2
-        elif self.unit1=='Cel' and self.unit2=='[degR]':
+        elif self.unit1=='Cel' and self.unit2=='degR':
             return ((magnitude1*9/5)+491.67)/(magnitude2*9/5)
-        elif self.unit1=='[degF]' and self.unit2=='K':
+        elif self.unit1=='degF' and self.unit2=='K':
             return (((magnitude1-32)*5/9)+273.15)/magnitude2
-        elif self.unit1=='[degF]' and self.unit2=='Cel':
+        elif self.unit1=='degF' and self.unit2=='Cel':
             return ((magnitude1-32)*5/9)/magnitude2
-        elif self.unit1=='[degF]' and self.unit2=='[degR]':
+        elif self.unit1=='degF' and self.unit2=='degR':
             return (magnitude1+459.67)/(magnitude2*9/5)
+        else:
+            raise Exception('Invalid conversion:', self.unit1, self.unit2)
+
+class LogarithmicConverter(Converter):
+
+    process: list = ['dBm','dBmW']
+    
+    def convert(self, magnitude1, magnitude2):
+        if self.unit1=='dBm' and self.unit2=='W':
+            return 234
+        else:
+            raise Exception('Invalid conversion:', self.unit1, self.unit2)
```

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.4.1/src/scinumtools/phys/units/UnitList.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import numpy as np        
+import numpy as np
+
+from .UnitConverters import *
         
 UnitPrefixes = {
     'Y':        (1.0e24,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e24',                   'yotta'            ), 
     'Z':        (1.0e21,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e21',                   'zetta'            ), 
     'E':        (1.0e18,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e18',                   'exa'              ), 
     'P':        (1.0e15,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e15',                   'peta'             ), 
     'T':        (1.0e12,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e12',                   'tera'             ), 
@@ -22,83 +24,97 @@
     'z':        (1.0e-21,        [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-21',                  'zepto'            ), 
     'y':        (1.0e-24,        [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-24',                  'yocto'            ), 
 }                                                                                        
             
 UnitBase = ['m','g','s','K','C','cd','mol','rad']
             
 UnitStandard = {
-    # physical units                        
+    # base physical units
     'm':        (1.0,            [ 1, 0, 0, 0, 0, 0, 0, 0],  None,                     'meter'            ),
     'g':        (1.0,            [ 0, 1, 0, 0, 0, 0, 0, 0],  None,                     'gram'             ),
     's':        (1.0,            [ 0, 0, 1, 0, 0, 0, 0, 0],  None,                     'second'           ),
     'K':        (1.0,            [ 0, 0, 0, 1, 0, 0, 0, 0],  None,                     'kelvin'           ),
     'C':        (1.0,            [ 0, 0, 0, 0, 1, 0, 0, 0],  None,                     'coulomb'          ),
     'cd':       (1.0,            [ 0, 0, 0, 0, 0, 1, 0, 0],  None,                     'candela'          ),
-    # numerical units            
+    # base numerical units
     'mol':      (1.0,            [ 0, 0, 0, 0, 0, 0, 1, 0],  None,                     'mole'             ),
     'rad':      (1.0,            [ 0, 0, 0, 0, 0, 0, 0, 1],  None,                     'radian'           ),
     # Derived units              
-    # SI units                                                                                    
     'sr':       (1.0e0,          [ 0, 0, 0, 0, 0, 0, 0, 2],  'rad2',                   'steradian'        ),
     'Hz':       (1.0e0,          [ 0, 0,-1, 0, 0, 0, 0, 0],  's-1',                    'hertz'            ),
-    'N':        (1.0e3,          [ 1, 1,-2, 0, 0, 0, 0, 0],  'kg*m/s2',                'newton'           ),
-    'Pa':       (1.0e3,          [-1, 1,-2, 0, 0, 0, 0, 0],  'N/m2',                   'pascal'           ),
-    'J':        (1.0e3,          [ 2, 1,-2, 0, 0, 0, 0, 0],  'N*m',                    'joule'            ),
     'W':        (1.0e3,          [ 2, 1,-3, 0, 0, 0, 0, 0],  'J/s',                    'watt'             ),
     'A':        (1.0e0,          [ 0, 0,-1, 0, 1, 0, 0, 0],  'C/s',                    'ampere'           ),
     'V':        (1.0e3,          [ 2, 1,-2, 0,-1, 0, 0, 0],  'J/C',                    'volt'             ),
     'F':        (1.0e-3,         [-2,-1, 2, 0, 2, 0, 0, 0],  'C/V',                    'farad'            ),
     'Ohm':      (1.0e3,          [ 2, 1,-1, 0,-2, 0, 0, 0],  'V/A',                    'ohm'              ),
     'S':        (1.0e-3,         [-2,-1, 1, 0, 2, 0, 0, 0],  'Ohm-1',                  'siemens'          ),
     'Wb':       (1.0e3,          [ 2, 1,-1, 0,-1, 0, 0, 0],  'V*s',                    'weber'            ),
-    'T':        (1.0e3,          [ 0, 1,-1, 0,-1, 0, 0, 0],  'Wb/m2',                  'tesla'            ),
     'H':        (1.0e3,          [ 2, 1, 0, 0,-2, 0, 0, 0],  'Wb/A',                   'henry'            ),
     'lm':       (1.0e0,          [ 0, 0, 0, 0, 0, 1, 0, 2],  'cd*sr',                  'lumen'            ),
     'lx':       (1.0e0,          [-2, 0, 0, 0, 0, 1, 0, 2],  'lm/m2',                  'lux'              ),
     'Bq':       (1.0e0,          [ 0, 0,-1, 0, 0, 0, 0, 0],  's-1',                    'becquerel'        ),
+    'ar':       (1.0e2,          [ 2, 0, 0, 0, 0, 0, 0, 0],  '100*m2',                 'are'              ),
+    # units of energy absorption
     'Gy':       (1.0e0,          [ 2, 0,-2, 0, 0, 0, 0, 0],  'J/kg',                   'gray'             ),
     'Sv':       (1.0e0,          [ 2, 0,-2, 0, 0, 0, 0, 0],  'J/kg',                   'sivert'           ),
-    # CGS units                                                                               
-    'dyn':      (1.0e-2,         [ 1, 1,-2, 0, 0, 0, 0, 0],  'g*cm/s2',                'dyne'             ),
-    'erg':      (1.0e-4,         [ 2, 1,-2, 0, 0, 0, 0, 0],  'dyn*cm',                 'erg'              ),
+    # units of magnetic flux density
+    'T':        (1.0e3,          [ 0, 1,-1, 0,-1, 0, 0, 0],  'Wb/m2',                  'tesla'            ),
     'G':        (1.0e-1,         [ 0, 1,-1, 0,-1, 0, 0, 0],  '1e-4*T',                 'Gauss'            ),
-    # other derived units                                                                        
+    # units of energy
+    'J':        (1.0e3,          [ 2, 1,-2, 0, 0, 0, 0, 0],  'N*m',                    'joule'            ),
+    'eV':       (1.60217733e-16, [ 2, 1,-2, 0, 0, 0, 0, 0],  '[e]*V',                  'electronvolt'     ),
+    'erg':      (1.0e-4,         [ 2, 1,-2, 0, 0, 0, 0, 0],  'dyn*cm',                 'erg'              ),
+    # units of pressure
+    'Pa':       (1.0e3,          [-1, 1,-2, 0, 0, 0, 0, 0],  'N/m2',                   'pascal'           ),
+    'atm':      (1.013250e8,     [-1, 1,-2, 0, 0, 0, 0, 0],  '101325*Pa',              'atm. pressure'    ),
+    # units of force
+    'N':        (1.0e3,          [ 1, 1,-2, 0, 0, 0, 0, 0],  'kg*m/s2',                'newton'           ),
+    'dyn':      (1.0e-2,         [ 1, 1,-2, 0, 0, 0, 0, 0],  'g*cm/s2',                'dyne'             ),
+    # angular units
     'deg':      (1.7453292e-2,   [ 0, 0, 0, 0, 0, 0, 0, 1],  '2*[pi]*rad/360',         'angle degree'     ),
     "'":        (2.908882e-4,    [ 0, 0, 0, 0, 0, 0, 0, 1],  'deg/60',                 'angle minute'     ),
     "''":       (4.848137e-6,    [ 0, 0, 0, 0, 0, 0, 0, 1],  "'/60",                   'angle second'     ),
+    # units of distance
+    'au':       (1.49597870e11,  [ 1, 0, 0, 0, 0, 0, 0, 0],  '149597.870691*Mm',       'astr. unit'       ),
+    'AU':       (1.49597870e11,  [ 1, 0, 0, 0, 0, 0, 0, 0],  'au',                     'astr. unit'       ),
+    'ly':       (9.460730e15,    [ 1, 0, 0, 0, 0, 0, 0, 0],  '[c]*yr_j',               'light-year'       ),
+    # units of volume
     'l':        (1e-3,           [ 3, 0, 0, 0, 0, 0, 0, 0],  'dm3',                    'liter'            ),
     'L':        (1e-3,           [ 3, 0, 0, 0, 0, 0, 0, 0],  'l',                      'liter'            ),
-    'ar':       (1e2,            [ 2, 0, 0, 0, 0, 0, 0, 0],  '100*m2',                 'are'              ),
+    # units of time
     'min':      (6.0e1,          [ 0, 0, 1, 0, 0, 0, 0, 0],  '60*s',                   'minute'           ),
     'h':        (3.6e3,          [ 0, 0, 1, 0, 0, 0, 0, 0],  '60*min',                 'hour'             ),
-    'd':        (8.64e4,         [ 0, 0, 1, 0, 0, 0, 0, 0],  '24*h',                   'day'              ),
-    'a_t':      (3.1556925e7,    [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.24219*d',            'tropical year'    ),
-    'a_j':      (3.1557600e7,    [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.25*d',               'Julian year'      ),
-    'a_g':      (3.155695e7,     [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.2425*d',             'Gregorian year'   ),
-    'a':        (3.155760e7,     [ 0, 0, 1, 0, 0, 0, 0, 0],  'a_j',                    'year'             ),
-    'eV':       (1.60217733e-16, [ 2, 1,-2, 0, 0, 0, 0, 0],  '[e]*V',                  'electronvolt'     ),
-    'au':       (1.49597870e11,  [ 1, 0, 0, 0, 0, 0, 0, 0],  '149597.870691*Mm',       'astr. unit'       ),
-    'AU':       (1.49597870e11,  [ 1, 0, 0, 0, 0, 0, 0, 0],  'au',                     'astr. unit'       ),
-    # natural units             
+    'day':      (8.64e4,         [ 0, 0, 1, 0, 0, 0, 0, 0],  '24*h',                   'day'              ),
+    'yr_t':     (3.1556925e7,    [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.24219*day',          'tropical year'    ),
+    'yr_j':     (3.1557600e7,    [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.25*day',             'Julian year'      ),
+    'yr_g':     (3.155695e7,     [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.2425*day',           'Gregorian year'   ),
+    'yr':       (3.155760e7,     [ 0, 0, 1, 0, 0, 0, 0, 0],  'yr_j',                   'year'             ),
+    # units of temperature
+    'Cel':      (1,              [ 0, 0, 0, 1, 0, 0, 0, 0],  TemperatureConverter,     'Degree Celsius'   ),
+    'degF':     (1,              [ 0, 0, 0, 1, 0, 0, 0, 0],  TemperatureConverter,     'Degree Fahrenheit'),
+    'degR':     (5/9,            [ 0, 0, 0, 1, 0, 0, 0, 0],  '5/9*K',                  'Degree Rankine'   ),
+    # logarithmic units and ratios
+    #'ratP':     (1,              [ 0, 0, 0, 0, 0, 0, 0, 0],  '1',                      'Power ratio'      ),      
+    #'ratA':     (1,              [ 0, 0, 0, 0, 0, 0, 0, 0],  '1',                      'Amplitude ratio'  ),      
+    #'B':        (1,              [ 0, 0, 0, 0, 0, 0, 0, 0],  None,                     'Bell'             ),
+    #'Np':       (1.151277918,    [ 0, 0, 0, 0, 0, 0, 0, 0],  '1.151277918*B',          'Nepers'           ),
+    'dBm':      (1,              [ 2, 1,-3, 0, 0, 0, 0, 0],  LogarithmicConverter,     'decibel-milliwatt'),
+    'dBmW':     (1,              [ 2, 1,-3, 0, 0, 0, 0, 0],  LogarithmicConverter,     'decibel-milliwatt'),
+    # percentages
+    '%':        (1e-2,           [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-2',                   'percent'          ),
+    'ppth':     (1e-3,           [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-3',                   'promile'          ),
+    # natural constants    
     '[c]':      (2.99792458e8,   [ 1, 0,-1, 0, 0, 0, 0, 0],  '299792458*m/s',          'velocity of light'),
     '[h]':      (6.626076e-31,   [ 2, 1,-1, 0, 0, 0, 0, 0],  '6.6260755e-34*J*s',      'Planck const.'    ),
     '[k]':      (1.380658e-20,   [ 2, 1,-2,-1, 0, 0, 0, 0],  '1.380658e-23*J/K',       'Boltzmann const.' ),
     '[eps_0]':  (8.854188e-15,   [-3,-1, 2, 0, 2, 0, 0, 0],  '8.854187817e-12*F/m',    'permit. of vac.'  ),
     '[mu_0]':   (1.256637e-3,    [ 1, 1, 0, 0,-2, 0, 0, 0],  '4*[pi]*1e-7*N/A2',       'permeab. of vac.' ),
     '[e]':      (1.60217733e-19, [ 0, 0, 0, 0, 1, 0, 0, 0],  '1.60217733e-19*C',       'elem. charge'     ),
     '[m_e]':    (9.109390e-28,   [ 0, 1, 0, 0, 0, 0, 0, 0],  '9.1093897e-28*g',        'electron mass'    ),
     '[m_p]':    (1.672623e-24,   [ 0, 1, 0, 0, 0, 0, 0, 0],  '1.6726231e-24*g',        'proton mass'      ),
     '[G]':      (6.672590e-14,   [ 3,-1,-2, 0, 0, 0, 0, 0],  '6.67259e-11*m3/(kg*s2)', 'grav. const.'     ),
     '[g]':      (9.806650e0,     [ 1, 0,-2, 0, 0, 0, 0, 0],  '9.80665*m/s2',           'grav. accel.'     ),
-    'atm':      (1.013250e8,     [-1, 1,-2, 0, 0, 0, 0, 0],  '101325*Pa',              'atm. pressure'    ),
-    'ly':       (9.460730e15,    [ 1, 0, 0, 0, 0, 0, 0, 0],  '[c]*a_j',                'light-year'       ),
-    # dimensionless units
+    # dimensionless constants
     '[pi]':     (np.pi,          [ 0, 0, 0, 0, 0, 0, 0, 0],  '3.1415926',              'pi'               ),
     '[euler]':  (np.e,           [ 0, 0, 0, 0, 0, 0, 0, 0],  '2.718282',               "Euler's num."     ),
     '[N_A]':    (6.0221367e23,   [ 0, 0, 0, 0, 0, 0, 0, 0],  '6.022137e23',            "Avogadro's num."  ),
-    '%':        (1e-2,           [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-2',                   'percent'          ),
-    '[ppth]':   (1e-3,           [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-3',                   'promile'          ),
-    '[degR]':   (5/9,            [ 0, 0, 0, 1, 0, 0, 0, 0],  '5/9*K',                  'Degree Rankine'   ),
-    # units defined by a nonlinear function
-    'Cel':      (1,              [ 0, 0, 0, 1, 0, 0, 0, 0],  None,                     'Degree Celsius'   ),
-    '[degF]':   (1,              [ 0, 0, 0, 1, 0, 0, 0, 0],  None,                     'Degree Fahrenheit'),
 }
```

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.4.1/src/scinumtools/structs/CollectorClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         pass
     
     def __init__(self, columns: list):
         self._columns = []
         for column in columns:
             setattr(self,column,[])
             self._columns.append(column)
+
+    def __str__(self):
+        return self.to_text()
         
     def append(self, values: list):
         """ Append a single row
 
         :param values: List of values for each column
         """
         for n, name in enumerate(self._columns):
@@ -112,14 +115,17 @@
                 setattr(self,column,np.array([],**kwargs))
                 self._columns.append(column)
         else:
             for column in columns:
                 setattr(self,column,np.array([]))
                 self._columns.append(column)
 
+    def __str__(self):
+        return self.to_text()
+    
     def append(self, values: list):
         """ Append a single row
 
         :param values: List of values for each column
         """
         for n, name in enumerate(self._columns):
             data = getattr(self,name)
```

### Comparing `scinumtools-1.4.0/tests/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.4.1/tests/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.4.0/.gitignore` & `scinumtools-1.4.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Byte-compiled / optimized / DLL files
-__pycache__/
+**/__pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
```

### Comparing `scinumtools-1.4.0/pyproject.toml` & `scinumtools-1.4.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.4.0/PKG-INFO` & `scinumtools-1.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.4.0
+Version: 1.4.1
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

