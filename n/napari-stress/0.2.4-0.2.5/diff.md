# Comparing `tmp/napari_stress-0.2.4.tar.gz` & `tmp/napari_stress-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_stress-0.2.4.tar", last modified: Tue May 30 10:22:21 2023, max compression
+gzip compressed data, was "napari_stress-0.2.5.tar", last modified: Tue Jun 27 18:10:00 2023, max compression
```

## Comparing `napari_stress-0.2.4.tar` & `napari_stress-0.2.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.527933 napari_stress-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-30 10:22:03.000000 napari_stress-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 10:22:03.000000 napari_stress-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-30 10:22:21.527933 napari_stress-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-30 10:22:03.000000 napari_stress-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-30 10:22:04.000000 napari_stress-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-30 10:22:21.527933 napari_stress-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 10:22:04.000000 napari_stress-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.515933 napari_stress-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/_approximation/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_approximation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_approximation/fit_ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/_measurements/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/curvature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/deviation_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/geodesics.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/stresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/temporal_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20106 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_napari_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/_plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_plotting/features_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/_reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/reconstruct_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/refine_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.523933 napari_stress-0.2.4/src/napari_stress/_sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)   354896 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/ExampleTifSequence.tif
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66687 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/dropplet_point_cloud.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1808756 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.523933 napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/spherical_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.523933 napari_stress-0.2.4/src/napari_stress/_stress/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/charts_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)    69024 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/euclidian_k_form_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)    21801 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/lebedev_info_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)   132687 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/lebedev_write_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)    63394 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/manifold_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/sph_func_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_surface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.527933 napari_stress-0.2.4/src/napari_stress/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_spherical_harmonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.527933 napari_stress-0.2.4/src/napari_stress/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_utils/coordinate_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_utils/fit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_utils/frame_by_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.533955 napari_stress-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-27 18:09:38.000000 napari_stress-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-27 18:09:38.000000 napari_stress-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-27 18:10:00.533955 napari_stress-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-27 18:09:38.000000 napari_stress-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-27 18:09:39.000000 napari_stress-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-27 18:10:00.533955 napari_stress-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-27 18:09:39.000000 napari_stress-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.517954 napari_stress-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.521954 napari_stress-0.2.5/src/napari_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.521954 napari_stress-0.2.5/src/napari_stress/_approximation/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_approximation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_approximation/fit_ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.521954 napari_stress-0.2.5/src/napari_stress/_measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/deviation_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/geodesics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/stresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/temporal_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20163 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/toolbox.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_measurements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_napari_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.521954 napari_stress-0.2.5/src/napari_stress/_plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_plotting/features_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.525954 napari_stress-0.2.5/src/napari_stress/_reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_reconstruction/reconstruct_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_reconstruction/refine_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_reconstruction/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_reconstruction/toolbox.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.529955 napari_stress-0.2.5/src/napari_stress/_sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   354896 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_sample_data/ExampleTifSequence.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66687 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_sample_data/dropplet_point_cloud.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1808756 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_sample_data/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.529955 napari_stress-0.2.5/src/napari_stress/_spherical_harmonics/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_spherical_harmonics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_spherical_harmonics/spherical_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.529955 napari_stress-0.2.5/src/napari_stress/_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_stress/charts_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69024 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_stress/euclidian_k_form_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21801 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_stress/lebedev_info_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132687 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_stress/lebedev_write_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63394 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_stress/manifold_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_stress/sph_func_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_surface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.533955 napari_stress-0.2.5/src/napari_stress/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19801 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_spherical_harmonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_tests/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.533955 napari_stress-0.2.5/src/napari_stress/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_utils/coordinate_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_utils/fit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_utils/frame_by_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-27 18:09:39.000000 napari_stress-0.2.5/src/napari_stress/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:10:00.521954 napari_stress-0.2.5/src/napari_stress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-27 18:10:00.000000 napari_stress-0.2.5/src/napari_stress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-27 18:10:00.000000 napari_stress-0.2.5/src/napari_stress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:10:00.000000 napari_stress-0.2.5/src/napari_stress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 18:10:00.000000 napari_stress-0.2.5/src/napari_stress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 18:10:00.000000 napari_stress-0.2.5/src/napari_stress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 18:10:00.000000 napari_stress-0.2.5/src/napari_stress.egg-info/top_level.txt
```

### Comparing `napari_stress-0.2.4/LICENSE` & `napari_stress-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/PKG-INFO` & `napari_stress-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_stress
-Version: 0.2.4
+Version: 0.2.5
 Summary: Interactive surface analysis in napari for measuring mechanical stresses in biological tissues
 Author: Johannes Soltwedel, Ben J. Gross, Elijah Shelton, Carlos Gomez, Otger Campas
 Author-email: johannes_richard.mueller@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/campaslab/napari-stress/issues
 Project-URL: Documentation, https://campaslab.github.io/napari-stress
 Project-URL: Source Code, https://github.com/campaslab/napari-stress
```

### Comparing `napari_stress-0.2.4/README.md` & `napari_stress-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/setup.cfg` & `napari_stress-0.2.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari_stress
-version = 0.2.4
+version = 0.2.5
 description = Interactive surface analysis in napari for measuring mechanical stresses in biological tissues
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Johannes Soltwedel, Ben J. Gross, Elijah Shelton, Carlos Gomez, Otger Campas
 author_email = johannes_richard.mueller@tu-dresden.de
 license = BSD-3-Clause
 license_file = LICENSE
```

### Comparing `napari_stress-0.2.4/src/napari_stress/__init__.py` & `napari_stress-0.2.5/src/napari_stress/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 from . import _measurements as measurements
 from . import _approximation as approximation
 from . import _reconstruction as reconstruction
 from . import _sample_data as sample_data
 
 from ._preprocess import rescale
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_approximation/fit_ellipsoid.py` & `napari_stress-0.2.5/src/napari_stress/_approximation/fit_ellipsoid.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 @register_function(menu="Points > Fit ellipsoid to pointcloud (n-STRESS)")
 @frame_by_frame
 def least_squares_ellipsoid(points: PointsData
                             ) -> VectorsData:
     """
     Fit ellipsoid to points with a last-squares approach.
 
+    This function takes a pointcloud and fits an ellipsoid to it using a
+    least-squares approach. The ellipsoid is returned as a set of vectors
+    representing the major and minor axes of the ellipsoid.
+
     Parameters
     ----------
     points : PointsData
 
     Returns
     -------
     VectorsData: Major/minor axis of the ellipsoid
@@ -33,15 +37,28 @@
 
     return vector
 
 
 @register_function(menu="Points > Calculate normals on ellipsoid (n-STRESS)")
 @frame_by_frame
 def normals_on_ellipsoid(points: PointsData) -> VectorsData:
-    """Retrieve normal vector on ellipsoid points."""
+    """
+    Fits an ellipsoid and calculates the normals vectors.
+
+    This function takes a pointcloud and calculates the normals on the
+    ellipsoid fitted to the pointcloud.
+
+    Parameters
+    ----------
+    points : PointsData
+
+    Returns
+    -------
+    VectorsData: Normals on the ellipsoid
+    """
     coefficients = _solve_ellipsoid_polynomial(points)
 
     A = coefficients.flatten()[0]
     B = coefficients.flatten()[1]	
     C = coefficients.flatten()[2]	
     D = coefficients.flatten()[3]	
     E = coefficients.flatten()[4]
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_deprecated.py` & `napari_stress-0.2.5/src/napari_stress/_deprecated.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/__init__.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
 from .geodesics import (geodesic_distance_matrix,
                         geodesic_path,
                         correlation_on_surface,
                         local_extrema_analysis)
 
 from .stresses import anisotropic_stress, tissue_stress_tensor, maximal_tissue_anisotropy
-from .toolbox import stress_analysis_toolbox, comprehensive_analysis
+from .toolbox import comprehensive_analysis
 from .measurements import distance_to_k_nearest_neighbors
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/curvature.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/curvature.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/deviation_analysis.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/deviation_analysis.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/geodesics.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/geodesics.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,33 +91,31 @@
     surface2: SurfaceData,
     distance_matrix: np.ndarray = None,
     maximal_distance: float = None,
 ) -> dict:
     """
     Calculate (auto-) correlation of features on surface.
 
+    This calculates the correlation of features on a surface with itself
+    (auto-correlation) or with another surface (cross-correlation).
+    If the two input surfaces are identical, this is the auto-correlation.
+
     Parameters
     ----------
     surface1 : SurfaceData
     surface2 : SurfaceData
 
     Returns
     -------
     dict
-        Dictionary with information about correlation between `feature1` and
-        `feature2` on a surface. The keys of the dictionary are:#
-            * `auto_corrs_microns_dists`: Distances for
-                which correlations were binned
-            * `auto_correlations_average`: Correlations
-                between averaged feature values
-            * `auto_correlations_normalized`: Normalized,
-                un-averaged correlations
-            * `auto_correlations_averaged_normalized`:
-                Normalized, averaged correlations
-
+        Dictionary with keys:
+            - auto_correlations_distances
+            - auto_correlations_average
+            - auto_correlations_normalized
+            - auto_correlations_averaged_normalized
     """
     if distance_matrix is None:
         distance_matrix = geodesic_distance_matrix(surface1)
 
     n_points = len(surface1[0])
     dists_lbdv_non0 = distance_matrix[np.triu_indices(n_points)]
 
@@ -218,30 +216,20 @@
     surface : SurfaceData
     distance_matrix : np.ndarray, optional
         geodesic distance matrix. The default is None.
 
     Returns
     -------
     List[LayerDataTuple]
-        local extrema: Points LayerDataTuple with extrema type
-        (maximum/minimum) stored in `features[local_max_and_min]`. The metadata
-        contain:
-            `nearest_min_max_dists`: The distances between every extremum and
-            its nearest other kind of extremum (Max-min distances + min-max
-            distances)
-            `nearest_min_max_dists`: Differene in feature value between
-            neighboring extrema
-            `min_max_pair_distances`: Mutual distances between all extrema
-            `min_max_pair_anisotropies`: Difference in feature expression
-            between all pairs of extrema
-        output_geodesics_min_max: Vectors LayerDataTuple with geodesic
-        distances between every minimum and its nearest maximum
-        output_geodesics_max_min: Vectors LayerDataTuple with geodesic
-        distances between every maximum and its nearest minimum
-
+        List of layer data tuples with features and metadata:
+            - local_max_and_min (features)
+            - nearest_min_max_dists (metadata)
+            - nearest_min_max_anisotropies (metadata)
+            - min_max_pair_distances (metadata)
+            - min_max_pair_anisotropies (metadata)
     """
     triangles = surface[1]
     feature = surface[2]
 
     quad_fit = len(feature)
 
     # should be -1 at local min, +1 at local max, 0 otherwise, 2 if both
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/measurements.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/measurements.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/stresses.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/stresses.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/temporal_correlation.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/temporal_correlation.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,16 @@
 
     def _run(self):
         """Call analysis function."""
         results = comprehensive_analysis(
             self.layer_select.value.data,
             max_degree=self.spinBox_max_degree.value(),
             n_quadrature_points=int(self.comboBox_quadpoints.currentData()),
-            gamma=self.doubleSpinBox_gamma.value()
+            gamma=self.doubleSpinBox_gamma.value(),
+            use_dask=self.checkBox_use_dask.isChecked()
             )
 
         for layer in results:
             _layer = Layer.create(data=layer[0],
                                   meta=layer[1],
                                   layer_type=layer[2])
             self.viewer.add_layer(_layer)
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.ui` & `napari_stress-0.2.5/src/napari_stress/_measurements/toolbox.ui`

 * *Files 2% similar despite different names*

#### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.ui` & `napari_stress-0.2.5/src/napari_stress/_measurements/toolbox.ui`

```diff
@@ -10,24 +10,28 @@
         <height>593</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QGridLayout" name="gridLayout_3">
+      <item row="4" column="0" colspan="2">
+        <widget class="QPushButton" name="pushButton_run">
+          <property name="text">
+            <string>Run</string>
+          </property>
+        </widget>
+      </item>
       <item row="0" column="0">
         <widget class="QLabel" name="label_3">
           <property name="text">
             <string>Input pointcloud</string>
           </property>
         </widget>
       </item>
-      <item row="0" column="1">
-        <widget class="QWidget" name="input_widget" native="true"/>
-      </item>
       <item row="1" column="0" colspan="2">
         <widget class="QGroupBox" name="groupBox_2">
           <property name="title">
             <string>Spherical harmonics</string>
           </property>
           <layout class="QGridLayout" name="gridLayout">
             <item row="0" column="0">
@@ -53,14 +57,30 @@
             </item>
             <item row="1" column="1">
               <widget class="QComboBox" name="comboBox_quadpoints"/>
             </item>
           </layout>
         </widget>
       </item>
+      <item row="5" column="1">
+        <spacer name="verticalSpacer">
+          <property name="orientation">
+            <enum>Qt::Vertical</enum>
+          </property>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>20</width>
+              <height>40</height>
+            </size>
+          </property>
+        </spacer>
+      </item>
+      <item row="0" column="1">
+        <widget class="QWidget" name="input_widget" native="true"/>
+      </item>
       <item row="2" column="0" colspan="2">
         <widget class="QGroupBox" name="groupBox_3">
           <property name="title">
             <string>Stress</string>
           </property>
           <layout class="QGridLayout" name="gridLayout_2">
             <item row="0" column="0">
@@ -72,39 +92,26 @@
             </item>
             <item row="0" column="1">
               <widget class="QDoubleSpinBox" name="doubleSpinBox_gamma">
                 <property name="decimals">
                   <number>3</number>
                 </property>
                 <property name="value">
-                  <double>26.000000000000000</double>
+                  <double>3.000000000000000</double>
                 </property>
               </widget>
             </item>
           </layout>
         </widget>
       </item>
-      <item row="3" column="0" colspan="2">
-        <widget class="QPushButton" name="pushButton_run">
+      <item row="3" column="0">
+        <widget class="QCheckBox" name="checkBox_use_dask">
           <property name="text">
-            <string>Run</string>
+            <string>Parallelize with dask (only timelapse)</string>
           </property>
         </widget>
       </item>
-      <item row="4" column="1">
-        <spacer name="verticalSpacer">
-          <property name="orientation">
-            <enum>Qt::Vertical</enum>
-          </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>20</width>
-              <height>40</height>
-            </size>
-          </property>
-        </spacer>
-      </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_measurements/utils.py` & `napari_stress-0.2.5/src/napari_stress/_measurements/utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_plotting/features_histogram.py` & `napari_stress-0.2.5/src/napari_stress/_plotting/features_histogram.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_preprocess.py` & `napari_stress-0.2.5/src/napari_stress/_preprocess.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_reconstruction/reconstruct_surface.py` & `napari_stress-0.2.5/src/napari_stress/_reconstruction/reconstruct_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_reconstruction/refine_surfaces.py` & `napari_stress-0.2.5/src/napari_stress/_reconstruction/refine_surfaces.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.py` & `napari_stress-0.2.5/src/napari_stress/_reconstruction/toolbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,36 @@
         self.comboBox_fluorescence_type.addItems(["interior", "surface"])
         self.comboBox_interpolation_method.addItems(["linear", "cubic"])
 
         # calculate density/point number
         self.spinBox_n_vertices.setValue(256)
 
         self.pushButton_run.clicked.connect(self._run)
+        self.image_layer_select.changed.connect(self._set_scales)
+
+        self._set_scales()
 
     def eventFilter(self, obj: QObject, event: QEvent):
         """https://forum.image.sc/t/composing-workflows-in-napari/61222/3."""
         if event.type() == QEvent.ParentChange:
             self.image_layer_select.parent_changed.emit(self.parent())
 
         return super().eventFilter(obj, event)
 
+    def _set_scales(self):
+        """Get scales from loaded data."""
+        try:
+            scales = self.image_layer_select.value.scale
+            scales = scales[-3:]  # scales may be 4D
+            self.doubleSpinBox_voxelsize_x.setValue(scales[2])
+            self.doubleSpinBox_voxelsize_y.setValue(scales[1])
+            self.doubleSpinBox_voxelsize_z.setValue(scales[0])
+        except Exception:
+            pass
+
     def _run(self):
         """Call analysis function."""
         import webbrowser
 
         current_voxel_size = np.asarray(
             [
                 self.doubleSpinBox_voxelsize_z.value(),
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.ui` & `napari_stress-0.2.5/src/napari_stress/_reconstruction/toolbox.ui`

 * *Files 19% similar despite different names*

#### Comparing `napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.ui` & `napari_stress-0.2.5/src/napari_stress/_reconstruction/toolbox.ui`

```diff
@@ -23,31 +23,34 @@
       </item>
       <item row="0" column="1">
         <widget class="QWidget" name="widget" native="true"/>
       </item>
       <item row="1" column="0" colspan="2">
         <widget class="QToolBox" name="toolBox">
           <property name="currentIndex">
-            <number>2</number>
+            <number>0</number>
           </property>
           <widget class="QWidget" name="page_3">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
                 <width>855</width>
-                <height>308</height>
+                <height>312</height>
               </rect>
             </property>
             <attribute name="label">
               <string>1. Rescaling</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_7">
               <item row="0" column="1">
                 <widget class="QDoubleSpinBox" name="doubleSpinBox_voxelsize_x">
+                  <property name="decimals">
+                    <number>4</number>
+                  </property>
                   <property name="value">
                     <double>1.000000000000000</double>
                   </property>
                 </widget>
               </item>
               <item row="1" column="0">
                 <widget class="QLabel" name="label_4">
@@ -61,14 +64,17 @@
                   <property name="text">
                     <string>Voxel size x [µm]</string>
                   </property>
                 </widget>
               </item>
               <item row="3" column="1">
                 <widget class="QDoubleSpinBox" name="doubleSpinBox_target_voxelsize">
+                  <property name="decimals">
+                    <number>4</number>
+                  </property>
                   <property name="value">
                     <double>1.000000000000000</double>
                   </property>
                 </widget>
               </item>
               <item row="2" column="0">
                 <widget class="QLabel" name="label_14">
@@ -82,21 +88,27 @@
                   <property name="text">
                     <string>Target voxel size [m]</string>
                   </property>
                 </widget>
               </item>
               <item row="1" column="1">
                 <widget class="QDoubleSpinBox" name="doubleSpinBox_voxelsize_y">
+                  <property name="decimals">
+                    <number>4</number>
+                  </property>
                   <property name="value">
                     <double>1.000000000000000</double>
                   </property>
                 </widget>
               </item>
               <item row="2" column="1">
                 <widget class="QDoubleSpinBox" name="doubleSpinBox_voxelsize_z">
+                  <property name="decimals">
+                    <number>4</number>
+                  </property>
                   <property name="value">
                     <double>1.000000000000000</double>
                   </property>
                 </widget>
               </item>
               <item row="4" column="0" colspan="2">
                 <spacer name="verticalSpacer_4">
@@ -115,15 +127,15 @@
           </widget>
           <widget class="QWidget" name="page">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
                 <width>855</width>
-                <height>308</height>
+                <height>312</height>
               </rect>
             </property>
             <attribute name="label">
               <string>2. Initial reconstruction</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_3">
               <item row="0" column="3">
@@ -195,17 +207,17 @@
               </item>
             </layout>
           </widget>
           <widget class="QWidget" name="page_2">
             <property name="geometry">
               <rect>
                 <x>0</x>
-                <y>-53</y>
+                <y>0</y>
                 <width>838</width>
-                <height>365</height>
+                <height>371</height>
               </rect>
             </property>
             <attribute name="label">
               <string>3. Surface tracing</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_2">
               <item row="2" column="0" colspan="2">
@@ -428,10 +440,30 @@
               <height>40</height>
             </size>
           </property>
         </spacer>
       </item>
     </layout>
   </widget>
+  <tabstops>
+    <tabstop>doubleSpinBox_voxelsize_x</tabstop>
+    <tabstop>doubleSpinBox_voxelsize_y</tabstop>
+    <tabstop>doubleSpinBox_voxelsize_z</tabstop>
+    <tabstop>doubleSpinBox_target_voxelsize</tabstop>
+    <tabstop>doubleSpinBox_gaussian_blur</tabstop>
+    <tabstop>spinBox_n_vertices</tabstop>
+    <tabstop>spinBox_n_smoothing</tabstop>
+    <tabstop>spinBox_n_refinement_steps</tabstop>
+    <tabstop>doubleSpinBox_sampling_length</tabstop>
+    <tabstop>comboBox_fittype</tabstop>
+    <tabstop>comboBox_fluorescence_type</tabstop>
+    <tabstop>doubleSpinBox_trace_length</tabstop>
+    <tabstop>doubleSpinBox_sampling_distance</tabstop>
+    <tabstop>comboBox_interpolation_method</tabstop>
+    <tabstop>checkBox_remove_outliers</tabstop>
+    <tabstop>doubleSpinBox_outlier_tolerance</tabstop>
+    <tabstop>pushButton_run</tabstop>
+    <tabstop>checkBox_use_dask</tabstop>
+  </tabstops>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_sample_data/ExampleTifSequence.tif` & `napari_stress-0.2.5/src/napari_stress/_sample_data/ExampleTifSequence.tif`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_sample_data/dropplet_point_cloud.csv` & `napari_stress-0.2.5/src/napari_stress/_sample_data/dropplet_point_cloud.csv`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv` & `napari_stress-0.2.5/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_sample_data/sample_data.py` & `napari_stress-0.2.5/src/napari_stress/_sample_data/sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/spherical_harmonics.py` & `napari_stress-0.2.5/src/napari_stress/_spherical_harmonics/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py` & `napari_stress-0.2.5/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_stress/charts_SPB.py` & `napari_stress-0.2.5/src/napari_stress/_stress/charts_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_stress/euclidian_k_form_SPB.py` & `napari_stress-0.2.5/src/napari_stress/_stress/euclidian_k_form_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_stress/lebedev_info_SPB.py` & `napari_stress-0.2.5/src/napari_stress/_stress/lebedev_info_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_stress/lebedev_write_SPB.py` & `napari_stress-0.2.5/src/napari_stress/_stress/lebedev_write_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_stress/manifold_SPB.py` & `napari_stress-0.2.5/src/napari_stress/_stress/manifold_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_stress/sph_func_SPB.py` & `napari_stress-0.2.5/src/napari_stress/_stress/sph_func_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_surface.py` & `napari_stress-0.2.5/src/napari_stress/_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_approximation.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_approximation.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_measurements.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_measurements.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,22 +187,24 @@
     H0 = measurements.average_mean_curvatures_on_manifold(manifold)[2]
     distance_matrix = measurements.haversine_distances(max_degree, 434)/H0
     
 
     measurements.spatio_temporal_autocorrelation(surfaces=surfaces_4d,
                                                  distance_matrix=distance_matrix)
 
+
 def test_autocorrelation():
     from napari_stress import measurements
     import numpy as np
     import pandas as pd
     
     n_frames = 10
     n_measurements = 100
 
+    np.random.seed(1)
     # create a set of features in multiple timepoints and add a bit more noise
     # in every frame - the autocorrelaiton should thus decrease monotonously
     frames = np.repeat(np.arange(n_frames), n_measurements)
     feature = np.ones(n_measurements)
     features = []
     features.append(feature)
     for i in range(1, n_frames):
@@ -210,14 +212,15 @@
 
     df = pd.DataFrame(np.concatenate(features), columns=['feature'])
     df['frame'] = frames
 
     gradient = np.gradient(measurements.temporal_autocorrelation(df, feature='feature'))
     assert np.all(gradient < 0)
 
+
 def test_haversine():
     from napari_stress import measurements
 
     distance_matrix = measurements.haversine_distances(degree_lebedev=10, n_lebedev_points=434)
 
     # the biggest possible distance on a unit sphere is pi/2
     assert np.allclose(distance_matrix.max(), np.pi/2)
@@ -253,32 +256,34 @@
     assert geodesic_vectors.shape[0] == 44
     assert geodesic_vectors.shape[1] == 2
     assert geodesic_vectors.shape[2] == 3
 
 
 def test_comprehenive_stress_toolbox(make_napari_viewer):
     from napari_stress import (get_droplet_point_cloud, measurements)
+    import napari_stress
 
     viewer = make_napari_viewer()
     pointcloud = get_droplet_point_cloud()[0]
     viewer.add_points(pointcloud[0][:, 1:], **pointcloud[1])
 
-    widget = measurements.stress_analysis_toolbox(viewer)
+    widget = napari_stress._measurements.toolbox.stress_analysis_toolbox(viewer)
     viewer.window.add_dock_widget(widget)
 
     widget._run()
 
 def test_comprehensive_stress_toolbox_4d(make_napari_viewer):
     from napari_stress import (get_droplet_point_cloud_4d, measurements)
+    import napari_stress
 
     viewer = make_napari_viewer()
     pointcloud = get_droplet_point_cloud_4d()[0]
     viewer.add_points(pointcloud[0], **pointcloud[1])
 
-    widget = measurements.stress_analysis_toolbox(viewer)
+    widget = napari_stress._measurements.toolbox.stress_analysis_toolbox(viewer)
     viewer.window.add_dock_widget(widget)
 
     widget._run()
 
 
 def test_curvature(make_napari_viewer):
     from napari_stress._spherical_harmonics.spherical_harmonics_napari import perform_lebedev_quadrature
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_plotting.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_processing.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_reconstruction.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_reconstruction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 
 
 def test_reconstruction(make_napari_viewer):
     from napari_stress import reconstruction, get_droplet_4d
     from napari.layers import Layer
+    import napari_stress
 
     viewer = make_napari_viewer()
     image = get_droplet_4d()[0][0]
-    viewer.add_image(image)
+    viewer.add_image(image, scale=[1.1, 1.1, 1.1], name='image')
 
-    widget = reconstruction.droplet_reconstruction_toolbox(viewer)
+    widget = napari_stress._reconstruction.toolbox.droplet_reconstruction_toolbox(viewer)
     viewer.window.add_dock_widget(widget)
 
+    assert widget.doubleSpinBox_voxelsize_x.value() == 1.1
+    assert widget.doubleSpinBox_voxelsize_y.value() == 1.1
+    assert widget.doubleSpinBox_voxelsize_z.value() == 1.1
+
     results = reconstruction.reconstruct_droplet(
         image,
         voxelsize=np.asarray([1.93, 1, 1]),
+        interpolation_method='linear',
         target_voxelsize=1
         )
 
     for result in results:
         layer = Layer.create(result[0], result[1], result[2])
         viewer.add_layer(layer)
 
     # test with dask
     results = reconstruction.reconstruct_droplet(
         image,
         voxelsize=np.asarray([1.93, 1, 1]),
         target_voxelsize=1,
+        interpolation_method='linear',
         resampling_length=1,
         use_dask=True
         )
 
 
 def test_quadrature_point_reconstuction(make_napari_viewer):
     from napari_stress import get_droplet_point_cloud, fit_spherical_harmonics
@@ -122,31 +129,32 @@
         trace_length=10,
         selected_fit_type=fit_type,
         interpolation_method='linear',
         remove_outliers=True)
     traced_points = results[0][0]
     assert len(traced_points.squeeze()) < len(surf_points)
 
-    # Now, let's test surface-labelled data
-    blurry_ring = filters.sobel(image)
+    # # Now, let's test surface-labelled data
+    # blurry_ring = filters.sobel(image)
 
-    surf_points = shapes.Sphere().points()
-    surf_points += (surf_points * true_radius + 2) + 50
+    # surf_points = shapes.Sphere().points()
+    # surf_points += (surf_points * true_radius + 2) + 50
 
-    fit_type = 'fancy'
-    results = reconstruction.trace_refinement_of_surface(
-        blurry_ring, surf_points,
-        trace_length=10,
-        sampling_distance=1,
-        selected_fit_type=fit_type,
-        selected_edge='surface',
-        remove_outliers=False)
-
-    fit_type = 'quick'
-    results = reconstruction.trace_refinement_of_surface(
-        blurry_ring, surf_points,
-        trace_length=10,
-        sampling_distance=1,
-        selected_fit_type=fit_type,
-        selected_edge='surface',
-        interpolation_method='linear',
-        remove_outliers=False)
+    # fit_type = 'fancy'
+    # results = reconstruction.trace_refinement_of_surface(
+    #     blurry_ring, surf_points,
+    #     trace_length=10,
+    #     sampling_distance=1,
+    #     selected_fit_type=fit_type,
+    #     interpolation_method='linear',
+    #     selected_edge='surface',
+    #     remove_outliers=False)
+
+    # fit_type = 'quick'
+    # results = reconstruction.trace_refinement_of_surface(
+    #     blurry_ring, surf_points,
+    #     trace_length=10,
+    #     sampling_distance=1,
+    #     selected_fit_type=fit_type,
+    #     selected_edge='surface',
+    #     interpolation_method='linear',
+    #     remove_outliers=False)
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_spherical_harmonic_fit.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_spherical_harmonic_fit.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_surface.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_types.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_types.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_utils.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_tests/test_vectors.py` & `napari_stress-0.2.5/src/napari_stress/_tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_utils/coordinate_conversion.py` & `napari_stress-0.2.5/src/napari_stress/_utils/coordinate_conversion.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_utils/fit_utils.py` & `napari_stress-0.2.5/src/napari_stress/_utils/fit_utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/_utils/frame_by_frame.py` & `napari_stress-0.2.5/src/napari_stress/_utils/frame_by_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from napari.types import PointsData, SurfaceData, ImageData, LabelsData, LayerDataTuple, VectorsData
 from napari.layers import Points, Layer
 
 from typing import List
 
 from functools import wraps
 import inspect
-from dask.distributed import Client
+from dask.distributed import Client, get_client
 
 import pandas as pd
 import tqdm
 
+
 def frame_by_frame(function: callable, progress_bar: bool = False):
 
     @wraps(function)
     def wrapper(*args, **kwargs):
 
         sig = inspect.signature(function)
         annotations = [
-            sig.parameters[key].annotation for key in sig.parameters.keys()
-            ]
+            sig.parameters[key].annotation for key in sig.parameters.keys()]
 
         converter = TimelapseConverter()
 
         args = list(args)
         n_frames = None
 
         # Inspect arguments and check if `use_dask` is passed as keyword argument
@@ -40,22 +40,21 @@
         for idx, arg in enumerate(args):
             if annotations[idx] in converter.supported_data:
                 args[idx] = converter.data_to_list_of_data(arg, annotations[idx])
                 index_of_converted_arg.append(idx)
                 n_frames = len(args[idx])
 
         # apply function frame by frame
-        #TODO: Put this in a thread by default?
         results = [None] * n_frames
         frames = tqdm.tqdm(range(n_frames)) if progress_bar else range(n_frames)
-        
+
         # start dask cluster client
         if use_dask:
             client = Client()
-            print('Dask client up an running', client, ' Log: https://localhost:8787')
+            print('Dask client up and running', client, f' Log: {client.dashboard_link}')
             jobs = []
 
         for t in frames:
             _args = args.copy()
 
             # Replace 4D argument by single frame (arg[t])
             for idx in index_of_converted_arg:
@@ -70,14 +69,15 @@
             # gather results
             results = client.gather(jobs)
             client.close()
 
         return converter.list_of_data_to_data(results, sig.return_annotation)
     return wrapper
 
+
 class TimelapseConverter:
     """
     This class allows converting napari 4D layer data between different formats.
     """
     def __init__(self):
 
         # Supported LayerData types
@@ -89,17 +89,15 @@
             ImageData: self._image_to_list_of_images,
             'napari.types.ImageData': self._image_to_list_of_images,
             LabelsData: self._image_to_list_of_images,
             'napari.types.LabelsData': self._image_to_list_of_images,
             VectorsData: self._vectors_to_list_of_vectors,
             Points: self._layer_to_list_of_layers,
             'napari.types.VectorsData': self._vectors_to_list_of_vectors,
-            Points: self._layer_to_list_of_layers,
-            str: None
-            }
+            str: None}
 
     # Supported list data types
         self.list_to_data_conversion_functions = {
             Layer: self._list_of_layers_to_layer,
             PointsData: self._list_of_points_to_points,
             'napari.types.PointsData': self._list_of_points_to_points,
             SurfaceData: self._list_of_surfaces_to_surface,
@@ -108,25 +106,23 @@
             'napari.types.ImageData': self._list_of_images_to_image,
             LabelsData: self._list_of_images_to_image,
             'napari.types.LabelsData': self._list_of_images_to_image,
             LayerDataTuple: self._list_of_layerdatatuple_to_layerdatatuple,
             List[LayerDataTuple]: self._list_of_multiple_ldtuples_to_multiple_ldt_tuples,
             VectorsData: self._list_of_vectors_to_vectors,
             'napari.types.VectorsData': self._list_of_vectors_to_vectors,
-            Points: self._list_of_layers_to_layer
-            }
+            Points: self._list_of_layers_to_layer}
 
         # This list of aliases allows to map LayerDataTuples to the correct napari.types
         self.tuple_aliases = {
             'points': PointsData,
             'surface': SurfaceData,
             'image': ImageData,
             'labels': LabelsData,
-            'vectors': VectorsData
-            }
+            'vectors': VectorsData}
 
         self.supported_data = list(self.list_to_data_conversion_functions.keys())
 
     def data_to_list_of_data(self, data, layertype: type) -> list:
         """
         Convert 4D data into a list of 3D data frames
 
@@ -143,15 +139,15 @@
             layertype
 
         Returns
         -------
         list: List of 3D objects of type `layertype`
 
         """
-        if not layertype in list(self.data_to_list_conversion_functions.keys()):
+        if layertype not in list(self.data_to_list_conversion_functions.keys()):
             raise TypeError(f'{layertype} data to list conversion currently not supported.')
 
         conversion_function = self.data_to_list_conversion_functions[layertype]
         return conversion_function(data)
 
     def list_of_data_to_data(self, data, layertype: type):
         """
@@ -170,31 +166,31 @@
             layertype
 
         Returns
         -------
         4D data of type `layertype`
 
         """
-        if not layertype in self.supported_data:
+        if layertype not in self.supported_data:
             raise TypeError(f'{layertype} list to data conversion currently not supported.')
         conversion_function = self.list_to_data_conversion_functions[layertype]
         return conversion_function(data)
 
     # =============================================================================
     # Layers
     # =============================================================================
 
     def _list_of_layers_to_layer(self, layer_list: list) -> Layer:
         """Convert a list of layers to single layer."""
         list_of_layerdatatuples = [layer.as_layerdatatuple() for layer in layer_list]
         layerdatatuple = self.list_of_layerdatatuple_to_layerdatatuple(list_of_layerdatatuples)
 
         converted_layer = Layer.create(layerdatatuple[0],
-                                       meta = layerdatatuple[1],
-                                       layer_type = layerdatatuple[2])
+                                       meta=layerdatatuple[1],
+                                       layer_type=layerdatatuple[2])
 
         return converted_layer
 
     def _layer_to_list_of_layer(self, layer: Layer) -> list:
         """Convert layer to list of layers."""
         ldtuple = layer.as_layer_data_tuple()
         list_of_ldtuples = self._ldtuple_to_list_of_ldtuple(ldtuple)
@@ -219,62 +215,56 @@
 
         else:
             # unstack features
             if 'features' in tuple_data[1].keys():
                 # group features by time-stamp
                 features = tuple_data[1]['features']
                 list_of_features = [
-                    x for _, x in features.groupby(tuple_data[0][:, 0])
-                    ]
+                    x for _, x in features.groupby(tuple_data[0][:, 0])]
 
             # unstack metadata
             if 'metadata' in tuple_data[1].keys():
                 metadata = tuple_data[1]['metadata']
                 list_of_metadata = [
                     {key : value[i] for key, value in metadata.items()}
-                    for i in range(len(list_of_data))
-                    ]
+                    for i in range(len(list_of_data))]
 
         list_of_props = [{'features': features, 'metadata': metadata}
                          for features, metadata in zip(
-                                 list_of_features, list_of_metadata
-                                 )]
+            list_of_features, list_of_metadata)]
 
         list_of_ldtuples = [(data, props, layertype)
                             for data, props in zip(list_of_data, list_of_props)]
 
         return list_of_ldtuples
 
-
     def _list_of_multiple_ldtuples_to_multiple_ldt_tuples(self,
                                                           tuple_data: list,
                                                           ) -> List[LayerDataTuple]:
         """If a function returns a list of LayerDataTuple"""
 
         # Convert data to array with dimensions [frame, results, data]
         data = np.stack(tuple_data)
 
         if len(data) == 1:
-            layertypes = data[:,..., -1].squeeze()
+            layertypes = data[:, ..., -1].squeeze()
         else:
-            layertypes = data[:,..., -1].squeeze()[0]
+            layertypes = data[:, ..., -1].squeeze()[0]
 
         converted_tuples = []
         for idx, res_type in enumerate(layertypes):
             tuples_to_convert = data[:, idx]
             converted_tuples.append(
-                self._list_of_layerdatatuple_to_layerdatatuple(list(tuples_to_convert))
-                )
+                self._list_of_layerdatatuple_to_layerdatatuple(list(tuples_to_convert)))
 
         return converted_tuples
 
-
     def _list_of_layerdatatuple_to_layerdatatuple(self,
-                                                 tuple_data: list
-                                                 ) -> LayerDataTuple:
+                                                  tuple_data: list
+                                                  ) -> LayerDataTuple:
         """
         Convert a list of 3D layerdatatuple objects to a single 4D LayerDataTuple
         """
         layertype = self.tuple_aliases[tuple_data[-1][-1]]
 
         # Convert data to array with dimensions [frame, data]
         data = np.stack(tuple_data)
@@ -310,17 +300,14 @@
         # exclude 'scale' from stacked metadata
         if 'scale' in layer_props.keys() and len(data) != 1:
             layer_props['scale'] = properties[0]['scale']
 
         for key in layer_props.keys():
             _properties[key] = layer_props[key]
 
-        # Reminder: Each list entry is tuple (data, properties, type)
-        results = [None] * len(data)  # allocate list for results
-
         dtype = data[0, -1]
         result = [None] * 3
         result[0] = self.list_to_data_conversion_functions[layertype]([x for x in data[:, 0]])
         result[1] = _properties
         result[2] = dtype
 
         return tuple(result)
@@ -380,29 +367,27 @@
         vectors = vectors[:, 1]
 
         # the vectors and points should abide to the same dimensions
         point_list = self._points_to_list_of_points(base_points)
         vector_list = self._points_to_list_of_points(vectors)
 
         output_vectors = [
-            np.stack([pt, vec]).transpose((1, 0, 2)) for pt, vec in zip (point_list, vector_list)
-            ]
+            np.stack([pt, vec]).transpose((1, 0, 2)) for pt, vec in zip(point_list, vector_list)]
         return output_vectors
 
     def _list_of_vectors_to_vectors(self, vectors: list) -> VectorsData:
         base_points = [v[:, 0] for v in vectors]
         directions = [v[:, 1] for v in vectors]
 
         base_points = self._list_of_points_to_points(base_points)
         directions = self._list_of_points_to_points(directions)
 
-        vectors = np.stack([base_points, directions]).transpose((1,0,2))
+        vectors = np.stack([base_points, directions]).transpose((1, 0, 2))
         return vectors
 
-
     # =============================================================================
     # Surfaces
     # =============================================================================
 
     def _surface_to_list_of_surfaces(self, surface: SurfaceData) -> list:
         """Convert a 4D surface to list of 3D surfaces"""
 
@@ -432,15 +417,15 @@
         surfaces = [None] * n_frames
         for t in range(n_frames):
 
             # Find points with correct frame index
             _points = points[points[:, 0] == t, 1:]
 
             # Get parts of faces array that correspond to this frame
-            _faces = faces[idx_face_new_frame[t] : idx_face_new_frame[t+1]] - sum(points_per_frame[:t])
+            _faces = faces[idx_face_new_frame[t] : idx_face_new_frame[t + 1]] - sum(points_per_frame[:t])
 
             # Get values that correspond to this frame
             if has_values:
                 _values = values[points[:, 0] == t]
             else:
                 _values = np.ones(len(_points))
 
@@ -477,35 +462,33 @@
         faces = np.vstack(faces)
 
         if values is None:
             return (vertices, faces)
         else:
             return (vertices, faces, values)
 
-
     # =============================================================================
     # Points
     # =============================================================================
 
     def _list_of_points_to_points(self, points: list) -> np.ndarray:
         """Convert list of 3D point data to single 4D point data."""
         n_frames = len(points)
         n_points = sum([len(frame) for frame in points])
-        if n_frames > 1: # actually a timelapse
+        if n_frames > 1:  # actually a timelapse
             t = np.concatenate([[idx] * len(frame) for idx, frame in enumerate(points)])
 
             points_out = np.zeros((n_points, 4))
             points_out[:, 1:] = np.vstack(points)
             points_out[:, 0] = t
         else:
             points_out = np.vstack(points)
 
         return points_out
 
-
     def _points_to_list_of_points(self, points: PointsData) -> list:
         """Convert a 4D point array to list of 3D points"""
 
         while points.shape[1] < 4:
             t = np.zeros(len(points), dtype=points.dtype)
             points = np.insert(points, 0, t, axis=1)
```

### Comparing `napari_stress-0.2.4/src/napari_stress/_vectors.py` & `napari_stress-0.2.5/src/napari_stress/_vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     Returns:
         napari.types.VectorsData: Normal vectors
     """
     import vedo
 
     pointcloud = vedo.pointcloud.Points(points)
-    center_of_mass = pointcloud.centerOfMass()
+    center_of_mass = pointcloud.center_of_mass()
     pointcloud.compute_normals_with_pca(orientation_point=center_of_mass)
 
     normals = pointcloud.pointdata["Normals"]
     normals = np.stack([points, normals]).transpose((1, 0, 2))
 
     return normals
```

### Comparing `napari_stress-0.2.4/src/napari_stress/napari.yaml` & `napari_stress-0.2.5/src/napari_stress/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress/types.py` & `napari_stress-0.2.5/src/napari_stress/types.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.4/src/napari_stress.egg-info/PKG-INFO` & `napari_stress-0.2.5/src/napari_stress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stress
-Version: 0.2.4
+Version: 0.2.5
 Summary: Interactive surface analysis in napari for measuring mechanical stresses in biological tissues
 Author: Johannes Soltwedel, Ben J. Gross, Elijah Shelton, Carlos Gomez, Otger Campas
 Author-email: johannes_richard.mueller@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/campaslab/napari-stress/issues
 Project-URL: Documentation, https://campaslab.github.io/napari-stress
 Project-URL: Source Code, https://github.com/campaslab/napari-stress
```

### Comparing `napari_stress-0.2.4/src/napari_stress.egg-info/SOURCES.txt` & `napari_stress-0.2.5/src/napari_stress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

