# Comparing `tmp/emsarray-0.4.2.tar.gz` & `tmp/emsarray-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emsarray-0.4.2.tar", last modified: Mon Apr 24 05:08:21 2023, max compression
+gzip compressed data, was "emsarray-0.4.3.tar", last modified: Tue Jun 27 03:16:35 2023, max compression
```

## Comparing `emsarray-0.4.2.tar` & `emsarray-0.4.3.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.395366 emsarray-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 05:08:11.000000 emsarray-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-24 05:08:21.395366 emsarray-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-24 05:08:11.000000 emsarray-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-24 05:08:11.000000 emsarray-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-24 05:08:21.395366 emsarray-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:08:11.000000 emsarray-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.387366 emsarray-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/accessors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/commands/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/commands/export_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/commands/extract_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/compat/shapely.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.395366 emsarray-0.4.2/src/emsarray/conventions/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45292 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/arakawa_c.py
--rw-r--r--   0 runner    (1001) docker     (123)    19472 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/shoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    52965 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/ugrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/nco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.395366 emsarray-0.4.2/src/emsarray/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/point_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/triangulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    23259 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.395366 emsarray-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_get_dataset_convention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_nco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.449473 emsarray-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-27 03:16:20.000000 emsarray-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-27 03:16:35.449473 emsarray-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-27 03:16:20.000000 emsarray-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-27 03:16:20.000000 emsarray-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-27 03:16:35.449473 emsarray-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 03:16:20.000000 emsarray-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.441473 emsarray-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.445473 emsarray-0.4.3/src/emsarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/accessors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.445473 emsarray-0.4.3/src/emsarray/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.445473 emsarray-0.4.3/src/emsarray/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/commands/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/commands/export_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/commands/extract_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/commands/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.449473 emsarray-0.4.3/src/emsarray/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/compat/shapely.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.449473 emsarray-0.4.3/src/emsarray/conventions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/conventions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46323 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/conventions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/conventions/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/conventions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/conventions/arakawa_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20656 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/conventions/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/conventions/shoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53189 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/conventions/ugrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/nco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.449473 emsarray-0.4.3/src/emsarray/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/operations/depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/operations/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/operations/point_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/operations/triangulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24309 2023-06-27 03:16:20.000000 emsarray-0.4.3/src/emsarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.445473 emsarray-0.4.3/src/emsarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-27 03:16:35.000000 emsarray-0.4.3/src/emsarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-27 03:16:35.000000 emsarray-0.4.3/src/emsarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:16:35.000000 emsarray-0.4.3/src/emsarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 03:16:35.000000 emsarray-0.4.3/src/emsarray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 03:16:35.000000 emsarray-0.4.3/src/emsarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 03:16:35.000000 emsarray-0.4.3/src/emsarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:16:35.449473 emsarray-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-27 03:16:20.000000 emsarray-0.4.3/tests/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-27 03:16:20.000000 emsarray-0.4.3/tests/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-27 03:16:20.000000 emsarray-0.4.3/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-27 03:16:20.000000 emsarray-0.4.3/tests/test_get_dataset_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-27 03:16:20.000000 emsarray-0.4.3/tests/test_nco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-27 03:16:20.000000 emsarray-0.4.3/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-06-27 03:16:20.000000 emsarray-0.4.3/tests/test_utils.py
```

### Comparing `emsarray-0.4.2/LICENSE` & `emsarray-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/PKG-INFO` & `emsarray-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: emsarray
-Version: 0.4.2
+Version: 0.4.3
 Summary: xarray extension that supports multiple geometry conventions
 Author: "Coastal Environmental Modelling team, Oceans and Atmosphere, CSIRO"
 Author-email: "coasts@csiro.au"
 License: "BSD-3-Clause"
 Project-URL: Documentation, https://emsarray.readthedocs.io/
-Project-URL: Release notes, https://emsarray.readthedocs.io/en/stable/releases/0.4.2/
+Project-URL: Release notes, https://emsarray.readthedocs.io/en/stable/releases/0.4.3/
 Project-URL: Source, https://github.com/csiro-coasts/emsarray/
 Description-Content-Type: text/markdown
 Provides-Extra: plot
 Provides-Extra: tutorial
 Provides-Extra: complete
 Provides-Extra: docs
 Provides-Extra: testing
```

### Comparing `emsarray-0.4.2/README.md` & `emsarray-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/pyproject.toml` & `emsarray-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/setup.cfg` & `emsarray-0.4.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = emsarray
 description = xarray extension that supports multiple geometry conventions
-version = 0.4.2
+version = 0.4.3
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = "Coastal Environmental Modelling team, Oceans and Atmosphere, CSIRO"
 author_email = "coasts@csiro.au"
 license = "BSD-3-Clause"
 project_urls = 
 	Documentation = https://emsarray.readthedocs.io/
-	Release notes = https://emsarray.readthedocs.io/en/stable/releases/0.4.2/
+	Release notes = https://emsarray.readthedocs.io/en/stable/releases/0.4.3/
 	Source = https://github.com/csiro-coasts/emsarray/
 
 [options]
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
@@ -28,14 +28,17 @@
 	pyshp >=2.3.0
 	xarray[parallel] >=0.18.2
 
 [options.packages.find]
 where = src
 include = emsarray*
 
+[options.package_data]
+emsarray = py.typed
+
 [options.extras_require]
 plot = 
 	cartopy >=0.21.1
 	matplotlib >=3.4.3
 	pykdtree >=1.2.2
 tutorial = 
 	pooch >=1.3.0
@@ -67,13 +70,14 @@
 	CFGrid1D = emsarray.conventions.grid:CFGrid1D
 	CFGrid2D = emsarray.conventions.grid:CFGrid2D
 	ShocSimple = emsarray.conventions.shoc:ShocSimple
 	ShocStandard = emsarray.conventions.shoc:ShocStandard
 	UGrid = emsarray.conventions.ugrid:UGrid
 
 [flake8]
+extend-select = E,W
 extend-ignore = E501,W503
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `emsarray-0.4.2/src/emsarray/__init__.py` & `emsarray-0.4.3/src/emsarray/__init__.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/accessors.py` & `emsarray-0.4.3/src/emsarray/accessors.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/cli/__init__.py` & `emsarray-0.4.3/src/emsarray/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/cli/command.py` & `emsarray-0.4.3/src/emsarray/cli/command.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/cli/commands/clip.py` & `emsarray-0.4.3/src/emsarray/cli/commands/clip.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/cli/commands/export_geometry.py` & `emsarray-0.4.3/src/emsarray/cli/commands/export_geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import xarray as xr
 
 import emsarray
 from emsarray.cli import BaseCommand, CommandException
 from emsarray.operations import geometry
 from emsarray.types import Pathish
-from emsarray.utils import PerfTimer
 
 logger = logging.getLogger(__name__)
 
 Writer = Callable[[xr.Dataset, Pathish], None]
 format_writers: Dict[str, Writer] = {
     'geojson': geometry.write_geojson,
     'shapefile': geometry.write_shapefile,
@@ -66,17 +65,16 @@
 
         output_path: Path = options.output_path
         output_format: str = options.format
         if output_format == 'auto':
             output_format = self.guess_format(output_path)
             logger.debug("Guessed output format as %r", output_format)
 
-        with PerfTimer() as t:
-            count = dataset.ems.polygons.size
-        logger.debug("Generated %d polygons in %f seconds", count, t.elapsed)
+        count = dataset.ems.polygons[dataset.ems.mask].size
+        logger.debug("Dataset contains %d polygons", count)
 
         try:
             writer = format_writers[output_format]
         except KeyError:
             raise CommandException(f"Unknown output format {output_format!r}")
 
         logger.debug("Exporting geometry as %r", output_format)
```

### Comparing `emsarray-0.4.2/src/emsarray/cli/commands/extract_points.py` & `emsarray-0.4.3/src/emsarray/cli/commands/extract_points.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/cli/utils.py` & `emsarray-0.4.3/src/emsarray/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from functools import wraps
 from pathlib import Path
 from typing import Callable, Iterator, List, Optional, Protocol
 
 from shapely.geometry import box, shape
 from shapely.geometry.base import BaseGeometry
 
+from emsarray.conventions._registry import entry_point_conventions
+
 from .exceptions import CommandException
 
 cli_logger = logging.getLogger('emsarray.cli')
 error_logger = cli_logger.getChild('errors')
 uncaught_exception_logger = error_logger.getChild('uncaught')
 command_exception_logger = error_logger.getChild('command')
 
@@ -206,14 +208,21 @@
     if level == 1:
         level_str = 'WARNING'
     elif level == 2:
         level_str = 'INFO'
     elif level >= 3:
         level_str = 'DEBUG'
 
+    # Include logging handlers for all plugins
+    entry_point_convention_modules = sorted({
+        convention.__module__
+        for convention in entry_point_conventions()
+        if not convention.__module__.startswith('emsarray.')
+    })
+
     logging.captureWarnings(True)
     logging.config.dictConfig({
         'version': 1,
         'formatters': {
             'default': {
                 'format': '[%(asctime)s %(levelname)s] %(name)s: %(message)s',
                 'datefmt': '%Y-%m-%d %H:%M:%S',
@@ -235,24 +244,28 @@
             },
         },
         'loggers': {
             'emsarray': {'handlers': ['console'], 'level': level_str},
             'emsarray.cli.errors': {
                 'handlers': ['error'], 'level': level_str, 'propagate': False
             },
+            **{
+                module: {'handlers': ['console'], 'level': level_str}
+                for module in entry_point_convention_modules
+            },
             'py.warnings': {'handlers': ['console'], 'level': 'WARNING'},
             '__main__': {'handlers': ['console'], 'level': level_str},
             'shapely': {'handlers': [], 'level': 60},
         },
         'root_logger': {'handlers': ['console'], 'level': 'WARNING'}
     })
 
 
 NUMBER = r'\d+(?:_\d+)*'
-DECIMAL = rf'({NUMBER}|{NUMBER}\.|\.{NUMBER}|{NUMBER}\.{NUMBER})'
+DECIMAL = rf'(-?(?:{NUMBER}|{NUMBER}\.|\.{NUMBER}|{NUMBER}\.{NUMBER}))'
 bounds_re = re.compile(r'\s*,\s*'.join([DECIMAL] * 4))
 
 
 def geometry_argument(argument_string: str) -> BaseGeometry:
     """Try and make some geometry from an argument.
     The following things are tried in order:
```

### Comparing `emsarray-0.4.2/src/emsarray/compat/shapely.py` & `emsarray-0.4.3/src/emsarray/compat/shapely.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/conventions/__init__.py` & `emsarray-0.4.3/src/emsarray/conventions/__init__.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/conventions/_base.py` & `emsarray-0.4.3/src/emsarray/conventions/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from __future__ import annotations
 
 import abc
 import dataclasses
 import enum
 import logging
+import warnings
 from functools import cached_property
 from typing import (
     TYPE_CHECKING, Any, Callable, Dict, FrozenSet, Generic, Hashable, List,
     Optional, Tuple, TypeVar, Union, cast
 )
 
 import numpy as np
 import xarray as xr
+from shapely import unary_union
 from shapely.geometry import Point, Polygon
 from shapely.geometry.base import BaseGeometry
 
 from emsarray import utils
 from emsarray.compat.shapely import SpatialIndex
 from emsarray.operations import depth
 from emsarray.plot import (
-    _requires_plot, animate_on_figure, plot_on_figure,
-    polygons_to_patch_collection
+    _requires_plot, animate_on_figure, plot_on_figure, polygons_to_collection
 )
 from emsarray.state import State
-from emsarray.types import Pathish
+from emsarray.types import Bounds, Pathish
 
 if TYPE_CHECKING:
     # Import these optional dependencies only during type checking
     from cartopy.crs import CRS
     from matplotlib.animation import FuncAnimation
     from matplotlib.axes import Axes
-    from matplotlib.collections import PatchCollection
+    from matplotlib.collections import PolyCollection
     from matplotlib.figure import Figure
     from matplotlib.quiver import Quiver
 
 logger = logging.getLogger(__name__)
 
 
 DataArrayOrName = Union[Hashable, xr.DataArray]
@@ -548,15 +549,15 @@
 
     @cached_property  # type: ignore
     @_requires_plot
     def data_crs(self) -> CRS:
         """
         The coordinate reference system that coordinates in this dataset are
         defined in.
-        Used by :meth:`.make_patch_collection` and :meth:`.make_quiver`.
+        Used by :meth:`.make_poly_collection` and :meth:`.make_quiver`.
         Defaults to :class:`cartopy.crs.PlateCarree`.
         """
         # Lazily imported here as cartopy is an optional dependency
         from cartopy.crs import PlateCarree
         return PlateCarree()
 
     @_requires_plot
@@ -742,43 +743,44 @@
             else:
                 title_bits.append('{}')
             kwargs['title'] = '\n'.join(title_bits)
 
         return animate_on_figure(figure, self, coordinate=coordinate, **kwargs)
 
     @_requires_plot
-    def make_patch_collection(
+    @utils.timed_func
+    def make_poly_collection(
         self,
         data_array: Optional[DataArrayOrName] = None,
         **kwargs: Any,
-    ) -> PatchCollection:
+    ) -> PolyCollection:
         """
-        Make a :class:`~matplotlib.collections.PatchCollection`
+        Make a :class:`~matplotlib.collections.PolyCollection`
         from the geometry of this :class:`~xarray.Dataset`.
         This can be used to make custom matplotlib plots from your data.
 
         If a :class:`~xarray.DataArray` is passed in,
-        the values of that are assigned to the PatchCollection `array` parameter.
+        the values of that are assigned to the PolyCollection `array` parameter.
 
         Parameters
         ----------
         data_array : Hashable or :class:`xarray.DataArray`, optional
             A data array, or the name of a data variable in this dataset. Optional.
             If given, the data array is :meth:`linearised <.make_linear>`
-            and passed to :meth:`PatchCollection.set_array() <matplotlib.cm.ScalarMappable.set_array>`.
+            and passed to :meth:`PolyCollection.set_array() <matplotlib.cm.ScalarMappable.set_array>`.
             The data is used to colour the patches.
             Refer to the matplotlib documentation for more information on styling.
         **kwargs
             Any keyword arguments are passed to the
-            :class:`~matplotlib.collections.PatchCollection` constructor.
+            :class:`~matplotlib.collections.PolyCollection` constructor.
 
         Returns
         -------
-        :class:`~matplotlib.collections.PatchCollection`
-            A PatchCollection constructed using the geometry of this dataset.
+        :class:`~matplotlib.collections.PolyCollection`
+            A PolyCollection constructed using the geometry of this dataset.
 
         Example
         -------
 
         .. code-block:: python
 
             import cartopy.crs as ccrs
@@ -787,26 +789,26 @@
 
             figure = plt.figure(figsize=(10, 8))
             axes = plt.subplot(projection=ccrs.PlateCarree())
             axes.set_aspect(aspect='equal', adjustable='datalim')
 
             ds = emsarray.open_dataset("./tests/datasets/ugrid_mesh2d.nc")
             ds = ds.isel(record=0, Mesh2_layers=-1)
-            patches = ds.ems.make_patch_collection('temp')
+            patches = ds.ems.make_poly_collection('temp')
             axes.add_collection(patches)
             figure.colorbar(patches, ax=axes, location='right', label='meters')
 
             axes.set_title("Depth")
             axes.autoscale()
             figure.show()
         """
         if data_array is not None:
             if 'array' in kwargs:
                 raise TypeError(
-                    "Can not pass both `data_array` and `array` to make_patch_collection"
+                    "Can not pass both `data_array` and `array` to make_poly_collection"
                 )
 
             data_array = self._get_data_array(data_array)
 
             data_array = self.make_linear(data_array)
             if len(data_array.dims) > 1:
                 raise ValueError(
@@ -817,15 +819,27 @@
             kwargs['array'] = values
             if 'clim' not in kwargs:
                 kwargs['clim'] = (np.nanmin(values), np.nanmax(values))
 
         if 'transform' not in kwargs:
             kwargs['transform'] = self.data_crs
 
-        return polygons_to_patch_collection(self.polygons[self.mask], **kwargs)
+        return polygons_to_collection(self.polygons[self.mask], **kwargs)
+
+    def make_patch_collection(
+        self,
+        data_array: Optional[DataArrayOrName] = None,
+        **kwargs: Any,
+    ) -> PolyCollection:
+        warnings.warn(
+            "Convention.make_patch_collection has been renamed to "
+            "Convention.make_poly_collection, and now returns a PolyCollection",
+            category=DeprecationWarning,
+        )
+        return self.make_poly_collection(data_array, **kwargs)
 
     @_requires_plot
     def make_quiver(
         self,
         axes: Axes,
         u: Optional[DataArrayOrName] = None,
         v: Optional[DataArrayOrName] = None,
@@ -925,14 +939,35 @@
         """
         mask = np.fromiter(
             (p is not None for p in self.polygons),
             dtype=bool, count=self.polygons.size)
         return cast(np.ndarray, mask)
 
     @cached_property
+    def geometry(self) -> Polygon:
+        """
+        A shapely :class:`Polygon` that represents the geometry of the entire dataset.
+
+        This is equivalent to the union of all polygons in the dataset,
+        although specific conventions may have a simpler way of constructing this.
+        """
+        return unary_union(self.polygons[self.mask])
+
+    @cached_property
+    def bounds(self) -> Bounds:
+        """
+        Returns minimum bounding region (minx, miny, maxx, maxy) of the entire dataset.
+
+        This is equivalent to the bounds of the dataset :attr:`geometry`,
+        although specific conventons may have a simpler way of constructing this.
+        """
+        return cast(Bounds, self.geometry.bounds)
+
+    @cached_property
+    @utils.timed_func
     def spatial_index(self) -> SpatialIndex[SpatialIndexItem[Index]]:
         """
         A shapely :class:`strtree.STRtree` spatial index of all cells in this dataset.
         This allows for fast spatial lookups, querying which cells lie at
         a point, or which cells intersect a geometry.
 
         Querying the index with :meth:`strtree.STRtree.query_items` will return a list
@@ -954,24 +989,20 @@
                 if polygon.intersects(shape)
             ]
 
         See also
         --------
         :class:`.SpatialIndexItem`
         """
-        logger.info("Building spatial index...")
-        with utils.PerfTimer() as timer:
-            items = [
-                (poly, SpatialIndexItem(index, self.unravel_index(index), poly))
-                for index, poly in enumerate(self.polygons)
-                if poly is not None
-            ]
-            spatial_index = SpatialIndex(items)
-        logger.debug("Build spatial index in %f seconds", timer.elapsed)
-        return spatial_index
+        items = [
+            (poly, SpatialIndexItem(index, self.unravel_index(index), poly))
+            for index, poly in enumerate(self.polygons)
+            if poly is not None
+        ]
+        return SpatialIndex(items)
 
     def get_index_for_point(
         self,
         point: Point,
     ) -> Optional[SpatialIndexItem[Index]]:
         """
         Find the index for a :class:`point <Point>` in the dataset.
```

### Comparing `emsarray-0.4.2/src/emsarray/conventions/_registry.py` & `emsarray-0.4.3/src/emsarray/conventions/_registry.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/conventions/_utils.py` & `emsarray-0.4.3/src/emsarray/conventions/_utils.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/conventions/arakawa_c.py` & `emsarray-0.4.3/src/emsarray/conventions/arakawa_c.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,14 +275,15 @@
             if dims.issuperset(grid_kind_dims):
                 topology = self._topology_for_grid_kind[grid_kind]
                 return grid_kind, topology.size
 
         raise ValueError("Data array did not match any known grids")
 
     @cached_property
+    @utils.timed_func
     def polygons(self) -> np.ndarray:
         # Make an array of shape (j, i, 2) of all the nodes
         grid = np.stack([self.node.longitude.values, self.node.latitude.values], axis=-1)
 
         # Transform this in to an array of shape (topology.size, 4, 2)
         points = np.stack([
             grid[:-1, :-1],
```

### Comparing `emsarray-0.4.2/src/emsarray/conventions/grid.py` & `emsarray-0.4.3/src/emsarray/conventions/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,44 @@
 from functools import cached_property
 from typing import (
     Dict, Generic, Hashable, Optional, Tuple, Type, TypeVar, cast
 )
 
 import numpy as np
 import xarray as xr
+from shapely.geometry import Polygon, box
 from shapely.geometry.base import BaseGeometry
 
 from emsarray import masking, utils
 from emsarray.exceptions import ConventionViolationWarning
-from emsarray.types import Pathish
+from emsarray.types import Bounds, Pathish
 
 from ._base import Convention, Specificity
 
 
 class CFGridKind(str, enum.Enum):
     """"""
     face = 'face'
 
 
 #: A two-tuple of ``(y, x)``.
 CFGridIndex = Tuple[int, int]
 
 
+CF_LATITUDE_UNITS = {
+    'degrees_north', 'degree_north', 'degree_N', 'degrees_N',
+    'degreeN', 'degreesN'
+}
+
+CF_LONGITUDE_UNITS = {
+    'degrees_east', 'degree_east', 'degree_E', 'degrees_E',
+    'degreeE', 'degreesE'
+}
+
+
 class CFGridTopology(abc.ABC):
     """
     A topology helper that keeps track of the latitude and longitude coordinates
     in a CF grid dataset.
     """
     def __init__(
         self,
@@ -64,41 +76,49 @@
     def latitude_name(self) -> Hashable:
         """
         The name of the latitude coordinate variable.
         Found by looking for a variable with either a
         ``standard_name = "latitude"`` or
         ``units = "degree_north"``
         attribute.
+
+        See also
+        --------
+        https://cfconventions.org/Data/cf-conventions/cf-conventions-1.10/cf-conventions.html#latitude-coordinate
         """
         try:
             return next(
                 name
                 for name, variable in self.dataset.variables.items()
-                if variable.attrs.get('standard_name') == 'latitude'
-                or variable.attrs.get('coordinate_type') == 'latitude'
-                or variable.attrs.get('units') == 'degree_north'
+                if variable.attrs.get('units') in CF_LATITUDE_UNITS
+                or variable.attrs.get('standard_name') == 'latitude'
+                or variable.attrs.get('axis') == 'Y'
             )
         except StopIteration:
             raise ValueError("Could not find latitude coordinate")
 
     @cached_property
     def longitude_name(self) -> Hashable:
         """
         The name of the longitude coordinate variable.
         Found by looking for a variable with either a
         ``standard_name = "longitude"`` or
         ``units = "degree_east"``
         attribute.
+
+        See also
+        --------
+        https://cfconventions.org/Data/cf-conventions/cf-conventions-1.10/cf-conventions.html#longitude-coordinate
         """
         try:
             return next(
                 name for name, variable in self.dataset.variables.items()
-                if variable.attrs.get('standard_name') == 'longitude'
-                or variable.attrs.get('coordinate_type') == 'longitude'
-                or variable.attrs.get('units') == 'degree_east'
+                if variable.attrs.get('units') in CF_LONGITUDE_UNITS
+                or variable.attrs.get('standard_name') == 'longitude'
+                or variable.attrs.get('axis') == 'X'
             )
         except StopIteration:
             raise ValueError("Could not find longitude coordinate")
 
     @property
     def latitude(self) -> xr.DataArray:
         """The latitude coordinate variable"""
@@ -219,14 +239,24 @@
             self.topology = topology
 
     @cached_property
     def topology(self) -> Topology:
         """A :class:`CFGridTopology` helper."""
         return self.topology_class(self.dataset)
 
+    @cached_property
+    def bounds(self) -> Bounds:
+        # This can be computed easily from the coordinate bounds
+        topology = self.topology
+        min_x = np.nanmin(topology.longitude_bounds)
+        max_x = np.nanmax(topology.longitude_bounds)
+        min_y = np.nanmin(topology.latitude_bounds)
+        max_y = np.nanmax(topology.latitude_bounds)
+        return (min_x, min_y, max_x, max_y)
+
     def unravel_index(
         self,
         index: int,
         grid_kind: Optional[CFGridKind] = None,
     ) -> CFGridIndex:
         y, x = map(int, np.unravel_index(index, self.topology.shape))
         return (y, x)
@@ -383,14 +413,15 @@
         # Must have one dimensional coordinates
         if len(latitude.dims) != 1 or len(longitude.dims) != 1:
             return None
 
         return Specificity.LOW
 
     @cached_property
+    @utils.timed_func
     def polygons(self) -> np.ndarray:
         lon_bounds = self.topology.longitude_bounds.values
         lat_bounds = self.topology.latitude_bounds.values
 
         # Make a bounds array as if this dataset had 2D coordinates.
         # 1D bounds are (min, max).
         # 2D bounds are (j-i, i-1), (j-1, i+1), (j+1, i+1), (j+1, i-1).
@@ -409,14 +440,20 @@
     @cached_property
     def face_centres(self) -> np.ndarray:
         topology = self.topology
         xx, yy = np.meshgrid(topology.longitude.values, topology.latitude.values)
         centres = np.column_stack((xx.flatten(), yy.flatten()))
         return cast(np.ndarray, centres)
 
+    @cached_property
+    def geometry(self) -> Polygon:
+        # As CFGrid1D is axis aligned,
+        # the geometry can be constructed from the bounds.
+        return box(*self.bounds)
+
 
 # 2D coordinate grids
 
 class CFGrid2DTopology(CFGridTopology):
     """
     Collects information about the topology of a gridded dataset
     so that you don't have to.
@@ -532,14 +569,15 @@
         # Must have two dimensional coordinates
         if len(latitude.dims) != 2 or len(longitude.dims) != 2:
             return None
 
         return Specificity.LOW
 
     @cached_property
+    @utils.timed_func
     def polygons(self) -> np.ndarray:
         # Construct polygons from the bounds of the cells
         lon_bounds = self.topology.longitude_bounds.values
         lat_bounds = self.topology.latitude_bounds.values
 
         # points is a (topology.size, 4, 2) array of the corners of each cell
         points = np.stack([lon_bounds, lat_bounds], axis=-1).reshape((-1, 4, 2))
```

### Comparing `emsarray-0.4.2/src/emsarray/conventions/shoc.py` & `emsarray-0.4.3/src/emsarray/conventions/shoc.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/conventions/ugrid.py` & `emsarray-0.4.3/src/emsarray/conventions/ugrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import xarray as xr
 from shapely.geometry.base import BaseGeometry
 
 from emsarray import utils
 from emsarray.exceptions import (
     ConventionViolationError, ConventionViolationWarning
 )
-from emsarray.types import Pathish
+from emsarray.types import Bounds, Pathish
 
 from ._base import Convention, Specificity
 
 logger = logging.getLogger(__name__)
 
 
 def _split_coord(attr: str) -> Tuple[str, str]:
@@ -223,21 +223,28 @@
     logger.debug("Reindexing %r", connectivity.name)
 
     # Offset the column_values for one-based indexing.
     start_index = _get_start_index(connectivity)
     if start_index != 0:
         column_values = column_values + start_index
 
+    dtype = connectivity.encoding.get('dtype', connectivity.dtype)
+
+    if dtype.kind == 'i':
+        # Ensure the fill value fits within the representable integers
+        max_representable = np.iinfo(dtype).max
+        if max_representable < fill_value:
+            fill_value = max_representable
+
     # We need to preseve the integer dtype,
     # while also accounting for masked values.
     # xarray does not make this easy.
     # By constructing the array using new_fill_value where needed,
     # setting the dtype explicitly, and adding the _FillValue attribute,
     # xarray will cooperate.
-    dtype = connectivity.encoding.get('dtype', connectivity.dtype)
     include_row = ~np.ma.getmask(row_indices)
     raw_values = np.array([
         [
             column_values[item] if item is not np.ma.masked else fill_value
             for item in row
         ]
         for row in old_array[include_row]
@@ -487,15 +494,19 @@
 
         values = data_array.values
 
         if not issubclass(values.dtype.type, np.integer):
             # If a data array has a fill value, xarray will convert that data array
             # to a floating point data type, and replace masked values with np.nan.
             # Here we convert a floating point array to a masked integer array.
-            values = np.ma.masked_invalid(values).astype(np.int_)
+            masked_values = np.ma.masked_invalid(values)
+            # numpy will emit a warning when converting an array with np.nan to int,
+            # even if the nans are masked out.
+            masked_values.data[masked_values.mask] = self.sensible_fill_value
+            values = masked_values.astype(self.sensible_dtype)
         elif '_FillValue' in data_array.attrs:
             # The data array has a fill value, but xarray has not applied it.
             # This implied the dataset was opened with mask_and_scale=False,
             # or was constructed in memory.
             # Convert it to a mask array with _FillValue masked out.
             values = np.ma.masked_equal(values, data_array.attrs['_FillValue'])
         else:
@@ -575,34 +586,33 @@
         if not self.has_edge_dimension:
             raise NoEdgeDimensionException
 
         if self.has_valid_edge_node_connectivity:
             return self._to_index_array(
                 self.edge_node_connectivity, self.edge_dimension)
 
-        logger.info("Building edge_node_array")
-        with utils.PerfTimer() as timer:
-            # Each edge is composed of two nodes. Each edge may be named twice,
-            # once for each face. To de-duplicate this, edges are built up using
-            # this dict-of-sets, where the dict index is the node with the
-            # lower index, and the set is the node indices of the other end.
-            low_highs: Dict[int, Set[int]] = defaultdict(set)
-
-            for face_index, node_pairs in self._face_and_node_pair_iter():
-                for pair in node_pairs:
-                    low, high = sorted(pair)
-                    low_highs[low].add(high)
-            edge_node = np.array([
-                [low, high]
-                for low, highs in low_highs.items()
-                for high in highs
-            ], dtype=self.sensible_dtype)
-        logger.debug("Built edge_node_array in %f seconds", timer.elapsed)
+        return self.make_edge_node_array()
 
-        return edge_node
+    @utils.timed_func
+    def make_edge_node_array(self) -> np.ndarray:
+        # Each edge is composed of two nodes. Each edge may be named twice,
+        # once for each face. To de-duplicate this, edges are built up using
+        # this dict-of-sets, where the dict index is the node with the
+        # lower index, and the set is the node indices of the other end.
+        low_highs: Dict[int, Set[int]] = defaultdict(set)
+
+        for face_index, node_pairs in self._face_and_node_pair_iter():
+            for pair in node_pairs:
+                low, high = sorted(pair)
+                low_highs[low].add(high)
+        return np.array([
+            [low, high]
+            for low, highs in low_highs.items()
+            for high in highs
+        ], dtype=self.sensible_dtype)
 
     @cached_property
     def has_valid_edge_face_connectivity(self) -> bool:
         """
         Does the dataset contain a valid edge_face_connectivity variable?
         Some datasets have an attribute naming a edge_face_connectivity
         variable, but the variable doesn't exist. Other times, the shape of the
@@ -646,34 +656,30 @@
         (:attr:`edge_dimension`, 2),
         indicating which faces border each edge.
         """
         if self.has_valid_edge_face_connectivity:
             return self._to_index_array(
                 self.edge_face_connectivity, self.edge_dimension)
 
-        # Access these outside of the timer below
-        fill_value = self.sensible_fill_value
-        face_edge = self.face_edge_array
-
-        # Build an edge_face_connectivity matrix
-        logger.info("Building edge_face_array")
-        with utils.PerfTimer() as timer:
-            # The edge_face connectivity matrix
-            shape = (self.edge_count, 2)
-            filled = np.full(shape, fill_value, dtype=self.sensible_dtype)
-            edge_face: np.ndarray = np.ma.masked_array(filled, mask=True)
-
-            # The number of faces already seen for this edge
-            edge_face_count = np.zeros(self.edge_count, dtype=self.sensible_dtype)
-
-            for face_index, edge_indices in enumerate(face_edge):
-                for edge_index in edge_indices.compressed():
-                    edge_face[edge_index, edge_face_count[edge_index]] = face_index
-                    edge_face_count[edge_index] += 1
-        logger.debug("Built edge_face_array in %f seconds", timer.elapsed)
+        return self.make_edge_face_array()
+
+    @utils.timed_func
+    def make_edge_face_array(self) -> np.ndarray:
+        # The edge_face connectivity matrix
+        shape = (self.edge_count, 2)
+        filled = np.full(shape, self.sensible_fill_value, dtype=self.sensible_dtype)
+        edge_face: np.ndarray = np.ma.masked_array(filled, mask=True)
+
+        # The number of faces already seen for this edge
+        edge_face_count = np.zeros(self.edge_count, dtype=self.sensible_dtype)
+
+        for face_index, edge_indices in enumerate(self.face_edge_array):
+            for edge_index in edge_indices.compressed():
+                edge_face[edge_index, edge_face_count[edge_index]] = face_index
+                edge_face_count[edge_index] += 1
 
         return edge_face
 
     @cached_property
     def has_valid_face_node_connectivity(self) -> bool:
         """
         Does the dataset contain a valid face_node_connectivity variable?
@@ -759,35 +765,32 @@
         (:attr:`face_dimension`, :attr:`max_node_dimension`),
         representing the edge indices that border each face.
         """
         if self.has_valid_face_edge_connectivity:
             return self._to_index_array(
                 self.face_edge_connectivity, self.face_dimension)
 
-        # Access these outside of the timer below
-        fill_value = self.sensible_fill_value
-        edge_node = self.edge_node_array
+        return self.make_face_edge_array()
 
+    @utils.timed_func
+    def make_face_edge_array(self) -> np.ndarray:
         # Build a face_edge_connectivity matrix
-        logger.info("Building face_edge_array")
-        with utils.PerfTimer() as timer:
-            shape = (self.face_count, self.max_node_count)
-            filled = np.full(shape, fill_value, dtype=self.sensible_dtype)
-            face_edge: np.ndarray = np.ma.masked_array(filled, mask=True)
-
-            node_pair_to_edge_index = {
-                frozenset(edge): edge_index
-                for edge_index, edge in enumerate(edge_node)
-            }
-
-            for face_index, node_pairs in self._face_and_node_pair_iter():
-                for column, node_pair in enumerate(node_pairs):
-                    edge_index = node_pair_to_edge_index[frozenset(node_pair)]
-                    face_edge[face_index, column] = edge_index
-        logger.debug("Built face_edge_array in %f seconds", timer.elapsed)
+        shape = (self.face_count, self.max_node_count)
+        filled = np.full(shape, self.sensible_fill_value, dtype=self.sensible_dtype)
+        face_edge: np.ndarray = np.ma.masked_array(filled, mask=True)
+
+        node_pair_to_edge_index = {
+            frozenset(edge): edge_index
+            for edge_index, edge in enumerate(self.edge_node_array)
+        }
+
+        for face_index, node_pairs in self._face_and_node_pair_iter():
+            for column, node_pair in enumerate(node_pairs):
+                edge_index = node_pair_to_edge_index[frozenset(node_pair)]
+                face_edge[face_index, column] = edge_index
 
         return face_edge
 
     @cached_property
     def has_valid_face_face_connectivity(self) -> bool:
         """
         Does the dataset contain a valid face_face_connectivity variable?
@@ -830,35 +833,31 @@
         (:attr:`face_dimension`, :attr:`max_node_dimension`),
         representing the indices of all faces that border a given face.
         """
         if self.has_valid_face_face_connectivity:
             return self._to_index_array(
                 self.face_face_connectivity, self.face_dimension)
 
-        # Access these outside of the timer below
-        fill_value = self.sensible_fill_value
-        edge_face = self.edge_face_array
+        return self.make_face_face_array()
 
+    def make_face_face_array(self) -> np.ndarray:
         # Build a face_face_connectivity matrix
-        logger.info("Building face_face_array")
-        with utils.PerfTimer() as timer:
-            face_count = np.zeros(self.face_count, dtype=self.sensible_dtype)
-            shape = (self.face_count, self.max_node_count)
-            filled = np.full(shape, fill_value, dtype=self.sensible_dtype)
-            face_face: np.ndarray = np.ma.masked_array(filled, mask=True)
-
-            for edge_index, face_indices in enumerate(edge_face):
-                if np.any(np.ma.getmask(face_indices)):
-                    continue
-                left, right = face_indices
-                face_face[left, face_count[left]] = right
-                face_face[right, face_count[right]] = left
-                face_count[left] += 1
-                face_count[right] += 1
-        logger.debug("Built face_face_array in %f seconds", timer.elapsed)
+        face_count = np.zeros(self.face_count, dtype=self.sensible_dtype)
+        shape = (self.face_count, self.max_node_count)
+        filled = np.full(shape, self.sensible_fill_value, dtype=self.sensible_dtype)
+        face_face: np.ndarray = np.ma.masked_array(filled, mask=True)
+
+        for edge_index, face_indices in enumerate(self.edge_face_array):
+            if np.any(np.ma.getmask(face_indices)):
+                continue
+            left, right = face_indices
+            face_face[left, face_count[left]] = right
+            face_face[right, face_count[right]] = left
+            face_count[left] += 1
+            face_count[right] += 1
 
         return face_face
 
     def _face_and_node_pair_iter(self) -> Iterable[Tuple[int, List[Tuple[int, int]]]]:
         """
         An iterator returning a tuple of ``(face_index, edges)``,
         where ``edges`` is a list of ``(node_index, node_index)`` tuples
@@ -1079,14 +1078,15 @@
         if self.topology.has_edge_dimension and self.topology.edge_dimension in data_array.dims:
             return (UGridKind.edge, self.topology.edge_count)
         if self.topology.node_dimension in data_array.dims:
             return (UGridKind.node, self.topology.node_count)
         raise ValueError("Data array did not have any face, edge, or node dimension")
 
     @cached_property
+    @utils.timed_func
     def polygons(self) -> np.ndarray:
         """Generate list of Polygons"""
         # X,Y coords of each node
         topology = self.topology
         node_x = topology.node_x.values
         node_y = topology.node_y.values
         face_node = topology.face_node_array
@@ -1110,14 +1110,23 @@
     def face_centres(self) -> np.ndarray:
         face_x, face_y = self.topology.face_x, self.topology.face_y
         if face_x is not None and face_y is not None:
             face_centres = np.column_stack((face_x, face_y))
             return cast(np.ndarray, face_centres)
         return super().face_centres
 
+    @cached_property
+    def bounds(self) -> Bounds:
+        topology = self.topology
+        min_x = np.nanmin(topology.node_x)
+        max_x = np.nanmax(topology.node_x)
+        min_y = np.nanmin(topology.node_y)
+        max_y = np.nanmax(topology.node_y)
+        return (min_x, min_y, max_x, max_y)
+
     def selector_for_index(self, index: UGridIndex) -> Dict[Hashable, int]:
         kind, i = index
         if kind is UGridKind.face:
             return {self.topology.face_dimension: i}
         if kind is UGridKind.edge:
             if self.topology.has_edge_dimension:
                 return {self.topology.edge_dimension: i}
@@ -1193,21 +1202,25 @@
 
         logger.debug("Slicing topology variables...")
         # Collect all the topology variables here. These need special handling,
         # compared to data variables. The mesh variable can be reused without
         # any changes.
         topology_variables: List[xr.DataArray] = [topology.mesh_variable]
 
+        # This is the fill value used in the mask.
+        new_fill_value = clip_mask.data_vars['new_node_index'].encoding['_FillValue']
+
         def integer_indices(data_array: xr.DataArray) -> np.ndarray:
-            masked = np.ma.masked_invalid(data_array.values)
-            masked_integers: np.ndarray = masked.astype(np.int_)
+            masked_values = np.ma.masked_invalid(data_array.values)
+            # numpy will emit a warning when converting an array with np.nan to int,
+            # even if the nans are masked out.
+            masked_values.data[masked_values.mask] = new_fill_value
+            masked_integers: np.ndarray = masked_values.astype(np.int_)
             return masked_integers
 
-        # This is the fill value used in the mask.
-        new_fill_value = clip_mask.data_vars['new_node_index'].encoding['_FillValue']
         new_node_indices = integer_indices(clip_mask.data_vars['new_node_index'])
         new_face_indices = integer_indices(clip_mask.data_vars['new_face_index'])
         has_edges = 'new_edge_index' in clip_mask.data_vars
         if has_edges:
             new_edge_indices = integer_indices(clip_mask.data_vars['new_edge_index'])
 
         # Re-index the face_node_connectivity variable
```

### Comparing `emsarray-0.4.2/src/emsarray/exceptions.py` & `emsarray-0.4.3/src/emsarray/exceptions.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/formats.py` & `emsarray-0.4.3/src/emsarray/formats.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/masking.py` & `emsarray-0.4.3/src/emsarray/masking.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/nco.py` & `emsarray-0.4.3/src/emsarray/nco.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/operations/depth.py` & `emsarray-0.4.3/src/emsarray/operations/depth.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,16 +184,16 @@
     # such as [1, 1, 1, nan, nan, nan].
     # `.cumsum()` will then add all the 1's up cumulatively,
     # giving something like `[1, 2, 3, nan, nan, nan]` for a column.
     # `.argmax()` will find the highest non-nan index, and we have our answer!
     #
     # Columns of all nans will have an argmax index of 0.
     # Item 0 in the column will be nan, resulting in nan in the output as desired.
-    depth_indices = (data_array * 0 + 1).cumsum(depth_dimension)
-    max_depth_indices = depth_indices.argmax(depth_dimension)
+    depth_indices = (data_array * 0 + 1).cumsum(str(depth_dimension))
+    max_depth_indices = depth_indices.argmax(str(depth_dimension))
     return cast(xr.DataArray, max_depth_indices)
 
 
 def normalize_depth_variables(
     dataset: xr.Dataset,
     depth_variables: List[Hashable],
     *,
```

### Comparing `emsarray-0.4.2/src/emsarray/operations/geometry.py` & `emsarray-0.4.3/src/emsarray/operations/geometry.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/operations/point_extraction.py` & `emsarray-0.4.3/src/emsarray/operations/point_extraction.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/operations/triangulate.py` & `emsarray-0.4.3/src/emsarray/operations/triangulate.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/plot.py` & `emsarray-0.4.3/src/emsarray/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 if TYPE_CHECKING:
     from .conventions import Convention
 
 try:
     import cartopy.crs
     from cartopy.feature import GSHHSFeature
     from cartopy.mpl import gridliner
-    from matplotlib import animation, patches
+    from matplotlib import animation
     from matplotlib.artist import Artist
     from matplotlib.axes import Axes
-    from matplotlib.collections import PatchCollection
+    from matplotlib.collections import PolyCollection
     from matplotlib.figure import Figure
     from shapely.geometry import Polygon
     CAN_PLOT = True
     IMPORT_EXCEPTION = None
 except ImportError as exc:
     CAN_PLOT = False
     IMPORT_EXCEPTION = exc
 
 
-__all___ = ['CAN_PLOT', 'plot_on_figure', 'polygon_to_patch']
+__all___ = ['CAN_PLOT', 'plot_on_figure', 'polygons_to_collection']
 
 
 _requires_plot = requires_extra(extra='plot', import_error=IMPORT_EXCEPTION)
 
 
 def add_coast(axes: Axes, **kwargs: Any) -> None:
     """
@@ -53,19 +53,19 @@
     kwargs = {
         'facecolor': (0.7, 0.7, 0.7, 0.5),
         'edgecolor': 'darkgrey',
         'linewidth': 0.5,
         **kwargs,
     }
     coast = GSHHSFeature()
-    axes.add_feature(coast,  **kwargs)
+    axes.add_feature(coast, **kwargs)
 
 
 def add_gridlines(axes: Axes) -> gridliner.Gridliner:
-    gridlines = axes.gridlines(draw_labels=True)
+    gridlines = axes.gridlines(draw_labels=True, auto_update=True)
     gridlines.top_labels = False
     gridlines.right_labels = False
     return gridlines
 
 
 def bounds_to_extent(bounds: Tuple[float, float, float, float]) -> List[float]:
     """
@@ -77,62 +77,58 @@
     Example
     -------
 
     .. code-block:: python
 
         import cartopy.crs as ccrs
         import matplotlib.pyplot as plt
-        from emsarray.plot import bounds_to_extent, polygon_to_patch
+        from emsarray.plot import bounds_to_extent
         from shapely.geometry import Polygon
 
         polygon = Polygon([
             (148.30, -40.75), (146.47, -41.19), (144.67, -40.62),
             (146.05, -43.53), (146.87, -43.60), (148.30, -40.75),
         ])
         figure = plt.figure(figsize=(10, 8), dpi=100)
         axes = plt.subplot(projection=ccrs.PlateCarree())
         axes.set_extent(bounds_to_extent(polygon.buffer(0.1).bounds))
-        axes.add_patch(polygon_to_patch(polygon))
-        figure.show()
     """
     minx, miny, maxx, maxy = bounds
     return [minx, maxx, miny, maxy]
 
 
 @_requires_plot
-def polygon_to_patch(polygon: Polygon, **kwargs: Any) -> patches.Polygon:
-    """
-    Convert a :class:`shapely.geometry.Polygon <Polygon>` to a
-    :class:`matplotlib.patches.Polygon`.
-    """
-    return patches.Polygon(np.transpose(polygon.exterior.xy), **kwargs)
-
-
-@_requires_plot
-def polygons_to_patch_collection(
+def polygons_to_collection(
     polygons: Iterable[Polygon],
     **kwargs: Any,
-) -> PatchCollection:
+) -> PolyCollection:
     """
     Convert a list of Shapely :class:`Polygons <Polygon>`
-    to a matplotlib :class:`~matplotlib.collections.PatchCollection`.
+    to a matplotlib :class:`~matplotlib.collections.PolyCollection`.
 
     Parameters
     ----------
-    polygons : iterable of `Polygon`
-        The polygons for the patch collection
+    polygons : iterable of Shapely :class:`Polygons <Polygon>`
+        The polygons for the poly collection
     **kwargs : Any
-        Keyword arguments to pass to the PatchCollection constructor.
+        Keyword arguments to pass to the PolyCollection constructor.
 
     Returns
     -------
-    :class:`matplotlib.collections.PatchCollection`
-        The PatchCollection made up of the polygons passed in.
+    :class:`matplotlib.collections.PolyCollection`
+        A PolyCollection made up of the polygons passed in.
     """
-    return PatchCollection(map(polygon_to_patch, polygons), **kwargs)
+    return PolyCollection(
+        verts=[
+            np.asarray(polygon.exterior.coords)
+            for polygon in polygons
+        ],
+        closed=False,
+        **kwargs
+    )
 
 
 @_requires_plot
 def plot_on_figure(
     figure: Figure,
     convention: Convention,
     *,
@@ -150,15 +146,15 @@
     figure
         The :class:`~matplotlib.figure.Figure` instace to plot on.
     convention
         The :class:`~emsarray.conventions.Convention` instance of the dataset.
         This is used to build the polygons and vector quivers.
     scalar : :class:`xarray.DataArray`, optional
         The data to plot as an :class:`xarray.DataArray`.
-        This will be passed to :meth:`.Convention.make_patch_collection`.
+        This will be passed to :meth:`.Convention.make_poly_collection`.
     vector : tuple of :class:`numpy.ndarray`, optional
         The *u* and *v* components of a vector field
         as a tuple of :class:`xarray.DataArray`.
         These will be passed to :meth:`.Convention.make_quiver`.
     title : str, optional
         The title of the plot. Optional.
     projection : :class:`~cartopy.crs.Projection`
@@ -171,26 +167,26 @@
         projection = cartopy.crs.PlateCarree()
 
     axes = figure.add_subplot(projection=projection)
     axes.set_aspect(aspect='equal', adjustable='datalim')
 
     if scalar is None and vector is None:
         # Plot the polygon shapes for want of anything else to draw
-        patches = convention.make_patch_collection()
-        axes.add_collection(patches)
+        collection = convention.make_poly_collection()
+        axes.add_collection(collection)
         if title is None:
             title = 'Geometry'
 
     if scalar is not None:
         # Plot a scalar variable on the polygons using a colour map
-        patches = convention.make_patch_collection(
+        collection = convention.make_poly_collection(
             scalar, cmap='jet', edgecolor='face')
-        axes.add_collection(patches)
+        axes.add_collection(collection)
         units = scalar.attrs.get('units')
-        figure.colorbar(patches, ax=axes, location='right', label=units)
+        figure.colorbar(collection, ax=axes, location='right', label=units)
 
     if vector is not None:
         # Plot a vector variable using a quiver
         quiver = convention.make_quiver(axes, *vector)
         axes.add_collection(quiver)
 
     if title:
@@ -226,15 +222,15 @@
     convention
         The :class:`~emsarray.conventions.Convention` instance of the dataset.
         This is used to build the polygons and vector quivers.
     coordinate : :class:`xarray.DataArray`
         The coordinate values to vary across frames in the animation.
     scalar : :class:`xarray.DataArray`, optional
         The data to plot as an :class:`xarray.DataArray`.
-        This will be passed to :meth:`.Convention.make_patch_collection`.
+        This will be passed to :meth:`.Convention.make_poly_collection`.
         It should have horizontal dimensions appropriate for this convention,
         and a dimension matching the ``coordinate`` parameter.
     vector : tuple of :class:`numpy.ndarray`, optional
         The *u* and *v* components of a vector field
         as a tuple of :class:`xarray.DataArray`.
         These will be passed to :meth:`.Convention.make_quiver`.
         These should have horizontal dimensions appropriate for this convention,
@@ -269,39 +265,39 @@
     if projection is None:
         projection = cartopy.crs.PlateCarree()
 
     axes = figure.add_subplot(projection=projection)
     axes.set_aspect(aspect='equal', adjustable='datalim')
     axes.title.set_animated(True)
 
-    patches = None
+    collection = None
     if scalar is not None:
         # Plot a scalar variable on the polygons using a colour map
         scalar_values = convention.make_linear(scalar).values[:, convention.mask]
-        patches = convention.make_patch_collection(
+        collection = convention.make_poly_collection(
             cmap='jet', edgecolor='face',
             clim=(np.nanmin(scalar_values), np.nanmax(scalar_values)))
-        axes.add_collection(patches)
-        patches.set_animated(True)
+        axes.add_collection(collection)
+        collection.set_animated(True)
         units = scalar.attrs.get('units')
-        figure.colorbar(patches, ax=axes, location='right', label=units)
+        figure.colorbar(collection, ax=axes, location='right', label=units)
 
     quiver = None
     if vector is not None:
         # Plot a vector variable using a quiver
         vector_u_values, vector_v_values = (
             convention.make_linear(vec).values
             for vec in vector)
         # Quivers must start with some data.
         # Vector arrows are scaled using this initial data.
         # Find the absolute maximum value in all directions for initial data
         # to make the autoscaling behave across all frames.
         coordinate_dim = coordinate.dims[0]
         initial_u, initial_v = (
-            abs(vec).max(dim=coordinate_dim, skipna=True)
+            abs(vec).max(dim=str(coordinate_dim), skipna=True)
             for vec in vector)
         quiver = convention.make_quiver(axes, initial_u, initial_v)
         quiver.set_animated(True)
         axes.add_collection(quiver)
 
     # Draw a coast overlay
     add_coast(axes)
@@ -329,17 +325,17 @@
         changes: List[Artist] = []
         coordinate_value = coordinate.values[index]
         axes.title.set_text(coordinate_callable(coordinate_value))
         changes.append(axes.title)
         changes.extend(gridlines.xline_artists)
         changes.extend(gridlines.yline_artists)
 
-        if patches is not None:
-            patches.set_array(scalar_values[index])
-            changes.append(patches)
+        if collection is not None:
+            collection.set_array(scalar_values[index])
+            changes.append(collection)
 
         if quiver is not None:
             quiver.set_UVC(vector_u_values[index], vector_v_values[index])
             changes.append(quiver)
 
         return changes
```

### Comparing `emsarray-0.4.2/src/emsarray/state.py` & `emsarray-0.4.3/src/emsarray/state.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/tutorial.py` & `emsarray-0.4.3/src/emsarray/tutorial.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/src/emsarray/utils.py` & `emsarray-0.4.3/src/emsarray/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,49 @@
         if self.running:
             raise RuntimeError("Timer is currently running")
         if not hasattr(self, "_start"):
             raise RuntimeError("Timer has not started yet")
         return self._stop - self._start
 
 
+def timed_func(fn: Callable[..., _T]) -> Callable[..., _T]:
+    """
+    Log the execution time of the decorated function.
+    Logs "Calling ``<func.__qualname__>``" before the wrapped function is called,
+    and "Completed ``<func.__qualname__>`` in ``<time>``s" after.
+    The name of the logger is taken from ``func.__module__``.
+
+    Example
+    -------
+
+    .. code-block:: python
+
+        class Grass(Convention):
+            @cached_property
+            @timed_func
+            def polygons(self):
+                return ...
+
+    When called, this will log something like::
+
+        DEBUG Calling Grass.polygons
+        DEBUG Completed Grass.polygons in 3.14s
+    """
+    fn_logger = logging.getLogger(fn.__module__)
+
+    @functools.wraps(fn)
+    def wrapper(*args: Any, **kwargs: Any) -> _T:
+        fn_logger.debug("Calling %s", fn.__qualname__)
+        with PerfTimer() as timer:
+            value = fn(*args, **kwargs)
+        fn_logger.debug("Completed %s in %fs", fn.__qualname__, timer.elapsed)
+        return value
+    return wrapper
+
+
 def to_netcdf_with_fixes(
     dataset: xr.Dataset,
     path: Pathish,
     time_variable: Optional[Hashable] = None,
     **kwargs: Any,
 ) -> None:
     """Saves a :class:`xarray.Dataset` to a netCDF4 file,
```

### Comparing `emsarray-0.4.2/src/emsarray.egg-info/PKG-INFO` & `emsarray-0.4.3/src/emsarray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: emsarray
-Version: 0.4.2
+Version: 0.4.3
 Summary: xarray extension that supports multiple geometry conventions
 Author: "Coastal Environmental Modelling team, Oceans and Atmosphere, CSIRO"
 Author-email: "coasts@csiro.au"
 License: "BSD-3-Clause"
 Project-URL: Documentation, https://emsarray.readthedocs.io/
-Project-URL: Release notes, https://emsarray.readthedocs.io/en/stable/releases/0.4.2/
+Project-URL: Release notes, https://emsarray.readthedocs.io/en/stable/releases/0.4.3/
 Project-URL: Source, https://github.com/csiro-coasts/emsarray/
 Description-Content-Type: text/markdown
 Provides-Extra: plot
 Provides-Extra: tutorial
 Provides-Extra: complete
 Provides-Extra: docs
 Provides-Extra: testing
```

### Comparing `emsarray-0.4.2/src/emsarray.egg-info/SOURCES.txt` & `emsarray-0.4.3/src/emsarray.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/emsarray/__main__.py
 src/emsarray/accessors.py
 src/emsarray/exceptions.py
 src/emsarray/formats.py
 src/emsarray/masking.py
 src/emsarray/nco.py
 src/emsarray/plot.py
+src/emsarray/py.typed
 src/emsarray/state.py
 src/emsarray/tutorial.py
 src/emsarray/types.py
 src/emsarray/utils.py
 src/emsarray.egg-info/PKG-INFO
 src/emsarray.egg-info/SOURCES.txt
 src/emsarray.egg-info/dependency_links.txt
@@ -25,14 +26,15 @@
 src/emsarray/cli/command.py
 src/emsarray/cli/exceptions.py
 src/emsarray/cli/utils.py
 src/emsarray/cli/commands/__init__.py
 src/emsarray/cli/commands/clip.py
 src/emsarray/cli/commands/export_geometry.py
 src/emsarray/cli/commands/extract_points.py
+src/emsarray/cli/commands/plot.py
 src/emsarray/compat/__init__.py
 src/emsarray/compat/shapely.py
 src/emsarray/conventions/__init__.py
 src/emsarray/conventions/_base.py
 src/emsarray/conventions/_registry.py
 src/emsarray/conventions/_utils.py
 src/emsarray/conventions/arakawa_c.py
```

### Comparing `emsarray-0.4.2/src/emsarray.egg-info/requires.txt` & `emsarray-0.4.3/src/emsarray.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/tests/test_accessors.py` & `emsarray-0.4.3/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/tests/test_binding.py` & `emsarray-0.4.3/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/tests/test_formats.py` & `emsarray-0.4.3/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/tests/test_get_dataset_convention.py` & `emsarray-0.4.3/tests/test_get_dataset_convention.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/tests/test_nco.py` & `emsarray-0.4.3/tests/test_nco.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.2/tests/test_plot.py` & `emsarray-0.4.3/tests/test_plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 import numpy as np
 import pytest
 from shapely.geometry import Polygon
 
-from emsarray.plot import polygon_to_patch, polygons_to_patch_collection
+from emsarray.plot import polygons_to_collection
 
 
 @pytest.mark.matplotlib
-def test_polygon_to_patch():
-    polygon = Polygon([(0, 0), (1, 0), (2, 2,), (0, 1), (0, 0)])
-    patch = polygon_to_patch(polygon)
-    for index, poly_coords in enumerate(polygon.exterior.coords):
-        patch_coords = patch.get_xy()[index]
-        assert tuple(poly_coords) == tuple(patch_coords)
-
-
-@pytest.mark.matplotlib
-def test_polygons_to_patch_collection():
+def test_polygons_to_collection():
     polygons = [
         Polygon([(i, 0), (i + 1, 0), (i + 1, 1), (i, 1), (i, 0)])
         for i in range(10)
     ]
     data = np.random.random(10) * 10
-    patch_collection = polygons_to_patch_collection(
+    patch_collection = polygons_to_collection(
         polygons, array=data, cmap='autumn', clim=(0, 10))
 
     # Check that the polygons came through
     assert len(patch_collection.get_paths()) == 10
 
     # Check that keyword arguments were passed through
     assert patch_collection.get_cmap().name == 'autumn'
```

### Comparing `emsarray-0.4.2/tests/test_utils.py` & `emsarray-0.4.3/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import datetime
+import logging
 import pathlib
 
 import netCDF4
 import numpy as np
 import numpy.testing
 import pandas as pd
 import pytest
 import xarray
 import xarray.testing
 
 from emsarray import utils
+from tests.utils import filter_warning
+
+logger = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize(
     ('existing', 'new'),
     [
         ('days since 1990-01-01T00:00:00+10:00', 'days since 1990-01-01 00:00:00 +10:00'),
         ('days since 1990-1-1 0:00:00 +10', 'days since 1990-01-01 00:00:00 +10:00'),
@@ -72,44 +76,65 @@
         np.arange(35, dtype=np.float64).reshape(5, 7),
         np.nan)
     float_with_fill_value_var = xarray.DataArray(data=f_data, dims=['j', 'i'])
     float_with_fill_value_var.encoding["_FillValue"] = np.nan
 
     td_data = np.where(
         np.tri(5, 7, dtype=bool),
-        np.arange(35).reshape(5, 7) * np.timedelta64(1, 'D'),
-        np.timedelta64('nat'))
+        np.arange(35).reshape(5, 7) * np.timedelta64(1, 'D').astype('timedelta64[ns]'),
+        np.timedelta64('nat', 'ns'))
+    logger.info('%r', td_data)
     timedelta_with_missing_value_var = xarray.DataArray(
         data=td_data, dims=['j', 'i'])
     timedelta_with_missing_value_var.encoding['missing_value'] = np.float64('1e35')
     timedelta_with_missing_value_var.encoding['units'] = 'days'
 
     dataset = xarray.Dataset(data_vars={
         "int_var": int_var,
         "float_var": float_var,
         "float_with_fill_value_var": float_with_fill_value_var,
         "timedelta_with_missing_value_var": timedelta_with_missing_value_var,
     })
 
     # Save to a netCDF4 and then prove that it is bad
-    dataset.to_netcdf(tmp_path / "bad.nc")
+    # This emits warnings in current versions of xarray / numpy.
+    # See https://github.com/pydata/xarray/issues/7942
+    with filter_warning(
+        'default', category=RuntimeWarning,
+        message='invalid value encountered in cast',
+        module=r'xarray\.coding\.times',
+        record=True,
+    ) as ws:
+        dataset.to_netcdf(tmp_path / "bad.nc")
+        assert len(ws) == 1
+
     with netCDF4.Dataset(tmp_path / "bad.nc", "r") as nc_dataset:
         # This one shouldn't be here because it is an integer datatype. xarray
         # does the right thing already in this case.
         assert '_FillValue' not in nc_dataset.variables["int_var"].ncattrs()
         # This one shouldn't be here as we didnt set it, and the array is full!
         # This is the problem we are trying to solve
         assert np.isnan(nc_dataset.variables["float_var"].getncattr("_FillValue"))
         # This one is quite alright, we did explicitly set it after all
         assert np.isnan(nc_dataset.variables["float_with_fill_value_var"].getncattr("_FillValue"))
         # This one is incorrect, a `missing_value` attribute has already been set
         assert np.isnan(nc_dataset.variables["timedelta_with_missing_value_var"].getncattr("_FillValue"))
 
     utils.disable_default_fill_value(dataset)
-    dataset.to_netcdf(tmp_path / "good.nc")
+
+    # See https://github.com/pydata/xarray/issues/7942
+    with filter_warning(
+        'default', category=RuntimeWarning,
+        message='invalid value encountered in cast',
+        module=r'xarray\.coding\.times',
+        record=True,
+    ) as ws:
+        dataset.to_netcdf(tmp_path / "good.nc")
+        assert len(ws) == 1
+
     with netCDF4.Dataset(tmp_path / "good.nc", "r") as nc_dataset:
         # This one should still be unset
         assert '_FillValue' not in nc_dataset.variables["int_var"].ncattrs()
         # This one should now be unset
         assert '_FillValue' not in nc_dataset.variables["float_var"].ncattrs()
         # Make sure this didn't get clobbered
         assert np.isnan(nc_dataset.variables["float_with_fill_value_var"].getncattr("_FillValue"))
```

