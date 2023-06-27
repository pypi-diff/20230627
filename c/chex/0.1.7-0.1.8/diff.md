# Comparing `tmp/chex-0.1.7.tar.gz` & `tmp/chex-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chex-0.1.7.tar", last modified: Mon Mar 27 10:44:05 2023, max compression
+gzip compressed data, was "chex-0.1.8.tar", last modified: Tue Jun 27 13:15:17 2023, max compression
```

## Comparing `chex-0.1.7.tar` & `chex-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:44:05.092654 chex-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-27 10:43:54.000000 chex-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-27 10:43:54.000000 chex-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-03-27 10:44:05.088654 chex-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-03-27 10:43:54.000000 chex-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:44:05.088654 chex-0.1.7/chex/
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-03-27 10:43:54.000000 chex-0.1.7/chex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:44:05.088654 chex-0.1.7/chex/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55449 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/asserts_chexify.py
--rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/asserts_chexify_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/asserts_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/asserts_internal_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    61737 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/asserts_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/dataclass_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/dimensions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/fake_set_n_cpu_devices_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/pytypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/restrict_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/restrict_backends_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20448 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-03-27 10:43:54.000000 chex-0.1.7/chex/_src/variants_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-27 10:43:54.000000 chex-0.1.7/chex/chex_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:43:54.000000 chex-0.1.7/chex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:44:05.088654 chex-0.1.7/chex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-03-27 10:44:05.000000 chex-0.1.7/chex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-27 10:44:05.000000 chex-0.1.7/chex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:44:05.000000 chex-0.1.7/chex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:44:05.000000 chex-0.1.7/chex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-27 10:44:05.000000 chex-0.1.7/chex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 10:44:05.000000 chex-0.1.7/chex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:44:05.088654 chex-0.1.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-27 10:43:54.000000 chex-0.1.7/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-27 10:43:54.000000 chex-0.1.7/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-27 10:43:54.000000 chex-0.1.7/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 10:44:05.092654 chex-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-27 10:43:54.000000 chex-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.489947 chex-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-27 13:15:05.000000 chex-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-27 13:15:05.000000 chex-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-27 13:15:17.489947 chex-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-06-27 13:15:05.000000 chex-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.485947 chex-0.1.8/chex/
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-27 13:15:05.000000 chex-0.1.8/chex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.489947 chex-0.1.8/chex/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64909 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_chexify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23171 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_chexify_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_internal_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73097 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/dataclass_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/dimensions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/fake_set_n_cpu_devices_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/restrict_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/restrict_backends_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20448 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/variants_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-27 13:15:05.000000 chex-0.1.8/chex/chex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:05.000000 chex-0.1.8/chex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.489947 chex-0.1.8/chex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.489947 chex-0.1.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 13:15:05.000000 chex-0.1.8/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 13:15:05.000000 chex-0.1.8/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 13:15:05.000000 chex-0.1.8/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:15:17.489947 chex-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-27 13:15:05.000000 chex-0.1.8/setup.py
```

### Comparing `chex-0.1.7/LICENSE` & `chex-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/PKG-INFO` & `chex-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chex
-Version: 0.1.7
+Version: 0.1.8
 Summary: Chex: Testing made fun, in JAX!
 Home-page: https://github.com/deepmind/chex
 Author: DeepMind
 Author-email: chex-dev@google.com
 License: Apache 2.0
 Keywords: jax testing debugging python machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chex
 
 ![CI status](https://github.com/deepmind/chex/workflows/ci/badge.svg)
 ![docs](https://readthedocs.org/projects/chex/badge/?version=latest)
```

### Comparing `chex-0.1.7/README.md` & `chex-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/__init__.py` & `chex-0.1.8/chex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,47 +22,51 @@
 from chex._src.asserts import assert_axis_dimension_lteq
 from chex._src.asserts import assert_devices_available
 from chex._src.asserts import assert_equal
 from chex._src.asserts import assert_equal_rank
 from chex._src.asserts import assert_equal_shape
 from chex._src.asserts import assert_equal_shape_prefix
 from chex._src.asserts import assert_equal_shape_suffix
+from chex._src.asserts import assert_equal_size
 from chex._src.asserts import assert_exactly_one_is_none
 from chex._src.asserts import assert_gpu_available
 from chex._src.asserts import assert_is_broadcastable
 from chex._src.asserts import assert_is_divisible
 from chex._src.asserts import assert_max_traces
 from chex._src.asserts import assert_not_both_none
 from chex._src.asserts import assert_numerical_grads
 from chex._src.asserts import assert_rank
 from chex._src.asserts import assert_scalar
 from chex._src.asserts import assert_scalar_in
 from chex._src.asserts import assert_scalar_negative
 from chex._src.asserts import assert_scalar_non_negative
 from chex._src.asserts import assert_scalar_positive
 from chex._src.asserts import assert_shape
+from chex._src.asserts import assert_size
 from chex._src.asserts import assert_tpu_available
 from chex._src.asserts import assert_tree_all_close  # Deprecated
 from chex._src.asserts import assert_tree_all_equal_comparator  # Deprecated
 from chex._src.asserts import assert_tree_all_equal_shapes  # Deprecated
 from chex._src.asserts import assert_tree_all_equal_structs  # Deprecated
 from chex._src.asserts import assert_tree_all_finite
 from chex._src.asserts import assert_tree_has_only_ndarrays
 from chex._src.asserts import assert_tree_is_on_device
 from chex._src.asserts import assert_tree_is_on_host
 from chex._src.asserts import assert_tree_is_sharded
 from chex._src.asserts import assert_tree_no_nones
 from chex._src.asserts import assert_tree_shape_prefix
 from chex._src.asserts import assert_tree_shape_suffix
 from chex._src.asserts import assert_trees_all_close
+from chex._src.asserts import assert_trees_all_close_ulp
 from chex._src.asserts import assert_trees_all_equal
 from chex._src.asserts import assert_trees_all_equal_comparator
 from chex._src.asserts import assert_trees_all_equal_dtypes
 from chex._src.asserts import assert_trees_all_equal_shapes
 from chex._src.asserts import assert_trees_all_equal_shapes_and_dtypes
+from chex._src.asserts import assert_trees_all_equal_sizes
 from chex._src.asserts import assert_trees_all_equal_structs
 from chex._src.asserts import assert_type
 from chex._src.asserts import clear_trace_counter
 from chex._src.asserts import disable_asserts
 from chex._src.asserts import enable_asserts
 from chex._src.asserts import if_args_not_none
 from chex._src.asserts_chexify import block_until_chexify_assertions_complete
@@ -96,15 +100,15 @@
 from chex._src.variants import all_variants
 from chex._src.variants import ChexVariantType
 from chex._src.variants import params_product
 from chex._src.variants import TestCase
 from chex._src.variants import variants
 
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 __all__ = (
     "all_variants",
     "Array",
     "ArrayBatched",
     "ArrayDevice",
     "ArrayDeviceTree",
@@ -122,47 +126,51 @@
     "assert_axis_dimension_lteq",
     "assert_devices_available",
     "assert_equal",
     "assert_equal_rank",
     "assert_equal_shape",
     "assert_equal_shape_prefix",
     "assert_equal_shape_suffix",
+    "assert_equal_size",
     "assert_exactly_one_is_none",
     "assert_gpu_available",
     "assert_is_broadcastable",
     "assert_is_divisible",
     "assert_max_traces",
     "assert_not_both_none",
     "assert_numerical_grads",
     "assert_rank",
     "assert_scalar",
     "assert_scalar_in",
     "assert_scalar_negative",
     "assert_scalar_non_negative",
     "assert_scalar_positive",
     "assert_shape",
+    "assert_size",
     "assert_tpu_available",
     "assert_tree_all_close",  # Deprecated
     "assert_tree_all_equal_comparator",  # Deprecated
     "assert_tree_all_equal_shapes",  # Deprecated
     "assert_tree_all_equal_structs",  # Deprecated
     "assert_tree_all_finite",
     "assert_tree_has_only_ndarrays",
     "assert_tree_is_on_device",
     "assert_tree_is_on_host",
     "assert_tree_is_sharded",
     "assert_tree_no_nones",
     "assert_tree_shape_prefix",
     "assert_tree_shape_suffix",
     "assert_trees_all_close",
+    "assert_trees_all_close_ulp",
     "assert_trees_all_equal",
     "assert_trees_all_equal_comparator",
     "assert_trees_all_equal_dtypes",
     "assert_trees_all_equal_shapes",
     "assert_trees_all_equal_shapes_and_dtypes",
+    "assert_trees_all_equal_sizes",
     "assert_trees_all_equal_structs",
     "assert_type",
     "block_until_chexify_assertions_complete",
     "chexify",
     "ChexVariantType",
     "clear_trace_counter",
     "dataclass",
```

### Comparing `chex-0.1.7/chex/_src/__init__.py` & `chex-0.1.8/chex/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/asserts.py` & `chex-0.1.8/chex/_src/asserts.py`

 * *Files 14% similar despite different names*

```diff
@@ -362,14 +362,95 @@
   """
   assert_scalar(x)
   if x >= 0:
     raise AssertionError(f"The argument must be negative, was {x}.")
 
 
 @_static_assertion
+def assert_equal_size(inputs: Sequence[Array]) -> None:
+  """Checks that all arrays have the same size.
+
+  Args:
+    inputs: A collection of arrays.
+
+  Raises:
+    AssertionError: If the size of all arrays do not match.
+  """
+  _ai.assert_collection_of_arrays(inputs)
+  size = inputs[0].size
+  expected_sizes = [size] * len(inputs)
+  sizes = [x.size for x in inputs]
+  if sizes != expected_sizes:
+    raise AssertionError(f"Arrays have different sizes: {sizes}")
+
+
+@_static_assertion
+def assert_size(
+    inputs: Union[Scalar, Union[Array, Sequence[Array]]],
+    expected_sizes: Union[_ai.TShapeMatcher,
+                          Sequence[_ai.TShapeMatcher]]) -> None:
+  """Checks that the size of all inputs matches specified ``expected_sizes``.
+  
+  Valid usages include:
+
+  .. code-block:: python
+
+    assert_size(x, 1)                   # x is scalar (size 1)
+    assert_size([x, y], (2, {1, 3}))    # x has size 2, y has size 1 or 3
+    assert_size([x, y], (2, ...))       # x has size 2, y has any size
+    assert_size([x, y], 1)              # x and y are scalar (size 1)
+    assert_size((x, y), (5, 2))         # x has size 5, y has size 2
+
+  Args:
+    inputs: An array or a sequence of arrays.
+    expected_sizes: A sqeuence of expected sizes associated with each input,
+      where the expected size is a sequence of integer and `None` dimensions;
+      if all inputs have same size, a single size may be passed as 
+      ``expected_sizes``.
+
+  Raises:
+    AssertionError: If the lengths of ``inputs`` and ``expected_sizes`` do not
+      match; if ``expected_sizes`` has wrong type; if size of ``input`` does
+      not match ``expected_sizes``.
+  """
+  # Ensure inputs and expected sizes are sequences.
+  if not isinstance(inputs, collections.abc.Sequence):
+    inputs = [inputs]
+
+  if isinstance(expected_sizes, int):
+    expected_sizes = [expected_sizes] * len(inputs)
+
+  if not isinstance(expected_sizes, (list, tuple)):
+    raise AssertionError(
+        "Error in size compatibility check: expected sizes should be an int, "
+        f"list, or tuple of ints, got {expected_sizes}.")  
+
+  if len(inputs) != len(expected_sizes):
+    raise AssertionError(
+        "Length of `inputs` and `expected_sizes` must match: "
+        f"{len(inputs)} is not equal to {len(expected_sizes)}.")
+
+  errors = []
+  for idx, (x, expected) in enumerate(zip(inputs, expected_sizes)):
+    size = getattr(x, "size", 1)  # scalars have size 1 by definition.
+    # Allow any size for the ellipsis case and allow handling of integer
+    # expected sizes or collection of acceptable expected sizes.
+    int_condition = expected in {Ellipsis, None} or size == expected
+    set_condition = (isinstance(expected, collections.abc.Collection) and
+                     size in expected)
+    if not (int_condition or set_condition):
+      errors.append((idx, size, expected))
+
+  if errors:
+    msg = "; ".join(
+        f"input {e[0]} has size {e[1]} but expected {e[2]}" for e in errors)
+    raise AssertionError(f"Error in size compatibility check: {msg}.")
+
+
+@_static_assertion
 def assert_equal_shape(
     inputs: Sequence[Array],
     *,
     dims: Optional[Union[int, Sequence[int]]] = None) -> None:
   """Checks that all arrays have the same shape.
 
   Args:
@@ -471,16 +552,16 @@
   return True
 
 
 def _shape_matches(actual_shape: Sequence[int],
                    expected_shape: _ai.TShapeMatcher) -> bool:
   """Returns True if `actual_shape` is compatible with `expected_shape`."""
   # Splits `expected_shape` based on the position of the ellipsis, if present.
-  expected_prefix: List[Union[int, Set[int]]] = []
-  expected_suffix: Optional[List[Union[int, Set[int]]]] = None
+  expected_prefix: List[_ai.TDimMatcher] = []
+  expected_suffix: Optional[List[_ai.TDimMatcher]] = None
   for dim in expected_shape:
     if dim is Ellipsis:
       if expected_suffix is not None:
         raise ValueError(
             "`expected_shape` may not contain more than one ellipsis, "
             f"but got {_ai.format_shape_matcher(expected_shape)}")
       expected_suffix = []
@@ -775,15 +856,16 @@
       false when the assertion should fail.
     error_string: string which is inserted in assertion failure messages -
       'expected tensor to have dimension {error_string} on axis ...'.
 
   Raises:
     AssertionError: if `pass_fn(tensor.shape[axis], val)` does not return true.
   """
-  tensor = jnp.asarray(tensor)
+  if not isinstance(tensor, (jax.Array, np.ndarray)):
+    tensor = np.asarray(tensor)  # np is broader than jnp (it supports strings)
   if axis >= len(tensor.shape) or axis < -len(tensor.shape):
     raise AssertionError(
         f"Expected tensor to have dim {error_string} on axis "
         f"'{axis}' but axis '{axis}' not available: tensor rank is "
         f"'{len(tensor.shape)}'.")
   if not pass_fn(tensor.shape[axis]):
     raise AssertionError(
@@ -983,14 +1065,15 @@
       return len(x.sharding.device_set) > 1
   # pytype: disable=attribute-error
   return (
       hasattr(jax, "pxla")
       and hasattr(jax.pxla, "ShardedDeviceArray")
       and isinstance(x, jax.pxla.ShardedDeviceArray)
   )
+  # pytype: enable=attribute-error
 
 
 @_static_assertion
 def assert_tree_is_on_host(
     tree: ArrayTree,
     *,
     allow_cpu_device: bool = True,
@@ -1194,14 +1277,17 @@
   Raises:
     AssertionError: If some leaf's shape doesn't start with ``shape_prefix``;
       if ``ignore_nones`` isn't set and the tree contains `None`.
   """
   if not ignore_nones:
     assert_tree_no_nones(tree)
 
+  # To compare with the leaf's `shape`, convert int sequence to tuple.
+  shape_prefix = tuple(shape_prefix)
+
   if not shape_prefix:
     return  # No prefix, this is trivially true.
 
   errors = []
 
   def _assert_fn(path, leaf):
     if leaf is None:
@@ -1242,14 +1328,18 @@
 
   Raises:
     AssertionError: If some leaf's shape doesn't start with ``shape_suffix``;
       if ``ignore_nones`` isn't set and the tree contains `None`.
   """
   if not ignore_nones:
     assert_tree_no_nones(tree)
+
+  # To compare with the leaf's `shape`, convert int sequence to tuple.
+  shape_suffix = tuple(shape_suffix)
+
   if not shape_suffix:
     return  # No suffix, this is trivially true.
 
   errors = []
 
   def _assert_fn(path, leaf):
     if leaf is None:
@@ -1402,14 +1492,34 @@
     return f"types: {arr_1.dtype} != {arr_2.dtype}"
 
   assert_trees_all_equal_comparator(
       cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones)
 
 
 @_static_assertion
+def assert_trees_all_equal_sizes(*trees: ArrayTree,
+                                 ignore_nones: bool = False) -> None:
+  """Checks that trees have the same structure and leaves' sizes.
+
+  Args:
+    *trees: A sequence of (at least 2) trees with array leaves.
+    ignore_nones: Whether to ignore `None` in the trees.
+
+  Raises:
+    AssertionError: If trees' structures or leaves' sizes are different;
+      if the trees contain `None` (with ``ignore_nones=False``).
+  """
+  cmp_fn = lambda arr_1, arr_2: arr_1.size == arr_2.size
+  err_msg_fn = lambda arr_1, arr_2: f"sizes: {arr_1.size} != {arr_2.size}"
+  assert_trees_all_equal_comparator(
+      cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones
+  )
+
+
+@_static_assertion
 def assert_trees_all_equal_shapes(*trees: ArrayTree,
                                   ignore_nones: bool = False) -> None:
   """Checks that trees have the same structure and leaves' shapes.
 
   Args:
     *trees: A sequence of (at least 2) trees with array leaves.
     ignore_nones: Whether to ignore `None` in the trees.
@@ -1489,35 +1599,39 @@
 assert_tree_all_finite = _value_assertion(
     assert_fn=_assert_tree_all_finite_static,
     jittable_assert_fn=_assert_tree_all_finite_jittable,
     name="assert_tree_all_finite")
 
 
 @_static_assertion
-def _assert_trees_all_equal_static(*trees: ArrayTree,
-                                   ignore_nones: bool = False) -> None:
+def _assert_trees_all_equal_static(
+    *trees: ArrayTree, ignore_nones: bool = False, strict: bool = False
+) -> None:
   """Checks that all trees have leaves with *exactly* equal values.
 
   If you are comparing floating point numbers, an exact equality check may not
   be appropriate; consider using ``assert_trees_all_close``.
 
   Args:
     *trees: A sequence of (at least 2) trees with array leaves.
     ignore_nones: Whether to ignore `None` in the trees.
+    strict: If True, disable special scalar handling as described in
+      `np.testing.assert_array_equals` notes section.
 
   Raises:
     AssertionError: If the leaf values actual and desired are not exactly equal,
       or the trees contain `None` (with ``ignore_nones=False``).
   """
 
   def assert_fn(arr_1, arr_2):
     np.testing.assert_array_equal(
         _ai.jnp_to_np_array(arr_1),
         _ai.jnp_to_np_array(arr_2),
-        err_msg="Error in value equality check: Values not exactly equal")
+        err_msg="Error in value equality check: Values not exactly equal",
+        strict=strict)
 
   def cmp_fn(arr_1, arr_2) -> bool:
     try:
       # Raises an AssertionError if values are not equal.
       assert_fn(arr_1, arr_2)
     except AssertionError:
       return False
@@ -1532,17 +1646,26 @@
     return ""
 
   assert_trees_all_equal_comparator(
       cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones)
 
 
 def _assert_trees_all_equal_jittable(
-    *trees: ArrayTree, ignore_nones: bool = False
+    *trees: ArrayTree, ignore_nones: bool = False, strict: bool = True,
 ) -> Array:
   """A jittable version of `_assert_trees_all_equal_static`."""
+  if not strict:
+    raise NotImplementedError(
+        "`strict=False` is not implemented by"
+        " `_assert_trees_all_equal_jittable`. This is a feature of"
+        " `np.testing.assert_array_equal` used in the static implementation of"
+        " `assert_trees_all_equal` that we do not implement in the jittable"
+        " version."
+    )
+
   if not ignore_nones:
     assert_tree_no_nones(trees)
 
   err_msg_template = "Values not exactly equal: {arr_1} != {arr_2}."
   cmp_fn = lambda x, y: jnp.array_equal(x, y, equal_nan=True)
   return _ai.assert_trees_all_eq_comparator_jittable(
       cmp_fn, err_msg_template, *trees
@@ -1628,7 +1751,135 @@
     jittable_assert_fn=_assert_trees_all_close_jittable,
     name="assert_trees_all_close")
 
 assert_tree_all_close = _ai.deprecation_wrapper(
     assert_trees_all_close,
     old_name="assert_tree_all_close",
     new_name="assert_trees_all_close")
+
+
+def _assert_trees_all_close_ulp_static(
+    *trees: ArrayTree,
+    maxulp: int = 1,
+    ignore_nones: bool = False,
+) -> None:
+  """Checks that tree leaves differ by at most `maxulp` Units in the Last Place.
+
+  This is the Chex version of np.testing.assert_array_max_ulp.
+
+  Assertions on floating point values are tricky because the precision varies
+  depending on the value. For example, with float32, the precision at 1 is
+  np.spacing(np.float32(1.0)) ≈ 1e-7, but the precision at 5,000,000 is only
+  np.spacing(np.float32(5e6)) = 0.5. This makes it hard to predict ahead of time
+  what tolerance to use when checking whether two numbers are equal: a
+  difference of only a couple of bits can equate to an arbitrarily large
+  absolute difference.
+
+  Assertions based on _relative_ differences are one solution to this problem,
+  but have the disadvantage that it's hard to choose the tolerance. If you want
+  to verify that two calculations produce _exactly_ the same result
+  modulo the inherent non-determinism of floating point operations, do you set
+  the tolerance to...0.01? 0.001? It's hard to be sure you've set it low enough
+  that you won't miss one of your computations being slightly wrong.
+
+  Assertions based on 'units in the last place' (ULP) instead solve this
+  problem by letting you specify tolerances in terms of the precision actually
+  available at the current scale of your values. The ULP at some value x is
+  essentially the spacing between the floating point numbers actually
+  representable in the vicinity of x - equivalent to the 'precision' we
+  discussed above. above. With a tolerance of, say, `maxulp=5`, you're saying
+  that two values are within 5 actually-representable-numbers of each other -
+  a strong guarantee that two computations are as close as possible to
+  identical, while still allowing reasonable wiggle room for small differences
+  due to e.g. different operator orderings.
+
+  Note that this function is not currently supported within JIT contexts,
+  and does not currently support bfloat16 dtypes.
+
+  Args:
+    *trees: A sequence of (at least 2) trees with array leaves.
+    maxulp: The maximum number of ULPs by which leaves may differ.
+    ignore_nones: Whether to ignore `None` in the trees.
+
+  Raises:
+    AssertionError: If actual and desired values are not equal up to
+      specified tolerance; if the trees contain `None` (with
+      ``ignore_nones=False``).
+  """
+
+  def assert_fn(arr_1, arr_2):
+    if (
+        getattr(arr_1, "dtype", None) == jnp.bfloat16
+        or getattr(arr_2, "dtype", None) == jnp.bfloat16
+    ):
+      # jnp_to_np_array currently converts bfloat16 to float32, which will cause
+      # assert_array_max_ulp to give incorrect results -
+      # and assert_array_max_ulp itself does not currently support bfloat16:
+      # https://github.com/jax-ml/ml_dtypes/issues/56
+      raise ValueError(
+          f"{_ai.ERR_PREFIX}ULP assertions are not currently supported for "
+          "bfloat16."
+      )
+    np.testing.assert_array_max_ulp(
+        _ai.jnp_to_np_array(arr_1),
+        _ai.jnp_to_np_array(arr_2),
+        maxulp=maxulp,
+    )
+
+  def cmp_fn(arr_1, arr_2) -> bool:
+    try:
+      # Raises an AssertionError if values are not close.
+      assert_fn(arr_1, arr_2)
+    except AssertionError:
+      return False
+    return True
+
+  def err_msg_fn(arr_1, arr_2) -> str:
+    try:
+      assert_fn(arr_1, arr_2)
+    except AssertionError as e:
+      return (
+          f"{str(e)} \nOriginal dtypes: "
+          f"{np.asarray(arr_1).dtype}, {np.asarray(arr_2).dtype}"
+      )
+    return ""
+
+  assert_trees_all_equal_comparator(
+      cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones
+  )
+
+
+# The return should be typing.NoReturn, but that would significantly complicate
+# the signature of _value_assertion, so we pretend the return is jax.Array.
+def _assert_trees_all_close_ulp_jittable(
+    *trees: ArrayTree,
+    maxulp: int = 1,
+    ignore_nones: bool = False,
+) -> jax.Array:
+  """A dummy jittable version of `_assert_trees_all_close_ulp_static`.
+
+  JAX does not yet have a native version of assert_array_max_ulp, so at the
+  moment making ULP assertions on tracer objects simply isn't supported.
+  This function exists only to make sure a sensible error is given.
+
+  Args:
+    *trees: Ignored.
+    maxulp: Ignored.
+    ignore_nones: Ignored.
+
+  Raises:
+    NotImplementedError: unconditionally.
+
+  Returns:
+    Never returns. (We pretend jax.Array to satisfy the type checker.)
+  """
+  raise NotImplementedError(
+      f"{_ai.ERR_PREFIX}assert_trees_all_close_ulp is not supported within JIT "
+      "contexts."
+  )
+
+
+assert_trees_all_close_ulp = _value_assertion(
+    assert_fn=_assert_trees_all_close_ulp_static,
+    jittable_assert_fn=_assert_trees_all_close_ulp_jittable,
+    name="assert_trees_all_close_ulp",
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chex-0.1.7/chex/_src/asserts_chexify.py` & `chex-0.1.8/chex/_src/asserts_chexify.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,23 @@
   """
   # Hardware/XLA failures can only happen on the C++ side. They are expected to
   # issue critical errors that will immediately crash the whole program.
   # Nevertheless, Chex sets its own timeout for every chexified XLA comp. to
   # ensure that a program never blocks on Chex side when running in async mode.
   async_timeout = 1800  # 30 minutes
 
+  # Get function name.
+  if isinstance(fn, functools.partial):
+    func_name = fn.func.__name__
+  else:
+    func_name = fn.__name__
+
   if async_check:
     # Spawn a thread for processing blocking calls.
-    thread_pool = futures.ThreadPoolExecutor(1, f'async_chex_{fn.__name__}')
+    thread_pool = futures.ThreadPoolExecutor(1, f'async_chex_{func_name}')
     # A deque for futures.
     async_check_futures = collections.deque()
 
   # Checkification.
   checkified_fn = checkify.checkify(fn, errors=errors)
 
   @functools.wraps(fn)
@@ -216,15 +222,15 @@
 
   # Add the callback to the chexified funtion's properties.
   if not hasattr(_chexified_fn, 'wait_checks'):
     _chexified_fn.wait_checks = _wait_checks
   else:
     logging.warning(
         "Function %s already defines 'wait_checks' method; "
-        'Chex will not redefine it.', _chexified_fn.__name__)
+        'Chex will not redefine it.', func_name)
 
   return _chexified_fn
 
 
 def with_jittable_assertions(fn: Callable[..., Any],
                              async_check: bool = True) -> Callable[..., Any]:
   """An alias for `chexify` (see the docs)."""
```

### Comparing `chex-0.1.7/chex/_src/asserts_chexify_test.py` & `chex-0.1.8/chex/_src/asserts_chexify_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,29 @@
       take_by_index_and_div_safe(jnp.ones(2), 1, 0)  # Div-by-0
 
     with self.assertRaisesRegex(
         asserts_chexify.checkify.JaxRuntimeError, 'out-of-bounds'
     ):
       take_by_index_and_div_safe(jnp.ones(2), 10, 0)  # OOB (first) & Div-by-0
 
+  def test_partial_python_fn(self):
+    def fn(x, y):
+      asserts.assert_trees_all_equal(x, y)
+      return jax.tree_map(jnp.add, x, y)
+
+    partial_fn = functools.partial(fn, y=jnp.array([1]))
+    chexified_fn = chexify_async(partial_fn)  # note: fn is not transformed
+
+    chexified_fn(jnp.array([1]))
+    chexified_fn.wait_checks()
+
+    with self.assertRaisesRegex(AssertionError, '0 and 1 differ'):
+      chexified_fn(jnp.array([2]))
+      chexified_fn.wait_checks()  # Fail: not equal
+
 
 class AssertsChexifyTestSuite(variants.TestCase):
   """Test suite for chexify assertions."""
 
   def run_test_suite(self, make_test_fn, all_valid_args, all_invalid_args,
                      failure_labels, jax_transform, run_pure):
     """Runs a set of tests for static & value assertions.
@@ -604,15 +619,17 @@
   def test_custom_message(self):
     @jax.jit
     def fn(x, y):
       asserts.assert_trees_all_equal(
           x,
           y,
           custom_message='sum(x)={}',
-          custom_message_format_vars=[sum(l.sum() for l in jax.tree_leaves(x))],
+          custom_message_format_vars=[
+              sum(l.sum() for l in jax.tree_util.tree_leaves(x))
+          ],
       )
       return jax.tree_map(jnp.add, x, y)
 
     chexified_fn = asserts_chexify.chexify(fn, async_check=False)
 
     tree_1 = {'a': jnp.array([3]), 'b': jnp.array([10, 10])}
     tree_2 = {'a': jnp.array([3]), 'b': jnp.array([10, 320])}
```

### Comparing `chex-0.1.7/chex/_src/asserts_internal.py` & `chex-0.1.8/chex/_src/asserts_internal.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/asserts_internal_test.py` & `chex-0.1.8/chex/_src/asserts_internal_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/asserts_test.py` & `chex-0.1.8/chex/_src/asserts_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -276,14 +276,90 @@
                                 _get_err_regex('argument must be in')):
       asserts.assert_scalar_in(0, 0, 1, included=False)
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('argument must be in')):
       asserts.assert_scalar_in(1, 0, 1, included=False)
 
 
+class EqualSizeAssertTest(parameterized.TestCase):
+
+  @parameterized.named_parameters(
+      ('scalar_vector_matrix', [1, 2, [3], [[4, 5]]]),
+      ('vector_matrix', [[1], [2], [[3, 5]]]),
+      ('matrix', [[[1, 2]], [[3], [4], [5]]]),
+  )
+  def test_equal_size_should_fail(self, arrays):
+    arrays = as_arrays(arrays)
+    with self.assertRaisesRegex(
+        AssertionError, _get_err_regex('Arrays have different sizes')
+    ):
+      asserts.assert_equal_size(arrays)
+
+  @parameterized.named_parameters(
+      ('scalar_vector_matrix', [1, 2, [3], [[4]]]),
+      ('vector_matrix', [[1], [2], [[3]]]),
+      ('matrix', [[[1, 2]], [[3], [4]]]),
+  )
+  def test_equal_size_should_pass(self, arrays):
+    arrays = as_arrays(arrays)
+    asserts.assert_equal_size(arrays)
+
+
+class SizeAssertTest(parameterized.TestCase):
+
+  @parameterized.named_parameters(
+      ('wrong_size', [1, 2], 2),
+      ('some_wrong_size', [[1, 2], [3, 4]], (2, 3)),
+      ('wrong_common_shape', [[1, 2], [3, 4, 3]], 3),
+      ('wrong_common_shape_2', [[1, 2, 3], [1, 2]], 2),
+      ('some_wrong_size_set', [[1, 2], [3, 4]], (2, {3, 4})),
+  )
+  def test_size_should_fail(self, arrays, sizes):
+    arrays = as_arrays(arrays)
+    with self.assertRaisesRegex(
+        AssertionError,
+        _get_err_regex('input .+ has size .+ but expected .+')):
+      asserts.assert_size(arrays, sizes)
+
+  @parameterized.named_parameters(
+      ('too_many_sizes', [[1]], (1, 1)),
+      ('not_enough_sizes', [[1, 2], [3, 4], [5, 6]], (2, 2)),
+  )
+  def test_size_should_fail_wrong_length(self, arrays, sizes):
+    arrays = as_arrays(arrays)
+    with self.assertRaisesRegex(
+        AssertionError,
+        _get_err_regex('Length of `inputs` and `expected_sizes` must match')):
+      asserts.assert_size(arrays, sizes)
+
+  @parameterized.named_parameters(
+      ('scalars', [1, 2], 1),
+      ('vectors', [[1, 2], [3, 4, 5]], [2, 3]),
+      ('matrices', [[[1, 2], [3, 4]]], 4),
+      ('common_size_set', [[[1, 2], [3, 4]], [[1], [3]]], (4, {1, 2})),
+  )
+  def test_size_should_pass(self, arrays, sizes):
+    arrays = as_arrays(arrays)
+    asserts.assert_size(arrays, sizes)
+
+  def test_pytypes_pass(self):
+    arrays = as_arrays([[[1, 2], [3, 4]], [[1], [3]]])
+    asserts.assert_size(arrays, (4, None))
+    asserts.assert_size(arrays, (4, {1, 2}))
+    asserts.assert_size(arrays, (4, ...))
+
+  @parameterized.named_parameters(
+      ('single_ellipsis', [[1, 2, 3, 4], [1, 2]], (..., 2)),
+      ('multiple_ellipsis', [[1, 2, 3], [1, 2, 3]], (..., ...)),
+  )
+  def test_ellipsis_should_pass(self, arrays, expected_size):
+    arrays = as_arrays(arrays)
+    asserts.assert_size(arrays, expected_size)
+
+
 class EqualShapeAssertTest(parameterized.TestCase):
 
   @parameterized.named_parameters(
       ('not_scalar', [1, 2, [3]]),
       ('wrong_rank', [[1], [2], 3]),
       ('wrong_length', [[1], [2], [3, 4]]),
   )
@@ -352,78 +428,106 @@
       ('some_wrong_shape', [[1, 2], [3, 4]], [(1, 2), (1, 3)]),
       ('wrong_common_shape', [[1, 2], [3, 4, 3]], (2,)),
       ('wrong_common_shape_2', [[1, 2, 3], [1, 2]], (2,)),
       ('some_wrong_shape_set', [[1, 2], [3, 4]], [(1, 2), (1, {3, 4})]),
   )
   def test_shape_should_fail(self, arrays, shapes):
     arrays = as_arrays(arrays)
-    with self.assertRaisesRegex(
-        AssertionError,
-        _get_err_regex('input .+ has shape .+ but expected .+')):
-      asserts.assert_shape(arrays, shapes)
+    with self.subTest('list'):
+      with self.assertRaisesRegex(
+          AssertionError,
+          _get_err_regex('input .+ has shape .+ but expected .+')):
+        asserts.assert_shape(arrays, list(shapes))
+    with self.subTest('tuple'):
+      with self.assertRaisesRegex(
+          AssertionError,
+          _get_err_regex('input .+ has shape .+ but expected .+')):
+        asserts.assert_shape(arrays, tuple(shapes))
 
   @parameterized.named_parameters(
       ('too_many_shapes', [[1]], [(1,), (2,)]),
       ('not_enough_shapes', [[1, 2], [3, 4]], [(3,)]),
   )
   def test_shape_should_fail_wrong_length(self, arrays, shapes):
     arrays = as_arrays(arrays)
     with self.assertRaisesRegex(
         AssertionError,
         _get_err_regex('Length of `inputs` and `expected_shapes` must match')):
-      asserts.assert_shape(arrays, shapes)
+      asserts.assert_shape(arrays, tuple(shapes))
+    with self.assertRaisesRegex(
+        AssertionError,
+        _get_err_regex('Length of `inputs` and `expected_shapes` must match')):
+      asserts.assert_shape(arrays, list(shapes))
 
   @parameterized.named_parameters(
       ('scalars', [1, 2], ()),
       ('vectors', [[1, 2], [3, 4, 5]], [(2,), (3,)]),
       ('matrices', [[[1, 2], [3, 4]]], (2, 2)),
       ('matrices_variable_shape', [[[1, 2], [3, 4]]], (None, 2)),
       ('vectors_common_shape', [[1, 2], [3, 4]], (2,)),
       ('variable_common_shape', [[[1, 2], [3, 4]], [[1], [3]]], (2, None)),
       ('common_shape_set', [[[1, 2], [3, 4]], [[1], [3]]], (2, {1, 2})),
   )
   def test_shape_should_pass(self, arrays, shapes):
     arrays = as_arrays(arrays)
-    asserts.assert_shape(arrays, shapes)
+    with self.subTest('tuple'):
+      asserts.assert_shape(arrays, tuple(shapes))
+    with self.subTest('list'):
+      asserts.assert_shape(arrays, list(shapes))
 
-  def test_pytypes_pass(self):
+  @parameterized.named_parameters(
+      ('variable_shape', (2, None)),
+      ('shape_set', (2, {1, 2})),
+      ('suffix', (2, ...)),
+  )
+  def test_pytypes_pass(self, shape):
     arrays = as_arrays([[[1, 2], [3, 4]], [[1], [3]]])
-    asserts.assert_shape(arrays, (2, None))
-    asserts.assert_shape(arrays, (2, {1, 2}))
-    asserts.assert_shape(arrays, (2, ...))
+    with self.subTest('tuple'):
+      asserts.assert_shape(arrays, tuple(shape))
+    with self.subTest('list'):
+      asserts.assert_shape(arrays, list(shape))
 
   @parameterized.named_parameters(
       ('prefix_2', array_from_shape(2, 3, 4, 5, 6), (..., 4, 5, 6)),
       ('prefix_1', array_from_shape(3, 4, 5, 6), (..., 4, 5, 6)),
       ('prefix_0', array_from_shape(4, 5, 6), (..., 4, 5, 6)),
       ('inner_2', array_from_shape(2, 3, 4, 5, 6), (2, 3, ..., 6)),
       ('inner_1', array_from_shape(2, 3, 4, 6), (2, 3, ..., 6)),
       ('inner_0', array_from_shape(2, 3, 6), (2, 3, ..., 6)),
       ('suffix_2', array_from_shape(2, 3, 4, 5, 6), (2, 3, 4, ...)),
       ('suffix_1', array_from_shape(2, 3, 4, 5), (2, 3, 4, ...)),
       ('suffix_0', array_from_shape(2, 3, 4), (2, 3, 4, ...)),
   )
   def test_ellipsis_should_pass(self, array, expected_shape):
-    asserts.assert_shape(array, expected_shape)
+    with self.subTest('list'):
+      asserts.assert_shape(array, list(expected_shape))
+    with self.subTest('tuple'):
+      asserts.assert_shape(array, tuple(expected_shape))
 
   @parameterized.named_parameters(
       ('prefix', array_from_shape(3, 1, 5), (..., 4, 5, 6)),
       ('inner_bad_prefix', array_from_shape(2, 1, 4, 6), (2, 3, ..., 6)),
       ('inner_bad_suffix', array_from_shape(2, 3, 1, 5), (2, 3, ..., 6)),
       ('inner_both_bad', array_from_shape(2, 1, 4, 5), (2, 3, ..., 6)),
       ('suffix', array_from_shape(2, 3, 1, 5), (2, 3, 4, ...)),
       ('short_rank_prefix', array_from_shape(2, 3), (..., 4, 5, 6)),
       ('short_rank_inner', array_from_shape(2, 3), (2, 3, ..., 6)),
       ('short_rank_suffix', array_from_shape(2, 3), (2, 3, 4, ...)),
   )
   def test_ellipsis_should_fail(self, array, expected_shape):
-    with self.assertRaisesRegex(
-        AssertionError,
-        _get_err_regex('input .+ has shape .+ but expected .+')):
-      asserts.assert_shape(array, expected_shape)
+    with self.subTest('tuple'):
+      with self.assertRaisesRegex(
+          AssertionError,
+          _get_err_regex('input .+ has shape .+ but expected .+')):
+        asserts.assert_shape(array, tuple(expected_shape))
+    with self.subTest('list'):
+      with self.assertRaisesRegex(
+          AssertionError,
+          _get_err_regex('input .+ has shape .+ but expected .+')):
+        asserts.assert_shape(array, list(expected_shape))
 
   @parameterized.named_parameters(
       ('prefix_and_suffix', array_from_shape(2, 3), (..., 2, 3, ...)),)
   def test_multiple_ellipses(self, array, expected_shape):
     with self.assertRaisesRegex(  # pylint: disable=g-error-prone-assert-raises
         ValueError,
         '`expected_shape` may not contain more than one ellipsis, but got .+'):
@@ -734,14 +838,19 @@
   def test_assert_axis_dimension_lteq_axis_invalid(self):
     tensor = jnp.ones((3, 2))
     for i in (2, -3):
       with self.assertRaisesRegex(AssertionError,
                                   _get_err_regex('not available')):
         asserts.assert_axis_dimension_lteq(tensor, axis=i, val=0)
 
+  def test_assert_axis_dimension_string_tensor(self):
+    tensor = ['ab', 'cddd']
+    asserts.assert_axis_dimension(tensor, axis=0, expected=2)
+    asserts.assert_axis_dimension(np.array(tensor), axis=0, expected=2)
+
 
 class TreeAssertionsTest(parameterized.TestCase):
 
   def _assert_tree_structs_validation(self, assert_fn):
     """Checks that assert_fn correctly processes invalid args' structs."""
 
     get_val = lambda: jnp.zeros([3])
@@ -830,14 +939,38 @@
     err_regex = _get_err_regex('`None` detected')
     with self.assertRaisesRegex(AssertionError, err_regex):
       asserts.assert_trees_all_equal(tree, tree, ignore_nones=False)
 
     with self.assertRaisesRegex(AssertionError, err_regex):
       asserts._assert_trees_all_equal_jittable(tree, tree, ignore_nones=False)
 
+  def test_assert_trees_all_equal_strict_mode(self):
+    # See 'notes' section of
+    # https://numpy.org/doc/stable/reference/generated/numpy.testing.assert_array_equal.html
+    # for details about the 'strict' mode of `numpy.testing.assert_array_equal`.
+    # tldr; it has special handling for scalar values (by default).
+    tree1 = {'a': jnp.array([1.0], dtype=jnp.float32), 'b': 0.0}
+    tree2 = {'a': jnp.array(1.0, dtype=jnp.float32), 'b': 0.0}
+
+    asserts.assert_trees_all_equal(tree1, tree2)
+    asserts.assert_trees_all_equal(tree1, tree2, strict=False)
+    err_regex = _get_err_regex(r'Trees 0 and 1 differ in leaves \'a\'')
+    with self.assertRaisesRegex(AssertionError, err_regex):
+      asserts.assert_trees_all_equal(tree1, tree2, strict=True)
+
+    err_regex = r'Trees 0 and 1 differ in leaves'
+    with self.assertRaisesRegex(ValueError, err_regex):
+      asserts._assert_trees_all_equal_jittable(tree1, tree2, strict=True)
+
+    # We do not implement this special scalar handling in the jittable
+    # assertion (it's possible, but doesn't seem worth the effort).
+    err_regex = r'`strict=False` is not implemented'
+    with self.assertRaisesRegex(NotImplementedError, err_regex):
+      asserts._assert_trees_all_equal_jittable(tree1, tree2, strict=False)
+
   def test_assert_trees_all_close_passes_same_tree(self):
     tree = {
         'a': [jnp.zeros((1,))],
         'b': ([0], (0,), 0),
     }
     asserts.assert_trees_all_close(tree, tree)
     tree = jax.tree_map(jnp.asarray, tree)
@@ -884,14 +1017,88 @@
       asserts._assert_trees_all_close_jittable(tree1, tree3)
 
     with self.assertRaisesRegex(AssertionError, err_regex):
       asserts.assert_trees_all_close(tree2, tree3)
     with self.assertRaisesRegex(ValueError, err_msg):
       asserts._assert_trees_all_close_jittable(tree2, tree3)
 
+  def test_assert_trees_all_close_ulp_jittable_raises_valueerror(self):
+    tree = (jnp.array([1.0]),)
+    err_msg = 'assert_trees_all_close_ulp is not supported within JIT contexts.'
+    err_regex = _get_err_regex(err_msg)
+    with self.assertRaisesRegex(RuntimeError, err_regex):
+      asserts._assert_trees_all_close_ulp_jittable(tree, tree)
+
+  def test_assert_trees_all_close_ulp_passes_same_tree(self):
+    tree = {
+        'a': [jnp.zeros((1,))],
+        'b': ([0], (0,), 0),
+    }
+    asserts.assert_trees_all_close_ulp(tree, tree)
+
+  def test_assert_trees_all_close_ulp_passes_values_equal(self):
+    tree1 = (jnp.array([0.0, 0.0]),)
+    tree2 = (jnp.array([0.0, 0.0]),)
+    try:
+      asserts.assert_trees_all_close_ulp(tree1, tree2)
+    except AssertionError:
+      self.fail('assert_trees_all_close_ulp raised AssertionError')
+
+  def test_assert_trees_all_close_ulp_passes_values_within_maxulp(self):
+    # np.spacing(np.float32(1 << 23)) == 1.0.
+    value_where_ulp_is_1 = np.float32(1 << 23)
+    tree1 = (jnp.array([value_where_ulp_is_1, value_where_ulp_is_1]),)
+    tree2 = (jnp.array([value_where_ulp_is_1, value_where_ulp_is_1 + 1.0]),)
+    assert tree2[0][0] != tree2[0][1]
+    try:
+      asserts.assert_trees_all_close_ulp(tree1, tree2, maxulp=2)
+    except AssertionError:
+      self.fail('assert_trees_all_close_ulp raised AssertionError')
+
+  def test_assert_trees_all_close_ulp_passes_values_maxulp_apart(self):
+    # np.spacing(np.float32(1 << 23)) == 1.0.
+    value_where_ulp_is_1 = np.float32(1 << 23)
+    tree1 = (jnp.array([value_where_ulp_is_1, value_where_ulp_is_1]),)
+    tree2 = (jnp.array([value_where_ulp_is_1, value_where_ulp_is_1 + 1.0]),)
+    assert tree2[0][0] != tree2[0][1]
+    try:
+      asserts.assert_trees_all_close_ulp(tree1, tree2, maxulp=1)
+    except AssertionError:
+      self.fail('assert_trees_all_close_ulp raised AssertionError')
+
+  def test_assert_trees_all_close_ulp_fails_values_gt_maxulp_apart(self):
+    # np.spacing(np.float32(1 << 23)) == 1.0.
+    value_where_ulp_is_1 = np.float32(1 << 23)
+    tree1 = (jnp.array([value_where_ulp_is_1, value_where_ulp_is_1]),)
+    tree2 = (jnp.array([value_where_ulp_is_1, value_where_ulp_is_1 + 2.0]),)
+    assert tree2[0][0] != tree2[0][1]
+    err_msg = re.escape(
+        'not almost equal up to 1 ULP (max difference is 2 ULP)'
+    )
+    err_regex = _get_err_regex(err_msg)
+    with self.assertRaisesRegex(AssertionError, err_regex):
+      asserts.assert_trees_all_close_ulp(tree1, tree2, maxulp=1)
+
+  def test_assert_trees_all_close_ulp_nones(self):
+    tree = {'a': [jnp.zeros((1,))], 'b': None}
+    asserts.assert_trees_all_close_ulp(tree, tree, ignore_nones=True)
+    err_regex = _get_err_regex('`None` detected')
+    with self.assertRaisesRegex(AssertionError, err_regex):
+      asserts.assert_trees_all_close_ulp(tree, tree, ignore_nones=False)
+
+  def test_assert_trees_all_close_ulp_fails_bfloat16(self):
+    tree_f32 = (jnp.array([0.0]),)
+    tree_bf16 = (jnp.array([0.0], dtype=jnp.bfloat16),)
+    err_msg = 'ULP assertions are not currently supported for bfloat16.'
+    err_regex = _get_err_regex(err_msg)
+    with self.assertRaisesRegex(ValueError, err_regex):  # pylint: disable=g-error-prone-assert-raises
+      asserts.assert_trees_all_close_ulp(tree_bf16, tree_bf16)
+    with self.assertRaisesRegex(ValueError, err_regex):  # pylint: disable=g-error-prone-assert-raises
+      asserts.assert_trees_all_close_ulp(tree_bf16, tree_f32)
+
   def test_assert_trees_all_equal_shapes_nones(self):
     tree = {'a': [jnp.zeros((1,))], 'b': None}
     asserts.assert_trees_all_equal_shapes(tree, tree, ignore_nones=True)
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('`None` detected')):
       asserts.assert_trees_all_equal_shapes(tree, tree, ignore_nones=False)
 
@@ -1221,14 +1428,38 @@
       asserts.assert_trees_all_close(tree1, tree2, atol=0.01)
 
     asserts.assert_trees_all_close(tree1, tree2, rtol=0.1)
     with self.assertRaisesRegex(
         AssertionError, _get_err_regex('Values not approximately equal')):
       asserts.assert_trees_all_close(tree1, tree2, rtol=0.01)
 
+  def test_assert_trees_all_equal_sizes(self):
+    get_val = lambda s1, s2: jnp.zeros([s1, s2])
+    tree1 = dict(a1=get_val(3, 1), d=dict(a2=get_val(4, 1), a3=get_val(5, 3)))
+    tree2 = dict(a1=get_val(3, 1), d=dict(a2=get_val(4, 1), a3=get_val(5, 3)))
+    tree3 = dict(a1=get_val(3, 1), d=dict(a2=get_val(4, 2), a3=get_val(5, 3)))
+
+    self._assert_tree_structs_validation(asserts.assert_trees_all_equal_sizes)
+    asserts.assert_trees_all_equal_sizes(tree1, tree1)
+    asserts.assert_trees_all_equal_sizes(tree2, tree1)
+
+    with self.assertRaisesRegex(
+        AssertionError,
+        _get_err_regex(
+            r'Trees 0 and 1 differ in leaves \'d/a2\': sizes: 4 != 8'
+        )):
+      asserts.assert_trees_all_equal_sizes(tree1, tree3)
+
+    with self.assertRaisesRegex(
+        AssertionError,
+        _get_err_regex(
+            r'Trees 0 and 3 differ in leaves \'d/a2\': sizes: 4 != 8'
+        )):
+      asserts.assert_trees_all_equal_sizes(tree1, tree2, tree2, tree3, tree1)
+
   def test_assert_trees_all_equal_shapes(self):
     get_val = lambda s: jnp.zeros([s])
     tree1 = dict(a1=get_val(3), d=dict(a2=get_val(4), a3=get_val(5)))
     tree2 = dict(a1=get_val(3), d=dict(a2=get_val(4), a3=get_val(5)))
     tree3 = dict(a1=get_val(3), d=dict(a2=get_val(7), a3=get_val(5)))
 
     self._assert_tree_structs_validation(asserts.assert_trees_all_equal_shapes)
@@ -1255,71 +1486,113 @@
     tree2 = [[get_val(), get_val()], get_val()]
     tree3 = [get_val(), [get_val(), get_val()]]
 
     asserts.assert_trees_all_equal_structs(tree1, tree2, tree2, tree1)
     asserts.assert_trees_all_equal_structs(tree3, tree3)
     self._assert_tree_structs_validation(asserts.assert_trees_all_equal_structs)
 
-  def test_assert_tree_shape_prefix(self):
+  @parameterized.named_parameters(
+      ('scalars', ()),
+      ('vectors', (3,)),
+      ('matrices', (3, 2)),
+  )
+  def test_assert_tree_shape_prefix(self, shape):
     tree = {'x': {'y': np.zeros([3, 2])}, 'z': np.zeros([3, 2, 1])}
-    asserts.assert_tree_shape_prefix(tree, ())
-    asserts.assert_tree_shape_prefix(tree, (3,))
-    asserts.assert_tree_shape_prefix(tree, (3, 2))
+    with self.subTest('tuple'):
+      asserts.assert_tree_shape_prefix(tree, tuple(shape))
+    with self.subTest('list'):
+      asserts.assert_tree_shape_prefix(tree, list(shape))
 
+  def test_leaf_shape_should_fail_wrong_length(self):
+    tree = {'x': {'y': np.zeros([3, 2])}, 'z': np.zeros([3, 2, 1])}
     with self.assertRaisesRegex(
         AssertionError,
         _get_err_regex(r'leaf \'x/y\' has a shape of length 2')):
       asserts.assert_tree_shape_prefix(tree, (3, 2, 1))
+    with self.assertRaisesRegex(
+        AssertionError,
+        _get_err_regex(r'leaf \'x/y\' has a shape of length 2')):
+      asserts.assert_tree_shape_prefix(tree, [3, 2, 1])
 
   def test_assert_tree_shape_prefix_none(self):
     tree = {'x': np.zeros([3]), 'n': None}
     asserts.assert_tree_shape_prefix(tree, (3,), ignore_nones=True)
+    asserts.assert_tree_shape_prefix(tree, [3], ignore_nones=True)
 
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('`None` detected')):
       asserts.assert_tree_shape_prefix(tree, (3,), ignore_nones=False)
 
-  def test_assert_tree_shape_suffix_matching(self):
+    with self.assertRaisesRegex(AssertionError,
+                                _get_err_regex('`None` detected')):
+      asserts.assert_tree_shape_prefix(tree, [3], ignore_nones=False)
+
+  @parameterized.named_parameters(
+      ('scalars', ()),
+      ('vectors', (1,)),
+      ('matrices', (2, 1)),
+  )
+  def test_assert_tree_shape_suffix_matching(self, shape):
     tree = {'x': {'y': np.zeros([4, 2, 1])}, 'z': np.zeros([2, 1])}
-    asserts.assert_tree_shape_suffix(tree, ())
-    asserts.assert_tree_shape_suffix(tree, (1,))
-    asserts.assert_tree_shape_suffix(tree, (2, 1))
+    with self.subTest('tuple'):
+      asserts.assert_tree_shape_suffix(tree, tuple(shape))
+    with self.subTest('list'):
+      asserts.assert_tree_shape_suffix(tree, list(shape))
 
-  def test_assert_tree_shape_suffix_mismatch(self):
+  @parameterized.named_parameters(
+      ('bad_suffix_leaf_1', 'z', (1, 1), (2, 1)),
+      ('bad_suffix_leaf_2', 'x/y', (2, 1), (1, 1)),
+  )
+  def test_assert_tree_shape_suffix_mismatch(self, leaf, shape_true, shape):
     tree = {'x': {'y': np.zeros([4, 2, 1])}, 'z': np.zeros([1, 1])}
 
-    with self.assertRaisesRegex(
-        AssertionError,
-        _get_err_regex(
-            r'Tree leaf \'z\'.*different from expected: \(1, 1\) != \(2, 1\)')):
-      asserts.assert_tree_shape_suffix(tree, (2, 1))
+    error_msg = (
+        r'Tree leaf \'' + str(leaf) + '\'.*different from expected: '
+        + re.escape(str(shape_true)) + ' != ' + re.escape(str(shape))
+    )
+    with self.subTest('tuple'):
+      with self.assertRaisesRegex(
+          AssertionError,
+          _get_err_regex(
+              error_msg)):
+        asserts.assert_tree_shape_suffix(tree, tuple(shape))
 
-    with self.assertRaisesRegex(
-        AssertionError,
-        _get_err_regex(
-            r'Tree leaf \'x/y\'.*different from expected: \(2, 1\) != \(1, 1\)')
-    ):
-      asserts.assert_tree_shape_suffix(tree, (1, 1))
+    with self.subTest('list'):
+      with self.assertRaisesRegex(
+          AssertionError,
+          _get_err_regex(
+              error_msg)):
+        asserts.assert_tree_shape_suffix(tree, list(shape))
 
   def test_assert_tree_shape_suffix_long_suffix(self):
     tree = {'x': {'y': np.zeros([4, 2, 1])}, 'z': np.zeros([4, 2, 1])}
     asserts.assert_tree_shape_suffix(tree, (4, 2, 1))
+    asserts.assert_tree_shape_suffix(tree, [4, 2, 1])
 
     with self.assertRaisesRegex(
         AssertionError, _get_err_regex('which is smaller than the expected')):
       asserts.assert_tree_shape_suffix(tree, (3, 4, 2, 1))
 
+    with self.assertRaisesRegex(
+        AssertionError, _get_err_regex('which is smaller than the expected')):
+      asserts.assert_tree_shape_suffix(tree, [3, 4, 2, 1])
+
   def test_assert_tree_shape_suffix_none(self):
     tree = {'x': np.zeros([3]), 'n': None}
     asserts.assert_tree_shape_suffix(tree, (3,), ignore_nones=True)
+    asserts.assert_tree_shape_suffix(tree, [3], ignore_nones=True)
 
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('`None` detected')):
       asserts.assert_tree_shape_suffix(tree, (3,), ignore_nones=False)
 
+    with self.assertRaisesRegex(AssertionError,
+                                _get_err_regex('`None` detected')):
+      asserts.assert_tree_shape_suffix(tree, [3], ignore_nones=False)
+
   def test_assert_trees_all_equal_dtypes(self):
     t_0 = {'x': np.zeros(3, dtype=np.int16), 'y': np.ones(2, dtype=np.float32)}
     t_1 = {'x': np.zeros(5, dtype=np.uint16), 'y': np.ones(4, dtype=np.float32)}
 
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('Trees 0 and 1 differ')):
       asserts.assert_trees_all_equal_dtypes(t_0, t_1)
```

### Comparing `chex-0.1.7/chex/_src/dataclass.py` & `chex-0.1.8/chex/_src/dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,16 +119,20 @@
       As a side-effect, e.g. `np.testing.assert_array_equal` will only check
       the field names are equal and not the content. Use `chex.assert_tree_*`
       instead.
 
   Returns:
     A JAX-friendly dataclass.
   """
-  dcls = _Dataclass(init, repr, eq, order, unsafe_hash, frozen,
-                    mappable_dataclass)
+  def dcls(cls):
+    # Make sure to create a separate _Dataclass instance for each `cls`.
+    return _Dataclass(
+        init, repr, eq, order, unsafe_hash, frozen, mappable_dataclass
+    )(cls)
+
   if cls is None:
     return dcls
   return dcls(cls)
 
 
 class _Dataclass():
   """JAX-friendly wrapper for `dataclasses.dataclass`."""
@@ -240,14 +244,23 @@
       object.__setattr__(dcls_object, field.name, attribute_dict[field.name])
   # Need to manual call post_init here as we have avoided calling __init__
   if getattr(dcls_object, "__post_init__", None):
     dcls_object.__post_init__()
   return dcls_object
 
 
+def _flatten_with_path(dcls):
+  path = []
+  keys = []
+  for k, v in sorted(dcls.__dict__.items()):
+    path.append((k, v))
+    keys.append(k)
+  return path, keys
+
+
 def register_dataclass_type_with_jax_tree_util(data_class):
   """Register an existing dataclass so JAX knows how to handle it.
 
   This means that functions in jax.tree_util operate over the fields
   of the dataclass. See
   https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees
   for further information.
@@ -256,11 +269,12 @@
     data_class: A class created using dataclasses.dataclass. It must be
       constructable from keyword arguments corresponding to the members exposed
       in instance.__dict__.
   """
   flatten = lambda d: jax.util.unzip2(sorted(d.__dict__.items()))[::-1]
   unflatten = functools.partial(_dataclass_unflatten, data_class)
   try:
-    jax.tree_util.register_pytree_node(
-        nodetype=data_class, flatten_func=flatten, unflatten_func=unflatten)
+    jax.tree_util.register_pytree_with_keys(
+        nodetype=data_class, flatten_with_keys=_flatten_with_path,
+        flatten_func=flatten, unflatten_func=unflatten)
   except ValueError:
     logging.info("%s is already registered as JAX PyTree node.", data_class)
```

### Comparing `chex-0.1.7/chex/_src/dataclass_test.py` & `chex-0.1.8/chex/_src/dataclass_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -337,14 +337,46 @@
   def test_dataclass_tree_map(self, frozen):
     factor = 5.
     obj = dummy_dataclass(frozen=frozen)
     target_obj = dummy_dataclass(factor=factor, frozen=frozen)
     asserts.assert_trees_all_close(
         jax.tree_util.tree_map(lambda t: factor * t, obj), target_obj)
 
+  def test_tree_flatten_with_keys(self):
+    obj = dummy_dataclass()
+    keys_and_leaves, treedef = jax.tree_util.tree_flatten_with_path(obj)
+    self.assertEqual([k for k, _ in keys_and_leaves],
+                     [('a', 'c'), ('a', 'd'), ('b',)])
+    leaves = [l for _, l in keys_and_leaves]
+    new_obj = treedef.unflatten(leaves)
+    self.assertEqual(new_obj, obj)
+
+  def test_tree_map_with_keys(self):
+    obj = dummy_dataclass()
+    def f(path, x):
+      value = obj
+      for key in path:
+        value = getattr(value, key)
+      np.testing.assert_allclose(value, x)
+      return path
+
+    out = jax.tree_util.tree_map_with_path(f, obj)
+    self.assertEqual(out.a.c, ('a', 'c'))
+    self.assertEqual(out.a.d, ('a', 'd'))
+    self.assertEqual(out.b, ('b',))
+
+  def test_tree_map_with_keys_traversal_order(self):
+    obj = ReverseOrderNestedDataclass(d=1, c=2)
+    leaves = []
+    def f(_, x):
+      leaves.append(x)
+
+    jax.tree_util.tree_map_with_path(f, obj)
+    self.assertEqual(leaves, jax.tree_util.tree_leaves(obj))
+
   @parameterized.parameters([True, False])
   def test_dataclass_replace(self, frozen):
     factor = 5.
     obj = dummy_dataclass(frozen=frozen)
     obj = obj.replace(a=obj.a.replace(c=factor * obj.a.c))
     obj = obj.replace(a=obj.a.replace(d=factor * obj.a.d))
     obj = obj.replace(b=factor * obj.b)
@@ -516,14 +548,32 @@
     self.assertCountEqual(
         (dcls.str_val, dcls.inner_dcls, dcls.dct['md1'], dcls.dct['md2']),
         leaves)
 
     asserts.assert_tree_all_equal_structs(
         jax.tree_util.tree_map(lambda x: x, dcls, is_leaf=_is_leaf), dcls)
 
+  def test_decorator_alias(self):
+    # Make sure, that creating a decorator alias works correctly.
+    configclass = chex_dataclass(frozen=True)
+
+    @configclass
+    class Foo:
+      bar: int = 1
+      toto: int = 2
+
+    @configclass
+    class Bar:
+      bar: int = 1
+      toto: int = 2
+
+    # Verify that both Foo and Bar are correctly registered with jax.tree_util.
+    self.assertLen(jax.tree_util.tree_flatten(Foo())[0], 2)
+    self.assertLen(jax.tree_util.tree_flatten(Bar())[0], 2)
+
   @parameterized.named_parameters(
       ('mappable', True),
       ('not_mappable', False),
   )
   def test_generic_dataclass(self, mappable):
     T = TypeVar('T')
```

### Comparing `chex-0.1.7/chex/_src/dimensions.py` & `chex-0.1.8/chex/_src/dimensions.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/dimensions_test.py` & `chex-0.1.8/chex/_src/dimensions_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/fake.py` & `chex-0.1.8/chex/_src/fake.py`

 * *Files 8% similar despite different names*

```diff
@@ -149,26 +149,50 @@
   @functools.wraps(fn)
   def wrapped_fn(*args, **kwargs):
     # Convert kwargs to varargs
     # This is a workaround for vmapped functions not working with kwargs
     call_args = convert_to_varargs(fn_signature, *args, **kwargs)
 
     if static_broadcasted_argnums:
+      # Make sure vmap does not try to map over `static_broadcasted_argnums`.
       if isinstance(in_axes, int):
-        vmap_in_axes = jax.tree_util.tree_map(lambda _: in_axes, call_args)
+        vmap_in_axes = [in_axes] * len(call_args)
       else:
-        vmap_in_axes = in_axes
-      vmap_in_axes = list(vmap_in_axes)
+        vmap_in_axes = list(in_axes)
       for argnum in static_broadcasted_argnums:
-        vmap_in_axes[argnum] = jax.tree_util.tree_map(
-            lambda _: None, call_args[argnum])
+        vmap_in_axes[argnum] = None
+
+      # To protect the arguments from `static_broadcasted_argnums`,
+      # from turning into tracers (because of vmap), we capture the original
+      # `call_args` and replace the passed in tracers with original values.
+      original_call_args = call_args
+
+      # A function passed to vmap, that will simply replace the static args
+      # with their original values.
+      def fn_without_statics(*args):
+        args_with_original_statics = [
+            orig_arg if i in static_broadcasted_argnums else arg
+            for i, (arg, orig_arg) in enumerate(zip(args, original_call_args))
+        ]
+        return fn(*args_with_original_statics)
+
+      # Make sure to avoid turning static args into tracers: Some python objects
+      # might not survive vmap. Just replace with an unused constant.
+      call_args = [
+          1 if i in static_broadcasted_argnums else arg
+          for i, arg in enumerate(call_args)
+      ]
+
     else:
       vmap_in_axes = in_axes
+      fn_without_statics = fn
 
-    vmapped_fn = jax.vmap(fn, in_axes=vmap_in_axes, axis_name=axis_name)
+    vmapped_fn = jax.vmap(
+        fn_without_statics, in_axes=vmap_in_axes, axis_name=axis_name
+    )
     if jit_result:
       vmapped_fn = jax.jit(vmapped_fn)
 
     if fake_parallel_axis:
       call_args = jax.tree_util.tree_map(
           lambda x: jnp.expand_dims(x, axis=0), call_args)
 
@@ -389,15 +413,15 @@
       fn_transformation: identifier of the function transformation e.g.
         'jax.jit', 'jax.pmap', ...
       callback_fn: A callback function which receives the transformed function
         and its arguments on every call.
     """
     self._fn_transformation = fn_transformation
     self._callback_fn = callback_fn
-    self._patch = None
+    self._patch: mock._patch[Callable[[Any], Any]] = None  # pylint: disable=unsubscriptable-object
     self._original_fn_transformation = None
 
   def __enter__(self):
 
     def _new_fn_transformation(fn, *args, **kwargs):
       """Returns a transformed version of the given function."""
       transformed_fn = self._original_fn_transformation(fn, *args, **kwargs)
```

### Comparing `chex-0.1.7/chex/_src/fake_set_n_cpu_devices_test.py` & `chex-0.1.8/chex/_src/fake_set_n_cpu_devices_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/fake_test.py` & `chex-0.1.8/chex/_src/fake_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for `fake.py`."""
 
+import dataclasses
 import functools
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from chex._src import asserts
 from chex._src import fake
 from chex._src import pytypes
@@ -227,37 +228,90 @@
   ])
   def test_with_static_broadcasted_argnums(self, fake_pmap, static_argnums):
     with fake.fake_pmap_and_jit(fake_pmap, enable_jit_patching=False):
       num_devices = len(jax.devices())
 
       # Note: mode='bar' is intended to test that we correctly handle kwargs
       # with defaults for which we don't pass a value at call time.
-      @functools.partial(jax.pmap,
-                         axis_size=num_devices,
-                         static_broadcasted_argnums=static_argnums)
-      @jax.jit
+      @functools.partial(
+          jax.pmap,
+          axis_size=num_devices,
+          static_broadcasted_argnums=static_argnums,
+      )
+      @functools.partial(
+          jax.jit,
+          static_argnums=static_argnums,
+      )
       def foo(x, multiplier, y, mode='bar'):
+        if static_argnums == 1 or 1 in static_argnums:
+          # Verify that the static arguments are not replaced with tracers.
+          self.assertIsInstance(multiplier, int)
+
         if mode == 'bar':
           return (x * multiplier) + y
         else:
           return x
 
       # pmap over all available devices
       inputs = jnp.array([1, 2])
       inputs = jnp.broadcast_to(inputs, (num_devices,) + inputs.shape)
-      func = lambda: foo(inputs, 100, inputs)   # Pass multiplier=100.
+      func = lambda: foo(inputs, 100, inputs)  # Pass multiplier=100.
 
       if static_argnums == 1:  # Should work.
         expected = jnp.broadcast_to(jnp.array([101, 202]), (num_devices, 2))
         result = func()
         asserts.assert_trees_all_close(result, expected)
       else:  # Should error.
         with self.assertRaises(ValueError):
           result = func()
 
+  @parameterized.parameters(1, [1])
+  def test_pmap_with_complex_static_broadcasted_object(self, static_argnums):
+
+    @dataclasses.dataclass
+    class Multiplier:
+      x: int
+      y: int
+
+    def foo(x, multiplier, y):
+      if static_argnums == 1 or 1 in static_argnums:
+        # Verify that the static arguments are not replaced with tracers.
+        self.assertIsInstance(multiplier, Multiplier)
+
+      return x * multiplier.x + y * multiplier.y
+
+    with fake.fake_pmap_and_jit():
+      num_devices = jax.device_count()
+
+      # pmap over all available devices
+      transformed_foo = jax.pmap(
+          foo,
+          axis_size=num_devices,
+          static_broadcasted_argnums=static_argnums,
+      )
+      x, y = jax.random.randint(
+          jax.random.PRNGKey(27), (2, num_devices, 3, 5), 0, 10
+      )
+
+      # Test 1.
+      mult = Multiplier(x=2, y=7)
+      asserts.assert_trees_all_equal(
+          transformed_foo(x, mult, y),
+          foo(x, mult, y),
+          x * mult.x + y * mult.y,
+      )
+
+      # Test 2.
+      mult = Multiplier(x=72, y=21)
+      asserts.assert_trees_all_equal(
+          transformed_foo(x, mult, y),
+          foo(x, mult, y),
+          x * mult.x + y * mult.y,
+      )
+
   @parameterized.named_parameters([
       ('fake_nothing', False, False),
       ('fake_pmap', True, False),
       ('fake_jit', False, True),
       ('fake_both', True, True),
   ])
   def test_with_partial(self, fake_pmap, fake_jit):
```

### Comparing `chex-0.1.7/chex/_src/pytypes.py` & `chex-0.1.8/chex/_src/pytypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,11 +47,11 @@
     ArrayNumpy, Iterable['ArrayNumpyTree'], Mapping[Any, 'ArrayNumpyTree']
 ]
 
 # Other types.
 Scalar = Union[float, int]
 Numeric = Union[Array, Scalar]
 Shape = jax.core.Shape
-PRNGKey = jax.random.KeyArray
+PRNGKey = Union[jax.random.KeyArray, jax.Array]
 PyTreeDef = jax.tree_util.PyTreeDef
 Device = jax.Device
 ArrayDType = type(jnp.float32)
```

### Comparing `chex-0.1.7/chex/_src/restrict_backends.py` & `chex-0.1.8/chex/_src/restrict_backends.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/restrict_backends_test.py` & `chex-0.1.8/chex/_src/restrict_backends_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/variants.py` & `chex-0.1.8/chex/_src/variants.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/_src/variants_test.py` & `chex-0.1.8/chex/_src/variants_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex/chex_test.py` & `chex-0.1.8/chex/chex_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/chex.egg-info/PKG-INFO` & `chex-0.1.8/chex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chex
-Version: 0.1.7
+Version: 0.1.8
 Summary: Chex: Testing made fun, in JAX!
 Home-page: https://github.com/deepmind/chex
 Author: DeepMind
 Author-email: chex-dev@google.com
 License: Apache 2.0
 Keywords: jax testing debugging python machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chex
 
 ![CI status](https://github.com/deepmind/chex/workflows/ci/badge.svg)
 ![docs](https://readthedocs.org/projects/chex/badge/?version=latest)
```

### Comparing `chex-0.1.7/chex.egg-info/SOURCES.txt` & `chex-0.1.8/chex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chex-0.1.7/setup.py` & `chex-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     packages=find_packages(exclude=['*_test.py']),
     install_requires=_parse_requirements(
         os.path.join(_CURRENT_DIR, 'requirements', 'requirements.txt')),
     tests_require=_parse_requirements(
         os.path.join(_CURRENT_DIR, 'requirements', 'requirements-test.txt')),
     zip_safe=False,  # Required for full installation.
     include_package_data=True,
-    python_requires='>=3.8',
+    python_requires='>=3.9',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
```

