# Comparing `tmp/iblutil-1.6.0.tar.gz` & `tmp/iblutil-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iblutil-1.6.0.tar", last modified: Tue Mar  7 11:54:20 2023, max compression
+gzip compressed data, was "iblutil-1.7.0.tar", last modified: Tue Jun 27 18:24:43 2023, max compression
```

## Comparing `iblutil-1.6.0.tar` & `iblutil-1.7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-03-07 11:54:20.970095 iblutil-1.6.0/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1087 2021-06-22 14:00:49.000000 iblutil-1.6.0/LICENSE
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      619 2023-03-07 11:54:20.970095 iblutil-1.6.0/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      355 2022-10-17 17:40:09.000000 iblutil-1.6.0/README.md
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-03-07 11:54:20.970095 iblutil-1.6.0/iblutil/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       22 2023-03-07 11:53:06.000000 iblutil-1.6.0/iblutil/__init__.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-03-07 11:54:20.970095 iblutil-1.6.0/iblutil/io/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2021-06-22 14:00:49.000000 iblutil-1.6.0/iblutil/io/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1234 2021-06-22 14:00:49.000000 iblutil-1.6.0/iblutil/io/hashfile.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      397 2021-06-22 14:00:49.000000 iblutil-1.6.0/iblutil/io/jsonable.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-03-07 11:54:20.970095 iblutil-1.6.0/iblutil/io/net/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       81 2023-02-08 12:06:46.000000 iblutil-1.6.0/iblutil/io/net/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    31021 2023-02-08 12:06:46.000000 iblutil-1.6.0/iblutil/io/net/app.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    16650 2023-03-07 11:53:06.000000 iblutil-1.6.0/iblutil/io/net/base.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4268 2023-02-08 12:06:46.000000 iblutil-1.6.0/iblutil/io/params.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2319 2021-06-22 14:00:49.000000 iblutil-1.6.0/iblutil/io/parquet.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    11320 2023-03-07 11:53:06.000000 iblutil-1.6.0/iblutil/numerical.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     7269 2023-02-08 12:06:46.000000 iblutil-1.6.0/iblutil/spacer.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     7109 2023-02-08 12:06:46.000000 iblutil-1.6.0/iblutil/util.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-03-07 11:54:20.970095 iblutil-1.6.0/iblutil.egg-info/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      619 2023-03-07 11:54:20.000000 iblutil-1.6.0/iblutil.egg-info/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      439 2023-03-07 11:54:20.000000 iblutil-1.6.0/iblutil.egg-info/SOURCES.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2023-03-07 11:54:20.000000 iblutil-1.6.0/iblutil.egg-info/dependency_links.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       70 2023-03-07 11:54:20.000000 iblutil-1.6.0/iblutil.egg-info/requires.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        8 2023-03-07 11:54:20.000000 iblutil-1.6.0/iblutil.egg-info/top_level.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2023-03-07 11:54:20.970095 iblutil-1.6.0/setup.cfg
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1709 2022-10-17 17:40:09.000000 iblutil-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:24:43.811814 iblutil-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-27 18:24:37.000000 iblutil-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-27 18:24:43.811814 iblutil-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 18:24:37.000000 iblutil-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:24:43.807814 iblutil-1.7.0/iblutil/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:24:43.811814 iblutil-1.7.0/iblutil/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/io/hashfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/io/jsonable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:24:43.811814 iblutil-1.7.0/iblutil/io/net/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/io/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31021 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/io/net/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/io/net/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/io/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/io/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/spacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-27 18:24:37.000000 iblutil-1.7.0/iblutil/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:24:43.807814 iblutil-1.7.0/iblutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-27 18:24:43.000000 iblutil-1.7.0/iblutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-27 18:24:43.000000 iblutil-1.7.0/iblutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:24:43.000000 iblutil-1.7.0/iblutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-27 18:24:43.000000 iblutil-1.7.0/iblutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 18:24:43.000000 iblutil-1.7.0/iblutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:24:43.811814 iblutil-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-27 18:24:37.000000 iblutil-1.7.0/setup.py
```

### Comparing `iblutil-1.6.0/LICENSE` & `iblutil-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iblutil-1.6.0/PKG-INFO` & `iblutil-1.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: iblutil
-Version: 1.6.0
+Version: 1.7.0
 Summary: IBL utilities
 Home-page: https://github.com/int-brain-lab/iblutil/
 Author: IBL Staff
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iblutil
 ![CI workflow](https://github.com/int-brain-lab/iblrplate/actions/workflows/main.yaml/badge.svg?branch=main)
 [![Coverage Status](https://coveralls.io/repos/github/int-brain-lab/iblrplate/badge.svg?branch=main)](https://coveralls.io/github/int-brain-lab/iblrplate?branch=main)
 
 Small utilities with minimal dependencies, tests run on Python v3.8
-
-
```

### Comparing `iblutil-1.6.0/iblutil/io/hashfile.py` & `iblutil-1.7.0/iblutil/io/hashfile.py`

 * *Files identical despite different names*

### Comparing `iblutil-1.6.0/iblutil/io/net/app.py` & `iblutil-1.7.0/iblutil/io/net/app.py`

 * *Files identical despite different names*

### Comparing `iblutil-1.6.0/iblutil/io/net/base.py` & `iblutil-1.7.0/iblutil/io/net/base.py`

 * *Files identical despite different names*

### Comparing `iblutil-1.6.0/iblutil/io/params.py` & `iblutil-1.7.0/iblutil/io/params.py`

 * *Files identical despite different names*

### Comparing `iblutil-1.6.0/iblutil/io/parquet.py` & `iblutil-1.7.0/iblutil/io/parquet.py`

 * *Files identical despite different names*

### Comparing `iblutil-1.6.0/iblutil/numerical.py` & `iblutil-1.7.0/iblutil/numerical.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TypeVar, Sequence, Union, Optional, Type
 
 import numpy as np
 from numba import jit
 
-D = TypeVar('D', bound=np.generic)
+D = TypeVar("D", bound=np.generic)
 Array = Union[np.ndarray, Sequence]
 
 
 def between_sorted(sorted_v, bounds=None):
     """
     Given a vector of sorted values, returns a boolean vector indices True when the value
     is between bounds. If multiple bounds are given, returns the equivalent OR of individual
@@ -22,15 +22,15 @@
     bounds = np.array(bounds)
     starts, stops = (np.take(bounds, 0, axis=-1), np.take(bounds, 1, axis=-1))
     sbounds = np.logical_and(starts <= sorted_v[-1], stops >= sorted_v[0])
     starts = starts[sbounds]
     stops = stops[sbounds]
     sel = sorted_v * 0
     sel[np.searchsorted(sorted_v, starts)] = 1
-    istops = np.searchsorted(sorted_v, stops, side='right')
+    istops = np.searchsorted(sorted_v, stops, side="right")
     sel[istops[istops < sorted_v.size]] += -1
     return np.cumsum(sel).astype(bool)
 
 
 def ismember(a, b):
     """
     equivalent of np.isin but returns indices as in the matlab ismember function
@@ -89,24 +89,86 @@
     :param a1:
     :param assume_unique: If True, the input arrays are both assumed to be unique,
     which can speed up the calculation.
     :return: intersection
     :return: index of a0 such as intersection = a0[ia, :]
     :return: index of b0 such as intersection = b0[ib, :]
     """
-    _, i0, i1 = np.intersect1d(a0[:, 0], a1[:, 0],
-                               return_indices=True, assume_unique=assume_unique)
+    _, i0, i1 = np.intersect1d(
+        a0[:, 0], a1[:, 0], return_indices=True, assume_unique=assume_unique
+    )
     for n in np.arange(1, a0.shape[1]):
-        _, ii0, ii1 = np.intersect1d(a0[i0, n], a1[i1, n],
-                                     return_indices=True, assume_unique=assume_unique)
+        _, ii0, ii1 = np.intersect1d(
+            a0[i0, n], a1[i1, n], return_indices=True, assume_unique=assume_unique
+        )
         i0 = i0[ii0]
         i1 = i1[ii1]
     return a0[i0, :], i0, i1
 
 
+def bincount2D(x, y, xbin=0, ybin=0, xlim=None, ylim=None, weights=None):
+    """
+    Computes a 2D histogram by aggregating values in a 2D array.
+
+    :param x: values to bin along the 2nd dimension (c-contiguous)
+    :param y: values to bin along the 1st dimension
+    :param xbin:
+        scalar: bin size along 2nd dimension
+        0: aggregate according to unique values
+        array: aggregate according to exact values (count reduce operation)
+    :param ybin:
+        scalar: bin size along 1st dimension
+        0: aggregate according to unique values
+        array: aggregate according to exact values (count reduce operation)
+    :param xlim: (optional) 2 values (array or list) that restrict range along 2nd dimension
+    :param ylim: (optional) 2 values (array or list) that restrict range along 1st dimension
+    :param weights: (optional) defaults to None, weights to apply to each value for aggregation
+    :return: 3 numpy arrays MAP [ny,nx] image, xscale [nx], yscale [ny]
+    """
+    # if no bounds provided, use min/max of vectors
+    if xlim is None:
+        xlim = [np.min(x), np.max(x)]
+    if ylim is None:
+        ylim = [np.min(y), np.max(y)]
+
+    def _get_scale_and_indices(v, bin, lim):
+        # if bin is a nonzero scalar, this is a bin size: create scale and indices
+        if np.isscalar(bin) and bin != 0:
+            scale = np.arange(lim[0], lim[1] + bin / 2, bin)
+            ind = (np.floor((v - lim[0]) / bin)).astype(np.int64)
+        # if bin == 0, aggregate over unique values
+        else:
+            scale, ind = np.unique(v, return_inverse=True)
+        return scale, ind
+
+    xscale, xind = _get_scale_and_indices(x, xbin, xlim)
+    yscale, yind = _get_scale_and_indices(y, ybin, ylim)
+    # aggregate by using bincount on absolute indices for a 2d array
+    nx, ny = [xscale.size, yscale.size]
+    ind2d = np.ravel_multi_index(np.c_[yind, xind].transpose(), dims=(ny, nx))
+    r = np.bincount(ind2d, minlength=nx * ny, weights=weights).reshape(ny, nx)
+
+    # if a set of specific values is requested output an array matching the scale dimensions
+    if not np.isscalar(xbin) and xbin.size > 1:
+        _, iout, ir = np.intersect1d(xbin, xscale, return_indices=True)
+        _r = r.copy()
+        r = np.zeros((ny, xbin.size))
+        r[:, iout] = _r[:, ir]
+        xscale = xbin
+
+    if not np.isscalar(ybin) and ybin.size > 1:
+        _, iout, ir = np.intersect1d(ybin, yscale, return_indices=True)
+        _r = r.copy()
+        r = np.zeros((ybin.size, r.shape[1]))
+        r[iout, :] = _r[ir, :]
+        yscale = ybin
+
+    return r, xscale, yscale
+
+
 @jit(nopython=True)
 def find_first_2d(mat, val):
     """
     Returns first index where
     The purpose of this function is performance: uses low level numba and avoids looping
     through the full array
     :param mat: np.array
@@ -116,33 +178,43 @@
     for i in np.arange(mat.shape[0]):
         if np.all(mat[i] == val):
             return i
 
 
 def rcoeff(x, y):
     """
-    Computes pairwise Person correlation coefficients for matrices.
+    Computes pairwise Pearson correlation coefficients for matrices.
+
     That is for 2 matrices the same size, computes the row to row coefficients and outputs
-    a vector corresponding to the number of rows of the first matrix
-    If the second array is a vector then computes the correlation coefficient for all rows
+    a vector corresponding to the number of rows of the first matrix.
+    If the second array is a vector then computes the correlation coefficient for all rows.
     :param x: np array [nc, ns]
     :param y: np array [nc, ns] or [ns]
     :return: r [nc]
     """
+
     def normalize(z):
         mean = np.mean(z, axis=-1)
         return z - mean if mean.size == 1 else z - mean[:, np.newaxis]
+
     xnorm = normalize(x)
     ynorm = normalize(y)
-    rcor = np.sum(xnorm * ynorm, axis=-1) / np.sqrt(np.sum(np.square(xnorm), axis=-1) * np.sum(np.square(ynorm), axis=-1))
+    rcor = np.sum(xnorm * ynorm, axis=-1) / np.sqrt(
+        np.sum(np.square(xnorm), axis=-1) * np.sum(np.square(ynorm), axis=-1)
+    )
     return rcor
 
 
-def within_ranges(x: np.ndarray, ranges: Array, labels: Optional[Array] = None,
-                  mode: str = 'vector', dtype: Type[D] = 'int8') -> np.ndarray:
+def within_ranges(
+    x: np.ndarray,
+    ranges: Array,
+    labels: Optional[Array] = None,
+    mode: str = "vector",
+    dtype: Type[D] = "int8",
+) -> np.ndarray:
     """
     Detects which points of the input vector lie within one of the ranges specified in the ranges.
     Returns an array the size of x with a 1 if the corresponding point is within a range.
 
     The function uses a stable sort algorithm (timsort) to find the edges within the input array.
     Edge behaviour is inclusive.
 
@@ -216,40 +288,42 @@
 
     # Get size info
     n_points = x.size
     n_ranges = ranges.shape[0]
 
     if labels is None:
         # In 'matrix' mode default row index is 0
-        labels = np.zeros((n_ranges,), dtype='uint32')
-        if mode == 'vector':  # Otherwise default numerical label is 1
+        labels = np.zeros((n_ranges,), dtype="uint32")
+        if mode == "vector":  # Otherwise default numerical label is 1
             labels += 1
-    assert len(labels) >= n_ranges, 'range labels do not match number of ranges'
+    assert len(labels) >= n_ranges, "range labels do not match number of ranges"
     n_labels = np.unique(labels).size
 
     # If no ranges given, short circuit function and return zeros
     if n_ranges == 0:
         return np.zeros_like(x, dtype=dtype)
 
     # Check end comes after start in each case
-    assert np.all(np.diff(ranges, axis=1) > 0), 'ranges ends must all be greater than starts'
+    assert np.all(
+        np.diff(ranges, axis=1) > 0
+    ), "ranges ends must all be greater than starts"
 
     # Make array containing points, starts and finishes
 
     # This order means it will be inclusive
     to_sort = np.concatenate((ranges[:, 0], x, ranges[:, 1]))
     # worst case O(n*log(n)) but will be better than this as most of the array is ordered;
     # memory overhead ~n/2
-    idx = np.argsort(to_sort, kind='stable')
+    idx = np.argsort(to_sort, kind="stable")
 
     # Make delta array containing 1 for every start and -1 for every stop
     # with one row for each range label
-    if mode == 'matrix':
+    if mode == "matrix":
         delta_shape = (n_labels, n_points + 2 * n_ranges)
-        delta = np.zeros(delta_shape, dtype='int8')
+        delta = np.zeros(delta_shape, dtype="int8")
 
         delta[labels, np.arange(n_ranges)] = 1
         delta[labels, n_points + n_ranges + np.arange(n_ranges)] = -1
 
         # Arrange in order
         delta_sorted = delta[:, idx]
 
@@ -257,17 +331,17 @@
         summed = np.cumsum(delta_sorted, axis=1)
 
         # Reorder back to original order
         reordered = np.zeros(delta_shape, dtype=dtype)
         reordered[:, idx] = summed.reshape(delta_shape[0], -1)
         return reordered[:, np.arange(n_ranges, n_points + n_ranges)]
 
-    elif mode == 'vector':
+    elif mode == "vector":
         delta_shape = (n_points + 2 * n_ranges,)
-        r_delta = np.zeros(delta_shape, dtype='int32')
+        r_delta = np.zeros(delta_shape, dtype="int32")
         r_delta[np.arange(n_ranges)] = labels
         r_delta[n_points + n_ranges + np.arange(n_ranges)] = -labels
 
         # Arrange in order
         r_delta_sorted = r_delta[idx]
 
         # Take cumulative sum
```

### Comparing `iblutil-1.6.0/iblutil/spacer.py` & `iblutil-1.7.0/iblutil/spacer.py`

 * *Files identical despite different names*

### Comparing `iblutil-1.6.0/iblutil/util.py` & `iblutil-1.7.0/iblutil/util.py`

 * *Files identical despite different names*

### Comparing `iblutil-1.6.0/iblutil.egg-info/PKG-INFO` & `iblutil-1.7.0/iblutil.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: iblutil
-Version: 1.6.0
+Version: 1.7.0
 Summary: IBL utilities
 Home-page: https://github.com/int-brain-lab/iblutil/
 Author: IBL Staff
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iblutil
 ![CI workflow](https://github.com/int-brain-lab/iblrplate/actions/workflows/main.yaml/badge.svg?branch=main)
 [![Coverage Status](https://coveralls.io/repos/github/int-brain-lab/iblrplate/badge.svg?branch=main)](https://coveralls.io/github/int-brain-lab/iblrplate?branch=main)
 
 Small utilities with minimal dependencies, tests run on Python v3.8
-
-
```

### Comparing `iblutil-1.6.0/setup.py` & `iblutil-1.7.0/setup.py`

 * *Files identical despite different names*

