# Comparing `tmp/odc-geo-0.4.0rc1.tar.gz` & `tmp/odc-geo-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odc-geo-0.4.0rc1.tar", last modified: Sat May 13 02:27:02 2023, max compression
+gzip compressed data, was "odc-geo-0.4.1.tar", last modified: Tue Jun 27 03:12:09 2023, max compression
```

## Comparing `odc-geo-0.4.0rc1.tar` & `odc-geo-0.4.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:27:02.470234 odc-geo-0.4.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-13 02:27:02.470234 odc-geo-0.4.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:27:02.462233 odc-geo-0.4.0rc1/odc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:27:02.466234 odc-geo-0.4.0rc1/odc/geo/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_rgba.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27368 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/_xr_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/crs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:27:02.466234 odc-geo-0.4.0rc1/odc/geo/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/data/gbox.css
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/data/ocean.geojson.xz
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    42911 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/geobox.py
--rw-r--r--   0 runner    (1001) docker     (123)    42282 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/gridspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    18767 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/overlap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/odc/geo/xr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:27:02.466234 odc-geo-0.4.0rc1/odc_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-13 02:27:02.000000 odc-geo-0.4.0rc1/odc_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-13 02:27:02.000000 odc-geo-0.4.0rc1/odc_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 02:27:02.000000 odc-geo-0.4.0rc1/odc_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 02:27:02.000000 odc-geo-0.4.0rc1/odc_geo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-13 02:27:02.000000 odc-geo-0.4.0rc1/odc_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-13 02:27:02.000000 odc-geo-0.4.0rc1/odc_geo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-13 02:27:02.470234 odc-geo-0.4.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:27:02.470234 odc-geo-0.4.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_dask_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_gbox_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_geobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_geoboxtiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    31468 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_gridspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_overlap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_rgba.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_rioxarray_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-05-13 02:26:44.000000 odc-geo-0.4.0rc1/tests/test_xr_interop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:12:09.907142 odc-geo-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 03:11:55.000000 odc-geo-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 03:11:55.000000 odc-geo-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-27 03:12:09.907142 odc-geo-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-27 03:11:55.000000 odc-geo-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:12:09.895141 odc-geo-0.4.1/odc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:12:09.903142 odc-geo-0.4.1/odc/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27370 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/_xr_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/crs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:12:09.903142 odc-geo-0.4.1/odc/geo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/data/gbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/data/ocean.geojson.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42921 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/geobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43118 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18935 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-27 03:11:55.000000 odc-geo-0.4.1/odc/geo/xr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:12:09.903142 odc-geo-0.4.1/odc_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-27 03:12:09.000000 odc-geo-0.4.1/odc_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-27 03:12:09.000000 odc-geo-0.4.1/odc_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:12:09.000000 odc-geo-0.4.1/odc_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:12:09.000000 odc-geo-0.4.1/odc_geo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-27 03:12:09.000000 odc-geo-0.4.1/odc_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 03:12:09.000000 odc-geo-0.4.1/odc_geo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 03:11:55.000000 odc-geo-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-27 03:12:09.907142 odc-geo-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 03:11:55.000000 odc-geo-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:12:09.907142 odc-geo-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_dask_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_gbox_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_geobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_geoboxtiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31910 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_rioxarray_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-06-27 03:11:55.000000 odc-geo-0.4.1/tests/test_xr_interop.py
```

### Comparing `odc-geo-0.4.0rc1/LICENSE` & `odc-geo-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/PKG-INFO` & `odc-geo-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.4.0rc1
+Version: 0.4.1
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-geo-0.4.0rc1/README.rst` & `odc-geo-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/__init__.py` & `odc-geo-0.4.1/odc/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/_blocks.py` & `odc-geo-0.4.1/odc/geo/_blocks.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/_cog.py` & `odc-geo-0.4.1/odc/geo/_cog.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/_compress.py` & `odc-geo-0.4.1/odc/geo/_compress.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/_dask.py` & `odc-geo-0.4.1/odc/geo/_dask.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/_interop.py` & `odc-geo-0.4.1/odc/geo/_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/_map.py` & `odc-geo-0.4.1/odc/geo/_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 
 # pylint: disable=import-outside-toplevel, redefined-builtin, too-many-locals
 def _add_to_folium(url, bounds, map, name=None, **kw):
     assert have.folium
 
     from folium.raster_layers import ImageOverlay
 
-    img_overlay = ImageOverlay(url, bounds, **kw)
-    img_overlay.add_to(map, name=name)
+    img_overlay = ImageOverlay(url, bounds, name=name, **kw)
+    img_overlay.add_to(map)
     return img_overlay
 
 
 def _add_to_ipyleaflet(url, bounds, map, name=None, **kw):
     assert have.ipyleaflet
 
     from ipyleaflet import ImageOverlay, Map
 
     assert isinstance(map, Map)
 
     if name is not None:
         kw.update(name=name)
 
     img_overlay = ImageOverlay(url=url, bounds=bounds, **kw)
-    map.add_layer(img_overlay)
+    map.add(img_overlay)
 
     return img_overlay
 
 
 def _get_add_to_method(map):
     if map is None:
         return None
@@ -74,15 +74,17 @@
 
     If map is not supplied, image data url and bounds are returned instead.
 
     :param xx: array to display
     :param map:
        Map object, :py:mod:`folium` and :py:mod:`ipyleaflet` are understood, can be ``None``.
 
-    :param name: Image layer name
+    :param name:
+       The name of the layer as it will appear in :py:mod:`folium` and :py:mod:`ipyleaflet`
+       Layer Controls. The default ``None`` will use the input array name (e.g. ``xx.name``) if it exists.
     :param fmt: compress image format, defaults to "png", can be "webp", "jpeg" as well.
     :param max_size:
        If longest dimension is bigger than this, shrink it down before compression, defaults to 4096
     :param transparent_pixel: Replace transparent pixels with this value, needed for "jpeg".
 
     :param cmap: If supplied array is not RGB use this colormap to turn it into one
     :param clip: When converting to RGB clip input values to fit ``cmap``.
@@ -101,14 +103,18 @@
 
     assert isinstance(xx, xr.DataArray)
     assert isinstance(xx.odc, ODCExtensionDa)
 
     _add_to = _get_add_to_method(map)  # raises on error
     _crs = map_crs(map)
 
+    # If array xx has a name (xx.name), use it by default
+    if (name is None) and (xx.name is not None):
+        name = xx.name if isinstance(xx.name, str) else str(xx.name)
+
     gbox0 = xx.odc.geobox
     assert gbox0 is not None
     native_crs = gbox0.crs
     assert native_crs is not None
     gbox = gbox0
 
     if isinstance(gbox, GCPGeoBox):
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/_rgba.py` & `odc-geo-0.4.1/odc/geo/_rgba.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,19 +160,19 @@
         x = x.astype("uint8")
     if clip:
         x = np.clip(x, 0, cmap.shape[0] - 1)
     return cmap[x]
 
 
 def _matplotlib_colorize(x, cmap, vmin=None, vmax=None, nodata=None, robust=False):
-    from matplotlib import cm
+    from matplotlib import colormaps
     from matplotlib.colors import Normalize
 
     if cmap is None or isinstance(cmap, str):
-        cmap = cm.get_cmap(cmap)
+        cmap = colormaps.get_cmap(cmap)
 
     if nodata is not None:
         x = np.where(x == nodata, np.float32("nan"), x)
 
     if robust:
         if x.dtype.kind != "f":
             x = x.astype("float32")
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/_xr_interop.py` & `odc-geo-0.4.1/odc/geo/_xr_interop.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,16 +251,16 @@
     Dictionary of Coordinates in xarray format.
 
     :param crs_coord_name:
        Use custom name for CRS coordinate, default is "spatial_ref". Set to ``None`` to not generate
        CRS coordinate at all.
 
     :returns:
-      Dictionary ``name:str -> xr.DataArray``. Where names are either ``y,x`` for projected or
-      ``latitude, longitude`` for geographic.
+       Dictionary ``name:str -> xr.DataArray``. Where names are either ``y,x`` for projected or
+       ``latitude, longitude`` for geographic.
 
     """
     attrs = {}
     crs = gbox.crs
     if crs is not None:
         attrs["crs"] = str(crs)
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/converters.py` & `odc-geo-0.4.1/odc/geo/converters.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/crs.py` & `odc-geo-0.4.1/odc/geo/crs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/data/__init__.py` & `odc-geo-0.4.1/odc/geo/data/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import lzma
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Optional, Tuple
+from warnings import catch_warnings, filterwarnings
 
 from ..crs import MaybeCRS, norm_crs
 from ..geom import Geometry, box, multigeom
 
 
 def data_path(fname: Optional[str] = None) -> Path:
     """Location of data folder or file within."""
@@ -25,15 +26,17 @@
 def ocean_geom(
     crs: MaybeCRS = None, bbox: Optional[Tuple[float, float, float, float]] = None
 ) -> Geometry:
     """Return world oceans geometry."""
     gjson = ocean_geojson()
     gg = multigeom([Geometry(f["geometry"], "epsg:4326") for f in gjson["features"]])
     if bbox is not None:
-        gg = gg & box(*bbox, "epsg:4326")
+        with catch_warnings():
+            filterwarnings("ignore")
+            gg = gg & box(*bbox, "epsg:4326")
     crs = norm_crs(crs)
     if crs is not None:
         gg = gg.to_crs(crs)
 
     return gg
 
 
@@ -48,13 +51,15 @@
     Extract geometry for a country from geopandas sample data.
     """
     # pylint: disable=import-outside-toplevel
     import geopandas as gpd
 
     from ..converters import from_geopandas
 
-    df = gpd.read_file(gpd.datasets.get_path("naturalearth_lowres"))
+    with catch_warnings():
+        filterwarnings("ignore", category=FutureWarning)
+        df = gpd.read_file(gpd.datasets.get_path("naturalearth_lowres"))
     (gg,) = from_geopandas(df[df.iso_a3 == iso3])
     crs = norm_crs(crs)
     if crs is not None:
         gg = gg.to_crs(crs)
     return gg
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/data/gbox.css` & `odc-geo-0.4.1/odc/geo/data/gbox.css`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/data/ocean.geojson.xz` & `odc-geo-0.4.1/odc/geo/data/ocean.geojson.xz`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/gcp.py` & `odc-geo-0.4.1/odc/geo/gcp.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/geobox.py` & `odc-geo-0.4.1/odc/geo/geobox.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 
 import numpy
 from affine import Affine
 
 from . import geom
 from .crs import CRS, MaybeCRS, SomeCRS, norm_crs
-from .geom import BoundingBox, Geometry, bbox_intersection, bbox_union, intersects
+from .geom import BoundingBox, Geometry, bbox_intersection, bbox_union
 from .math import (
     clamp,
     is_affine_st,
     is_almost_int,
     maybe_zero,
     resolution_from_affine,
     snap_grid,
@@ -222,15 +222,15 @@
         :param crs: CRS of the destination
         :param buffer: amount to buffer in source pixels before transforming
         :param npoints: number of points per-side to use, higher number
                         is slower but more accurate
         """
         assert self.crs is not None
         ext = self.extent
-        if buffer > 0:
+        if buffer != 0:
             buffer = buffer * max(*self.resolution.xy)
             ext = ext.buffer(buffer)
 
         return ext.to_crs(crs, resolution=self._reproject_resolution(npoints)).dropna()
 
     @property
     def geographic_extent(self) -> Geometry:
@@ -1304,20 +1304,20 @@
         return range(y1, y2 + 1), range(x1, x2 + 1)
 
     def tiles(self, polygon: Geometry) -> Iterable[Tuple[int, int]]:
         """Return tile indexes overlapping with a given geometry."""
         target_crs = self._gbox.crs
         poly = polygon
         if target_crs is not None and poly.crs != target_crs:
-            poly = poly.to_crs(target_crs)
+            poly = poly.to_crs(target_crs, check_and_fix=True)
 
         yy, xx = self.range_from_bbox(poly.boundingbox)
         for idx in itertools.product(yy, xx):
             gbox = self[idx]
-            if intersects(gbox.extent, poly):
+            if not poly.disjoint(gbox.extent):
                 yield idx
 
     def grid_intersect(
         self, src: "GeoboxTiles"
     ) -> Dict[Tuple[int, int], List[Tuple[int, int]]]:
         """
         Figure out tile to tile overlap graph between two grids.
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/geom.py` & `odc-geo-0.4.1/odc/geo/geom.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,14 +469,16 @@
     def clone(self) -> "Geometry":
         return Geometry(self)
 
     # fmt: off
     @wrap_shapely
     def contains(self, other: "Geometry") -> bool: return self.contains(other)
     @wrap_shapely
+    def covers(self, other: "Geometry") -> bool: return self.covers(other)
+    @wrap_shapely
     def crosses(self, other: "Geometry") -> bool: return self.crosses(other)
     @wrap_shapely
     def disjoint(self, other: "Geometry") -> bool: return self.disjoint(other)
     @wrap_shapely
     def intersects(self, other: "Geometry") -> bool: return self.intersects(other)
     @wrap_shapely
     def touches(self, other: "Geometry") -> bool: return self.touches(other)
@@ -632,14 +634,16 @@
         return Geometry(ops.transform(self.crs.transformer_to_crs(crs), self.geom), crs)
 
     def to_crs(
         self,
         crs: SomeCRS,
         resolution: Union[float, Literal["auto"], None] = None,
         wrapdateline: bool = False,
+        *,
+        check_and_fix: bool = False,
     ) -> "Geometry":
         """
         Convert geometry to a different Coordinate Reference System.
 
         :param crs:
           CRS to convert to
 
@@ -657,14 +661,18 @@
 
           If not supplied project the geometry as is without adding any extra points.
 
         :param wrapdateline:
            Attempt to gracefully handle geometry that intersects the dateline when converting to
            geographic projections. Currently only works in few specific cases (source CRS is smooth
            over the dateline).
+
+        :param check_and_fix:
+           When ``True`` remove vertices that didn't project cleanly and apply ``.buffer(0)`` is geometry
+           is not valid after projection.
         """
         crs = norm_crs_or_error(crs, self)
         if self.crs == crs:
             return self
 
         if self.crs is None:
             raise ValueError("Cannot project geometries without CRS")
@@ -673,23 +681,31 @@
             resolution = _auto_resolution(self)
 
         if resolution is not None and math.isfinite(resolution):
             geom = self.segmented(resolution)
         else:
             geom = self
 
+        def maybe_fix(g: Geometry) -> Geometry:
+            if not check_and_fix or g.is_valid:
+                return g
+            g = g.dropna()
+            if g.geom_type in ["Polygon", "MultiPolygon"] and not g.is_valid:
+                g = g.buffer(0)
+            return g
+
         eps = 1e-4
         if wrapdateline and crs.geographic:
             # TODO: derive precision from resolution by converting to degrees
             precision = 0.1
             chopped = chop_along_antimeridian(geom, precision)
-            chopped_lonlat = chopped._to_crs(crs)
+            chopped_lonlat = maybe_fix(chopped._to_crs(crs))
             return clip_lon180(chopped_lonlat, eps)
 
-        return geom._to_crs(crs)
+        return maybe_fix(geom._to_crs(crs))
 
     def assign_crs(self, crs: MaybeCRS) -> "Geometry":
         """
         Same geometry but with crs changed.
         """
         return Geometry(self.geom, crs=crs)
 
@@ -871,14 +887,16 @@
             ]
             # prune inner polygons that don't have enough points
             inners = [ring for ring in inners if len(ring) >= 3]
             return polygon(pts, self.crs, *inners)
 
         if self.geom_type in ("LinearRing", "LineString"):
             pts = [(x, y) for x, y in self.points if pred(x, y)]
+            if len(pts) == 1:
+                pts = []  # need at least 2 points for this type
             _geom = type(self.geom)(pts)
             return Geometry(_geom, self.crs)
 
         if self.geom_type == "Point":
             x, y = self.coords[0]
             if pred(x, y):
                 return self
@@ -942,14 +960,16 @@
     tr = CRS("EPSG:4326").transformer_to_crs(crs)
     xx_, yy_ = tr(xx, yy)
     pts = [
         (float(x), float(y))
         for x, y in zip(xx_, yy_)
         if math.isfinite(x) and math.isfinite(y)
     ]
+    if len(pts) < 2:
+        return line([], crs)
     return line(pts, crs)
 
 
 def clip_lon180(geom: Geometry, tol=1e-6) -> Geometry:
     """
     Tweak Geometry in the vicinity of longitude discontinuity.
 
@@ -1130,14 +1150,15 @@
 
 
 def _multigeom(geoms: List[base.BaseGeometry]) -> base.BaseGeometry:
     src_type = {g.geom_type for g in geoms}
     if len(src_type) > 1:
         return geometry.GeometryCollection(geoms)
 
+    geoms = [g for g in geoms if not g.is_empty]
     src_type = src_type.pop()
     if src_type == "Polygon":
         return geometry.MultiPolygon(geoms)
     if src_type == "Point":
         return geometry.MultiPoint(geoms)
     if src_type == "LineString":
         return geometry.MultiLineString(geoms)
@@ -1291,15 +1312,15 @@
 
     if resolution == "auto":
         resolution = _auto_resolution(geom)
 
     if resolution is not None and math.isfinite(resolution):
         geom = geom.segmented(resolution)
 
-    bbox = geom.to_crs("EPSG:4326").boundingbox
+    bbox = geom.to_crs("EPSG:4326", check_and_fix=True).boundingbox
 
     xx_range = bbox.range_x
     if mode == "safe":
         # If range in Longitude is more than 180 then it's probably wrapped
         # around 180 (X-360 for X > 180), so we add back 360 but only for X<0
         # values. This only works if input geometry doesn't span more than half
         # a globe, so we need to check for that too, but this is not yet
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/gridspec.py` & `odc-geo-0.4.1/odc/geo/gridspec.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Dict, Iterator, Optional, Tuple
 
 from affine import Affine
 
 from . import geom
 from .crs import SomeCRS, norm_crs_or_error
 from .geobox import GeoBox
-from .geom import BoundingBox, Geometry, intersects
+from .geom import BoundingBox, Geometry
 from .math import Bin1D
 from .types import (
     XY,
     Index2d,
     Shape2d,
     SomeIndex2d,
     SomeResolution,
@@ -141,30 +141,31 @@
         rx, ry = self.resolution.xy
         return GeoBox(self._shape, crs=self.crs, affine=Affine(rx, 0, tx, 0, ry, ty))
 
     def __getitem__(self, idx: SomeIndex2d) -> GeoBox:
         """Lookup :py:class:`~odc.geo.geobox.GeoBox` of a given tile."""
         return self.tile_geobox(idx)
 
-    def idx_bounds(self, bounds: BoundingBox) -> BoundingBox:
+    def idx_bounds(self, bounds: BoundingBox) -> Tuple[int, int, int, int]:
         """
         Convert bounds from CRS to index space.
 
         :param bounds: Query bounding box
-        :return: Bounding box in tile index space
+        :return: ``x1, y1, x2, y2``, with closed/open range, i.e. ``[x1, x2), [y1, y2)``
         """
         assert self.crs == bounds.crs
+        tol = 1e-8
 
         x1, y1, x2, y2 = bounds
-        ix1, iy1 = self.pt2idx(x1, y1).xy
-        ix2, iy2 = self.pt2idx(x2, y2).xy
+        ix1, iy1 = self.pt2idx(x1 + tol, y1 + tol).xy
+        ix2, iy2 = self.pt2idx(x2 - tol, y2 - tol).xy
 
         ix1, ix2 = sorted([ix1, ix2])
         iy1, iy2 = sorted([iy1, iy2])
-        return BoundingBox(ix1, iy1, ix2, iy2, self.crs)
+        return ix1, iy1, ix2 + 1, iy2 + 1
 
     def tiles(
         self, bounds: BoundingBox, geobox_cache: Optional[dict] = None
     ) -> Iterator[Tuple[Tuple[int, int], GeoBox]]:
         """
         Query tiles overlapping with bounding box.
 
@@ -191,16 +192,16 @@
             if gbox is None:
                 gbox = self.tile_geobox(tile_index)
                 geobox_cache[tile_index] = gbox
             return gbox
 
         ix1, iy1, ix2, iy2 = map(int, self.idx_bounds(bounds))
 
-        for iy in range(iy1, iy2 + 1):
-            for ix in range(ix1, ix2 + 1):
+        for iy in range(iy1, iy2):
+            for ix in range(ix1, ix2):
                 tile_index = (ix, iy)
                 yield tile_index, geobox(tile_index)
 
     def tiles_from_geopolygon(
         self,
         geopolygon: Geometry,
         geobox_cache: Optional[dict] = None,
@@ -212,19 +213,19 @@
 
         :param geopolygon:
           Polygon to tile
         :param geobox_cache:
           Optional cache to re-use geoboxes instead of creating new one each turn: iterator of grid
           cells with :py:class:`odc.geo.geobox.GeoBox` tiles
         """
-        geopolygon = geopolygon.to_crs(self.crs)
+        geopolygon = geopolygon.to_crs(self.crs, check_and_fix=True)
         bbox = geopolygon.boundingbox
 
         for tile_index, tile_geobox in self.tiles(bbox, geobox_cache):
-            if intersects(tile_geobox.extent, geopolygon):
+            if not geopolygon.disjoint(tile_geobox.extent):
                 yield (tile_index, tile_geobox)
 
     def __str__(self) -> str:
         return f"GridSpec(crs={self.crs}, tile_shape={self._shape}, resolution={self.resolution})"
 
     def __repr__(self) -> str:
         return self.__str__()
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/math.py` & `odc-geo-0.4.1/odc/geo/math.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/overlap.py` & `odc-geo-0.4.1/odc/geo/overlap.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,18 @@
 
     Used to pick overview level for reading. A value of ``3`` means you can
     shrink every ``3x3`` pixel block of the source image down to a single pixel,
     and still have higher resolution than requested.
     """
 
     scale: float
-    """Scale change as a single number."""
+    """Scale change as a single number. (the min of scale2)"""
+
+    scale2: XY[float]
+    """Full 2D Scale change as an XY."""
 
     transform: PointTransform
     """Mapping from src pixels to destination pixels."""
 
 
 def get_scale_from_linear_transform(A: Affine) -> XY[float]:
     """
@@ -497,20 +500,22 @@
         if not roi_is_empty(roi_dst):
             center_pt = xy_(roi_center(roi_dst)[::-1])
             scale2 = get_scale_at_point(center_pt, tr.back)
             scale = min(scale2.xy)
             read_shrink = _pick_read_scale(scale)
         else:
             scale = 0
+            scale2 = XY(x=0, y=0)
             read_shrink = 1
 
         return ReprojectInfo(
             roi_src=roi_src,
             roi_dst=roi_dst,
             scale=scale,
+            scale2=scale2,
             paste_ok=False,
             read_shrink=read_shrink,
             transform=tr,
         )
 
     # Same projection case
     #
@@ -542,14 +547,15 @@
             src, dst, tr, pts_per_side=2, padding=padding, align=align
         )
 
     return ReprojectInfo(
         roi_src=roi_src,
         roi_dst=roi_dst,
         scale=scale,
+        scale2=scale2,
         paste_ok=paste_ok,
         read_shrink=read_shrink,
         transform=tr,
     )
 
 
 def compute_output_geobox(
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/roi.py` & `odc-geo-0.4.1/odc/geo/roi.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/testutils.py` & `odc-geo-0.4.1/odc/geo/testutils.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/types.py` & `odc-geo-0.4.1/odc/geo/types.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc/geo/ui.py` & `odc-geo-0.4.1/odc/geo/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,25 @@
     return N // at_least
 
 
 @lru_cache
 def _ocean_svg_path(ndecimal=3, clip_bbox=None):
     from .data import ocean_geom
 
-    g = ocean_geom()
-    if clip_bbox is not None:
-        g = g & geom.box(*clip_bbox, crs=g.crs)
+    g = ocean_geom(bbox=clip_bbox)
     return g.svg_path(ndecimal)
 
 
 def _compute_display_box(
     span: XY[float], sz: int, min_sz: int, tol: float = 1e-6
 ) -> Tuple[Shape2d, float]:
     """
     return: shape in pixels, ``s`` maps sizes from world to pix
     """
-    span_x, span_y = span.xy
+    span_x, span_y = ((v if math.isfinite(v) else 0) for v in span.xy)
     if max(span_x, span_y) < tol:
         # both too small, make it square
         span_x = span_y = tol
         w, h = sz, sz
         s = w / span_x
     elif span_x > span_y:
         # wide case: w = sz, span_x == sz
@@ -87,15 +85,15 @@
     map_svg_path=None,
     target=None,
 ):
     clip_bbox = None
     if bbox is not None:
         clip_bbox = geom.bbox_intersection(
             [geom.BoundingBox(*bbox).buffered(1), geom.BoundingBox(-180, -90, 180, 90)]
-        )
+        ).bbox
     else:
         bbox = (-180, -90, 180, 90)
 
     if map_svg_path is None:
         map_svg_path = _ocean_svg_path(clip_bbox=clip_bbox)
 
     x0, y0, x1, y1 = bbox
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/warp.py` & `odc-geo-0.4.1/odc/geo/warp.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,14 +171,25 @@
     src_nodata: Nodata = None,
     dst_nodata: Nodata = None,
     **kwargs,
 ) -> np.ndarray:
     assert src.ndim == dst.ndim
     assert src.ndim == 2
 
+    if "XSCALE" not in kwargs and "YSCALE" not in kwargs:
+        # Work around for issue in GDAL
+        #    https://github.com/OSGeo/gdal/issues/7750
+        # Force GDAL into performing bilinear,cubic,lanczos with raidius=1px.
+        # GDAL is trying to be smart and pick sampling radius based on scale
+        # change, but does it without consideration for rotational component
+        # of the transform, leading to blury output in some situations
+        # See also:
+        #    https://github.com/opendatacube/datacube-core/issues/1448
+        kwargs.update(XSCALE=1, YSCALE=1)
+
     dtype_remap = {"int8": "int16", "bool": "uint8"}
 
     def _alias_or_convert(arr: np.ndarray) -> Tuple[np.ndarray, bool]:
         if arr.dtype.name not in dtype_remap:
             return arr, False
         wk_dtype = dtype_remap[arr.dtype.name]
         if arr.dtype.name == "bool":
```

### Comparing `odc-geo-0.4.0rc1/odc/geo/xr.py` & `odc-geo-0.4.1/odc/geo/xr.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/odc_geo.egg-info/PKG-INFO` & `odc-geo-0.4.1/odc_geo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.4.0rc1
+Version: 0.4.1
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-geo-0.4.0rc1/odc_geo.egg-info/SOURCES.txt` & `odc-geo-0.4.1/odc_geo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/pyproject.toml` & `odc-geo-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/setup.cfg` & `odc-geo-0.4.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 warp = 
 	rasterio
 all = 
 	%(warp)s
 	%(xr)s
 test = 
 	pytest
+	geopandas
+	dask
 
 [options.packages.find]
 include = 
 	odc*
 
 [options.package_data]
 odc.geo =
```

### Comparing `odc-geo-0.4.0rc1/tests/test_bbox.py` & `odc-geo-0.4.1/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_blocks.py` & `odc-geo-0.4.1/tests/test_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 @pytest.mark.parametrize("dtype", ["int8", "uint16", "float32"])
 def test_block_assembler(tiles: RoiTiles, idx, dtype):
     dtype = np.dtype(dtype)
     Z = np.zeros(tiles.base.shape, dtype)
     for v, _i in enumerate(idx, start=1):
         Z[tiles[_i]] = v
-    Zf = Z.astype(np.floating).copy()
+    Zf = Z.astype(np.float32).copy()
     Zf[Z == 0] = np.nan
 
     blocks = {i: Z[tiles[i]].copy() for i in idx}
     ba = BlockAssembler(blocks, tiles.chunks)
     assert ba.shape == Z.shape
     assert ba.ndim == Z.ndim
     assert ba.dtype == dtype
```

### Comparing `odc-geo-0.4.0rc1/tests/test_cog.py` & `odc-geo-0.4.1/tests/test_cog.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_converters.py` & `odc-geo-0.4.1/tests/test_converters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 # pylint: disable=wrong-import-position
 from pathlib import Path
+from unittest.mock import MagicMock
+from warnings import catch_warnings, filterwarnings
 
 import pytest
-from mock import MagicMock
 
 rasterio = pytest.importorskip("rasterio")
 gpd = pytest.importorskip("geopandas")
 gpd_datasets = pytest.importorskip("geopandas.datasets")
 
 from odc.geo._interop import have
 from odc.geo.converters import extract_gcps, from_geopandas, map_crs, rio_geobox
 from odc.geo.gcp import GCPGeoBox
 from odc.geo.geobox import GeoBox, GeoBoxBase
 
 
-def test_from_geopandas():
-    df = gpd.read_file(gpd_datasets.get_path("naturalearth_lowres"))
+@pytest.fixture
+def ne_lowres_path():
+    with catch_warnings():
+        filterwarnings("ignore")
+        path = gpd_datasets.get_path("naturalearth_lowres")
+    yield path
+
+
+def test_from_geopandas(ne_lowres_path):
+    df = gpd.read_file(ne_lowres_path)
     gg = from_geopandas(df)
     assert isinstance(gg, list)
     assert len(gg) == len(df)
     assert gg[0].crs == "epsg:4326"
 
     (au,) = from_geopandas(df[df.iso_a3 == "AUS"].to_crs(epsg=3577))
     assert au.crs.epsg == 3577
```

### Comparing `odc-geo-0.4.0rc1/tests/test_crs.py` & `odc-geo-0.4.1/tests/test_crs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_dask_interop.py` & `odc-geo-0.4.1/tests/test_dask_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_datasets.py` & `odc-geo-0.4.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_gbox_ops.py` & `odc-geo-0.4.1/tests/test_gbox_ops.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_gcp.py` & `odc-geo-0.4.1/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_geobox.py` & `odc-geo-0.4.1/tests/test_geobox.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_geoboxtiles.py` & `odc-geo-0.4.1/tests/test_geoboxtiles.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_geom.py` & `odc-geo-0.4.1/tests/test_geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,14 +362,26 @@
 
     poly = geom.polygon([(0, 0), (0, 5), (10, 5)], None)
     assert poly.crs is None
     with pytest.raises(ValueError):
         poly.to_crs(epsg3857)
 
 
+def test_to_crs_with_check():
+    crs = "+proj=ortho +lat0=40"
+    gg = geom.line([[-180, 0], [180, 0]], 4326).segmented(5)
+    assert gg.to_crs(crs).is_valid is False
+    assert gg.to_crs(crs, check_and_fix=True).is_valid is True
+
+    gg = gg.buffer(1.1) & geom.box(-180, -90, 180, 90, 4326)
+
+    assert gg.to_crs(crs).is_valid is False
+    assert gg.to_crs(crs, check_and_fix=True).is_valid is True
+
+
 def test_to_crs_utm():
     poly = geom.box(0.1, 43, 1.3, 44, epsg4326)
     assert poly.to_crs("utm").crs.epsg == 32631
     assert poly.to_crs("utm") == poly.to_crs(32631)
     assert poly.to_crs("utm-s").crs.epsg == 32731
 
     poly = geom.box(0.1, -44, 1.3, -43, epsg4326)
@@ -420,14 +432,15 @@
     box1 = geom.box(10, 10, 30, 30, crs=epsg4326)
     box2 = geom.box(15, 10, 35, 30, crs=epsg4326)
     box3 = geom.box(20, 10, 40, 30, crs=epsg4326)
     box4 = geom.box(25, 10, 45, 30, crs=epsg4326)
     box5 = geom.box(30, 10, 50, 30, crs=epsg4326)
     box6 = geom.box(35, 10, 55, 30, crs=epsg4326)
 
+    assert geom.intersects(box1, box2)
     inter1 = geom.unary_intersection([box1])
     assert bool(inter1)
     assert inter1 == box1
 
     inter2 = geom.unary_intersection([box1, box2])
     assert bool(inter2)
     assert inter2.area == 300.0
```

### Comparing `odc-geo-0.4.0rc1/tests/test_gridspec.py` & `odc-geo-0.4.1/tests/test_gridspec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is part of the Open Data Cube, see https://opendatacube.org for more information
 #
 # Copyright (c) 2015-2020 ODC Contributors
 # SPDX-License-Identifier: Apache-2.0
+import itertools
 import math
 
 import numpy
 import pytest
 from pytest import approx
 
 from odc.geo import CRS, res_, resyx_, xy_, yx_
@@ -100,14 +101,31 @@
 
     gs = GridSpec.web_tiles(1)
     assert gs.crs == epsg3857
     assert gs.tile_shape == (256, 256)
     assert gs.tile_size.xy == approx((TSZ0 / 2, TSZ0 / 2))
 
 
+@pytest.mark.parametrize(
+    "gs, tiles_to_check",
+    [
+        (GridSpec.web_tiles(3), itertools.product(range(8), range(8))),
+        (GridSpec(4326, (360, 360), 0.01), [(0, 0), (1, 3), (2, 1)]),
+    ],
+)
+def test_tiles_tight_query_issue_97(gs: GridSpec, tiles_to_check):
+    for idx in tiles_to_check:
+        bbox = gs[idx].boundingbox
+        tiles = list(gs.tiles(bbox))
+        assert len(tiles) == 1
+        ((_idx, gbox),) = tiles
+        assert idx == _idx
+        assert gs[idx] == gbox
+
+
 def test_geojson():
     gs = GridSpec.web_tiles(3)
     gjson = gs.geojson()
 
     assert gjson["type"] == "FeatureCollection"
     assert len(gjson["features"]) == (2**3) ** 2
```

### Comparing `odc-geo-0.4.0rc1/tests/test_map.py` & `odc-geo-0.4.1/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_math.py` & `odc-geo-0.4.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_overlap.py` & `odc-geo-0.4.1/tests/test_overlap.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,27 +161,29 @@
         src.extent.to_crs(epsg3857).buffer(10), resolution=src.resolution
     )
 
     rr = compute_reproject_roi(src, dst)
 
     assert rr.roi_src == np.s_[0 : src.height, 0 : src.width]
     assert 0 < rr.scale < 1
+    assert all(0 < scale < 1 for scale in rr.scale2.xy)
     assert rr.transform.linear is None
     assert rr.transform.back is not None
     assert rr.transform.back.linear is None
 
     # check pure translation case
     roi_ = np.s_[113:-100, 33:-10]
     rr = compute_reproject_roi(src, src[roi_])
     assert rr.roi_src == roi_normalise(roi_, src.shape)
     assert rr.scale == 1
 
     rr = compute_reproject_roi(src, src[roi_], padding=0, align=0)
     assert rr.roi_src == roi_normalise(roi_, src.shape)
     assert rr.scale == 1
+    assert rr.scale2.xy == (1, 1)
 
     # check pure translation case
     roi_ = np.s_[113:-100, 33:-10]
     rr = compute_reproject_roi(src, src[roi_], align=256)
 
     assert rr.roi_src == np.s_[0 : src.height, 0 : src.width]
     assert rr.scale == 1
```

### Comparing `odc-geo-0.4.0rc1/tests/test_rgba.py` & `odc-geo-0.4.1/tests/test_rgba.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from odc.geo._interop import is_dask_collection
 from odc.geo._rgba import is_rgb
 from odc.geo.testutils import daskify
 from odc.geo.xr import ODCExtensionDa, ODCExtensionDs
 
 try:
     import matplotlib
-    import matplotlib.cm
 except ImportError:
     matplotlib = None
 
 
 def test_colorize(ocean_raster: xr.DataArray):
     xx = ocean_raster
 
@@ -57,15 +56,15 @@
     xx = ocean_raster
     cc = xx.odc.colorize("jet")
     assert isinstance(cc.odc, ODCExtensionDa)
     assert cc.odc.geobox == xx.odc.geobox
     assert cc.dtype == "uint8"
     assert cc.shape == (*xx.shape, 4)
 
-    cc = xx.astype("float32").odc.colorize(matplotlib.cm.get_cmap("viridis"))
+    cc = xx.astype("float32").odc.colorize(matplotlib.colormaps.get_cmap("viridis"))
     assert isinstance(cc.odc, ODCExtensionDa)
     assert cc.odc.geobox == xx.odc.geobox
     assert cc.dtype == "uint8"
     assert cc.shape == (*xx.shape, 4)
 
     cc = xx.astype("float32").odc.colorize()
     assert isinstance(cc.odc, ODCExtensionDa)
```

### Comparing `odc-geo-0.4.0rc1/tests/test_rioxarray_interop.py` & `odc-geo-0.4.1/tests/test_rioxarray_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_roi.py` & `odc-geo-0.4.1/tests/test_roi.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_types.py` & `odc-geo-0.4.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_ui.py` & `odc-geo-0.4.1/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0rc1/tests/test_xr_interop.py` & `odc-geo-0.4.1/tests/test_xr_interop.py`

 * *Files identical despite different names*

