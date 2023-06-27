# Comparing `tmp/gpm_api-0.2.2.tar.gz` & `tmp/gpm_api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpm_api-0.2.2.tar", last modified: Tue Jun 27 10:24:09 2023, max compression
+gzip compressed data, was "gpm_api-0.2.3.tar", last modified: Mon Mar 20 16:38:47 2023, max compression
```

## Comparing `gpm_api-0.2.2.tar` & `gpm_api-0.2.3.tar`

### file list

```diff
@@ -1,120 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.451550 gpm_api-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-27 10:23:56.000000 gpm_api-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-27 10:23:56.000000 gpm_api-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-27 10:23:56.000000 gpm_api-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-27 10:23:56.000000 gpm_api-0.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 10:23:56.000000 gpm_api-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-27 10:23:56.000000 gpm_api-0.2.2/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 10:23:56.000000 gpm_api-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 10:23:56.000000 gpm_api-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-06-27 10:24:09.451550 gpm_api-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-27 10:23:56.000000 gpm_api-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.435550 gpm_api-0.2.2/gpm_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 10:24:09.000000 gpm_api-0.2.2/gpm_api/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.435550 gpm_api-0.2.2/gpm_api/accessor/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/accessor/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.435550 gpm_api-0.2.2/gpm_api/bucket/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/bucket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/bucket/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.439550 gpm_api-0.2.2/gpm_api/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/dataset/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/dataset/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/dataset/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/dataset/decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/dataset/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/dataset/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22100 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/dataset/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.439550 gpm_api-0.2.2/gpm_api/etc/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/etc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/etc/country_acronyms.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/etc/country_bounds.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/etc/country_extent.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.439550 gpm_api-0.2.2/gpm_api/io/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)    27280 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/pps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/products.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/io/scan_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.439550 gpm_api-0.2.2/gpm_api/overpass/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/overpass/TODO_GPM_OVERPASS.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/overpass/TODO_OVERPASS_STATS.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/overpass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.443549 gpm_api-0.2.2/gpm_api/patch/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/patch/image_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    20347 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/patch/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/patch/labels_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/patch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.443549 gpm_api-0.2.2/gpm_api/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/scripts/download_daily_gpm_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/scripts/download_monthly_gpm_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.447550 gpm_api-0.2.2/gpm_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/__init__
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.447550 gpm_api-0.2.2/gpm_api/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/io/test_00_24_granules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/io/test_GPM_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/io/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/io/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/io/test_find_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_crs_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_dataset_regularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_dataset_valid_geolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_image_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_image_labels_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_plot_multiorbit_gmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_plot_multiorbit_pmw_polar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_plot_orbit_pmw_custom_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_pmw_channel_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_pps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/tests/test_unvalid_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.447550 gpm_api-0.2.2/gpm_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/area.py
--rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/continents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/geospatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/utils_HDF5.py
--rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/utils_cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/utils_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/utils/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.451550 gpm_api-0.2.2/gpm_api/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/visualization/OLD_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/visualization/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/visualization/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/visualization/orbit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/visualization/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/visualization/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-27 10:23:56.000000 gpm_api-0.2.2/gpm_api/visualization/title.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:24:09.435550 gpm_api-0.2.2/gpm_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-06-27 10:24:09.000000 gpm_api-0.2.2/gpm_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-27 10:24:09.000000 gpm_api-0.2.2/gpm_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:24:09.000000 gpm_api-0.2.2/gpm_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-27 10:24:09.000000 gpm_api-0.2.2/gpm_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-27 10:24:09.000000 gpm_api-0.2.2/gpm_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 10:24:09.000000 gpm_api-0.2.2/gpm_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-27 10:23:56.000000 gpm_api-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:24:09.451550 gpm_api-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 10:23:56.000000 gpm_api-0.2.2/setup.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.540668 gpm_api-0.2.3/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      426 2023-01-10 16:54:13.000000 gpm_api-0.2.3/.flake8
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2245 2023-03-20 15:40:03.000000 gpm_api-0.2.3/.gitignore
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1469 2023-01-10 16:53:38.000000 gpm_api-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      296 2023-01-10 16:18:06.000000 gpm_api-0.2.3/.prospector.yaml
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      607 2023-01-10 16:15:28.000000 gpm_api-0.2.3/.readthedocs.yml
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      379 2023-01-10 10:59:57.000000 gpm_api-0.2.3/AUTHORS.md
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      262 2023-01-10 11:04:08.000000 gpm_api-0.2.3/CHANGELOG.md
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      376 2023-01-10 11:07:49.000000 gpm_api-0.2.3/CITATION.bib
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1071 2023-01-11 11:18:26.000000 gpm_api-0.2.3/LICENSE
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)       50 2023-03-09 16:06:33.000000 gpm_api-0.2.3/MANIFEST.in
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    12447 2023-03-20 16:38:47.540668 gpm_api-0.2.3/PKG-INFO
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)     9425 2023-03-20 16:31:47.000000 gpm_api-0.2.3/README.md
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.532667 gpm_api-0.2.3/gpm_api/
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)     1401 2023-03-20 08:32:18.000000 gpm_api-0.2.3/gpm_api/__init__.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      160 2023-03-20 16:38:47.000000 gpm_api-0.2.3/gpm_api/_version.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.532667 gpm_api-0.2.3/gpm_api/accessor/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      174 2022-12-09 17:33:33.000000 gpm_api-0.2.3/gpm_api/accessor/__init__.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    14757 2023-03-20 08:32:18.000000 gpm_api-0.2.3/gpm_api/accessor/methods.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     3777 2023-03-20 08:32:18.000000 gpm_api-0.2.3/gpm_api/configs.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.532667 gpm_api-0.2.3/gpm_api/dataset/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    26189 2023-03-09 16:06:33.000000 gpm_api-0.2.3/gpm_api/dataset/crs.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     7249 2023-03-02 12:53:24.000000 gpm_api-0.2.3/gpm_api/dataset/decoding.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    37729 2023-03-20 09:24:36.000000 gpm_api-0.2.3/gpm_api/dataset/reader.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.532667 gpm_api-0.2.3/gpm_api/etc/
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)      109 2023-03-08 09:55:29.000000 gpm_api-0.2.3/gpm_api/etc/__init__.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2269 2022-12-10 15:14:42.000000 gpm_api-0.2.3/gpm_api/etc/country_acronyms.yaml
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    15062 2022-12-10 15:20:09.000000 gpm_api-0.2.3/gpm_api/etc/country_bounds.yaml
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    15062 2022-12-10 15:20:09.000000 gpm_api-0.2.3/gpm_api/etc/country_extent.yaml
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.536667 gpm_api-0.2.3/gpm_api/io/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      143 2023-03-08 10:01:55.000000 gpm_api-0.2.3/gpm_api/io/__init__.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     7156 2023-01-04 21:00:12.000000 gpm_api-0.2.3/gpm_api/io/checks.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    14480 2023-01-04 23:34:53.000000 gpm_api-0.2.3/gpm_api/io/directories.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     7964 2023-03-20 08:32:18.000000 gpm_api-0.2.3/gpm_api/io/disk.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    28890 2023-03-20 08:32:18.000000 gpm_api-0.2.3/gpm_api/io/download.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    10400 2022-12-09 17:33:34.000000 gpm_api-0.2.3/gpm_api/io/filter.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     6052 2022-12-09 23:14:49.000000 gpm_api-0.2.3/gpm_api/io/info.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    12920 2022-12-10 19:54:21.000000 gpm_api-0.2.3/gpm_api/io/patterns.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    10804 2023-03-20 08:32:18.000000 gpm_api-0.2.3/gpm_api/io/pps.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     9802 2022-12-09 17:33:34.000000 gpm_api-0.2.3/gpm_api/io/products.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     3717 2023-01-16 22:06:32.000000 gpm_api-0.2.3/gpm_api/io/scan_modes.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.536667 gpm_api-0.2.3/gpm_api/overpass/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     3754 2022-12-09 17:33:34.000000 gpm_api-0.2.3/gpm_api/overpass/TODO_GPM_OVERPASS.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     5994 2022-12-09 17:33:34.000000 gpm_api-0.2.3/gpm_api/overpass/TODO_OVERPASS_STATS.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      108 2022-08-14 22:17:13.000000 gpm_api-0.2.3/gpm_api/overpass/__init__.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.536667 gpm_api-0.2.3/gpm_api/patch/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      108 2022-08-14 22:17:13.000000 gpm_api-0.2.3/gpm_api/patch/__init__.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1797 2023-01-15 13:47:14.000000 gpm_api-0.2.3/gpm_api/patch/image_patch.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    14959 2023-01-19 15:13:14.000000 gpm_api-0.2.3/gpm_api/patch/labels.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    11499 2023-01-16 16:56:44.000000 gpm_api-0.2.3/gpm_api/patch/labels_patch.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    11959 2023-01-15 15:29:02.000000 gpm_api-0.2.3/gpm_api/patch/utils.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.536667 gpm_api-0.2.3/gpm_api/scripts/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2412 2023-03-20 16:01:49.000000 gpm_api-0.2.3/gpm_api/scripts/download_daily_gpm_data.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2364 2023-03-20 08:32:18.000000 gpm_api-0.2.3/gpm_api/scripts/download_monthly_gpm_data.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.540668 gpm_api-0.2.3/gpm_api/tests/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      108 2022-12-09 11:42:05.000000 gpm_api-0.2.3/gpm_api/tests/__init__
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1423 2022-11-01 14:15:04.000000 gpm_api-0.2.3/gpm_api/tests/info.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.540668 gpm_api-0.2.3/gpm_api/tests/io/
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)     4298 2022-10-13 13:08:58.000000 gpm_api-0.2.3/gpm_api/tests/io/test_00_24_granules.py
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)     2036 2022-10-13 13:14:59.000000 gpm_api-0.2.3/gpm_api/tests/io/test_GPM_products.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     6852 2022-10-13 21:10:14.000000 gpm_api-0.2.3/gpm_api/tests/io/test_dataset.py
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)     2886 2022-10-13 20:58:32.000000 gpm_api-0.2.3/gpm_api/tests/io/test_downloads.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2377 2022-10-13 20:36:12.000000 gpm_api-0.2.3/gpm_api/tests/io/test_find_filters.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1769 2023-02-06 08:39:42.000000 gpm_api-0.2.3/gpm_api/tests/test_archive.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     3169 2023-03-08 10:10:01.000000 gpm_api-0.2.3/gpm_api/tests/test_crs_cf.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      619 2023-03-08 09:55:14.000000 gpm_api-0.2.3/gpm_api/tests/test_dataset.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2781 2023-01-04 23:28:47.000000 gpm_api-0.2.3/gpm_api/tests/test_dataset_regularity.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1934 2023-01-04 23:45:11.000000 gpm_api-0.2.3/gpm_api/tests/test_dataset_valid_geolocation.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1332 2022-12-09 15:53:22.000000 gpm_api-0.2.3/gpm_api/tests/test_disk.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     9253 2022-12-10 14:05:51.000000 gpm_api-0.2.3/gpm_api/tests/test_download.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1734 2022-12-10 13:47:00.000000 gpm_api-0.2.3/gpm_api/tests/test_filter.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     4327 2023-01-12 11:41:58.000000 gpm_api-0.2.3/gpm_api/tests/test_image_labels.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     3179 2023-01-15 15:27:28.000000 gpm_api-0.2.3/gpm_api/tests/test_image_labels_patch.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      563 2022-12-09 11:42:05.000000 gpm_api-0.2.3/gpm_api/tests/test_io.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      442 2022-12-10 19:23:23.000000 gpm_api-0.2.3/gpm_api/tests/test_plot.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2830 2023-01-04 23:26:47.000000 gpm_api-0.2.3/gpm_api/tests/test_plot_multiorbit_gmi.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1965 2023-01-09 19:44:37.000000 gpm_api-0.2.3/gpm_api/tests/test_plot_multiorbit_pmw_polar.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2214 2023-01-09 21:03:45.000000 gpm_api-0.2.3/gpm_api/tests/test_plot_orbit_pmw_custom_kwargs.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1442 2023-01-05 17:31:52.000000 gpm_api-0.2.3/gpm_api/tests/test_pmw_channel_coords.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2393 2022-12-10 13:50:49.000000 gpm_api-0.2.3/gpm_api/tests/test_pps.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2013 2023-03-02 12:53:24.000000 gpm_api-0.2.3/gpm_api/tests/test_unvalid_coordinates.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.540668 gpm_api-0.2.3/gpm_api/utils/
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)      108 2022-12-09 17:33:34.000000 gpm_api-0.2.3/gpm_api/utils/__init__.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    22943 2023-03-20 08:32:18.000000 gpm_api-0.2.3/gpm_api/utils/archive.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     8476 2023-01-09 19:45:27.000000 gpm_api-0.2.3/gpm_api/utils/area.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    37037 2023-03-02 12:53:24.000000 gpm_api-0.2.3/gpm_api/utils/checks.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     1928 2023-01-16 20:59:52.000000 gpm_api-0.2.3/gpm_api/utils/continents.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2789 2023-01-16 20:04:14.000000 gpm_api-0.2.3/gpm_api/utils/countries.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     8655 2023-03-09 16:06:33.000000 gpm_api-0.2.3/gpm_api/utils/geospatial.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    15246 2023-03-02 12:53:24.000000 gpm_api-0.2.3/gpm_api/utils/slices.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     6960 2023-01-05 00:34:44.000000 gpm_api-0.2.3/gpm_api/utils/time.py
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)     9614 2023-01-11 09:08:00.000000 gpm_api-0.2.3/gpm_api/utils/utils_HDF5.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    22720 2023-01-16 21:39:36.000000 gpm_api-0.2.3/gpm_api/utils/utils_cmap.py
+-rwxr-xr-x   0 ghiggi   (125850) lte      (20185)     7279 2022-12-09 17:33:34.000000 gpm_api-0.2.3/gpm_api/utils/utils_string.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      259 2023-01-19 15:13:14.000000 gpm_api-0.2.3/gpm_api/utils/warnings.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      439 2022-12-10 19:54:21.000000 gpm_api-0.2.3/gpm_api/utils/xarray.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.540668 gpm_api-0.2.3/gpm_api/visualization/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     6684 2022-12-09 17:33:34.000000 gpm_api-0.2.3/gpm_api/visualization/OLD_comparison.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      108 2022-09-09 10:14:47.000000 gpm_api-0.2.3/gpm_api/visualization/__init__.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     5865 2023-01-19 15:13:14.000000 gpm_api-0.2.3/gpm_api/visualization/grid.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     5401 2023-01-16 16:57:07.000000 gpm_api-0.2.3/gpm_api/visualization/labels.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     8474 2023-03-02 12:53:24.000000 gpm_api-0.2.3/gpm_api/visualization/orbit.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    16214 2023-01-16 21:46:32.000000 gpm_api-0.2.3/gpm_api/visualization/plot.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     9477 2022-12-10 19:54:21.000000 gpm_api-0.2.3/gpm_api/visualization/profile.py
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     4216 2022-12-10 19:54:21.000000 gpm_api-0.2.3/gpm_api/visualization/title.py
+drwxr-xr-x   0 ghiggi   (125850) lte      (20185)        0 2023-03-20 16:38:47.532667 gpm_api-0.2.3/gpm_api.egg-info/
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)    12447 2023-03-20 16:38:47.000000 gpm_api-0.2.3/gpm_api.egg-info/PKG-INFO
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     2733 2023-03-20 16:38:47.000000 gpm_api-0.2.3/gpm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)        1 2023-03-20 16:38:47.000000 gpm_api-0.2.3/gpm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      204 2023-03-20 16:38:47.000000 gpm_api-0.2.3/gpm_api.egg-info/entry_points.txt
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)      340 2023-03-20 16:38:47.000000 gpm_api-0.2.3/gpm_api.egg-info/requires.txt
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)        8 2023-03-20 16:38:47.000000 gpm_api-0.2.3/gpm_api.egg-info/top_level.txt
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)     4224 2023-03-20 08:32:18.000000 gpm_api-0.2.3/pyproject.toml
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)       38 2023-03-20 16:38:47.540668 gpm_api-0.2.3/setup.cfg
+-rw-r--r--   0 ghiggi   (125850) lte      (20185)       87 2023-01-10 15:50:35.000000 gpm_api-0.2.3/setup.py
```

### Comparing `gpm_api-0.2.2/.gitignore` & `gpm_api-0.2.3/.gitignore`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
 _version.py
 gpm_api/_version.py
 
-
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
 # Installer logs
@@ -150,7 +149,8 @@
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 train_interactive.py
 tmp_fig.py
 log.txt
+
```

### Comparing `gpm_api-0.2.2/LICENSE` & `gpm_api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.2/PKG-INFO` & `gpm_api-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpm_api
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python API for the Global Precipitation Mission Data Archive
 Author-email: Gionata Ghiggi <gionata.ghiggi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2023 Gionata Ghiggi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,131 +53,133 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: image
 Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: tests
 License-File: LICENSE
 
 # Welcome to GPM-API
 [![DOI](https://zenodo.org/badge/286664485.svg)](https://zenodo.org/badge/latestdoi/286664485)
 [![PyPI version](https://badge.fury.io/py/gpm_api.svg)](https://badge.fury.io/py/gpm_api)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gpm_api.svg)](https://anaconda.org/conda-forge/gpm_api)
-[![Tests](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml/badge.svg)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml)
+[![Build Status](https://github.com/ghiggi/gpm_api/workflows/Continuous%20Integration/badge.svg?branch=main)](https://github.com/ghiggi/gpm_api/actions)
 [![Coverage Status](https://coveralls.io/repos/github/ghiggi/gpm_api/badge.svg?branch=main)](https://coveralls.io/github/ghiggi/gpm_api?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/gpm_api/badge/?version=latest)](https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/?badge=stable)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![License](https://img.shields.io/github/license/ghiggi/gpm_api)](https://github.com/ghiggi/gpm_api/blob/master/LICENSE)
 
 The GPM-API is still in development. Feel free to try it out and to report issues or to suggest changes.
 
 ## Quick start
-GPM-API provides an easy-to-use python interface to download, read, process and visualize most
-of the products of the Global Precipitation Measurement Mission (GPM) data archive.
+GPM-API provides an easy-to-use python interface to download, read, process and visualize most 
+of the products of the Global Precipitation Measurement Mission (GPM) data archive. 
 
-The list of available products can be retrieved using:
+The list of available products can be retrieved using: 
 
 ```python
 import gpm_api
 
 gpm_api.available_products(product_type="RS")  # research products
 gpm_api.available_products(product_type="NRT") # near-real-time products
 
 ```
 
-Before starting using GPM-API, we highly suggest to save into a configuration file:
-1. your credentials to access the [NASA Precipitation Processing System (PPS) servers][PPS_link]
-2. the directory on the local disk where to save the GPM dataset of interest.
+Before starting using GPM-API, we highly suggest to save into a configuration file: 
+1. your credentials to access the [NASA Precipitation Processing System (PPS) servers][PPS_link] 
+2. the directory on the local disk where to save the GPM dataset of interest. 
 
-To facilitate the creation of the configuration file, you can run the following script:
+To facilitate the creation of the configuration file, you can run the following script: 
 
 ```python
 import gpm_api
 
-username = "<your PPS username>" # likely your mail
-password = "<your PPS password>" # likely your mail
+username = "<your PPS username>" # likely your mail 
+password = "<your PPS password>" # likely your mail 
 gpm_base_dir = "<path/to/directory/GPM"  # path to the directory where to download the data
-gpm_api.define_configs(gpm_username=username,
-                       gpm_password=password,
+gpm_api.define_configs(gpm_username=username, 
+                       gpm_password=password, 
                        gpm_base_dir=gpm_base_dir)
 
 # You can check that the config file has been correctly created with:
 configs = gpm_api.read_configs()
 print(configs)
 
 ```
 
-Now you can either start to download GPM data within python:
+Now you can either start to download GPM data within python: 
 
 ```python
 import gpm_api
-import datetime
+import datetime 
 
 product = "2A-DPR"
 product_type = "RS"
 version = 7
 
 start_time = datetime.datetime(2020,7, 22, 0, 1, 11)
 end_time = datetime.datetime(2020,7, 22, 0, 23, 5)
 
-gpm_api.download(product=product,
+gpm_api.download(product=product, 
                  product_type=product_type,
                  version=version,
                  n_threads=2,
-                 start_time=start_time,
+                 start_time=start_time, 
                  end_time=end_time)
 
 ```
 
 or from the terminal using i.e. `download_daily_gpm_data <product> <year> <month> <day>`:
 
 ```bash
     download_daily_gpm_data 2A-DPR 2022 7 22
 ```
 
-A GPM granule can be opened in python using:
+A GPM granule can be opened in python using: 
 
 ```python
 import gpm_api
 
 ds = gpm_api.open_granule(<path_to_granule>)
 
 ```
 
-while multiple granules over a specific time period can be opened using:
+while multiple granules over a specific time period can be opened using: 
 
 ```python
 import gpm_api
-import datetime
+import datetime 
 
 product = "2A-DPR"
 product_type = "RS"
 version = 7
 
 start_time = datetime.datetime(2020,7, 22, 0, 1, 11)
 end_time = datetime.datetime(2020,7, 22, 0, 23, 5)
-ds = gpm_api.open_dataset(product=product,
+ds = gpm_api.open_dataset(product=product, 
                           product_type=product_type,
                           version=version
-                          start_time=start_time,
+                          start_time=start_time, 
                           end_time=end_time)
 ```
 
 Look at the [Tutorials][tutorial_link] to learn how to analyse and visualize the GPM products !
 
 ## Installation
 
 
 ### pip
 
 GPM-API can be installed via [pip][pip_link] on Linux, Mac, and Windows.
 On Windows you can install [WinPython][winpy_link] to get Python and pip
 running.
-Prior installation of GPM-API, to avoid [GEOS](https://libgeos.org/) library version incompatibilities when
+Prior installation of GPM-API, to avoid [GEOS](https://libgeos.org/) library version incompatibilities when 
 installing the Cartopy package, we highly suggest to install first Cartopy using `conda install cartopy>=0.21.0`.
 
 Then, install the GPM-API package by typing the following command in the command terminal:
 
     pip install gpm_api
 
 To install the latest development version via pip, see the
@@ -209,15 +211,15 @@
 - 2. Introduction to the PMW 2A products [[Notebook][tut2_pmw2a_link]][[Colab][colab2_pmw2a_link]]
 - 2. Introduction to the RADAR 2A products [[Notebook][tut2_radar_2a_link]][[Colab][colab2_radar_2a_link]]
 - 2. Introduction to the CORRA 2B products [[Notebook][tut2_corra_2b_link]][[Colab][colab2_corra_2b_link]]
 - 2. Introduction to the Latent Heating products [[Notebook][tut2_lh_link]][[Colab][colab2_lh_link]]
 - 2. Introduction to the ENVironment products [[Notebook][tut2_env_link]][[Colab][colab2_env_link]]
 - 3. Introduction to image labeling and patch extraction [[Notebook][tut3_label_link]][[Colab][colab3_label_link]]
 - 3. Introduction to image patch extraction [[Notebook][tut3_patch_link]][[Colab][colab3_patch_link]]
-
+ 
 The associated python scripts are also provided in the `tutorial` folder.
 
 ## Citation
 
 If you are using GPM-API in your publication please cite our paper:
 
 TODO: GMD
@@ -242,26 +244,29 @@
 
 - [zarr](https://zarr.readthedocs.io/en/stable/)
 - [dask_image](https://image.dask.org/en/latest/)
 - [skimage](https://scikit-image.org/)
 
 ## License
 
-The content of this repository is released under the terms of the [MIT](LICENSE) license.
+[MIT][license_link] © 2021-2023
+
 
 [PPS_link]: https://gpm.nasa.gov/data/sources/pps-research
 [tutorial_link]: https://github.com/ghiggi/gpm_api/tree/master#tutorials-and-examples
 
 [pip_link]: https://pypi.org/project/gstools
 [conda_link]: https://docs.conda.io/en/latest/miniconda.html
 [conda_forge_link]: https://github.com/conda-forge/gpm_api-feedstock#installing-gpm_api
 [conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
 [pipiflag]: https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html?highlight=i#cmdoption-i
 [winpy_link]: https://winpython.github.io/
 
+[license_link]: https://github.com/ghiggi/gpm_api/blob/main/LICENSE
+ 
 [doc_link]: https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/
 [doc_install_link]: https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/#pip
 
 [tut1_download_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab1_download_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut2_imerg_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
@@ -286,7 +291,9 @@
 [colab2_env_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut3_label_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab3_label_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut3_patch_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab3_patch_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
+ 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpm_api-0.2.2/README.md` & `gpm_api-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,122 +1,122 @@
 # Welcome to GPM-API
 [![DOI](https://zenodo.org/badge/286664485.svg)](https://zenodo.org/badge/latestdoi/286664485)
 [![PyPI version](https://badge.fury.io/py/gpm_api.svg)](https://badge.fury.io/py/gpm_api)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gpm_api.svg)](https://anaconda.org/conda-forge/gpm_api)
-[![Tests](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml/badge.svg)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml)
+[![Build Status](https://github.com/ghiggi/gpm_api/workflows/Continuous%20Integration/badge.svg?branch=main)](https://github.com/ghiggi/gpm_api/actions)
 [![Coverage Status](https://coveralls.io/repos/github/ghiggi/gpm_api/badge.svg?branch=main)](https://coveralls.io/github/ghiggi/gpm_api?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/gpm_api/badge/?version=latest)](https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/?badge=stable)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![License](https://img.shields.io/github/license/ghiggi/gpm_api)](https://github.com/ghiggi/gpm_api/blob/master/LICENSE)
 
 The GPM-API is still in development. Feel free to try it out and to report issues or to suggest changes.
 
 ## Quick start
-GPM-API provides an easy-to-use python interface to download, read, process and visualize most
-of the products of the Global Precipitation Measurement Mission (GPM) data archive.
+GPM-API provides an easy-to-use python interface to download, read, process and visualize most 
+of the products of the Global Precipitation Measurement Mission (GPM) data archive. 
 
-The list of available products can be retrieved using:
+The list of available products can be retrieved using: 
 
 ```python
 import gpm_api
 
 gpm_api.available_products(product_type="RS")  # research products
 gpm_api.available_products(product_type="NRT") # near-real-time products
 
 ```
 
-Before starting using GPM-API, we highly suggest to save into a configuration file:
-1. your credentials to access the [NASA Precipitation Processing System (PPS) servers][PPS_link]
-2. the directory on the local disk where to save the GPM dataset of interest.
+Before starting using GPM-API, we highly suggest to save into a configuration file: 
+1. your credentials to access the [NASA Precipitation Processing System (PPS) servers][PPS_link] 
+2. the directory on the local disk where to save the GPM dataset of interest. 
 
-To facilitate the creation of the configuration file, you can run the following script:
+To facilitate the creation of the configuration file, you can run the following script: 
 
 ```python
 import gpm_api
 
-username = "<your PPS username>" # likely your mail
-password = "<your PPS password>" # likely your mail
+username = "<your PPS username>" # likely your mail 
+password = "<your PPS password>" # likely your mail 
 gpm_base_dir = "<path/to/directory/GPM"  # path to the directory where to download the data
-gpm_api.define_configs(gpm_username=username,
-                       gpm_password=password,
+gpm_api.define_configs(gpm_username=username, 
+                       gpm_password=password, 
                        gpm_base_dir=gpm_base_dir)
 
 # You can check that the config file has been correctly created with:
 configs = gpm_api.read_configs()
 print(configs)
 
 ```
 
-Now you can either start to download GPM data within python:
+Now you can either start to download GPM data within python: 
 
 ```python
 import gpm_api
-import datetime
+import datetime 
 
 product = "2A-DPR"
 product_type = "RS"
 version = 7
 
 start_time = datetime.datetime(2020,7, 22, 0, 1, 11)
 end_time = datetime.datetime(2020,7, 22, 0, 23, 5)
 
-gpm_api.download(product=product,
+gpm_api.download(product=product, 
                  product_type=product_type,
                  version=version,
                  n_threads=2,
-                 start_time=start_time,
+                 start_time=start_time, 
                  end_time=end_time)
 
 ```
 
 or from the terminal using i.e. `download_daily_gpm_data <product> <year> <month> <day>`:
 
 ```bash
     download_daily_gpm_data 2A-DPR 2022 7 22
 ```
 
-A GPM granule can be opened in python using:
+A GPM granule can be opened in python using: 
 
 ```python
 import gpm_api
 
 ds = gpm_api.open_granule(<path_to_granule>)
 
 ```
 
-while multiple granules over a specific time period can be opened using:
+while multiple granules over a specific time period can be opened using: 
 
 ```python
 import gpm_api
-import datetime
+import datetime 
 
 product = "2A-DPR"
 product_type = "RS"
 version = 7
 
 start_time = datetime.datetime(2020,7, 22, 0, 1, 11)
 end_time = datetime.datetime(2020,7, 22, 0, 23, 5)
-ds = gpm_api.open_dataset(product=product,
+ds = gpm_api.open_dataset(product=product, 
                           product_type=product_type,
                           version=version
-                          start_time=start_time,
+                          start_time=start_time, 
                           end_time=end_time)
 ```
 
 Look at the [Tutorials][tutorial_link] to learn how to analyse and visualize the GPM products !
 
 ## Installation
 
 
 ### pip
 
 GPM-API can be installed via [pip][pip_link] on Linux, Mac, and Windows.
 On Windows you can install [WinPython][winpy_link] to get Python and pip
 running.
-Prior installation of GPM-API, to avoid [GEOS](https://libgeos.org/) library version incompatibilities when
+Prior installation of GPM-API, to avoid [GEOS](https://libgeos.org/) library version incompatibilities when 
 installing the Cartopy package, we highly suggest to install first Cartopy using `conda install cartopy>=0.21.0`.
 
 Then, install the GPM-API package by typing the following command in the command terminal:
 
     pip install gpm_api
 
 To install the latest development version via pip, see the
@@ -148,15 +148,15 @@
 - 2. Introduction to the PMW 2A products [[Notebook][tut2_pmw2a_link]][[Colab][colab2_pmw2a_link]]
 - 2. Introduction to the RADAR 2A products [[Notebook][tut2_radar_2a_link]][[Colab][colab2_radar_2a_link]]
 - 2. Introduction to the CORRA 2B products [[Notebook][tut2_corra_2b_link]][[Colab][colab2_corra_2b_link]]
 - 2. Introduction to the Latent Heating products [[Notebook][tut2_lh_link]][[Colab][colab2_lh_link]]
 - 2. Introduction to the ENVironment products [[Notebook][tut2_env_link]][[Colab][colab2_env_link]]
 - 3. Introduction to image labeling and patch extraction [[Notebook][tut3_label_link]][[Colab][colab3_label_link]]
 - 3. Introduction to image patch extraction [[Notebook][tut3_patch_link]][[Colab][colab3_patch_link]]
-
+ 
 The associated python scripts are also provided in the `tutorial` folder.
 
 ## Citation
 
 If you are using GPM-API in your publication please cite our paper:
 
 TODO: GMD
@@ -181,26 +181,29 @@
 
 - [zarr](https://zarr.readthedocs.io/en/stable/)
 - [dask_image](https://image.dask.org/en/latest/)
 - [skimage](https://scikit-image.org/)
 
 ## License
 
-The content of this repository is released under the terms of the [MIT](LICENSE) license.
+[MIT][license_link] © 2021-2023
+
 
 [PPS_link]: https://gpm.nasa.gov/data/sources/pps-research
 [tutorial_link]: https://github.com/ghiggi/gpm_api/tree/master#tutorials-and-examples
 
 [pip_link]: https://pypi.org/project/gstools
 [conda_link]: https://docs.conda.io/en/latest/miniconda.html
 [conda_forge_link]: https://github.com/conda-forge/gpm_api-feedstock#installing-gpm_api
 [conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
 [pipiflag]: https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html?highlight=i#cmdoption-i
 [winpy_link]: https://winpython.github.io/
 
+[license_link]: https://github.com/ghiggi/gpm_api/blob/main/LICENSE
+ 
 [doc_link]: https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/
 [doc_install_link]: https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/#pip
 
 [tut1_download_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab1_download_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut2_imerg_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
@@ -225,7 +228,9 @@
 [colab2_env_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut3_label_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab3_label_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut3_patch_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab3_patch_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
+ 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpm_api-0.2.2/gpm_api/__init__.py` & `gpm_api-0.2.3/gpm_api/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Mon Aug  3 11:22:04 2020
 
 @author: ghiggi
 """
-# import os
-# os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"  # noqa
-import gpm_api.accessor  # noqa
-from importlib.metadata import PackageNotFoundError, version
-
+import os 
+os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"
+import gpm_api.accessor  # .methods
+from importlib.metadata import version, PackageNotFoundError
 from gpm_api.configs import define_gpm_api_configs as define_configs
 from gpm_api.configs import read_gpm_api_configs as read_configs
+
+from gpm_api.io.download import download_data as download
 from gpm_api.dataset.reader import (
-    open_dataset,
     open_granule,
+    open_dataset,
 )
 from gpm_api.io.disk import find_filepaths as find_files
-from gpm_api.io.download import download_data as download
-from gpm_api.io.products import available_products
-from gpm_api.io.scan_modes import available_scan_modes
-from gpm_api.utils.archive import download_daily_data, download_monthly_data
 from gpm_api.utils.checks import (
-    check_contiguous_scans,
-    check_missing_granules,
     check_regular_time,
+    check_contiguous_scans,
     check_valid_geolocation,
+    check_missing_granules,
 )
+from gpm_api.io.products import available_products
+from gpm_api.io.scan_modes import available_scan_modes
+from gpm_api.utils.archive import download_daily_data, download_monthly_data
 
 __all__ = [
     "define_configs",
     "read_configs",
     "available_products",
     "available_scan_modes",
     "download",
-    "download_daily_data",
+    "download_daily_data", 
     "download_monthly_data",
     "find_files",
     "open_granule",
     "open_dataset",
     "check_regular_time",
     "check_contiguous_scans",
     "check_valid_geolocation",
```

### Comparing `gpm_api-0.2.2/gpm_api/accessor/methods.py` & `gpm_api-0.2.3/gpm_api/accessor/methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Wed Aug 17 09:31:39 2022
 
 @author: ghiggi
 """
 import numpy as np
 import xarray as xr
@@ -23,39 +24,39 @@
         return crop(self._obj, extent)
 
     def crop_by_country(self, name):
         """Crop xarray object by country name."""
         from gpm_api.utils.geospatial import crop_by_country
 
         return crop_by_country(self._obj, name)
-
+    
     def crop_by_continent(self, name):
         """Crop xarray object by continent name."""
         from gpm_api.utils.geospatial import crop_by_continent
 
         return crop_by_continent(self._obj, name)
-
+    
     def get_crop_slices_by_extent(self, extent):
         """Get subsetting slices given the extent."""
         from gpm_api.utils.geospatial import get_crop_slices_by_extent
 
         return get_crop_slices_by_extent(self._obj, extent)
-
+    
     def get_crop_slices_by_country(self, name):
         """Get subsetting slices given the country name."""
         from gpm_api.utils.geospatial import get_crop_slices_by_country
 
         return get_crop_slices_by_country(self._obj, name)
-
+    
     def get_crop_slices_by_continent(self, name):
         """Get subsetting slices given the continent name."""
         from gpm_api.utils.geospatial import get_crop_slices_by_continent
 
         return get_crop_slices_by_continent(self._obj, name)
-
+    
     @property
     def pyresample_area(self):
         from gpm_api.utils.geospatial import get_pyresample_area
 
         return get_pyresample_area(self._obj)
 
     @property
@@ -89,47 +90,47 @@
         return has_regular_time(self._obj)
 
     @property
     def has_contiguous_scans(self):
         from gpm_api.utils.checks import has_contiguous_scans
 
         return has_contiguous_scans(self._obj)
-
+    
     @property
     def has_missing_granules(self):
         from gpm_api.utils.checks import has_missing_granules
 
         return has_missing_granules(self._obj)
 
     @property
     def has_valid_geolocation(self):
         from gpm_api.utils.checks import has_valid_geolocation
 
         return has_valid_geolocation(self._obj)
-
+    
     @property
-    def start_time(self):
+    def start_time(self): 
         if "time" in self._obj.coords:
-            start_time = self._obj["time"].values[0]
+            start_time = self._obj["time"].values[0] 
         elif "gpm_time" in self._obj.coords:
-            start_time = self._obj["gpm_time"].values[0]
-        else:
+            start_time = self._obj["gpm_time"].values[0] 
+        else: 
             raise ValueError("Time coordinate not found")
-        return start_time
-
+        return start_time 
+    
     @property
     def end_time(self):
         if "time" in self._obj.coords:
-            end_time = self._obj["time"].values[-1]
+            end_time = self._obj["time"].values[-1] 
         elif "gpm_time" in self._obj.coords:
-            end_time = self._obj["gpm_time"].values[-1]
-        else:
+            end_time = self._obj["gpm_time"].values[-1] 
+        else: 
             raise ValueError("Time coordinate not found")
-        return end_time
-
+        return end_time 
+    
     def subset_by_time(self, start_time=None, end_time=None):
         from gpm_api.utils.time import subset_by_time
 
         return subset_by_time(self._obj, start_time=start_time, end_time=end_time)
 
     def subset_by_time_slice(self, slice):
         from gpm_api.utils.time import subset_by_time_slice
@@ -146,65 +147,63 @@
 
         return get_slices_contiguous_scans(self._obj, min_size=min_size)
 
     def get_slices_contiguous_granules(self, min_size=2):
         from gpm_api.utils.checks import get_slices_contiguous_granules
 
         return get_slices_contiguous_granules(self._obj, min_size=min_size)
-
+    
     def get_slices_valid_geolocation(self, min_size=2):
         from gpm_api.utils.checks import get_slices_valid_geolocation
 
         return get_slices_valid_geolocation(self._obj, min_size=min_size)
-
+    
     def get_slices_regular(self, min_size=2):
         from gpm_api.utils.checks import get_slices_regular
 
         return get_slices_regular(self._obj, min_size=min_size)
-
-    def plot_transect_line(self, ax=None, color="black"):
+    
+    def plot_transect_line(self, ax, color="black"):
         from gpm_api.visualization.profile import plot_transect_line
 
         p = plot_transect_line(self._obj, ax=ax, color=color)
         return p
 
-    def plot_swath_lines(self, ax=None, **kwargs):
+    def plot_swath_lines(self, ax, **kwargs):
         from gpm_api.visualization.orbit import plot_swath_lines
 
         p = plot_swath_lines(self._obj, ax=ax, **kwargs)
         return p
-
-    def label_object(
-        self,
-        variable=None,
-        min_value_threshold=0.1,
-        max_value_threshold=np.inf,
-        min_area_threshold=1,
-        max_area_threshold=np.inf,
-        footprint=None,
-        sort_by="area",
-        sort_decreasing=True,
-        label_name="label",
-    ):
+    
+    def label_object(self, 
+                     variable=None,
+                     min_value_threshold=0.1,
+                     max_value_threshold=np.inf,
+                     min_area_threshold=1,
+                     max_area_threshold=np.inf,
+                     footprint=None,
+                     sort_by="area",
+                     sort_decreasing=True,
+                     label_name="label"):
         from gpm_api.patch.labels import label_xarray_object
-
+        
         xr_obj = label_xarray_object(
             self._obj,
-            variable=variable,
+            variable=variable, 
             # Labels options
             min_value_threshold=min_value_threshold,
             max_value_threshold=max_value_threshold,
             min_area_threshold=min_area_threshold,
             max_area_threshold=max_area_threshold,
             footprint=footprint,
             sort_by=sort_by,
-            sort_decreasing=sort_decreasing,
-        )
+            sort_decreasing=sort_decreasing
+            )
         return xr_obj
-
+           
     def labels_patch_generator(
         self,
         variable=None,
         min_value_threshold=0.1,
         max_value_threshold=np.inf,
         min_area_threshold=1,
         max_area_threshold=np.inf,
@@ -215,30 +214,30 @@
         padding=None,
         min_patch_size=None,
     ):
         from gpm_api.patch.labels_patch import labels_patch_generator
 
         gen = labels_patch_generator(
             self._obj,
-            variable=variable,
+            variable=variable, 
             # Labels options
             min_value_threshold=min_value_threshold,
             max_value_threshold=max_value_threshold,
             min_area_threshold=min_area_threshold,
             max_area_threshold=max_area_threshold,
             footprint=footprint,
             sort_by=sort_by,
             sort_decreasing=sort_decreasing,
             # Patch options
             n_patches=n_patches,
             padding=padding,
             min_patch_size=min_patch_size,
         )
         return gen
-
+    
 
 @xr.register_dataset_accessor("gpm_api")
 class GPM_Dataset_Accessor(GPM_Base_Accessor):
     def __init__(self, xarray_obj):
         super().__init__(xarray_obj)
 
     def title(
@@ -255,84 +254,57 @@
             add_timestep=add_timestep,
             time_idx=time_idx,
             resolution=resolution,
             timezone=timezone,
         )
         return title
 
-    def plot_map(
-        self,
-        variable,
-        ax=None,
-        add_colorbar=True,
-        add_swath_lines=True,
-        interpolation="nearest",  # used only for GPM grid object
-        fig_kwargs={},
-        subplot_kwargs={},
-        cbar_kwargs={},
-        **plot_kwargs,
-    ):
+    def plot_map(self,
+                 variable, 
+                 ax=None, 
+                 add_colorbar=True,
+                 add_swath_lines=True, 
+                 interpolation="nearest", # used only for GPM grid object
+                 fig_kwargs={}, 
+                 subplot_kwargs={},
+                 cbar_kwargs={},
+                 **plot_kwargs,
+                 ):
         from gpm_api.visualization.plot import plot_map
-
         da = self._obj[variable]
-        p = plot_map(
-            ax=ax,
-            da=da,
-            add_colorbar=add_colorbar,
-            add_swath_lines=add_swath_lines,
-            interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
-            subplot_kwargs=subplot_kwargs,
-            cbar_kwargs=cbar_kwargs,
-            **plot_kwargs,
-        )
+        p = plot_map(ax=ax, da=da,
+                     add_colorbar=add_colorbar,
+                     add_swath_lines=add_swath_lines, 
+                     interpolation=interpolation, 
+                     fig_kwargs=fig_kwargs, 
+                     subplot_kwargs=subplot_kwargs,
+                     cbar_kwargs=cbar_kwargs,
+                     **plot_kwargs,
+                     )
         return p
 
-    def plot_image(
-        self,
-        variable,
-        ax=None,
-        add_colorbar=True,
-        interpolation="nearest",
-        fig_kwargs={},
-        cbar_kwargs={},
-        **plot_kwargs,
-    ):
-        from gpm_api.visualization.plot import plot_image
-
-        da = self._obj[variable]
-        p = plot_image(
-            da,
-            ax=ax,
-            add_colorbar=add_colorbar,
-            interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
-            cbar_kwargs=cbar_kwargs,
-            **plot_kwargs,
-        )
-        return p
 
     def plot_patches(
         self,
         variable,
         min_value_threshold=-np.inf,
         max_value_threshold=np.inf,
         min_area_threshold=1,
         max_area_threshold=np.inf,
         footprint=None,
         sort_by="area",
         sort_decreasing=True,
         n_patches=None,
         min_patch_size=None,
         padding=None,
-        add_colorbar=True,
+        add_colorbar=True, 
         interpolation="nearest",
-        fig_kwargs={},
+        fig_kwargs={}, 
         cbar_kwargs={},
-        **plot_kwargs,
+        **plot_kwargs
     ):
         from gpm_api.visualization.labels import plot_patches
 
         data_array = self._obj[variable]
         plot_patches(
             data_array=data_array,
             min_value_threshold=min_value_threshold,
@@ -341,39 +313,39 @@
             max_area_threshold=max_area_threshold,
             footprint=footprint,
             sort_by=sort_by,
             sort_decreasing=sort_decreasing,
             n_patches=n_patches,
             min_patch_size=min_patch_size,
             padding=padding,
-            add_colorbar=add_colorbar,
+            add_colorbar=add_colorbar, 
             interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
 
 
 @xr.register_dataarray_accessor("gpm_api")
 class GPM_DataArray_Accessor(GPM_Base_Accessor):
+    
     def __init__(self, xarray_obj):
         super().__init__(xarray_obj)
-
+    
     def get_slices_var_equals(self, dim, values, union=True, criteria="all"):
         from gpm_api.utils.checks import get_slices_var_equals
 
-        return get_slices_var_equals(
-            self._obj, dim=dim, values=values, union=union, criteria=criteria
-        )
-
+        return get_slices_var_equals(self._obj, dim=dim, values=values, 
+                                     union=union, criteria=criteria)
+    
     def get_slices_var_between(self, dim, vmin=-np.inf, vmax=np.inf, criteria="all"):
         from gpm_api.utils.checks import get_slices_var_between
-
+        
         return get_slices_var_between(self._obj, dim=dim, vmin=vmin, vmax=vmax, criteria=criteria)
-
+    
     def title(
         self,
         prefix_product=True,
         add_timestep=True,
         time_idx=None,
         resolution="m",
         timezone="UTC",
@@ -386,104 +358,93 @@
             add_timestep=add_timestep,
             time_idx=time_idx,
             resolution=resolution,
             timezone=timezone,
         )
         return title
 
-    def plot_map(
-        self,
-        ax=None,
-        add_colorbar=True,
-        add_swath_lines=True,
-        interpolation="nearest",  # used only for GPM grid object
-        fig_kwargs={},
-        subplot_kwargs={},
-        cbar_kwargs={},
-        **plot_kwargs,
-    ):
+    def plot_map(self, ax=None, 
+                 add_colorbar=True,
+                 add_swath_lines=True, 
+                 interpolation="nearest", # used only for GPM grid object
+                 fig_kwargs={}, 
+                 subplot_kwargs={},
+                 cbar_kwargs={},
+                 **plot_kwargs,
+                 ):
         from gpm_api.visualization.plot import plot_map
-
         da = self._obj
-        p = plot_map(
-            ax=ax,
-            da=da,
-            add_colorbar=add_colorbar,
-            add_swath_lines=add_swath_lines,
-            interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
-            subplot_kwargs=subplot_kwargs,
-            cbar_kwargs=cbar_kwargs,
-            **plot_kwargs,
-        )
+        p = plot_map(ax=ax, da=da,
+                     add_colorbar=add_colorbar,
+                     add_swath_lines=add_swath_lines, 
+                     interpolation=interpolation, 
+                     fig_kwargs=fig_kwargs, 
+                     subplot_kwargs=subplot_kwargs,
+                     cbar_kwargs=cbar_kwargs,
+                     **plot_kwargs,
+                     )
         return p
 
-    def plot_map_mesh(
-        self,
-        ax=None,
-        edgecolors="k",
-        linewidth=0.1,
-        fig_kwargs={},
-        subplot_kwargs={},
-        **plot_kwargs,
-    ):
+    def plot_map_mesh(self, ax=None, 
+                      edgecolors="k",
+                      linewidth=0.1, 
+                      fig_kwargs={}, 
+                      subplot_kwargs={},
+                      **plot_kwargs,
+                      ):
         from gpm_api.visualization.plot import plot_map_mesh
 
         da = self._obj
-        p = plot_map_mesh(
-            ax=ax,
-            da=da,
-            edgecolors=edgecolors,
-            linewidth=linewidth,
-            fig_kwargs=fig_kwargs,
-            subplot_kwargs=subplot_kwargs,
-            **plot_kwargs,
+        p = plot_map_mesh(ax=ax, da=da,
+                          edgecolors=edgecolors,
+                          linewidth=linewidth,
+                          fig_kwargs=fig_kwargs, 
+                          subplot_kwargs=subplot_kwargs,
+                          **plot_kwargs,
         )
         return p
 
-    def plot_image(
-        self,
-        ax=None,
-        add_colorbar=True,
-        interpolation="nearest",
-        fig_kwargs={},
-        cbar_kwargs={},
-        **plot_kwargs,
-    ):
+    def plot_image(self, ax=None,
+                   add_colorbar=True, 
+                   interpolation="nearest",
+                   fig_kwargs={}, 
+                   cbar_kwargs={},
+                   **plot_kwargs,
+                   ):
         from gpm_api.visualization.plot import plot_image
 
         da = self._obj
         p = plot_image(
-            da,
-            ax=ax,
+            da, ax=ax, 
             add_colorbar=add_colorbar,
             interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
         return p
 
+
     def plot_patches(
         self,
         min_value_threshold=0.1,
         max_value_threshold=np.inf,
         min_area_threshold=1,
         max_area_threshold=np.inf,
         footprint=None,
         sort_by="area",
         sort_decreasing=True,
         n_patches=None,
         min_patch_size=None,
         padding=None,
-        add_colorbar=True,
+        add_colorbar=True, 
         interpolation="nearest",
-        fig_kwargs={},
+        fig_kwargs={}, 
         cbar_kwargs={},
-        **plot_kwargs,
+        **plot_kwargs
     ):
         from gpm_api.visualization.labels import plot_patches
 
         plot_patches(
             data_array=self._obj,
             min_value_threshold=min_value_threshold,
             max_value_threshold=max_value_threshold,
@@ -491,13 +452,13 @@
             max_area_threshold=max_area_threshold,
             footprint=footprint,
             sort_by=sort_by,
             sort_decreasing=sort_decreasing,
             n_patches=n_patches,
             min_patch_size=min_patch_size,
             padding=padding,
-            add_colorbar=add_colorbar,
+            add_colorbar=add_colorbar, 
             interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
```

### Comparing `gpm_api-0.2.2/gpm_api/configs.py` & `gpm_api-0.2.3/gpm_api/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Thu Mar  9 11:46:07 2023
 
 @author: ghiggi
 """
-import os
+import os 
+import yaml 
 from typing import Dict
 
-import yaml
-
 
 def _read_yaml_file(fpath):
     """Read a YAML file into dictionary."""
-    with open(fpath) as f:
+    with open(fpath, "r") as f:
         dictionary = yaml.safe_load(f)
     return dictionary
 
 
 def _write_yaml_file(dictionary, fpath, sort_keys=False):
     """Write dictionary to YAML file."""
     with open(fpath, "w") as f:
         yaml.dump(dictionary, f, sort_keys=sort_keys)
-    return
+    return None
 
 
-def define_gpm_api_configs(gpm_username: str, gpm_password: str, gpm_base_dir: str):
+def define_gpm_api_configs(gpm_username : str,
+                           gpm_password : str,
+                           gpm_base_dir: str):
     """
     Defines the GPM-API configuration file with the given credentials and base directory.
 
     Parameters
     ----------
     gpm_username : str
         The username for the NASA GPM PPS account.
@@ -38,32 +40,32 @@
         The base directory where GPM data are stored.
 
     Notes
     -----
     This function writes a YAML file to the user's home directory at ~/.config_gpm_api.yml
     with the given GPM-API credentials and base directory. The configuration file can be
     used for authentication when making GPM-API requests.
-
+    
     """
     config_dict = {}
     config_dict["gpm_username"] = gpm_username
     config_dict["gpm_password"] = gpm_password
     config_dict["gpm_base_dir"] = gpm_base_dir
-
-    # Retrieve user home directory
-    home_directory = os.path.expanduser("~")
-
+    
+    # Retrieve user home directory 
+    home_directory = os.path.expanduser( '~' )
+    
     # Define path to .config_gpm_api.yaml file
     fpath = os.path.join(home_directory, ".config_gpm_api.yml")
-
-    # Write the config file
+    
+    # Write the config file 
     _write_yaml_file(config_dict, fpath, sort_keys=False)
-
-    print("The GPM-API config file has been written successfully!")
-    return
+    
+    print ("The GPM-API config file has been written successfully!")
+    return None
 
 
 def read_gpm_api_configs() -> Dict[str, str]:
     """
     Reads the GPM-API configuration file and returns a dictionary with the configuration settings.
 
     Returns
@@ -79,33 +81,31 @@
         specify the configuration file path and settings.
 
     Notes
     -----
     This function reads the YAML configuration file located at ~/.config_gpm_api.yml, which
     should contain the GPM-API credentials and base directory specified by `gpm_api.define_configs()`.
     """
-    # Retrieve user home directory
-    home_directory = os.path.expanduser("~")
-    # Define path where .config_gpm_api.yaml file should be located
+    # Retrieve user home directory 
+    home_directory = os.path.expanduser( '~' )
+    # Define path where .config_gpm_api.yaml file should be located 
     fpath = os.path.join(home_directory, ".config_gpm_api.yml")
     if not os.path.exists(fpath):
-        raise ValueError(
-            "The GPM-API config file has not been specified. Use gpm_api.define_configs to specify it !"
-        )
-    # Read the GPM-API config file
+        raise ValueError("The GPM-API config file has not been specified. Use gpm_api.define_configs to specify it !")
+    # Read the GPM-API config file  
     config_dict = _read_yaml_file(fpath)
-    return config_dict
+    return config_dict 
 
 
 ####--------------------------------------------------------------------------.
-def _get_config_key(key, value=None):
+def _get_config_key(key, value=None): 
     """Return the config key if `value` is None."""
-    if value is None:
-        value = read_gpm_api_configs()[key]
-    return value
+    if value is None: 
+        value = read_gpm_api_configs()[key] 
+    return value 
 
 
 def get_gpm_base_dir(gpm_base_dir=None):
     """Return the GPM base directory."""
     return _get_config_key(key="gpm_base_dir", value=gpm_base_dir)
 
 
@@ -113,7 +113,8 @@
     """Return the GPM-API PPS username."""
     return _get_config_key(key="gpm_username", value=gpm_username)
 
 
 def get_gpm_password(gpm_password=None):
     """Return the GPM-API PPS password."""
     return _get_config_key(key="gpm_password", value=gpm_password)
+
```

### Comparing `gpm_api-0.2.2/gpm_api/dataset/crs.py` & `gpm_api-0.2.3/gpm_api/dataset/crs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Tue Mar  7 17:27:48 2023
 
 @author: ghiggi
 """
 
+import pyproj
 import warnings
-
 import numpy as np
-import pyproj
-import xarray as xr
+import xarray as xr 
 from xarray import Variable
 
-# If the longitude, latitude, vertical or time coordinate is multi-valued,
-# varies in only one dimension, and varies independently of other spatiotemporal coordinates,
-# it is not permitted to store it as an auxiliary coordinate variable.
+# If the longitude, latitude, vertical or time coordinate is multi-valued, 
+# varies in only one dimension, and varies independently of other spatiotemporal coordinates, 
+# it is not permitted to store it as an auxiliary coordinate variable. 
 # This is both to enhance conformance to COARDS and to facilitate the
 # use of generic applications that recognize the NUG convention for coordinate variables.
-# An application that is trying to find the latitude coordinate of a variable
+# An application that is trying to find the latitude coordinate of a variable 
 # should always look first to see if any of the variable’s dimensions correspond to a latitude coordinate variable.
 # If the latitude coordinate is not found this way, then the auxiliary coordinate variables
 # listed by the coordinates attribute should be checked.
 # Note that it is permissible, but optional, to list coordinate variables
 # as well as auxiliary coordinate variables in the coordinates attribute
 # --> https://github.com/pydata/xarray/issues/6310
-# --> https://github.com/pydata/xarray/pull/6366
-# --> Coordinates in encoding ? Why ?
-# --> Rioxarray save grid_mapping in the encoding !
+# --> https://github.com/pydata/xarray/pull/6366 
+# --> Coordinates in encoding ? Why ? 
+# --> Rioxarray save grid_mapping in the encoding ! 
 
-# --> In https://cfconventions.org/cf-conventions/cf-conventions.html#coordinate-system, search for: coordinates =
+# --> In https://cfconventions.org/cf-conventions/cf-conventions.html#coordinate-system, search for: coordinates = 
 
 # --> https://github.com/corteva/rioxarray/pull/284
 # --> https://github.com/opendatacube/datacube-core/issues/1084
 
-# Others work:
-# - https://github.com/dcherian/xindexes/blob/main/crsindex.ipynb
+# Others work: 
+# - https://github.com/dcherian/xindexes/blob/main/crsindex.ipynb 
 # - https://github.com/xarray-contrib/cf-xarray
 # - https://cf-xarray.readthedocs.io/en/latest/grid_mappings.html
 # - https://cf-xarray.readthedocs.io/en/latest/roadmap.html
 
-# ------------------------------------------------------------------------------.
-#### CF-Writers
-## coord attributes
-# - axis if projection
+#------------------------------------------------------------------------------.
+#### CF-Writers 
+## coord attributes 
+# - axis if projection 
 # - units, standard_name, long_name
-# - GEO_exception:
+# - GEO_exception: 
 #   --> For geostationary crs save radians instead of x, y ? or meters?
-#   --> In _get_projection_coords_attrs, define units specification
-
+#   --> In _get_projection_coords_attrs, define units specification 
+    
 ## var attributes
-# AreaDefinition
-# - Only projection coordinates
-#   grid_mapping = "crsOSGB"
-#   grid_mapping = "crsOSGB: x y"
+# AreaDefinition  
+# - Only projection coordinates 
+#   grid_mapping = "crsOSGB" 
+#   grid_mapping = "crsOSGB: x y" 
 
-# - Projection coordinates + WGS84 coordinates
+# - Projection coordinates + WGS84 coordinates 
 #   coordinates = "lat lon"
-#   grid_mapping = "crsOSGB: x y crsWGS84: lat lon"
+#   grid_mapping = "crsOSGB: x y crsWGS84: lat lon" 
 
-# - SwathDefinition
-#   coordinates = "lat lon"
+# - SwathDefinition   
+#   coordinates = "lat lon"    
 #   grid_mapping = "crsWGS84"
 
-# ------------------------------------------------------------------------------.
-#### CF-Readers
-# - If CRS not geographic
-#   --> AreaDefinition
-#   --> If geostationary,
-#       - If x,y units = meter, deal with that
-#       - If x,y units = radian (or radians), do as now
-# - If CRS is geographic
-#   - If dimensional coordinates are 1D --> AreaDefinition
-#   - If dimensional coordinates are 2D --> Swath Definition
+#------------------------------------------------------------------------------.
+#### CF-Readers 
+# - If CRS not geographic 
+#   --> AreaDefinition 
+#   --> If geostationary, 
+#       - If x,y units = meter, deal with that 
+#       - If x,y units = radian (or radians), do as now 
+# - If CRS is geographic 
+#   - If dimensional coordinates are 1D --> AreaDefinition 
+#   - If dimensional coordinates are 2D --> Swath Definition 
 
 # - If two CRS specified (projection and crs), returns AreaDefinition
 
 ####---------------------------------------------------------------------------.
-#### CF-Writers utility
+#### CF-Writers utility 
 
 
 def _get_pyproj_crs_cf_dict(crs):
     """Return the CF-compliant CRS attributes."""
-    # Retrieve CF-compliant CRS information
+    # Retrieve CF-compliant CRS information 
     attrs = crs.to_cf()
-    # Add spatial_ref for compatibility with GDAL
-    #  - GDAL: Only OGC WKT GEOGCS and PROJCS Projections supported
-    #  - PYPROJ write crs_wkt starting with GEOGCRS instead of GEOGCS !
+    # Add spatial_ref for compatibility with GDAL 
+    #  - GDAL: Only OGC WKT GEOGCS and PROJCS Projections supported  
+    #  - PYPROJ write crs_wkt starting with GEOGCRS instead of GEOGCS ! 
     if "crs_wkt" in attrs:
         spatial_ref = attrs["crs_wkt"]
         spatial_ref = spatial_ref.replace("GEOGCRS", "GEOGCS")
         attrs["spatial_ref"] = spatial_ref
     # Return attributes
-    return attrs
+    return attrs 
 
 
 def _get_proj_coord_unit(crs, dim):
     "Return the coordinate unit of a projected CRS."
     axis_info = crs.axis_info[dim]
     units = None
     if hasattr(axis_info, "unit_conversion_factor"):
         unit_factor = axis_info.unit_conversion_factor
-        units = f"{unit_factor} metre" if unit_factor != 1 else "metre"
+        if unit_factor != 1:
+            units = f"{unit_factor} metre"
+        else:
+            units = "metre"
         return units
-    return None
-
-
+     
+    
 def _get_obj(ds, inplace=False):
     """Return a dataset copy if inplace=False."""
     if inplace:
         return ds
     else:
-        return ds.copy(deep=True)
+        return  ds.copy(deep=True)
 
 
 def _get_dataarray_with_spatial_dims(xr_obj):
-    # TODO: maybe select variable with spatial dimensions !
+    # TODO: maybe select variable with spatial dimensions ! 
     if isinstance(xr_obj, xr.Dataset):
         variables = list(xr_obj.data_vars)
         if len(variables) == 0:
             raise ValueError("The dataset has no variables")
         var = variables[0]
         xr_obj = xr_obj[var]
     return xr_obj
@@ -128,16 +130,16 @@
     """Get coordinates attributes of geographic crs."""
     # X or lon coordinate
     x_coord_attrs = {}
     x_coord_attrs["long_name"] = "longitude"
     x_coord_attrs["standard_name"] = "longitude"
     x_coord_attrs["units"] = "degrees_east"
     x_coord_attrs["coverage_content_type"] = "coordinate"
-    # Y or latitude coordinate
-    y_coord_attrs = {}
+    # Y or latitude coordinate 
+    y_coord_attrs = {} 
     y_coord_attrs["long_name"] = "latitude"
     y_coord_attrs["standard_name"] = "latitude"
     y_coord_attrs["units"] = "degrees_north"
     y_coord_attrs["coverage_content_type"] = "coordinate"
     return x_coord_attrs, y_coord_attrs
 
 
@@ -149,579 +151,580 @@
     x_coord_attrs["long_name"] = "x coordinate of projection"
     x_coord_attrs["standard_name"] = "projection_x_coordinate"
     x_coord_attrs["coverage_content_type"] = "coordinate"
     units = _get_proj_coord_unit(crs, dim=0)
     if units:
         x_coord_attrs["units"] = units
     # Add Y metadata
-    y_coord_attrs = {}
+    y_coord_attrs = {} 
     y_coord_attrs["axis"] = "Y"
     y_coord_attrs["long_name"] = "y coordinate of projection"
     y_coord_attrs["standard_name"] = "projection_y_coordinate"
     y_coord_attrs["coverage_content_type"] = "coordinate"
-    units = _get_proj_coord_unit(crs, dim=1)
+    units = _get_proj_coord_unit(crs, dim=1)  
     if units:
         y_coord_attrs["units"] = units
     return x_coord_attrs, y_coord_attrs
 
-
+    
 def _get_proj_dim_coords(xr_obj):
     """Determine the spatial 1D dimensions of the `xarray.DataArray`
-
+    
     Parameters
     ----------
     xr_obj : xr.Dataset or xr.DataArray
-
+    
     Returns
     -------
-    (x_dim, y_dim) tuple
+    (x_dim, y_dim) tuple 
         Tuple with the name of the spatial dimensions.
-    """
+    """      
     # Check for classical options
-    list_options = [("x", "y"), ("lon", "lat"), ("longitude", "latitude")]
-    for dims in list_options:
+    list_options = [("x","y"), ("lon", "lat"), ("longitude", "latitude")]
+    for dims in list_options: 
         dim_x = dims[0]
         dim_y = dims[1]
         if dim_x in xr_obj.coords and dim_y in xr_obj.coords:
-            if xr_obj[dim_x].dims == (dim_x,) and xr_obj[dim_y].dims == (dim_y,):
+            if xr_obj[dim_x].dims == (dim_x,) and xr_obj[dim_y].dims == (dim_y,):   
                 return dims
-    # Otherwise look at available coordinates, and search for CF attributes
+    # Otherwise look at available coordinates, and search for CF attributes 
     else:
         x_dim = None
-        y_dim = None
+        y_dim = None 
         coords_names = list(xr_obj.coords)
         for coord in coords_names:
-            # Select only 1D coordinates with dimension name as the coordinate
+            # Select only 1D coordinates with dimension name as the coordinate 
             if xr_obj[coord].dims != (coord,):
                 continue
             # Retrieve coordinate attribute
             attrs = xr_obj[coord].attrs
             if (attrs.get("axis", "").upper() == "X") or (
-                attrs.get("standard_name", "").lower() in ("longitude", "projection_x_coordinate")
-            ):
-                x_dim = coord
+                attrs.get("standard_name", "").lower() in ("longitude", "projection_x_coordinate")):
+                 x_dim = coord
             elif (attrs.get("axis", "").upper() == "Y") or (
-                attrs.get("standard_name", "").lower() in ("latitude", "projection_y_coordinate")
-            ):
-                y_dim = coord
-    return x_dim, y_dim
+                  attrs.get("standard_name", "").lower() in ("latitude", "projection_y_coordinate")):
+                 y_dim = coord
+    return x_dim, y_dim 
 
 
 def _get_swath_dim_coords(xr_obj):
     """Determine the spatial 1D dimensions of the `xarray.DataArray`
-
+    
     Parameters
     ----------
     xr_obj : xr.Dataset or xr.DataArray
-
+    
     Returns
     -------
-    (x_dim, y_dim) tuple
+    (x_dim, y_dim) tuple 
         Tuple with the name of the swath coordinates.
-    """
+    """      
     # Check for classical options
     list_options = [("lon", "lat"), ("longitude", "latitude")]
-    for dims in list_options:
+    for dims in list_options: 
         dim_x = dims[0]
         dim_y = dims[1]
         if dim_x in xr_obj.coords and dim_y in xr_obj.coords:
             if len(xr_obj[dim_x].dims) == 2 and len(xr_obj[dim_y].dims) == 2:
-                return dim_x, dim_y
+                return dim_x, dim_y 
 
     # Otherwise look at available coordinates, and search for CF attributes
     # --> Look if coordinate has  2D dimension
     # --> Look if coordinate has standard_name "longitude" or "latitude"
     else:
         x_dim = None
-        y_dim = None
+        y_dim = None 
         coords_names = list(xr_obj.coords)
         for coord in coords_names:
-            # Select only lon/lat swath coordinates with dimension like ('y','x')
-            if len(xr_obj[coord].dims) != 2:  # ('y', 'x'), ('cross_track', 'along_track')
+            # Select only lon/lat swath coordinates with dimension like ('y','x')   
+            if len(xr_obj[coord].dims) != 2: # ('y', 'x'), ('cross_track', 'along_track')
                 continue
             attrs = xr_obj[coord].attrs
             if attrs.get("standard_name", "").lower() in ("longitude"):
-                x_dim = coord
+                 x_dim = coord
             elif attrs.get("standard_name", "").lower() in ("latitude"):
-                y_dim = coord
-    return x_dim, y_dim
+                 y_dim = coord
+    return x_dim, y_dim 
 
 
 def has_swath_coords(xr_obj):
     lon_coord, lat_coord = _get_swath_dim_coords(xr_obj)
-    return bool(lon_coord is not None and lat_coord is not None)
+    if lon_coord is not None and lat_coord is not None: 
+        return True
+    else: 
+        return False 
 
 
 def has_proj_coords(xr_obj):
     x_coord, y_coord = _get_proj_dim_coords(xr_obj)
-    return bool(x_coord is not None and y_coord is not None)
+    if x_coord is not None and y_coord is not None: 
+        return True
+    else: 
+        return False 
 
 
 def _add_swath_coords_attrs(ds, crs) -> xr.Dataset:
     """
     Add CF-compliant CRS attributes to the coordinates of a swath.
-
+    
     Parameters
     ----------
     ds : xarray.Dataset
     crs : :py:class:`~pyproj.crs.CoordinateSystem`
         CRS information to be added to the xr.Dataset
-
+        
     Returns
     -------
     :obj:`xarray.Dataset` | :obj:`xarray.DataArray`:
         Dataset with CF-compliant dimension coordinate attributes
     """
-    if not crs.is_geographic:
+    if not crs.is_geographic: 
         raise ValueError("A swath require a geographic CRS.")
-    # Get swath coordinates
+    # Get swath coordinates 
     lon_coord, lat_coord = _get_swath_dim_coords(ds)
-    # Retrieve existing coordinate attributes
+    # Retrieve existing coordinate attributes 
     src_lon_coord_attrs = dict(ds[lon_coord].attrs)
     src_lat_coord_attrs = dict(ds[lat_coord].attrs)
     # Drop axis if present (should not be added to swath objects)
-    src_lon_coord_attrs.pop("axis", None)
-    src_lat_coord_attrs.pop("axis", None)
+    src_lon_coord_attrs.pop("axis", None) 
+    src_lat_coord_attrs.pop("axis", None) 
     # Get geographic coordinate attributes
-    lon_coord_attrs, lat_coord_attrs = _get_geographic_coord_attrs()
-    # Update attributes
+    lon_coord_attrs, lat_coord_attrs = _get_geographic_coord_attrs() 
+    # Update attributes 
     src_lon_coord_attrs.update(lon_coord_attrs)
     src_lat_coord_attrs.update(lat_coord_attrs)
     # Add updated coordinate attributes
     ds[lon_coord].attrs = src_lon_coord_attrs
     ds[lat_coord].attrs = src_lat_coord_attrs
     return ds
-
+    
 
 def _add_proj_coords_attrs(ds, crs) -> xr.Dataset:
     """
     Add CF-compliant attributes to the dimension coordinates of a projected CRS.
-
+    
     Note: The WGS84 grid is considered a projected CRS here !
 
     Parameters
     ----------
     ds : xarray.Dataset
     crs : :py:class:`~pyproj.crs.CoordinateSystem`
         CRS information to be added to the xr.Dataset
-
+        
     Returns
     -------
     :obj:`xarray.Dataset` | :obj:`xarray.DataArray`:
         Dataset with CF-compliant dimension coordinate attributes
     """
-    # Retrieve CRS information
+    # Retrieve CRS information 
     is_projected = crs.is_projected
     is_geographic = crs.is_geographic
-
+    
     # Identify spatial dimension coordinates
     x_dim, y_dim = _get_proj_dim_coords(ds)
-
-    # If available, add attributes
+    
+    # If available, add attributes 
     if x_dim is not None and y_dim is not None:
-
-        # Retrieve existing coordinate attributes
+        
+        # Retrieve existing coordinate attributes 
         src_x_coord_attrs = dict(ds[x_dim].attrs)
         src_y_coord_attrs = dict(ds[y_dim].attrs)
-
-        # Attributes for projected CRS
+        
+        # Attributes for projected CRS 
         if is_projected:
-            # Get projection coordinate attributes
+            # Get projection coordinate attributes 
             x_coord_attrs, y_coord_attrs = _get_projection_coords_attrs(crs)
-            # If unit is already present, do not overwrite it !
-            # --> Example: for compatibility with GEOS area (metre or radians)
-            if "units" in src_x_coord_attrs:
-                _ = x_coord_attrs.pop("units", None)
-                _ = y_coord_attrs.pop("units", None)
-            # Update attributes
+            # If unit is already present, do not overwrite it ! 
+            # --> Example: for compatibility with GEOS area (metre or radians) 
+            if "units" in src_x_coord_attrs: 
+               _ = x_coord_attrs.pop("units", None)
+               _ = y_coord_attrs.pop("units", None)
+            # Update attributes 
             src_x_coord_attrs.update(x_coord_attrs)
             src_y_coord_attrs.update(y_coord_attrs)
-
-        # Attributes for geographic CRS
+            
+        # Attributes for geographic CRS 
         elif is_geographic:
             # Get geographic coordinate attributes
-            x_coord_attrs, y_coord_attrs = _get_geographic_coord_attrs()
-            # Add axis attribute
+            x_coord_attrs, y_coord_attrs = _get_geographic_coord_attrs() 
+            # Add axis attribute 
             x_coord_attrs["axis"] = "X"
             y_coord_attrs["axis"] = "Y"
-            # Update attributes
+            # Update attributes 
             src_x_coord_attrs.update(x_coord_attrs)
             src_y_coord_attrs.update(y_coord_attrs)
-
+            
         # Add coordinate attributes
         ds.coords[x_dim].attrs = src_x_coord_attrs
         ds.coords[y_dim].attrs = src_y_coord_attrs
-
+ 
     return ds
 
 
 def _add_coords_crs_attrs(ds, crs):
     """
     Add CF-compliant attributes to the CRS dimension coordinates.
 
     Parameters
     ----------
     ds : xarray.Dataset
     crs : :py:class:`~pyproj.crs.CoordinateSystem`
         CRS information to be added to the xr.Dataset
-
+        
     Returns
     -------
     :obj:`xarray.Dataset` | :obj:`xarray.DataArray`:
         Dataset with CF-compliant dimension coordinate attributes
     """
-    # Projected CRS
+    # Projected CRS 
     if crs.is_projected:
         ds = _add_proj_coords_attrs(ds, crs)
     # Geographic CRS
     else:
         if has_swath_coords(ds):
             ds = _add_swath_coords_attrs(ds, crs)
-        else:
+        else: 
             ds = _add_proj_coords_attrs(ds, crs)
-    return ds
-
-
+    return ds 
+    
+    
+    
 def _add_crs_coord(ds, crs, grid_mapping_name="spatial_ref"):
     """Add ``name`` coordinate derived from :py:class:`pyproj.crs.CoordinateSystem`.
-
+    
     Parameters
     ----------
     ds : xarray.Dataset
     crs : :py:class:`~pyproj.crs.CoordinateSystem`
         CRS information to be added to the xr.Dataset
     grid_mapping_name : str
-        Name of the grid_mapping coordinate to store the CRS information
+        Name of the grid_mapping coordinate to store the CRS information 
         The default is ``spatial_ref``.
         Other common names are ``grid_mapping`` and ``crs``.
 
     Returns
     -------
     ds : xarray.Dataset
         Dataset including the CRS ``name`` coordinate.
-    """
+    """    
     spatial_ref = Variable((), 0)
-    # Retrieve CF-compliant CRS dictionary information
+    # Retrieve CF-compliant CRS dictionary information 
     attrs = _get_pyproj_crs_cf_dict(crs)
-    # Add attributes to CRS variable
+    # Add attributes to CRS variable 
     spatial_ref.attrs.update(attrs)
     # Add the CRS coordinate to the xr.Dataset
     ds = ds.assign_coords({grid_mapping_name: spatial_ref})
     return ds
 
 
 def _grid_mapping_reference(ds, crs, grid_mapping_name):
     """Define the grid_mapping value to attach to the variables."""
     # Projected CRS
-    if crs.is_projected:
+    if crs.is_projected: 
         x_dim, y_dim = _get_proj_dim_coords(ds)
-        if x_dim is None or y_dim is None:
+        if x_dim is None or y_dim is None: 
             warnings.warn("Projection coordinates are not present.")
             output = f"{grid_mapping_name}"
-        else:
+        else: 
             output = f"{grid_mapping_name}: {x_dim} {y_dim}"
     # Geographic CRS
-    else:
+    else: 
         # If swath
         if has_swath_coords(ds):
             lon_coord, lat_coord = _get_swath_dim_coords(ds)
             output = f"{grid_mapping_name}: {lat_coord} {lon_coord}"
-        else:
+        else: 
             x_dim, y_dim = _get_proj_dim_coords(ds)
-            if x_dim is None or y_dim is None:
+            if x_dim is None or y_dim is None: 
                 warnings.warn("Projection coordinates are not present.")
                 output = f"{grid_mapping_name}"
             output = f"{grid_mapping_name}: {x_dim} {y_dim}"
-    return output
+    return output 
 
 
 def _simplify_grid_mapping_value(grid_mapping_value):
-    """Simplify grid_mapping value.
-
+    """Simplify grid_mapping value. 
+    
     GDAL does not support grid_mapping defined as "crs_wgs84: lat lon"
     If only 1 CRS is specified in such format, it returns "crs_wgs84"
     """
     n_crs = grid_mapping_value.count(":")
-    if n_crs == 1:
+    if n_crs == 1: 
         grid_mapping_value = grid_mapping_value.split(":")[0]
     return grid_mapping_value
 
 
 def simplify_grid_mapping_values(ds):
-    """Simplify grid_mapping value.
-
+    """Simplify grid_mapping value. 
+    
     GDAL does not support grid_mapping defined as "crs_wgs84: lat lon"
     If only 1 CRS is specified in such format, it returns "crs_wgs84"
     """
     keys = list(ds.coords) + list(ds.data_vars)
     for key in keys:
         if "grid_mapping" in ds[key].attrs:
-            ds[key].attrs["grid_mapping"] = _simplify_grid_mapping_value(
-                ds[key].attrs["grid_mapping"]
-            )
-    return ds
+            ds[key].attrs["grid_mapping"] = _simplify_grid_mapping_value(ds[key].attrs["grid_mapping"])
+    return ds 
 
 
-def _get_spatial_coordinates(xr_obj):
+def _get_spatial_coordinates(xr_obj): 
     """Return the spatial coordinates."""
     coords1 = _get_proj_dim_coords(xr_obj)
     coords2 = _get_swath_dim_coords(xr_obj)
     coords = [coord for coord in (coords1 + coords2) if coord is not None]
     return coords
 
-
+ 
 def _get_spatial_dims(xr_obj):
     """Return the spatial dimensions."""
-    coords = _get_spatial_coordinates(xr_obj)  # can be []
-    list_dims = []
-    for coord in coords:
+    coords = _get_spatial_coordinates(xr_obj) # can be []
+    list_dims = [] 
+    for coord in coords: 
         _ = [list_dims.append(dim) for dim in list(xr_obj[coord].dims)]
     spatial_dims = list(set(list_dims))
-    return spatial_dims
+    return spatial_dims 
 
 
-def _get_variables_with_spatial_dims(ds):
+def _get_variables_with_spatial_dims(ds): 
     """Return variables and coordinates depending on spatial dimensions.
-
-    A coordinate with dimension (time, y, x) is selected
+    
+    A coordinate with dimension (time, y, x) is selected 
     The spatial coordinates (y, x) or (latitude, longitude) are not selected.
     """
-    spatial_dims = _get_spatial_dims(ds)  # can be []
+    spatial_dims = _get_spatial_dims(ds) # can be []
     spatial_dims = set(spatial_dims)
-    if len(spatial_dims) == 0:
+    if len(spatial_dims) == 0: 
         raise ValueError("No spatial dimension identified in the dataset.")
     variables = list(ds.coords) + list(ds.data_vars)
     list_spatial_variables = []
-    for var in variables:
+    for var in variables: 
         if set(ds[var].dims).issuperset(spatial_dims):
             list_spatial_variables.append(var)
-    # Remove spatial coordinates from the list
+    # Remove spatial coordinates from the list 
     coords = _get_spatial_coordinates(ds)
     spatial_variables = set(list_spatial_variables).difference(coords)
-    return spatial_variables
+    return spatial_variables 
 
 
 def _add_variables_crs_attrs(ds, crs, grid_mapping_name):
     """Add 'grid_mapping' and 'coordinates' (for swath only) attributes to the variable.
-
+    
     If a grid_mapping attribute is already existing, add also the new one !
-    """
+    """    
     # Retrieve grid_mapping attributes value
     grid_mapping_value = _grid_mapping_reference(ds, crs=crs, grid_mapping_name=grid_mapping_name)
-
+    
     # Retrieve variables (and coordinates) requiring the crs attribute
     variables = _get_variables_with_spatial_dims(ds)
-
-    for var in variables:
+    
+    for var in variables:  
         grid_mapping = ds[var].attrs.get("grid_mapping", "")
-        grid_mapping = (
-            grid_mapping_value if grid_mapping == "" else grid_mapping + " " + grid_mapping_value
-        )
+        if grid_mapping == "": 
+            grid_mapping = grid_mapping_value
+        else: 
+            grid_mapping = grid_mapping + " " + grid_mapping_value
         ds[var].attrs["grid_mapping"] = grid_mapping
-
+        
     # Add coordinates attribute if swath data
-    if has_swath_coords(ds):
+    if has_swath_coords(ds): 
         lon_coord, lat_coord = _get_swath_dim_coords(ds)
         for var in variables:
             da_coords = ds[var].coords
             if lon_coord in da_coords and lat_coord in da_coords:
                 ds[var].attrs["coordinates"] = f"{lat_coord} {lon_coord}"
-    return ds
+    return ds 
 
 
 def _get_name_existing_crs_coords(xr_obj):
     """Return a list with the name of CRS coordinates."""
     list_crs_coords = []
     for coord in list(xr_obj.coords):
         if "crs_wkt" in xr_obj[coord].attrs or "grid_mapping_name" in xr_obj[coord].attrs:
             list_crs_coords.append(coord)
     return list_crs_coords
 
 
 def remove_existing_crs_info(ds):
     """Remove existing grid_mapping attributes."""
-    for var in ds.data_vars:
+    for var in ds.data_vars: 
         _ = ds[var].attrs.pop("grid_mapping", None)
         _ = ds[var].attrs.pop("coordinates", None)
         _ = ds[var].encoding.pop("coordinates", None)
     crs_coords = _get_name_existing_crs_coords(ds)
     ds = ds.drop(crs_coords)
     return ds
 
 
-def set_dataset_single_crs(ds, crs, grid_mapping_name="spatial_ref", inplace=False):
+def set_dataset_single_crs(ds, crs, grid_mapping_name="spatial_ref", inplace=False): 
     """Add CF-compliant CRS information to an xr.Dataset
-
-    It assumes all dataset variables have same CRS !
-    For projected CRS, it expects that the CRS dimension coordinates are specified.
+    
+    It assumes all dataset variables have same CRS ! 
+    For projected CRS, it expects that the CRS dimension coordinates are specified. 
     For swath dataset, it expects that the geographic coordinates are specified.
-
+        
     Parameters
     ----------
     ds : xarray.Dataset
     crs : :py:class:`~pyproj.crs.CoordinateSystem`
         CRS information to be added to the xr.Dataset
     grid_mapping_name : str
-        Name of the grid_mapping coordinate to store the CRS information
+        Name of the grid_mapping coordinate to store the CRS information 
         The default is ``spatial_ref``.
         Other common names are ``grid_mapping`` and ``crs``.
-
+    
     Returns
     -------
     ds : xarray.Dataset
         Dataset with CF-compliant CRS information.
     """
     # Get dataset copy if inplace=False
     ds = _get_obj(ds=ds, inplace=inplace)
-
+    
     # Add coordinate with CRS information
     ds = _add_crs_coord(ds, crs=crs, grid_mapping_name=grid_mapping_name)
-
+    
     # Add CF attributes to CRS coordinates
     ds = _add_coords_crs_attrs(ds, crs=crs)
-
-    # Add CF attributes 'grid_mapping' (and 'coordinates' for swath)
-    # - To relevant variables and coordinates
+    
+    # Add CF attributes 'grid_mapping' (and 'coordinates' for swath) 
+    # - To relevant variables and coordinates 
     ds = _add_variables_crs_attrs(ds=ds, crs=crs, grid_mapping_name=grid_mapping_name)
     return ds
-
-
+    
+    
 def set_dataset_crs(ds, crs, grid_mapping_name="spatial_ref", inplace=False):
     """Add CF-compliant CRS information to an xr.Dataset
-
-    It assumes all dataset variables have same CRS !
-    For projected CRS, it expects that the CRS dimension coordinates are specified.
+    
+    It assumes all dataset variables have same CRS ! 
+    For projected CRS, it expects that the CRS dimension coordinates are specified. 
     For swath dataset, it expects that the geographic coordinates are specified.
-
-    For projected CRS, if 2D latitude/longitude arrays are specified,
+    
+    For projected CRS, if 2D latitude/longitude arrays are specified, 
     it assumes they refer to the WGS84 CRS !
-
+        
     Parameters
     ----------
     ds : xarray.Dataset
     crs : :py:class:`~pyproj.crs.CoordinateSystem`
         CRS information to be added to the xr.Dataset
     grid_mapping_name : str
-        Name of the grid_mapping coordinate to store the CRS information
+        Name of the grid_mapping coordinate to store the CRS information 
         The default is ``spatial_ref``.
         Other common names are ``grid_mapping`` and ``crs``.
-
+    
     Returns
     -------
     ds : xarray.Dataset
         Dataset with CF-compliant CRS information.
-    """
+    """ 
     ds = remove_existing_crs_info(ds)
-    ds = set_dataset_single_crs(
-        ds=ds, crs=crs, grid_mapping_name=grid_mapping_name, inplace=inplace
-    )
+    ds = set_dataset_single_crs(ds=ds, crs=crs, grid_mapping_name=grid_mapping_name, inplace=inplace)
     # If CRS is projected and 2D lon/lat are available, also add the WGS84 CRS
     if crs.is_projected and has_swath_coords(ds):
         crs_wgs84 = pyproj.CRS(proj="longlat", ellps="WGS84")
-        ds = set_dataset_single_crs(
-            ds=ds, crs=crs_wgs84, grid_mapping_name="crsWGS84", inplace=inplace
-        )
-    # Simplify grid_mapping if possible
-    # - For compatibility with GDAL, if only 1 CRS is specified !
+        ds = set_dataset_single_crs(ds=ds, crs=crs_wgs84, grid_mapping_name="crsWGS84", inplace=inplace)
+    # Simplify grid_mapping if possible 
+    # - For compatibility with GDAL, if only 1 CRS is specified ! 
     ds = simplify_grid_mapping_values(ds)
-    return ds
+    return ds 
 
 
 ####---------------------------------------------------------------------------.
-#### TODO: Writers
-# coord attributes
+#### TODO: Writers 
+# coord attributes 
 # --> For geostationary crs save radians instead of x, y ? or meters?
-# --> In _get_projection_coords_attrs, define units specification
+# --> In _get_projection_coords_attrs, define units specification 
 
 
 # def _add_crs_proj_coords(ds, crs, width, height, affine):
 #     # https://github.com/corteva/rioxarray/blob/master/rioxarray/rioxarray.py#L118
-#     # TODO:
+#     # TODO: 
 #     # for AreaDefinition. x_coord, y_coord = area_dej.get_proj_coords()
-#     # for SwathDefinition: do nothing because expect already present
-
-#     #  _generate_spatial_coords
-#     # https://github.com/corteva/rioxarray/blob/master/rioxarray/rioxarray.py#L118
-#     pass
+#     # for SwathDefinition: do nothing because expect already present 
+    
+#     #  _generate_spatial_coords 
+#     # https://github.com/corteva/rioxarray/blob/master/rioxarray/rioxarray.py#L118 
+#     pass 
 
 
 ####---------------------------------------------------------------------------.
-#### CF-Readers
-
+#### CF-Readers 
 
+ 
 def _get_crs_coordinates(xr_obj):
     """Return a list with the name(s) of the CRS coordinate(s)."""
-    list_crs_names = []
-    crs_attributes = ["grid_mapping_name", "crs_wkt", "spatial_ref"]
+    list_crs_names = [] 
+    crs_attributes = ["grid_mapping_name", "crs_wkt","spatial_ref"]
     for coord in list(xr_obj.coords):
         if np.any(np.isin(crs_attributes, list(xr_obj[coord].attrs))):
             list_crs_names.append(coord)
     return list_crs_names
 
 
 def _get_list_pyproj_crs(xr_obj):
     """Return a list of pyproj specified CRS."""
     list_crs_names = _get_crs_coordinates(xr_obj)
-    if len(list_crs_names) == 0:
+    if len(list_crs_names) == 0: 
         raise ValueError("No CRS coordinate in the dataset.")
     list_crs = [pyproj.CRS.from_cf(xr_obj[crs_coord].attrs) for crs_coord in list_crs_names]
-    return list_crs
+    return list_crs 
 
 
-def _get_geographic_crs(xr_obj):
+def _get_geographic_crs(xr_obj): 
     list_crs = _get_list_pyproj_crs(xr_obj)
     list_geographic_crs = [proj_crs for proj_crs in list_crs if proj_crs.is_geographic]
     if len(list_geographic_crs) > 1:
-        raise ValueError("More than 1 geographic CRS is specified")
+           raise ValueError("More than 1 geographic CRS is specified")
     if len(list_geographic_crs) == 0:
-        raise ValueError("No geographic CRS is specified")
+           raise ValueError("No geographic CRS is specified")
     crs = list_geographic_crs[0]
     return crs
 
 
 def get_pyproj_crs(xr_obj):
-    """Return :py:class:`pyproj.crs.CoordinateSystem` from CRS coordinate(s).
-
+    """Return :py:class:`pyproj.crs.CoordinateSystem` from CRS coordinate(s). 
+    
     If a geographic and projected CRS are present, it returns the projected.
-
+    
     Parameters
     ----------
     xr_obj : xarray.Dataset or xarray.DataArray
 
     Returns
     -------
     proj_crs : :py:class:`~pyproj.crs.CoordinateSystem`
     """
     list_crs = _get_list_pyproj_crs(xr_obj)
-    # If two crs are provided, select the projected !
-    if len(list_crs) == 2:
+    # If two crs are provided, select the projected ! 
+    if len(list_crs) == 2: 
         list_crs = [proj_crs for proj_crs in list_crs if proj_crs.is_projected]
-        if len(list_crs) != 1:
+        if len(list_crs) != 1 :
             raise ValueError("A DataArray should have only 1 projected CRS.")
     # Return crs
     crs = list_crs[0]
-    return crs
+    return crs 
 
 
 def get_pyresample_swath(xr_obj):
     from pyresample import SwathDefinition
-
+    
     if not has_swath_coords(xr_obj):
         raise ValueError("Not a swath object.")
-
+        
     # Identify name of longitude and latitude coordinates
     lons, lats = _get_swath_dim_coords(xr_obj)
-
+    
     # Retrieve geographic CRS if available
-    try:
+    try: 
         pyproj_crs = _get_geographic_crs(xr_obj)
-    except Exception:
-        pyproj_crs = None
-    # Define SwathDefinition
-    swath_def = SwathDefinition(xr_obj[lons], xr_obj[lats], crs=pyproj_crs)
+    except Exception: 
+        pyproj_crs = None 
+    # Define SwathDefinition 
+    swath_def = SwathDefinition(xr_obj[lons], xr_obj[lats], crs=pyproj_crs) 
     return swath_def
 
 
-# def get_pyresample_area(xr_obj) --> pyresample cf area
-# def _get_ds_area_extent
-# def _get_ds_resolution
-# def _get_ds_shape
+# def get_pyresample_area(xr_obj) --> pyresample cf area 
+# def _get_ds_area_extent  
+# def _get_ds_resolution 
+# def _get_ds_shape 
+
```

### Comparing `gpm_api-0.2.2/gpm_api/dataset/decoding.py` & `gpm_api-0.2.3/gpm_api/dataset/decoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Mon Aug 15 00:12:47 2022
 
 @author: ghiggi
 """
-import warnings
-
 import numpy as np
 import xarray as xr
-
+import warnings
 from gpm_api.utils.warnings import GPM_Warning
-
 ####--------------------------------------------------------------------------.
 #### Attributes cleaning
 
 
 def clean_dataarrays_attrs(ds, product):
     for var, da in ds.items():
         ds[var] = _format_dataarray_attrs(da, product)
     return ds
 
 
 def _format_dataarray_attrs(da, product=None):
     attrs = da.attrs
 
     # Convert CodeMissingValue' to _FillValue if available
-    if not attrs.get("_FillValue", False) and attrs.get("CodeMissingValue", False):
-        attrs["_FillValue"] = attrs.pop("CodeMissingValue")
+    if not attrs.get("_FillValue", False):
+        if attrs.get("CodeMissingValue", False):
+            attrs["_FillValue"] = attrs.pop("CodeMissingValue")
 
     # Remove 'CodeMissingValue'
     attrs.pop("CodeMissingValue", None)
 
     # Convert 'Units' to 'units'
-    if not attrs.get("units", False) and attrs.get("Units", False):
-        attrs["units"] = attrs.pop("Units")
+    if not attrs.get("units", False):
+        if attrs.get("Units", False):
+            attrs["units"] = attrs.pop("Units")
 
     # Remove 'Units'
     attrs.pop("Units", None)
 
     # Remove 'DimensionNames'
     attrs.pop("DimensionNames", None)
 
@@ -117,31 +117,29 @@
 # if (var == 'typePrecip'):
 #   print('Decoding of typePrecip not yet implemented')
 
 
 def ensure_valid_coords(ds, raise_error=False):
     # invalid_coords = np.logical_or(ds["lon"].data == -9999.9,
     #                                ds["lat"].data == -9999.9)
-    invalid_coords = np.logical_or(
-        np.logical_or(ds["lon"].data < -180, ds["lon"].data > 180),
-        np.logical_or(ds["lat"].data < -90, ds["lat"].data > 90),
-    )
+    invalid_coords = np.logical_or(np.logical_or(ds["lon"].data < -180, ds["lon"].data > 180),
+                                   np.logical_or(ds["lat"].data < -90, ds["lat"].data > 90))
     if np.any(invalid_coords):
-        # Raise error or add warning
+        # Raise error or add warning 
         msg = "Invalid coordinate in the granule."
         if raise_error:
             raise ValueError(msg)
         else:
             warnings.warn(msg, GPM_Warning)
 
         da_invalid_coords = ds["lon"].copy()
         da_invalid_coords.data = invalid_coords
         # For each variable, set NaN value where invalid coordinates
         ds = ds.where(~da_invalid_coords)
-        # Add NaN to longitude and latitude
+        # Add NaN to longitude and latitude 
         ds["lon"] = ds["lon"].where(~da_invalid_coords)
         ds["lat"] = ds["lat"].where(~da_invalid_coords)
     return ds
 
 
 def apply_custom_decoding(ds, product):
     # Ensure valid coordinates
@@ -153,55 +151,59 @@
         range_id = np.arange(ds.dims["range"])
         ds = ds.assign_coords({"gpm_range_id": ("range", range_id)})
 
     # Clean attributes
     ds = clean_dataarrays_attrs(ds, product)
 
     # Add coordinates
-    if product == "2A-DPR" and "frequency" in list(ds.dims):
-        ds = ds.assign_coords({"frequency": ["Ku", "Ka"]})
-
-    if product in ["2A-DPR", "2A-Ku", "2A-Ka"] and "paramDSD" in list(ds):
-        ds = ds.assign_coords({"DSD_params": ["Nw", "Dm"]})
-
-    if product in ["2A-DPR", "2A-Ku", "2A-Ka"] and "height" in list(ds):
-        ds = ds.set_coords("height")
-
-    if product in ["2A-GPM-SLH", "2B-GPM-CSH"] and "nlayer" in list(ds.dims):
-        # Fixed heights for 2HSLH and 2HCSH
-        # - FileSpec v7: p.2395, 2463
-        height = np.linspace(0.25 / 2, 20 - 0.25 / 2, 80) * 1000  # in meters
-        ds = ds.rename_dims({"nlayer": "height"})
-        ds = ds.assign_coords({"height": height})
-        ds["height"].attrs["units"] = "km a.s.l"
+    if product == "2A-DPR":
+        if "frequency" in list(ds.dims):
+            ds = ds.assign_coords({"frequency": ["Ku", "Ka"]})
+
+    if product in ["2A-DPR", "2A-Ku", "2A-Ka"]:
+        if "paramDSD" in list(ds):
+            ds = ds.assign_coords({"DSD_params": ["Nw", "Dm"]})
+
+    if product in ["2A-DPR", "2A-Ku", "2A-Ka"]:
+        if "height" in list(ds):
+            ds = ds.set_coords("height")
+
+    if product in ["2A-GPM-SLH", "2B-GPM-CSH"]:
+        if "nlayer" in list(ds.dims):
+            # Fixed heights for 2HSLH and 2HCSH
+            # - FileSpec v7: p.2395, 2463
+            height = np.linspace(0.25 / 2, 20 - 0.25 / 2, 80) * 1000  # in meters
+            ds = ds.rename_dims({"nlayer": "height"})
+            ds = ds.assign_coords({"height": height})
+            ds["height"].attrs["units"] = "km a.s.l"
 
     # Modify variables
     dataset_vars = list(ds.data_vars)
     if "precipWaterIntegrated" in dataset_vars:
         ds["precipWaterIntegrated_Liquid"] = ds["precipWaterIntegrated"][:, :, 0]
         ds["precipWaterIntegrated_Solid"] = ds["precipWaterIntegrated"][:, :, 1]
         ds = ds.drop_vars(names="precipWaterIntegrated")
         ds["precipWaterIntegrated"] = (
             ds["precipWaterIntegrated_Liquid"] + ds["precipWaterIntegrated_Solid"]
         )
 
     if "flagBB" in dataset_vars and product == "2A-DPR":
         ds["flagBB"].attrs[
             "description"
-        ] = """Flag for Bright Band:
+        ] = """Flag for Bright Band: 
                                                 0 : BB not detected
                                                 1 : Bright Band detected by Ku and DFRm
                                                 2 : Bright Band detected by Ku only
                                                 3 : Bright Band detected by DFRm only
                                             """
-    # if ds.attrs.get("TotalQualityCode"):
-    #     TotalQualityCode = ds.attrs.get("TotalQualityCode")
-    #     ds["TotalQualityCode"] = xr.DataArray(
-    #         np.repeat(TotalQualityCode, ds.dims["along_track"]), dims=["along_track"]
-    #     )
+    if ds.attrs.get("TotalQualityCode"):
+        TotalQualityCode = ds.attrs.get("TotalQualityCode")
+        ds["TotalQualityCode"] = xr.DataArray(
+            np.repeat(TotalQualityCode, ds.dims["along_track"]), dims=["along_track"]
+        )
 
     # Correct for misreported _FillValue
     if "surfacePrecipitation" in dataset_vars:
         # _FillValue often reported as -9999.9, but in data the values are -9999.0 !
         # --> Example 2A-MHS-METOB
         da = ds["surfacePrecipitation"]
         ds["surfacePrecipitation"] = da.where(da != -9999.0)
```

### Comparing `gpm_api-0.2.2/gpm_api/etc/country_acronyms.yaml` & `gpm_api-0.2.3/gpm_api/etc/country_acronyms.yaml`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.2/gpm_api/etc/country_bounds.yaml` & `gpm_api-0.2.3/gpm_api/etc/country_bounds.yaml`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.2/gpm_api/etc/country_extent.yaml` & `gpm_api-0.2.3/gpm_api/etc/country_extent.yaml`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.2/gpm_api/io/checks.py` & `gpm_api-0.2.3/gpm_api/io/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sun Aug 14 20:02:18 2022
 @author: ghiggi
 """
-import datetime
 import os
-
+import datetime
 import numpy as np
 
 
 def is_not_empty(x):
-    return bool(x)
+    return not not x
 
 
 def is_empty(x):
     return not x
 
 
 def check_base_dir(base_dir):
@@ -70,26 +70,34 @@
     elif isinstance(groups, list):
         groups = np.array(groups)
     return groups
 
 
 def check_version(version):
     if not isinstance(version, int):
-        raise ValueError("Please specify the GPM version with an integer between 5 and 7.")
+        raise ValueError(
+            "Please specify the GPM version with an integer between 5 and 7."
+        )
     if version not in [5, 6, 7]:
-        raise ValueError("Download/Reading have been implemented only for GPM versions 5, 6 and 7.")
+        raise ValueError(
+            "Download/Reading have been implemented only for GPM versions 5, 6 and 7."
+        )
 
 
 def check_product(product, product_type):
     from gpm_api.io.products import available_products
 
     if not isinstance(product, str):
-        raise ValueError("'Ask for a single product at time.'product' must be a single string.")
+        raise ValueError(
+            "'Ask for a single product at time.'product' must be a single string."
+        )
     if product not in available_products(product_type=product_type):
-        raise ValueError("Please provide a valid GPM product --> gpm_api.available_products().")
+        raise ValueError(
+            "Please provide a valid GPM product --> gpm_api.available_products()."
+        )
 
 
 def check_product_type(product_type):
     if not isinstance(product_type, str):
         raise ValueError("Please specify the product_type as 'RS' or 'NRT'.")
     if product_type not in ["RS", "NRT"]:
         raise ValueError("Please specify the product_type as 'RS' or 'NRT'.")
@@ -109,30 +117,20 @@
 
     Returns
     -------
     time : datetime.datetime
         datetime.datetime object.
 
     """
-    if not isinstance(time, (datetime.datetime, datetime.date, np.datetime64, np.ndarray, str)):
+    if not isinstance(time, (datetime.datetime, datetime.date, np.datetime64, str)):
         raise TypeError(
             "Specify time with datetime.datetime objects or a "
             "string of format 'YYYY-MM-DD hh:mm:ss'."
         )
-    # If numpy array with datetime64 (and size=1)
-    if isinstance(time, np.ndarray):
-        if np.issubdtype(time.dtype, np.datetime64):
-            if time.size == 1:
-                time = time.astype("datetime64[s]").tolist()
-            else:
-                raise ValueError("Expecting a single timestep!")
-        else:
-            raise ValueError("The numpy array does not have a np.datetime64 dtype!")
-
-    # If np.datetime64, convert to datetime.datetime
+    # If np.datetime, convert to datetime.datetime
     if isinstance(time, np.datetime64):
         time = time.astype("datetime64[s]").tolist()
     # If datetime.date, convert to datetime.datetime
     if not isinstance(time, (datetime.datetime, str)):
         time = datetime.datetime(time.year, time.month, time.day, 0, 0, 0)
     if isinstance(time, str):
         try:
@@ -176,21 +174,25 @@
     if scan_mode is None:
         scan_mode = scan_modes[0]
         if len(scan_modes) > 1:
             print(f"'scan_mode' has not been specified. Default to {scan_mode}.")
 
     # -------------------------------------------------------------------------.
     # Check that a single scan mode is specified
-    if scan_mode is not None and not isinstance(scan_mode, str):
-        raise ValueError("Specify a single 'scan_mode'.")
+    if scan_mode is not None:
+        if not isinstance(scan_mode, str):
+            raise ValueError("Specify a single 'scan_mode'.")
 
     # -------------------------------------------------------------------------.
     # Check that a valid scan mode is specified
-    if scan_mode is not None and scan_mode not in scan_modes:
-        raise ValueError(f"For {product} product, valid scan_modes are {scan_modes}.")
+    if scan_mode is not None:
+        if not scan_mode in scan_modes:
+            raise ValueError(
+                f"For {product} product, valid scan_modes are {scan_modes}."
+            )
 
     # -------------------------------------------------------------------------.
     return scan_mode
 
 
 def check_bbox(bbox):
     """
```

### Comparing `gpm_api-0.2.2/gpm_api/io/directories.py` & `gpm_api-0.2.3/gpm_api/io/directories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Thu Oct 13 16:48:22 2022
 
 @author: ghiggi
 """
 
 ##----------------------------------------------------------------------------.
-import datetime
 import os
-
+import datetime
 from gpm_api.io.checks import check_base_dir
 from gpm_api.io.products import (
+    GPM_NRT_products,
+    GPM_RS_products,
+    GPM_RADAR_NRT_products,
+    GPM_PMW_NRT_products,
+    # CMB NRT?
+    GPM_RADAR_RS_products,
+    GPM_PMW_RS_products,
+    GPM_CMB_RS_products,
     GPM_1B_RS_products,
     GPM_1C_NRT_products,
-    GPM_CMB_2B_RS_products,
-    GPM_CMB_RS_products,
+    # GPM_RADAR_1B_NRT_products,
+    GPM_RADAR_2A_NRT_products,
+    GPM_PMW_1B_NRT_products,
+    GPM_PMW_2A_GPROF_NRT_products,
+    GPM_PMW_2A_PRPS_NRT_products,
     # CMB NRT?
     GPM_IMERG_NRT_products,
-    GPM_IMERG_RS_products,
-    GPM_NRT_products,
+    GPM_RADAR_2A_RS_products,
     GPM_PMW_1A_RS_products,
-    GPM_PMW_1B_NRT_products,
     GPM_PMW_1C_RS_products,
-    GPM_PMW_2A_GPROF_NRT_products,
-    GPM_PMW_2A_GPROF_RS_products,
-    GPM_PMW_2A_PRPS_NRT_products,
     GPM_PMW_2A_PRPS_RS_products,
-    GPM_PMW_NRT_products,
-    GPM_PMW_RS_products,
-    # GPM_RADAR_1B_NRT_products,
-    GPM_RADAR_2A_NRT_products,
-    GPM_RADAR_2A_RS_products,
-    GPM_RADAR_NRT_products,
-    # CMB NRT?
-    GPM_RADAR_RS_products,
-    GPM_RS_products,
+    GPM_PMW_2A_GPROF_RS_products,
+    GPM_CMB_2B_RS_products,
+    GPM_IMERG_RS_products,
 )
 
 ####--------------------------------------------------------------------------.
 ####################
 #### LOCAL DISK ####
 ####################
 
@@ -95,15 +95,17 @@
         raise ValueError("Valid product_type: 'RS' and 'NRT'.")
 
     # Define pattern
     if product_type == "NRT":
         dir_structure = os.path.join("GPM", product_type, product_category, product)
     else:  # product_type == "RS"
         version_str = "V0" + str(int(version))
-        dir_structure = os.path.join("GPM", product_type, version_str, product_category, product)
+        dir_structure = os.path.join(
+            "GPM", product_type, version_str, product_category, product
+        )
     return dir_structure
 
 
 def get_disk_directory(base_dir, product, product_type, date, version):
     """
     Provide the disk repository path where the requested GPM data are stored/need to be saved.
 
@@ -237,15 +239,17 @@
             folder_name = "imerg/early"
         elif product == "IMERG-LR":
             folder_name = "imerg/late"
         else:
             raise ValueError("BUG - Some product option is missing.")
 
         #### Specify the directory structure for the daily list of IMERG NRT products
-        dir_structure = os.path.join(folder_name, datetime.datetime.strftime(date, "%Y%m"))
+        dir_structure = os.path.join(
+            folder_name, datetime.datetime.strftime(date, "%Y%m")
+        )
         return dir_structure
     # ------------------------------------------------------------------------.
     else:
         raise ValueError("BUG - Some product option is missing.")
 
     #### Specify the directory structure for daily list of NRT data (exect IMERG)
     dir_structure = folder_name
```

### Comparing `gpm_api-0.2.2/gpm_api/io/disk.py` & `gpm_api-0.2.3/gpm_api/io/disk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Mon Aug 15 00:18:13 2022
 
 @author: ghiggi
 """
-import datetime
 import os
-
+import datetime
 import pandas as pd
-
+from gpm_api.io import GPM_VERSION # CURRENT GPM VERSION
 from gpm_api.configs import get_gpm_base_dir
-from gpm_api.io import GPM_VERSION  # CURRENT GPM VERSION
 from gpm_api.io.checks import (
-    check_base_dir,
     check_date,
+    check_start_end_time,
     check_product,
     check_product_type,
-    check_start_end_time,
     check_version,
+    check_base_dir,
     is_empty,
 )
-from gpm_api.io.directories import get_disk_directory
 from gpm_api.io.filter import filter_filepaths
+from gpm_api.io.directories import get_disk_directory
+
 
 ####--------------------------------------------------------------------------.
 ######################
 #### Find utility ####
 ######################
-
-
-def _get_disk_daily_filepaths(base_dir, product, product_type, date, version, verbose=True):
+            
+            
+def _get_disk_daily_filepaths(
+    base_dir, product, product_type, date, version, verbose=True
+):
     """
     Retrieve GPM data filepaths on the local disk directory of a specific day and product.
 
     Parameters
     ----------
     base_dir : str
         The base directory where to store GPM data.
@@ -154,17 +156,17 @@
     ##------------------------------------------------------------------------.
     return filepaths
 
 
 def find_filepaths(
     product,
     start_time,
-    end_time,
-    product_type="RS",
-    version=GPM_VERSION,
+    end_time, 
+    product_type="RS", 
+    version=GPM_VERSION, 
     verbose=True,
     base_dir=None,
 ):
     """
     Retrieve GPM data filepaths on local disk for a specific time period and product.
 
     Parameters
@@ -178,28 +180,28 @@
     product_type : str, optional
         GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
     version : int, optional
         GPM version of the data to retrieve if product_type = 'RS'.
     verbose : bool, optional
         Whether to print processing details. The default is True.
     base_dir : str, optional
-        The path to the GPM base directory. If None, it use the one specified
-        in the GPM-API config file.
+        The path to the GPM base directory. If None, it use the one specified 
+        in the GPM-API config file. 
         The default is None.
-
+        
     Returns
     -------
     filepaths : list
         List of GPM filepaths.
 
     """
     # -------------------------------------------------------------------------.
     # Retrieve GPM-API configs
     base_dir = get_gpm_base_dir(base_dir)
-
+ 
     # -------------------------------------------------------------------------.
     ## Checks input arguments
     check_version(version=version)
     base_dir = check_base_dir(base_dir)
     check_product_type(product_type=product_type)
     check_product(product=product, product_type=product_type)
     start_time, end_time = check_start_end_time(start_time, end_time)
```

### Comparing `gpm_api-0.2.2/gpm_api/io/download.py` & `gpm_api-0.2.3/gpm_api/io/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Mon Aug 15 00:18:33 2022
 
 @author: ghiggi
 """
 
-import concurrent.futures
-import datetime
-import ftplib
 import os
+import ftplib
+import datetime
 import subprocess
-import warnings
-
 import pandas as pd
+import concurrent.futures
 from tqdm import tqdm
-
-from gpm_api.configs import get_gpm_base_dir, get_gpm_password, get_gpm_username
-from gpm_api.io import GPM_VERSION  # CURRENT GPM VERSION
+from gpm_api.io.pps import _find_pps_daily_filepaths #, find_pps_filepaths
+from gpm_api.utils.utils_string import subset_list_by_boolean
+from gpm_api.utils.archive import (
+    check_file_integrity, 
+    get_corrupted_filepaths,
+    remove_corrupted_filepaths,
+)
 from gpm_api.io.checks import (
     check_base_dir,
-    check_date,
+    check_version,
     check_product,
     check_product_type,
     check_start_end_time,
-    check_version,
+    check_date,
     is_empty,
 )
+from gpm_api.io.info import get_start_time_from_filepaths, get_info_from_filepath
 from gpm_api.io.directories import get_disk_directory, get_pps_directory
-from gpm_api.io.info import get_info_from_filepath, get_start_time_from_filepaths
-from gpm_api.io.pps import _find_pps_daily_filepaths  # , find_pps_filepaths
-from gpm_api.utils.archive import (
-    check_file_integrity,
-    get_corrupted_filepaths,
-    remove_corrupted_filepaths,
-)
-from gpm_api.utils.utils_string import subset_list_by_boolean
-from gpm_api.utils.warnings import GPMDownloadWarning
+from gpm_api.io import GPM_VERSION # CURRENT GPM VERSION
+from gpm_api.configs import get_gpm_base_dir, get_gpm_username, get_gpm_password
 
 ### Currently we open a connection for every file
 ### We might want to launch wget in parallel directly
 ### - And then loop by day or month to display progress
 
 ## For https connection, it requires Authorization header: <type><credentials>
 # - type: "Basic"
@@ -163,44 +160,47 @@
     if n_threads < 1:
         n_threads = 1
     n_threads = min(n_threads, 10)
     n_cmds = len(commands)
     ##------------------------------------------------------------------------.
     # Run with progress bar
     if progress_bar is True:
-        with tqdm(total=n_cmds) as pbar, concurrent.futures.ThreadPoolExecutor(
-            max_workers=n_threads
-        ) as executor:
-            dict_futures = {
-                executor.submit(
-                    subprocess.check_call,
-                    cmd,
-                    shell=True,
-                    stdout=subprocess.DEVNULL,
-                    stderr=subprocess.DEVNULL,
-                ): cmd
-                for cmd in commands
-            }
-            # List cmds that didn't work
-            l_cmd_error = []
-            for future in concurrent.futures.as_completed(dict_futures.keys()):
-                pbar.update(1)  # Update the progress bar
-                # Collect all commands that caused problems
-                if future.exception() is not None:
-                    l_cmd_error.append(dict_futures[future])
+        with tqdm(total=n_cmds) as pbar:
+            with concurrent.futures.ThreadPoolExecutor(
+                max_workers=n_threads
+            ) as executor:
+                dict_futures = {
+                    executor.submit(
+                        subprocess.check_call,
+                        cmd,
+                        shell=True,
+                        stdout=subprocess.DEVNULL,
+                        stderr=subprocess.DEVNULL,
+                    ): cmd
+                    for cmd in commands
+                }
+                # List cmds that didn't work
+                l_cmd_error = []
+                for future in concurrent.futures.as_completed(dict_futures.keys()):
+                    pbar.update(1)  # Update the progress bar
+                    # Collect all commands that caused problems
+                    if future.exception() is not None:
+                        l_cmd_error.append(dict_futures[future])
     ##------------------------------------------------------------------------.
     # Run without progress bar
     else:
         if (n_threads == 1) and (verbose is True):
             # print("Here")
             # print(commands)
             _ = [subprocess.run(cmd, shell=True) for cmd in commands]
             l_cmd_error = []
         else:
-            with concurrent.futures.ThreadPoolExecutor(max_workers=n_threads) as executor:
+            with concurrent.futures.ThreadPoolExecutor(
+                max_workers=n_threads
+            ) as executor:
                 # Run commands and list those didn't work
                 dict_futures = {
                     executor.submit(
                         subprocess.check_call,
                         cmd,
                         shell=True,
                         stdout=subprocess.DEVNULL,
@@ -236,68 +236,66 @@
         with open(disk_path, "wb") as file:
             ftps.retrbinary(f"RETR {server_path}", file.write)
     except EOFError:
         return f"Impossible to download {server_path}"
 
     # Close the FTP connection
     ftps.close()
-    return None
 
 
 def ftplib_download(server_paths, disk_paths, username, password, n_threads=10):
     # Download file concurrently
     n_files = len(server_paths)
-    with tqdm(total=n_files) as pbar, concurrent.futures.ThreadPoolExecutor(
-        max_workers=n_threads
-    ) as executor:
-        dict_futures = {
-            executor.submit(
-                _download_with_ftlib,
-                server_path=server_path,
-                disk_path=disk_path,
-                username=username,
-                password=password,
-            ): server_path
-            for server_path, disk_path in zip(server_paths, disk_paths)
-        }
-        # List cmds that didn't work
-        l_cmd_error = []
-        for future in concurrent.futures.as_completed(dict_futures.keys()):
-            pbar.update(1)  # Update the progress bar
-            # Collect all commands that caused problems
-            if future.exception() is not None:
-                l_cmd_error.append(dict_futures[future])
-
-
-def _download_files(
-    src_fpaths,
-    dst_fpaths,
-    username,
-    password,
-    transfer_tool="wget",
-    n_threads=4,
-    progress_bar=True,
-    verbose=False,
-):
+    with tqdm(total=n_files) as pbar:
+        with concurrent.futures.ThreadPoolExecutor(max_workers=n_threads) as executor:
+            dict_futures = {
+                executor.submit(
+                    _download_with_ftlib,
+                    server_path=server_path,
+                    disk_path=disk_path,
+                    username=username,
+                    password=password,
+                ): server_path
+                for server_path, disk_path in zip(server_paths, disk_paths)
+            }
+            # List cmds that didn't work
+            l_cmd_error = []
+            for future in concurrent.futures.as_completed(dict_futures.keys()):
+                pbar.update(1)  # Update the progress bar
+                # Collect all commands that caused problems
+                if future.exception() is not None:
+                    l_cmd_error.append(dict_futures[future])
+
 
+def _download_files(src_fpaths, 
+                    dst_fpaths, 
+                    username,
+                    password,
+                    transfer_tool="wget", 
+                    n_threads=4,
+                    progress_bar=True,
+                    verbose=False):
+    
     if transfer_tool == "curl":
         list_cmd = [
             curl_cmd(src_path, dst_path, username, username)
             for src_path, dst_path in zip(src_fpaths, dst_fpaths)
         ]
     elif transfer_tool == "wget":
         list_cmd = [
             wget_cmd(src_path, dst_path, username, username)
             for src_path, dst_path in zip(src_fpaths, dst_fpaths)
         ]
     else:
         raise NotImplementedError("Download is available with 'wget' or 'curl'.")
     # -------------------------------------------------------------------------.
     ## Download the data (in parallel)
-    bad_cmds = run(list_cmd, n_threads=n_threads, progress_bar=progress_bar, verbose=verbose)
+    bad_cmds = run(
+        list_cmd, n_threads=n_threads, progress_bar=progress_bar, verbose=verbose
+    )
     return bad_cmds
 
 
 ####--------------------------------------------------------------------------.
 ############################
 #### Filtering routines ####
 ############################
@@ -349,44 +347,47 @@
     start_time = info_dict["start_time"]
     date = start_time.date()
     list_dirs = filepath.split(os.path.sep)
     product = list_dirs[-5]
     version = int(list_dirs[-7][2])
     product_type = list_dirs[-8]
     # base_dir = os.path.join(os.path.sep, *list_dirs[0:-8])
-
-    # Retrieve PPS filepath
-    url_data_server, url_file_list = get_pps_directory(
-        product=product, product_type=product_type, date=date, version=version
-    )
+    
+    # Retrieve PPS filepath 
+    url_data_server, url_file_list = get_pps_directory(product=product,
+                                                       product_type=product_type, 
+                                                       date=date,
+                                                       version=version)
     dir_tree = os.path.join(*url_file_list.split(os.path.sep)[4:])
     pps_filepath = os.path.join(url_data_server, dir_tree, filename)
     return pps_filepath
-
+    
 
 def convert_disk_to_pps_filepaths(filepaths):
     """
-    Convert GPM filename or filepaths to PPS filepaths.
+    Convert disk filepaths to PPS filepaths.
 
     Parameters
     ----------
     filepaths : list
         GPM file paths on disk.
-
+    
     Returns
     -------
     pps_filepaths : list
         List of file paths on PPS.
 
     """
     pps_fpaths = [_convert_disk_to_pps_fpath(fpath) for fpath in filepaths]
     return pps_fpaths
 
 
-def convert_pps_to_disk_filepaths(pps_filepaths, base_dir, product, product_type, version):
+def convert_pps_to_disk_filepaths(
+    pps_filepaths, base_dir, product, product_type, version
+):
     """
     Convert PPS filepaths to local disk filepaths.
 
     Parameters
     ----------
     pps_filepaths : list
         File paths on the PPS server.
@@ -432,15 +433,14 @@
     start_time=None,
     end_time=None,
     n_threads=10,
     transfer_tool="curl",
     progress_bar=True,
     force_download=False,
     verbose=True,
-    warn_missing_files=True,
 ):
     """
     Download GPM data from NASA servers using curl or wget.
 
     Parameters
     ----------
     base_dir : str
@@ -507,54 +507,50 @@
         base_dir=base_dir,
         product=product,
         product_type=product_type,
         version=version,
     )
     # -------------------------------------------------------------------------.
     ## If no file to retrieve on NASA PPS, return None
-    if is_empty(pps_filepaths) and warn_missing_files:
-        msg = f"No data found on PPS on date {date} for product {product}"
-        warnings.warn(msg, GPMDownloadWarning)
+    if is_empty(pps_filepaths):
+        # print("No data found on PPS on Date", Date, "for product", product)
         return None
 
     # -------------------------------------------------------------------------.
     ## If force_download is False, select only data not present on disk
     pps_filepaths, disk_filepaths = filter_download_list(
         disk_paths=disk_filepaths,
         server_paths=pps_filepaths,
         force_download=force_download,
     )
     # -------------------------------------------------------------------------.
     # Retrieve commands
-    bad_cmds = _download_files(
-        src_fpaths=pps_filepaths,
-        dst_fpaths=disk_filepaths,
-        username=username,
-        password=password,
-        n_threads=n_threads,
-        progress_bar=progress_bar,
-        verbose=verbose,
-    )
+    bad_cmds = _download_files(src_fpaths=pps_filepaths,
+                               dst_fpaths=disk_filepaths,
+                               username=username,
+                               password=password, 
+                               n_threads=n_threads,
+                               progress_bar=progress_bar,
+                               verbose=verbose)
     return bad_cmds
 
-
 ##-----------------------------------------------------------------------------.
 def download_data(
     product,
     start_time,
     end_time,
     product_type="RS",
     version=GPM_VERSION,
     n_threads=10,
     transfer_tool="curl",
     progress_bar=False,
     force_download=False,
     check_integrity=True,
     remove_corrupted=True,
-    retry=1,
+    retry=1, 
     verbose=True,
     base_dir=None,
     username=None,
     password=None,
 ):
     """
     Download GPM data from NASA servers (day by day).
@@ -584,43 +580,43 @@
         Whether to print processing details. The default is False.
     check_integrity: bool, optional
         Check integrity of the downloaded files.
         By default is True.
     remove_corrupted: bool, optional
         Whether to remove the corrupted files.
         By default is True.
-    retry : int, optional,
+    retry : int, optional, 
         The number of attempts to redownload the corrupted files. The default is 1.
         Only applies if check_integrity is True !
     base_dir : str, optional
-        The path to the GPM base directory. If None, it use the one specified
-        in the GPM-API config file.
+        The path to the GPM base directory. If None, it use the one specified 
+        in the GPM-API config file. 
         The default is None.
     username: str, optional
         Email address with which you registered on the NASA PPS.
-        If None, it uses the one specified in the GPM-API config file.
+        If None, it uses the one specified in the GPM-API config file. 
         The default is None.
     password: str, optional
         Email address with which you registered on the NASA PPS.
-        If None, it uses the one specified in the GPM-API config file.
+        If None, it uses the one specified in the GPM-API config file. 
         The default is None.
-
+    
     Returns
     -------
 
     boolean: int
         0 if everything went fine.
 
     """
     # -------------------------------------------------------------------------.
     # Retrieve GPM-API configs
     base_dir = get_gpm_base_dir(base_dir)
     username = get_gpm_username(username)
     password = get_gpm_password(password)
-
+    
     # -------------------------------------------------------------------------.
     ## Checks input arguments
     check_product_type(product_type=product_type)
     check_product(product=product, product_type=product_type)
     check_version(version=version)
     base_dir = check_base_dir(base_dir)
     start_time, end_time = check_start_end_time(start_time, end_time)
@@ -633,87 +629,71 @@
     start_date = start_date - datetime.timedelta(days=1)
     end_date = datetime.datetime(end_time.year, end_time.month, end_time.day)
     date_range = pd.date_range(start=start_date, end=end_date, freq="D")
     dates = list(date_range.to_pydatetime())
 
     # -------------------------------------------------------------------------.
     # Loop over dates and download the files
-    for i, date in enumerate(dates):
-        if i == 0:
-            warn_missing_files = False
-        else:
-            warn_missing_files = True
-
+    for date in dates:
         _ = _download_daily_data(
             base_dir=base_dir,
             username=username,
-            password=password,
             date=date,
             version=version,
             product=product,
             product_type=product_type,
             start_time=start_time,
             end_time=end_time,
             n_threads=n_threads,
             transfer_tool=transfer_tool,
             progress_bar=progress_bar,
             force_download=force_download,
             verbose=verbose,
-            warn_missing_files=warn_missing_files,
         )
 
     # -------------------------------------------------------------------------.
     if verbose:
-        print(f"The available GPM {product} product files are on disk.")
+        print(f"Download of available GPM {product} product completed.")
     if check_integrity:
         l_corrupted = check_file_integrity(
             base_dir=base_dir,
             product=product,
             start_time=start_time,
             end_time=end_time,
             version=version,
             product_type=product_type,
             remove_corrupted=remove_corrupted,
             verbose=verbose,
         )
         if verbose:
-            print("Integrity checking of GPM files has completed.")
-        if retry > 0 and remove_corrupted and len(l_corrupted) > 0:
-            if verbose:
-                print("Start attempts to redownload the corrupted files.")
-            l_corrupted = redownload_from_filepaths(
-                filepaths=l_corrupted,
-                username=username,
-                n_threads=n_threads,
-                transfer_tool=transfer_tool,
-                progress_bar=progress_bar,
-                verbose=verbose,
-                retry=retry,
-            )
+            print("Checking integrity of GPM files completed.")
+        if retry > 0 and remove_corrupted:
             if verbose:
-                if len(l_corrupted) == 0:
-                    print("All corrupted files have been redownloaded successively.")
-                else:
-                    print("Some corrupted files couldn't been redownloaded.")
-                    print("Returning the list of corrupted files.")
-                    return l_corrupted
+                print("Attempt to redownload the corrupted files.")
+            l_corrupted = redownload_from_filepaths(filepaths=l_corrupted,
+                                                    username=username,
+                                                    n_threads=n_threads,
+                                                    transfer_tool=transfer_tool,
+                                                    progress_bar=progress_bar,
+                                                    verbose=verbose,
+                                                    retry=retry)
+        return l_corrupted
     return None
 
 
 ####--------------------------------------------------------------------------.
-def redownload_from_filepaths(
-    filepaths,
-    n_threads=4,
-    transfer_tool="wget",
-    progress_bar=False,
-    verbose=True,
-    retry=1,
-    username=None,
-    password=None,
-):
+def redownload_from_filepaths(filepaths,
+                              n_threads=4,
+                              transfer_tool="wget",
+                              progress_bar=False,
+                              verbose=True,
+                              retry=1,
+                              username=None,
+                              password=None,
+                              ):
     """
     Redownload GPM files from the PPS archive.
 
     Parameters
     ----------
     filepaths : list
         List of disk filepaths.
@@ -721,74 +701,101 @@
         Number of parallel downloads. The default is set to 10.
     progress_bar : bool, optional
         Wheter to display progress. The default is True.
     transfer_tool : str, optional
         Wheter to use curl or wget for data download. The default is "curl".
     verbose : bool, optional
         Whether to print processing details. The default is False.
-    retry : int, optional,
+    retry : int, optional, 
         The number of attempts to redownload the corrupted files. The default is 1.
     username: str, optional
         Email address with which you registered on the NASA PPS.
-        If None, it uses the one specified in the GPM-API config file.
+        If None, it uses the one specified in the GPM-API config file. 
         The default is None.
     password: str, optional
         Email address with which you registered on the NASA PPS.
-        If None, it uses the one specified in the GPM-API config file.
+        If None, it uses the one specified in the GPM-API config file. 
         The default is None.
-
+          
     Returns
     -------
     l_corrupted : list
         List of remaining corrupted file paths.
     """
-    if isinstance(filepaths, type(None)):
-        return None
+    if isinstance(filepaths, type(None)): 
+        return None 
     if not isinstance(filepaths, list):
         raise TypeError("Expecting a list of filepaths.")
-    if len(filepaths) == 0:
+    if len(filepaths) == 0: 
         return None
-
+    
     # -------------------------------------------------------------------------.
     # Retrieve GPM-API configs
     username = get_gpm_username(username)
     password = get_gpm_password(password)
-
+    
     # -------------------------------------------------------------------------.
     # Attempt to redownload the corrupted files
-    if verbose:
+    if verbose: 
         n_files = len(filepaths)
         print(f"Attempt to redownload {n_files}.")
-
-    # Retrieve the PPS file paths
+        
+    # Retrieve the PPS file paths 
     pps_filepaths = convert_disk_to_pps_filepaths(filepaths)
-
-    # Download files
-    _ = _download_files(
-        src_fpaths=pps_filepaths,
-        dst_fpaths=filepaths,
-        username=username,
-        password=password,
-        n_threads=n_threads,
-        progress_bar=progress_bar,
-        verbose=verbose,
-    )
-
-    # Get corrupted filepaths
+       
+    # Download files     
+    _ = _download_files(src_fpaths=pps_filepaths,
+                        dst_fpaths=filepaths,
+                        username=username,
+                        password=password, 
+                        n_threads=n_threads,
+                        progress_bar=progress_bar,
+                        verbose=verbose)
+    
+    # Get corrupted filepaths 
     l_corrupted = get_corrupted_filepaths(filepaths)
-
     # Remove corrupted filepaths
     remove_corrupted_filepaths(filepaths=l_corrupted, verbose=verbose)
-
-    # Retry download if retry > 1 as input argument
-    if len(l_corrupted) > 0 and retry > 1:
+    # Retry download if retry > 1 as input argument 
+    if len(l_corrupted) > 0 and retry > 1: 
         l_corrupted = redownload_from_filepaths(
             filepaths=l_corrupted,
-            username=username,
+            username=username, 
             n_threads=n_threads,
             transfer_tool=transfer_tool,
             progress_bar=progress_bar,
             verbose=verbose,
-            retry=retry - 1,
-        )
-
-    return l_corrupted
+            retry=retry-1,
+            )
+        
+    ### Old single process, slow 
+    # for fpath in filepaths:
+    #     # Extract file information from filepath
+    #     info_dict = get_info_from_filepath(fpath)
+    #     start_time = info_dict["start_time"]
+    #     end_time = info_dict["end_time"]
+    #     list_dirs = fpath.split(os.path.sep)
+    #     product = list_dirs[-5]
+    #     version = int(list_dirs[-7][2])
+    #     product_type = list_dirs[-8]
+    #     base_dir = os.path.join(os.path.sep, *list_dirs[0:-8])
+    #     # Redownload the file 
+    #     l_corrupted_fpath = download_data(
+    #         base_dir=base_dir,
+    #         username=username,
+    #         product=product,
+    #         start_time=start_time,
+    #         end_time=end_time,
+    #         product_type=product_type,
+    #         version=version,
+    #         n_threads=1,
+    #         transfer_tool=transfer_tool,
+    #         progress_bar=progress_bar,
+    #         force_download=force_download,
+    #         check_integrity=True,
+    #         remove_corrupted=True,
+    #         verbose=verbose,
+    #         retry=retry-1,
+    #     )
+    #     if len(l_corrupted_fpath) != 0:
+    #         l_corrupted.append(l_corrupted_fpath[0])
+    return l_corrupted
```

### Comparing `gpm_api-0.2.2/gpm_api/io/filter.py` & `gpm_api-0.2.3/gpm_api/io/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Thu Oct 13 11:30:46 2022
 
 @author: ghiggi
 """
-import datetime
 import re
-
+import datetime
 import numpy as np
-
 from gpm_api.io.checks import (
-    check_filepaths,
     check_product,
+    check_filepaths,
     check_start_end_time,
     check_version,
 )
+from gpm_api.utils.utils_string import str_subset
+from gpm_api.io.patterns import GPM_products_pattern_dict
 from gpm_api.io.info import (
-    get_info_from_filepath,
     get_start_end_time_from_filepaths,
     get_version_from_filepaths,
+    get_info_from_filepath,
 )
-from gpm_api.io.patterns import GPM_products_pattern_dict
-from gpm_api.utils.utils_string import str_subset
 
 
 def is_granule_within_time(start_time, end_time, file_start_time, file_end_time):
     """Check if a granule is within start_time and end_time."""
     # - Case 1
     #     s               e
     #     |               |
@@ -49,15 +48,17 @@
 
 ####--------------------------------------------------------------------------.
 ##########################
 #### Filter filepaths ####
 ##########################
 
 
-def _filter_filepath(filepath, product=None, version=None, start_time=None, end_time=None):
+def _filter_filepath(
+    filepath, product=None, version=None, start_time=None, end_time=None
+):
     """
     Check if a single filepath pass the filtering parameters.
 
     If do not match the filtering criteria, it returns None.
 
     Parameters
     ----------
@@ -86,15 +87,15 @@
     """
 
     info_dict = get_info_from_filepath(filepath)
 
     # Filter by version
     if version is not None:
         file_version = info_dict["version"]
-        file_version = int(re.findall("\\d+", file_version)[0])
+        file_version = int(re.findall("\d+", file_version)[0])
         if file_version != version:
             return None
 
     # Filter by product
     # - TODO with info_dict once we have dictionary mapping patterns to filepath product acronyms
     if product is not None:
         gpm_pattern_dict = GPM_products_pattern_dict()
@@ -102,15 +103,17 @@
         if filepath is None:
             return None
 
     # Filter by start_time and end_time
     if start_time is not None and end_time is not None:
         file_start_time = info_dict["start_time"]
         file_end_time = info_dict["end_time"]
-        if not is_granule_within_time(start_time, end_time, file_start_time, file_end_time):
+        if not is_granule_within_time(
+            start_time, end_time, file_start_time, file_end_time
+        ):
             return None
 
     return filepath
 
 
 def filter_filepaths(
     filepaths,
```

### Comparing `gpm_api-0.2.2/gpm_api/io/info.py` & `gpm_api-0.2.3/gpm_api/io/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sun Aug 14 20:49:06 2022
 
 @author: ghiggi
 """
-import datetime
-import os
 import re
-
+import os
+import datetime
 import numpy as np
 from trollsift import Parser
-
 from gpm_api.io.patterns import GPM_products_pattern_dict
 
 ####---------------------------------------------------------------------------
 ########################
 #### FNAME PATTERNS ####
 ########################
 # General pattern for all GPM products
-NASA_FNAME_PATTERN = "{product_level:s}.{satellite:s}.{sensor:s}.{algorithm:s}.{start_date:%Y%m%d}-S{start_time:%H%M%S}-E{end_time:%H%M%S}.{granule_id}.{version}.{data_format}"  # noqa
+NASA_FNAME_PATTERN = "{product_level:s}.{satellite:s}.{sensor:s}.{algorithm:s}.{start_date:%Y%m%d}-S{start_time:%H%M%S}-E{end_time:%H%M%S}.{granule_id}.{version}.{data_format}"
 # General pattern for all JAXA products
 # - Pattern for 1B-Ku and 1B-Ka
-JAXA_FNAME_PATTERN = "{mission_id}_{sensor:s}_{start_date_time:%y%m%d%H%M}_{end_time:%H%M}_{granule_id}_{product_level:2s}{product_type}_{algorithm:s}_{version}.{data_format}"  # noqa
+JAXA_FNAME_PATTERN = "{mission_id}_{sensor:s}_{start_date_time:%y%m%d%H%M}_{end_time:%H%M}_{granule_id}_{product_level:2s}{product_type}_{algorithm:s}_{version}.{data_format}"
 
 ####---------------------------------------------------------------------------.
 ##########################
 #### Filename parsers ####
 ##########################
 
 
@@ -147,22 +146,24 @@
     list_product = [get_product_from_filepath(fpath) for fpath in filepaths]
     return list_product
 
 
 def get_version_from_filepath(filepath, integer=True):
     version = get_key_from_filepath(filepath, key="version")
     if integer:
-        version = int(re.findall("\\d+", version)[0])
+        version = int(re.findall("\d+", version)[0])
     return version
 
 
 def get_version_from_filepaths(filepaths, integer=True):
     if isinstance(filepaths, str):
         filepaths = [filepaths]
-    list_version = [get_version_from_filepath(fpath, integer=integer) for fpath in filepaths]
+    list_version = [
+        get_version_from_filepath(fpath, integer=integer) for fpath in filepaths
+    ]
     return list_version
 
 
 def get_granule_from_filepaths(filepaths):
     list_id = get_key_from_filepaths(filepaths, key="granule_id")
     return list_id
```

### Comparing `gpm_api-0.2.2/gpm_api/io/patterns.py` & `gpm_api-0.2.3/gpm_api/io/patterns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Thu Oct 13 11:12:31 2022
 
 @author: ghiggi
 """
 # ----------------------------------------------------------------------------.
 #################################
@@ -14,16 +15,16 @@
     GPM_dict = {"1B-PR": "1B.TRMM.PR*", "1B-Ka": "GPMCOR_KAR*", "1B-Ku": "GPMCOR_KUR*"}
     return GPM_dict
 
 
 def GPM_RADAR_2A_RS_pattern_dict():
     """Return the filename pattern* associated to GPM DPR 2A RS products."""
     GPM_dict = {
-        "2A-PR": "2A.TRMM.PR.V\\d-*",  # to distinguish from SLH
-        "2A-DPR": "2A.GPM.DPR.V\\d-*",  # to distinguish from SLH
+        "2A-PR": "2A.TRMM.PR.V\d-*",  # to distinguish from SLH
+        "2A-DPR": "2A.GPM.DPR.V\d-*",  # to distinguish from SLH
         "2A-Ka": "2A.GPM.Ka.V*",
         "2A-Ku": "2A.GPM.Ku.V*",
         "2A-ENV-PR": "2A-ENV.TRMM.PR.V*",
         "2A-ENV-DPR": "2A-ENV.GPM.DPR.V*",
         "2A-ENV-Ka": "2A-ENV.GPM.Ka.V*",
         "2A-ENV-Ku": "2A-ENV.GPM.Ku.V*",
         "2A-GPM-SLH": "2A.GPM.DPR.GPM-SLH*",
@@ -31,15 +32,15 @@
     }
     return GPM_dict
 
 
 def GPM_RADAR_2A_NRT_pattern_dict():
     """Return the filename pattern* associated to GPM DPR 2A NRT products."""
     GPM_dict = {
-        "2A-DPR": "2A.GPM.DPR.V\\d-*",  # to distinguish from SLH
+        "2A-DPR": "2A.GPM.DPR.V\d-*",  # to distinguish from SLH
         "2A-Ka": "2A.GPM.Ka.V*",
         "2A-Ku": "2A.GPM.Ku.V*",
     }
     return GPM_dict
 
 
 def GPM_RADAR_RS_pattern_dict():
```

### Comparing `gpm_api-0.2.2/gpm_api/io/pps.py` & `gpm_api-0.2.3/gpm_api/io/pps.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,37 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Thu Oct 13 17:45:37 2022
 
 @author: ghiggi
 """
-import datetime
 import os
-import subprocess
-
 import dask
-import numpy as np
+import datetime
+import subprocess
 import pandas as pd
 
-from gpm_api.configs import get_gpm_password, get_gpm_username
-from gpm_api.io import GPM_VERSION  # CURRENT GPM VERSION
 from gpm_api.io.checks import (
     check_date,
+    check_start_end_time,
     check_product,
     check_product_type,
-    check_start_end_time,
     check_version,
     is_empty,
 )
-from gpm_api.io.directories import get_pps_directory
 from gpm_api.io.filter import filter_filepaths
-from gpm_api.io.info import get_version_from_filepaths
-
-
-def _check_correct_version(filepaths, product, version):
-    """Check correct file version.
-
-    If 'version' is the last version, we retrieve data from 'gpmalldata' directory.
-    But many products are not available to the last version.
-    So to archive data correctly on the user side, we check that the file version
-    actually match the asked version, and otherwise we suggest the last available version.
-    """
-    file_versions = np.unique(get_version_from_filepaths(filepaths, integer=True)).tolist()
-    if len(file_versions) > 1:
-        raise ValueError(
-            f"Multiple file versions found: {file_versions}. Please report their occurence !"
-        )
-    file_version = file_versions[0]
-    if file_version != version:
-        raise ValueError(
-            f"The last available version for {product} product is version {file_version} !"
-        )
-    return filepaths
+from gpm_api.io.directories import get_pps_directory
+from gpm_api.io import GPM_VERSION # CURRENT GPM VERSION
+from gpm_api.configs import get_gpm_username, get_gpm_password
 
 
-def _get_pps_file_list(username, password, url_file_list, product, date, version, verbose=True):
+def _get_pps_file_list(username, 
+                       password, 
+                       url_file_list, product, date, version, verbose=True):
     """
     Retrieve the filepaths of the files available on the NASA PPS server for a specific day and product.
 
     The query is done using https !
     The function does not return the full PPS server url, but the filepath
     from the server root: i.e: '/gpmdata/2020/07/05/radar/<...>.HDF5'
 
@@ -91,15 +70,17 @@
         )
         raise ValueError("Sorry for the incovenience.")
 
     # Check if data are available
     if stdout[0] == "<":
         if verbose:
             version_str = str(int(version))
-            print(f"No data found on PPS on date {date} for product {product} (V0{version_str})")
+            print(
+                f"No data found on PPS on date {date} for product {product} (V0{version_str})"
+            )
         return []
     else:
         # Retrieve filepaths
         filepaths = stdout.split()
 
     # Return file paths
     return filepaths
@@ -155,15 +136,15 @@
 
 
 ##-----------------------------------------------------------------------------.
 
 
 def _find_pps_daily_filepaths(
     username,
-    password,
+    password, 
     date,
     product,
     product_type,
     version,
     start_time=None,
     end_time=None,
     verbose=False,
@@ -204,26 +185,22 @@
     # Check date
     date = check_date(date)
 
     ##------------------------------------------------------------------------.
     # Retrieve list of available files on pps
     filepaths = _get_pps_daily_filepaths(
         username=username,
-        password=password,
         product=product,
         product_type=product_type,
         date=date,
         version=version,
         verbose=verbose,
     )
     if is_empty(filepaths):
         return []
-    ## -----------------------------------------------------------------------.
-    ## Check correct version
-    filepaths = _check_correct_version(filepaths=filepaths, product=product, version=version)
 
     ##------------------------------------------------------------------------.
     # Filter the GPM daily file list (for product, start_time & end time)
     filepaths = filter_filepaths(
         filepaths,
         product=product,
         product_type=product_type,
@@ -241,15 +218,15 @@
     product,
     start_time,
     end_time,
     product_type="RS",
     version=GPM_VERSION,
     verbose=True,
     parallel=True,
-    username=None,
+    username=None, 
     password=None,
 ):
     """
     Retrieve GPM data filepaths on NASA PPS server a specific time period and product.
 
     Parameters
     ----------
@@ -263,37 +240,37 @@
         GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
     version : int, optional
         GPM version of the data to retrieve if product_type = 'RS'.
     parallel : bool, optional
         Whether to loop over dates in parallel.
         The default is True.
     base_dir : str, optional
-        The path to the GPM base directory. If None, it use the one specified
-        in the GPM-API config file.
+        The path to the GPM base directory. If None, it use the one specified 
+        in the GPM-API config file. 
         The default is None.
     username: str, optional
         Email address with which you registered on the NASA PPS.
-        If None, it uses the one specified in the GPM-API config file.
+        If None, it uses the one specified in the GPM-API config file. 
         The default is None.
     password: str, optional
         Password to access the NASA PPS server.
-        If None, it uses the one specified in the GPM-API config file.
+        If None, it uses the one specified in the GPM-API config file. 
         The default is None.
-
+        
     Returns
     -------
     filepaths : list
         List of GPM filepaths.
 
     """
     # -------------------------------------------------------------------------.
     # Retrieve GPM-API configs
     username = get_gpm_username(username)
     password = get_gpm_password(password)
-
+    
     # -------------------------------------------------------------------------.
     ## Checks input arguments
     check_version(version=version)
     check_product_type(product_type=product_type)
     check_product(product=product, product_type=product_type)
     start_time, end_time = check_start_end_time(start_time, end_time)
     # Retrieve sequence of dates
```

### Comparing `gpm_api-0.2.2/gpm_api/io/products.py` & `gpm_api-0.2.3/gpm_api/io/products.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Thu Oct 13 11:13:15 2022
 
 @author: ghiggi
 """
 import numpy as np
-
 from gpm_api.io.patterns import (
     GPM_1B_NRT_pattern_dict,
-    GPM_1B_RS_pattern_dict,
     GPM_2A_NRT_pattern_dict,
-    GPM_2A_RS_pattern_dict,
     GPM_2B_NRT_pattern_dict,
+    GPM_1B_RS_pattern_dict,
+    GPM_2A_RS_pattern_dict,
     GPM_2B_RS_pattern_dict,
-    GPM_CMB_2B_NRT_pattern_dict,
-    GPM_CMB_2B_RS_pattern_dict,
-    GPM_CMB_NRT_pattern_dict,
-    GPM_CMB_RS_pattern_dict,
-    GPM_IMERG_NRT_pattern_dict,
-    GPM_IMERG_pattern_dict,
-    GPM_IMERG_RS_pattern_dict,
+    GPM_RADAR_1B_RS_pattern_dict,
+    GPM_RADAR_2A_RS_pattern_dict,
+    GPM_RADAR_2A_NRT_pattern_dict,
     GPM_PMW_1A_RS_pattern_dict,
-    GPM_PMW_1B_NRT_pattern_dict,
     GPM_PMW_1B_RS_pattern_dict,
-    GPM_PMW_1C_NRT_pattern_dict,
     GPM_PMW_1C_RS_pattern_dict,
-    GPM_PMW_2A_GPROF_NRT_pattern_dict,
+    GPM_PMW_2A_PRPS_RS_pattern_dict,
     GPM_PMW_2A_GPROF_RS_pattern_dict,
+    GPM_PMW_1B_NRT_pattern_dict,
+    GPM_PMW_1C_NRT_pattern_dict,
     GPM_PMW_2A_PRPS_NRT_pattern_dict,
-    GPM_PMW_2A_PRPS_RS_pattern_dict,
-    GPM_PMW_NRT_pattern_dict,
+    GPM_PMW_2A_GPROF_NRT_pattern_dict,
+    GPM_CMB_2B_NRT_pattern_dict,
+    GPM_CMB_2B_RS_pattern_dict,
+    GPM_RADAR_RS_pattern_dict,
     GPM_PMW_RS_pattern_dict,
-    GPM_RADAR_1B_RS_pattern_dict,
-    GPM_RADAR_2A_NRT_pattern_dict,
-    GPM_RADAR_2A_RS_pattern_dict,
+    GPM_CMB_RS_pattern_dict,
+    GPM_IMERG_RS_pattern_dict,
     GPM_RADAR_NRT_pattern_dict,
-    GPM_RADAR_RS_pattern_dict,
+    GPM_CMB_NRT_pattern_dict,
+    GPM_PMW_NRT_pattern_dict,
+    GPM_IMERG_NRT_pattern_dict,
+    GPM_IMERG_pattern_dict,
 )
 
-
 ####--------------------------------------------------------------------------.
 ###########################
 ### Available products ####
 ###########################
 ##----------------------------------------------------------------------------.
 #### RADAR
 def GPM_RADAR_1B_RS_products():
```

### Comparing `gpm_api-0.2.2/gpm_api/io/scan_modes.py` & `gpm_api-0.2.3/gpm_api/io/scan_modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Thu Oct 13 11:26:27 2022
 
 @author: ghiggi
 """
 from gpm_api.io.products import (
     GPM_IMERG_products,
```

### Comparing `gpm_api-0.2.2/gpm_api/overpass/TODO_GPM_OVERPASS.py` & `gpm_api-0.2.3/gpm_api/overpass/TODO_GPM_OVERPASS.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # /usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Tue Aug  2 10:43:23 2022
 
 @author: ghiggi
 """
-import datetime
 import os
-
 import dask
-import numpy as np
+import datetime
 import pandas as pd
-from dask.diagnostics import ProgressBar
+import numpy as np
 
-from gpm_api.dataset import GPM_Dataset
-from gpm_api.io import GPM_PMW_2A_GPROF_RS_products, download_GPM_data
+from gpm_api.io import download_GPM_data, GPM_PMW_2A_GPROF_RS_products
+from gpm_api.dataset import GPM_Dataset, GPM_variables, read_GPM, GPM_Dataset
+from dask.diagnostics import ProgressBar
 
 BASE_DIR = "/home/ghiggi"
 OVERPASS_TABLE_DIR = "/home/ghiggi/Overpass/Tables"
 username = "gionata.ghiggi@epfl.ch"
 
 #### Define analysis time period
 start_time = datetime.datetime.strptime("2020-08-01 12:00:00", "%Y-%m-%d %H:%M:%S")
```

### Comparing `gpm_api-0.2.2/gpm_api/overpass/TODO_OVERPASS_STATS.py` & `gpm_api-0.2.3/gpm_api/overpass/TODO_OVERPASS_STATS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import datetime
 import os
+import datetime
 import time
-
 import numpy as np
 import pandas as pd
-
-from gpm_api.io import GPM_PMW_2A_GPROF_RS_products
+import dask.dataframe as dd
+from gpm_api.io import download_GPM_data, GPM_PMW_2A_GPROF_RS_products
+from gpm_api.dataset import GPM_Dataset, GPM_variables, read_GPM, GPM_Dataset
 
 # from distributed import Client, LocalCluster
 # # Set Dask Client
 # client = Client(processes=False)
 # client = Client(processes=True)  # LTESRV1 DEFAULT: 6 PROCESSES AND 4 THREADS EACH
 # cluster = LocalCluster(n_workers = 12,        # n processes
 #                        threads_per_worker=2, # n_workers*threads_per_worker
```

### Comparing `gpm_api-0.2.2/gpm_api/patch/labels.py` & `gpm_api-0.2.3/gpm_api/patch/labels.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,329 +1,292 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Wed Oct 19 19:34:53 2022
 
 @author: ghiggi
 """
+import numpy as np
+import xarray as xr
 # import dask_image.ndmeasure
 # from dask_image.ndmeasure import as dask_label_image
 import dask_image.ndmeasure
-import numpy as np
-import xarray as xr
 from skimage.measure import label as label_image
 from skimage.morphology import binary_dilation, disk
 
-# TODO:
+# TODO: 
 # - xr_get_label_stats
 # - Enable to label in n-dimensions
 #   - (2D+VERTICAL) --> CORE PROFILES
 #   - (2D+TIME) --> TRACKING
 
-# Future internal renaming:
+# Future internal renaming: 
 # - get_areas_labels --> get_labels
 # - xr_get_areas_labels --> xr_get_labels
 
 # Note
 # - label_xarray_object available as ds.gpm_api.label_object
 
 ####--------------------------------------------------------------------------.
 #####################
 #### Area labels ####
 #####################
 def _mask_buffer(mask, footprint):
     """Dilate the mask by n pixel in all directions.
-
+    
     If footprint = 0 or None, no dilation occur.
     If footprint is a positive integer, it create a disk(footprint)
-    If footprint is a 2D array, it must represent the neighborhood expressed
+    If footprint is a 2D array, it must represent the neighborhood expressed 
     as a 2-D array of 1’s and 0’s.
     For more info: https://scikit-image.org/docs/stable/api/skimage.morphology.html#skimage.morphology.binary_dilation
-
+    
     """
     # scikitimage > 0.19
     if not isinstance(footprint, (int, np.ndarray, type(None))):
         raise TypeError("`footprint` must be an integer, numpy 2D array or None.")
-    if isinstance(footprint, np.ndarray) and footprint.ndim != 2:
-        raise ValueError("If providing the footprint for dilation as np.array, it must be 2D.")
+    if isinstance(footprint, np.ndarray): 
+        if footprint.ndim != 2: 
+            raise ValueError("If providing the footprint for dilation as np.array, it must be 2D.")
     if isinstance(footprint, int):
-        if footprint < 0:
+        if footprint < 0: 
             raise ValueError("Footprint must be equal or larger than 1.")
-        footprint = None if footprint == 0 else disk(radius=footprint)
+        if footprint == 0: 
+            footprint = None 
+        else:
+            footprint = disk(radius=footprint)
     # Apply dilation
     if footprint is not None:
         mask = binary_dilation(mask, footprint=footprint)
-    return mask
-
+    return mask    
 
 def _check_array(arr):
-    """Check array and return a numpy array."""
     shape = arr.shape
     if len(shape) != 2:
         raise ValueError("Expecting a 2D array.")
     if np.any(np.array(shape) == 0):
         raise ValueError("Expecting non-zero dimensions.")
 
     if not isinstance(arr, np.ndarray):
         arr = arr.compute()
     return arr
 
 
 def _no_labels_result(arr):
-    """Define results for array without labels."""
     labels = np.zeros(arr.shape)
     n_labels = 0
-    values = []
-    return labels, n_labels, values
+    counts = []
+    return labels, n_labels, counts
 
-
-def check_sort_by(stats):
-    """Check 'sort_by' argument."""
-    if not (callable(stats) or isinstance(stats, str)):
-        raise TypeError("'sort_by' must be a string or a function.")
-    if isinstance(stats, str):
-        valid_stats = [
-            "area",
-            "maximum",
-            "mininum",
-            "mean",
-            "median",
-            "sum",
-            "standard_deviation",
-            "variance",
-        ]
-        if stats not in valid_stats:
-            raise ValueError(f"Valid 'sort_by' values are: {valid_stats}.")
-
-
-def _check_stats(stats):
-    """Check 'stats' argument."""
-    if not (callable(stats) or isinstance(stats, str)):
-        raise TypeError("'stats' must be a string or a function.")
-    if isinstance(stats, str):
-        valid_stats = [
-            "area",
-            "maximum",
-            "mininum",
-            "mean",
-            "median",
-            "sum",
-            "standard_deviation",
-            "variance",
-        ]
-        if stats not in valid_stats:
-            raise ValueError(f"Valid 'stats' values are: {valid_stats}.")
-    # TODO: check stats function works on a dummy array (reduce to single value)
-    return stats
+    
+def check_sort_by(value):
+    valid_values = ["area", "max", "min", "sum", "mean", "median", "sd"]
+    if not isinstance(value, str):
+        raise TypeError(
+            f"'sort_by' must be a string. Valid values are: {valid_values} ."
+        )
+    if value not in valid_values:
+        raise TypeError(f"Valid 'sort_by' values are: {valid_values}.")
 
 
 def _get_label_value_stats(arr, label_arr, label_indices=None, stats="area"):
     """Compute label value statistics over which to later sort on.
-
-    If label_indices is None, by default would return the stats of the entire array
-    If label_indices is 0, return nan
-    If label_indices is not inside label_arr, return 0
+    
+    If labels_indices is None, it compute the statistic for each label.
     """
-    # Check stats argument and label indices
-    stats = _check_stats(stats)
+    # For custom function:
+    # https://image.dask.org/en/latest/dask_image.ndmeasure.html#dask_image.ndmeasure.labeled_comprehension
+    # Note:
+    # - if label_indices None, by default would return the stats of the entire array  
+    # - if label_indices is 0, return nan
+    # - If label_indices is not inside label_arr, return 0 
+    
     if label_indices is None:
         label_indices = np.unique(label_arr)
-    # Compute labels stats values
-    if callable(stats):
-        values = dask_image.ndmeasure.labeled_comprehension(
-            image=arr,
-            label_image=label_arr,
-            index=label_indices,
-            func=stats,
-            out_dtype=float,
-            pass_positions=False,
+        
+    if stats == "area":
+        values = dask_image.ndmeasure.area(
+            image=arr, label_image=label_arr, index=label_indices
+        )
+    elif stats == "max":
+        values = dask_image.ndmeasure.maximum(
+            image=arr, label_image=label_arr, index=label_indices
+        )
+    elif stats == "min":
+        values = dask_image.ndmeasure.minimum(
+            image=arr, label_image=label_arr, index=label_indices
+        )
+    elif stats == "mean":
+        values = dask_image.ndmeasure.mean(
+            image=arr, label_image=label_arr, index=label_indices
+        )
+    elif stats == "median":
+        values = dask_image.ndmeasure.median(
+            image=arr, label_image=label_arr, index=label_indices
+        )
+    elif stats == "sum":
+        values = dask_image.ndmeasure.sum_labels(
+            image=arr, label_image=label_arr, index=label_indices
+        )
+    elif stats == "sd":
+        values = dask_image.ndmeasure.standard_deviation(
+            image=arr, label_image=label_arr, index=label_indices
         )
     else:
-        func = getattr(dask_image.ndmeasure, stats)
-        values = func(image=arr, label_image=label_arr, index=label_indices)
+        raise NotImplementedError()
     # Compute values
     values = values.compute()
     # Return values
     return values
 
 
-def get_labels_stats(arr, label_arr, label_indices=None, stats="area", sort_decreasing=True):
+def get_labels_stats(arr, 
+                     label_arr,
+                     label_indices=None, 
+                     stats="area",
+                     sort_decreasing=True):
     """Return label and label statistics sorted by statistic value."""
-    # Get labels area values
+    # Get labels area values 
     values = _get_label_value_stats(
         arr, label_arr=label_arr, label_indices=label_indices, stats=stats
     )
-    # Get sorting index based on values
-    sort_index = np.argsort(values)[::-1] if sort_decreasing else np.argsort(values)
+    # Get sorting index based on values 
+    if sort_decreasing:
+        sort_index = np.argsort(values)[::-1]
+    else:
+        sort_index = np.argsort(values)
 
     # Sort values
     values = values[sort_index]
     label_indices = label_indices[sort_index]
-
-    return label_indices, values
+    
+    return label_indices, values 
 
 
 def _vec_translate(arr, my_dict):
     """Remap array <value> based on the dictionary key-value pairs.
 
     This function is used to redefine label array integer values based on the
     label area_size/max_intensity value.
 
     """
     return np.vectorize(my_dict.__getitem__)(arr)
 
 
+
 def get_labels_with_requested_occurence(label_arr, vmin, vmax):
     "Get label indices with requested occurence."
-    # Compute label occurence
+    # Compute label occurence 
     label_indices, label_occurence = np.unique(label_arr, return_counts=True)
 
-    # Remove label 0 and associate pixel count if present
-    if label_indices[0] == 0:
+    # Remove label 0 and associate pixel count if present 
+    if label_indices[0] == 0: 
         label_indices = label_indices[1:]
         label_occurence = label_occurence[1:]
-    # Get index with required occurence
-    valid_area_indices = np.where(np.logical_and(label_occurence >= vmin, label_occurence <= vmax))[
-        0
-    ]
-    # Return list of valid label indices
-    label_indices = label_indices[valid_area_indices] if len(valid_area_indices) > 0 else []
+    # Get index with required occurence 
+    valid_area_indices = np.where(
+        np.logical_and(
+            label_occurence >= vmin,
+            label_occurence <= vmax))[0]
+    # Return list of valid label indices 
+    if len(valid_area_indices) > 0:
+        label_indices = label_indices[valid_area_indices]
+    else: 
+        label_indices = []
     return label_indices
 
 
-def redefine_label_array(label_arr, label_indices=None):
+def redefine_label_array(label_arr, label_indices=None): 
     """Redefine labels of a label array from 0 to len(label_indices).
-
+    
     If label_indices is None, it takes the unique values of label_arr.
-    If label_indices contains a 0, it is discarded !
+    If label_indices contains a 0, it is discarded ! 
     If label_indices is not unique, raise an error !
-
+    
     Native label values not present in label_indices are set to 0.
     The first label in label_indices becomes 1, the second 2, and so on.
     """
-    if label_indices is None:
+    if label_indices is None: 
         label_indices = np.unique(label_arr)
-    else:
-        # Check unique values are provided
+    else: 
+        # Check unique values are provided 
         _, c = np.unique(label_indices, return_counts=True)
         if np.any(c > 1):
             raise ValueError("'label_indices' must be uniques.")
-
-    # Remove 0 and nan if present in label_indices
+            
+    # Remove 0 and nan if present in label_indices 
     label_indices = np.delete(label_indices, np.where(label_indices == 0)[0].flatten())
     label_indices = np.delete(label_indices, np.where(np.isnan(label_indices))[0].flatten())
-
-    # Ensure label indices are integer
+    
+    # Ensure label indices are integer 
     label_indices = label_indices.astype(int)
-
-    # Remove nan from label_arr
+    
+    # Remove nan from label_arr 
     label_arr[np.isnan(label_arr)] = 0
-
-    # Compute max label index
+    
+    # Compute max label index 
     max_label = max(label_indices)
-
+    
     # Set to 0 labels in label_arr larger than max_label
     # - These are some of the labels that were set to 0 because of mask or area filtering
-    label_arr[label_arr > max_label] = 0
-
+    label_arr[label_arr > max_label] = 0 
+    
     # Initialize dictionary with keys corresponding to all possible labels indices
-    val_dict = {k: 0 for k in range(0, max_label + 1)}
-
+    val_dict = {k: 0 for k in range(0, max_label+1)}
+    
     # Update the dictionary keys with the selected label_indices
     # - Assume 0 not in label_indices
     n_labels = len(label_indices)
     label_indices = label_indices.tolist()
     label_indices_new = np.arange(1, n_labels + 1).tolist()
     for k, v in zip(label_indices, label_indices_new):
         val_dict[k] = v
-
-    # Remove keys not in label_arr
-    # TODO: to speed up _vec_translate maybe
-
-    # Redefine the id of the labels
+        
+    # Remove keys not in label_arr 
+    # TODO: to speed up _vec_translate maybe 
+    
+    # Redefine the id of the labels 
     labels_arr = _vec_translate(label_arr, val_dict)
-
+    
     return labels_arr
 
-
+    
 ####--------------------------------------------------------------------------.
 def get_areas_labels(
     arr,
     min_value_threshold=-np.inf,
     max_value_threshold=np.inf,
     min_area_threshold=1,
     max_area_threshold=np.inf,
     footprint=None,
     sort_by="area",
     sort_decreasing=True,
 ):
-    """
-    Function deriving the labels array and associated labels info.
-
-    Parameters
-    ----------
-    arr : TYPE
-        DESCRIPTION.
-    min_value_threshold : float, optional
-        The minimum value to define the interior of a label.
-        The default is -np.inf.
-    max_value_threshold : float, optional
-        The maximum value to define the interior of a label.
-        The default is np.inf.
-    min_area_threshold : float, optional
-        The minimum number of connected pixels to be defined as a label.
-        The default is 1.
-    max_area_threshold : float, optional
-        The maximum number of connected pixels to be defined as a label.
-        The default is np.inf.
-    footprint : (int, np.ndarray or None), optional
-        This argument enables to dilate the mask derived after applying
-        min_value_threshold and max_value_threshold.
-        If footprint = 0 or None, no dilation occur.
-        If footprint is a positive integer, it create a disk(footprint)
-        If footprint is a 2D array, it must represent the neighborhood expressed
-        as a 2-D array of 1’s and 0’s.
-        The default is None (no dilation).
-    sort_by : (callable or str), optional
-        A function or statistics to define the order of the labels.
-        Valid string statistics are "area", "maximum", "mininum", "mean",
-        "median", "sum", "standard_deviation", "variance".
-        The default is "area".
-    sort_decreasing : bool, optional
-        If True, sort labels by decreasing 'sort_by' value.
-        The default is True.
-
-    Returns
-    -------
-    labels_arr, np.ndarray
-        Label array. 0 values corresponds to no label.
-    n_labels, int
-        Number of labels in the labels array.
-    values, np.arrays
-        Array of length n_labels with the stats values associated to each label.
-    """
+    # footprint: The neighborhood expressed as a 2-D array of 1’s and 0’s.
     # ---------------------------------.
     # TODO: this could be extended to work with dask >2D array
     # - dask_image.ndmeasure.label  https://image.dask.org/en/latest/dask_image.ndmeasure.html
     # - dask_image.ndmorph.binary_dilation https://image.dask.org/en/latest/dask_image.ndmorph.html#dask_image.ndmorph.binary_dilation
 
     # ---------------------------------.
     # Check array validity
     arr = _check_array(arr)
 
     # Check input arguments
     check_sort_by(sort_by)
 
     # ---------------------------------.
     # Define masks
-    # - mask_native: True when between min and max thresholds
+    # - mask_native: True when between min and max thresholds 
     # - mask_nan: True where is not finite (inf or nan)
-    mask_native = np.logical_and(arr >= min_value_threshold, arr <= max_value_threshold)
+    mask_native = np.logical_and(
+        arr >= min_value_threshold, arr <= max_value_threshold
+    )
     mask_nan = ~np.isfinite(arr)
     # ---------------------------------.
-    # Dilate (buffer) the native mask
+    # Dilate (buffer) the native mask 
     # - This enable to assign closely connected mask_native areas to the same label
     mask = _mask_buffer(mask_native, footprint=footprint)
 
     # ---------------------------------.
     # Get area labels
     # - 0 represent the outer area
     label_arr = label_image(mask)  # 0.977-1.37 ms
@@ -343,34 +306,30 @@
     # Set areas outside the mask_native to label value 0
     label_arr[~mask_native] = 0
 
     # Set NaN pixels to label value 0
     label_arr[mask_nan] = 0
 
     # ---------------------------------.
-    # Filter label by area
-    label_indices = get_labels_with_requested_occurence(
-        label_arr=label_arr, vmin=min_area_threshold, vmax=max_area_threshold
-    )
+    # Filter label by area 
+    label_indices = get_labels_with_requested_occurence(label_arr=label_arr,
+                                                        vmin=min_area_threshold,
+                                                        vmax=max_area_threshold)
     if len(label_indices) == 0:
         return _no_labels_result(arr)
 
     # ---------------------------------.
     # Sort labels by statistics (i.e. label area, label max value ...)
-    label_indices, values = get_labels_stats(
-        arr=arr,
-        label_arr=label_arr,
-        label_indices=label_indices,
-        stats=sort_by,
-        sort_decreasing=sort_decreasing,
+    label_indices, values = get_labels_stats(arr=arr,
+                                             label_arr=label_arr,
+                                             label_indices=label_indices,
+                                             stats=sort_by,
+                                             sort_decreasing=sort_decreasing, 
     )
-    # ---------------------------------.
-    # TODO: optionally here calculate a list of label_stats
-    # -> values would be a n_label_stats x n_labels array !
-
+    
     # ---------------------------------.
     # Relabel labels array (from 1 to n_labels)
     labels_arr = redefine_label_array(label_arr=label_arr, label_indices=label_indices)
     n_labels = len(label_indices)
     # ---------------------------------.
     # Return infos
     return labels_arr, n_labels, values
@@ -382,64 +341,17 @@
     max_value_threshold=np.inf,
     min_area_threshold=1,
     max_area_threshold=np.inf,
     footprint=None,
     sort_by="area",
     sort_decreasing=True,
 ):
-    """
-    Function deriving the labels array and associated labels info.
-
-    Parameters
-    ----------
-    data_array : xr.DataArray
-        DataArray object.
-    min_value_threshold : float, optional
-        The minimum value to define the interior of a label.
-        The default is -np.inf.
-    max_value_threshold : float, optional
-        The maximum value to define the interior of a label.
-        The default is np.inf.
-    min_area_threshold : float, optional
-        The minimum number of connected pixels to be defined as a label.
-        The default is 1.
-    max_area_threshold : float, optional
-        The maximum number of connected pixels to be defined as a label.
-        The default is np.inf.
-    footprint : (int, np.ndarray or None), optional
-        This argument enables to dilate the mask derived after applying
-        min_value_threshold and max_value_threshold.
-        If footprint = 0 or None, no dilation occur.
-        If footprint is a positive integer, it create a disk(footprint)
-        If footprint is a 2D array, it must represent the neighborhood expressed
-        as a 2-D array of 1’s and 0’s.
-        The default is None (no dilation).
-    sort_by : (callable or str), optional
-        A function or statistics to define the order of the labels.
-        Valid string statistics are "area", "maximum", "mininum", "mean",
-        "median", "sum", "standard_deviation", "variance".
-        The default is "area".
-    sort_decreasing : bool, optional
-        If True, sort labels by decreasing 'sort_by' value.
-        The default is True.
-
-    Returns
-    -------
-    labels_arr, xr.DataArray
-        Label DataArray. 0 values corresponds to no label.
-        The DataArray name is defined as "labels_{sort_by}".
-    n_labels, int
-        Number of labels in the labels array.
-    values, np.arrays
-        Array of length n_labels with the stats values associated to each label.
-    """
     # Extract data from DataArray
     if not isinstance(data_array, xr.DataArray):
         raise TypeError("Expecting xr.DataArray.")
-
     # Get labels
     labels_arr, n_labels, values = get_areas_labels(
         arr=data_array.data,
         min_value_threshold=min_value_threshold,
         max_value_threshold=max_value_threshold,
         min_area_threshold=min_area_threshold,
         max_area_threshold=max_area_threshold,
@@ -454,91 +366,47 @@
     da_labels.name = f"labels_{sort_by}"
     da_labels.attrs = {}
     return da_labels, n_labels, values
 
 
 def _check_xr_obj(xr_obj, variable):
     """Check xarray object and variable validity."""
-    # Check inputs
+    # Check inputs 
     if not isinstance(xr_obj, (xr.Dataset, xr.DataArray)):
         raise TypeError("'xr_obj' must be a xr.Dataset or xr.DataArray.")
     if isinstance(xr_obj, xr.Dataset):
-        # Check valid variable is specified
-        if variable is None:
+        # Check valid variable is specified 
+        if variable is None: 
             raise ValueError("An xr.Dataset 'variable' must be specified.")
         if variable not in xr_obj.data_vars:
             raise ValueError(f"'{variable}' is not a variable of the xr.Dataset.")
-    else:
-        if variable is not None:
+    else: 
+        if variable is not None: 
             raise ValueError("'variable' must not be specified when providing a xr.DataArray.")
 
 
-def label_xarray_object(
-    xr_obj,
-    variable=None,
-    min_value_threshold=-np.inf,
-    max_value_threshold=np.inf,
-    min_area_threshold=1,
-    max_area_threshold=np.inf,
-    footprint=None,
-    sort_by="area",
-    sort_decreasing=True,
-    label_name="label",
-):
-    """
-    Compute labels and and add as a coordinates to an xarray object.
-
-    Parameters
-    ----------
-    xr_obj : (xr.DataArray or xr.Dataset)
-        xarray object.
-    variable : str, optional
-        Dataset variable to exploit to derive the labels array.
-        Must be specified only if the input object is an xr.Dataset.
-    min_value_threshold : float, optional
-        The minimum value to define the interior of a label.
-        The default is -np.inf.
-    max_value_threshold : float, optional
-        The maximum value to define the interior of a label.
-        The default is np.inf.
-    min_area_threshold : float, optional
-        The minimum number of connected pixels to be defined as a label.
-        The default is 1.
-    max_area_threshold : float, optional
-        The maximum number of connected pixels to be defined as a label.
-        The default is np.inf.
-    footprint : (int, np.ndarray or None), optional
-        This argument enables to dilate the mask derived after applying
-        min_value_threshold and max_value_threshold.
-        If footprint = 0 or None, no dilation occur.
-        If footprint is a positive integer, it create a disk(footprint)
-        If footprint is a 2D array, it must represent the neighborhood expressed
-        as a 2-D array of 1’s and 0’s.
-        The default is None (no dilation).
-    sort_by : (callable or str), optional
-        A function or statistics to define the order of the labels.
-        Valid string statistics are "area", "maximum", "mininum", "mean",
-        "median", "sum", "standard_deviation", "variance".
-        The default is "area".
-    sort_decreasing : bool, optional
-        If True, sort labels by decreasing 'sort_by' value.
-        The default is True.
-
-    Returns
-    -------
-    xr_obj : (xr.DataArray or xr.Dataset)
-        xarray object with the new label coordinate.
-        In the label coordinate, non-labels values are set to np.nan.
-    """
+def label_xarray_object(xr_obj, 
+                        variable=None,
+                        min_value_threshold=-np.inf,
+                        max_value_threshold=np.inf,
+                        min_area_threshold=1,
+                        max_area_threshold=np.inf,
+                        footprint=None,
+                        sort_by="area",
+                        sort_decreasing=True,
+                        label_name="label"):
     # Check xarray input
     _check_xr_obj(xr_obj=xr_obj, variable=variable)
-
+    
     # Retrieve labels (if available)
-    data_array_to_label = xr_obj[variable] if isinstance(xr_obj, xr.Dataset) else xr_obj
-
+    if isinstance(xr_obj, xr.Dataset):
+        data_array_to_label = xr_obj[variable]
+    else:
+        data_array_to_label = xr_obj
+    
     da_labels, n_labels, values = xr_get_areas_labels(
         data_array=data_array_to_label,
         min_value_threshold=min_value_threshold,
         max_value_threshold=max_value_threshold,
         min_area_threshold=min_area_threshold,
         max_area_threshold=max_area_threshold,
         footprint=footprint,
@@ -546,22 +414,14 @@
         sort_decreasing=sort_decreasing,
     )
     if n_labels == 0:
         raise ValueError(
             "No patch available. You might want to change the patch generator parameters."
         )
 
-    # Set labels values == 0 to np.nan  (useful for plotting)
     da_labels = da_labels.where(da_labels > 0)
 
     # Assign label to xr.DataArray  coordinate
     xr_obj = xr_obj.assign_coords({label_name: da_labels})
-
+    
     return xr_obj
 
-
-def highlight_label(xr_obj, label_name, label_id):
-    """Set all labels values to 0 except for 'label_id'."""
-    label_arr = xr_obj[label_name].data
-    label_arr[label_arr != label_id] = 0
-    xr_obj[label_name].data = label_arr
-    return xr_obj
```

### Comparing `gpm_api-0.2.2/gpm_api/patch/labels_patch.py` & `gpm_api-0.2.3/gpm_api/patch/labels_patch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,152 +1,149 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Wed Oct 19 19:40:12 2022
 
 @author: ghiggi
 """
+import warnings
 import numpy as np
-
-from gpm_api.patch.labels import highlight_label, label_xarray_object
+import xarray as xr
+from gpm_api.patch.labels import label_xarray_object
 from gpm_api.utils.slices import (
-    enlarge_slices,
+    get_slice_size,
+    get_idx_bounds_from_slice,
     get_slice_from_idx_bounds,
     pad_slices,
+    enlarge_slices,
 )
-
 # Note
 # - labels_patch_generator available as ds.gpm_api.labels_patch_generator
-# - get_labeled_object_patches used in gpm_api/visualization.labels
+# - get_labeled_object_patches used in gpm_api/visualization.labels 
 
-# gpm_api accessor
-# - gpm_api.label_object
+# gpm_api accessor 
+# - gpm_api.label_object 
 # - gpm_api.labels_patch_generator
 
 ####--------------------------------------------------------------------------.
 #######################################
 #### Patch-Around-Label Generator  ####
 #######################################
 
 
-def _is_natural_numbers(arr):
+def _is_natural_numbers(arr): 
     """
     Check if all values in the input numpy array are natural numbers (positive integers or positive floats)
-
+    
     Parameters
     ----------
     arr : (list, tuple, np.ndarray)
        List, tuple or array of values to be checked.
 
     Returns
     -------
     bool
         True if all values in the array are natural numbers, False otherwise..
 
     """
-    return bool(
-        np.all(
-            np.logical_and(
-                np.greater(arr, 0), np.isclose(arr, np.round(arr), atol=1e-12, rtol=1e-12)
-            )
-        )
-    )
-
-
-def _check_label_arr(label_arr):
-    """Check label_arr."""
-    # Note: If label array is all zero or nan, labels_id will be []
+    if np.all(np.logical_and(np.greater(arr, 0), np.isclose(arr, np.round(arr), atol=1e-12, rtol=1e-12))):
+        return True
+    else:
+        return False  
+    
 
+def _check_label_arr(label_arr):   
+    # Note: If label array is all zero or nan, labels_id will be []       
+    
     # Put label array in memory
     label_arr = np.asanyarray(label_arr)
 
     # Set 0 label to nan
-    label_arr = label_arr.astype(float)  # otherwise if int throw an error when assigning nan
+    label_arr = label_arr.astype(float) # otherwise if int throw an error when assigning nan
     label_arr[label_arr == 0] = np.nan
-
-    # Check labels_id are natural number >= 1
+        
+    # Check labels_id are natural number >= 1 
     valid_labels = np.unique(label_arr[~np.isnan(label_arr)])
     if not _is_natural_numbers(valid_labels):
         raise ValueError("The label array contains non positive natural numbers.")
 
     return label_arr
 
 
 def _check_labels_id(labels_id, label_arr):
-    """Check labels_id."""
     # Check labels_id type
     if not isinstance(labels_id, (type(None), list, np.ndarray)):
         raise TypeError("labels_id must be None or a list or a np.array.")
-    # Get list of valid labels
+    # Get list of valid labels 
     valid_labels = np.unique(label_arr[~np.isnan(label_arr)])
-    # If labels_id is None, assign the valid_labels
+    # If labels_id is None, assign the valid_labels 
     if isinstance(labels_id, type(None)):
         labels_id = valid_labels
         return labels_id
-    # If input labels_id is a list, make it a np.array
+    # If input labels_id is a list, make it a np.array       
     labels_id = np.array(labels_id).astype(int)
     # Check labels_id are natural number >= 1
-    if np.any(labels_id == 0):
+    if np.any(labels_id == 0): 
         raise ValueError("labels id must not contain the 0 value.")
-    if not _is_natural_numbers(labels_id):
+    if not _is_natural_numbers(labels_id): 
         raise ValueError("labels id must be positive natural numbers.")
     # Check labels_id are number present in the label_arr
     unvalid_labels = labels_id[~np.isin(labels_id, valid_labels)]
     if unvalid_labels.size != 0:
         unvalid_labels = unvalid_labels.astype(int)
         raise ValueError(f"The following labels id are not valid: {unvalid_labels}")
     return labels_id
-
-
+ 
+    
 def _check_patch_size(patch_size, array_shape):
     """
     Check the validity of the patch_size argument based on the array_shape.
-
+    
     Parameters
     ----------
     patch_size : (None, int, float, list or tuple)
-        The size of the patch to extract from the array.
-        If None, it set a patch size of 2 in all directions.
+        The size of the patch to extract from the array. 
+        If None, it set a patch size 2 all directions.
         If int or float, the patch is a hypercube of size patch_size.
         If list or tuple, the patch has the shape specified by the elements of the list or tuple.
         The patch size must be equal or larger than 2, but smaller than the corresponding array shape.
     array_shape : tuple
         The shape of the array.
 
     Returns
     -------
     patch_size (None, tuple)
         The shape of the patch.
     """
+ 
     n_dims = len(array_shape)
     if patch_size is None:
-        patch_size = 2
+        patch_size = 2 
     elif isinstance(patch_size, (int, float)):
         patch_size = tuple([patch_size] * n_dims)
     elif isinstance(patch_size, (list, tuple)) and len(patch_size) == n_dims:
-        if not _is_natural_numbers(patch_size):  # [0,1,..., Inf)
-            raise ValueError("Invalid patch size. Must be composed of natural numbers.")
-        # Check patch size is smaller than array shape
-        idx_valid = [x <= max_val for x, max_val in zip(patch_size, array_shape)]
-        if not all(idx_valid):
-            raise ValueError(f"The maximum patch size is {array_shape}")
+         if not _is_natural_numbers(patch_size):  # [0,1,..., Inf)
+             raise ValueError("Invalid patch size. Must be composed of natural numbers.")
+         # Check patch size is smaller than array shape 
+         idx_valid = [x <= max_val for x, max_val in zip(patch_size, array_shape)]
+         if not all(idx_valid):
+             raise ValueError(f"The maximum patch size is {array_shape}")         
     else:
-        raise ValueError(
-            f"Invalid patch size. Should be None, int, float, list or tuple of length {n_dims}."
-        )
+        raise ValueError(f"Invalid patch size. Should be None, int, float, list or tuple of length {n_dims}.")
     return patch_size
 
 
 def _check_padding(padding, array_shape):
     """
     Check the validity of the padding argument based on the array_shape.
-
+    
     Parameters
     ----------
     padding : (None, int, float, list or tuple)
-        The size of the padding to apply to the array.
+        The size of the padding to apply to the array. 
         If None, zero padding is assumed.
         If int or float, equal padding is set on each dimension of the array.
         If list or tuple, the padding has the shape specified by the elements of the list or tuple.
     array_shape : tuple
         The shape of the array.
 
     Returns
@@ -156,239 +153,168 @@
     """
     n_dims = len(array_shape)
     if padding is None:
         padding = 0
     elif isinstance(padding, (int, float)):
         padding = tuple([padding] * n_dims)
     elif isinstance(padding, (list, tuple)) and len(padding) == n_dims:
-        if not _is_natural_numbers(padding):
-            raise ValueError("Invalid padding. Must be composed of natural numbers.")
+         if not _is_natural_numbers(padding):
+             raise ValueError("Invalid padding. Must be composed of natural numbers.")   
     else:
-        raise ValueError(
-            f"Invalid padding. Should be None, int, float, list or tuple of length {n_dims}."
-        )
+        raise ValueError(f"Invalid padding. Should be None, int, float, list or tuple of length {n_dims}.")
     return padding
 
 
 def _get_labels_bbox_slices(arr):
     """
     Compute the bounding box slices of non-zero elements in a n-dimensional numpy array.
 
     Parameters
     ----------
     arr : np.ndarray
         n-dimensional numpy array.
-
+.
     Returns
     -------
     list_slices : list
         List of slices to extract the region with non-zero elements in the input array.
     """
     ndims = arr.ndim
     coords = np.nonzero(arr)
-    list_slices = [
-        get_slice_from_idx_bounds(np.min(coords[i]), np.max(coords[i])) for i in range(ndims)
-    ]
-    return list_slices
-
-
-def _get_patch_list_slices(label_arr, label_id, padding, min_patch_size):
-    """Get patch subsetting isel dictionary for a given label."""
-    # Get label bounding box slices
-    list_slices = _get_labels_bbox_slices(label_arr == label_id)
-    # Apply padding to the slices
-    list_slices = pad_slices(list_slices, padding=padding, valid_shape=label_arr.shape)
-    # Increase slices to match min_patch_size
-    list_slices = enlarge_slices(list_slices, min_size=min_patch_size, valid_shape=label_arr.shape)
+    list_slices = [get_slice_from_idx_bounds(np.min(coords[i]), np.max(coords[i])) for i in range(ndims)]
     return list_slices
 
 
 def get_labeled_object_patches(
-    xr_obj,
-    label_name,
-    n_patches=None,
-    labels_id=None,
-    padding=None,
-    min_patch_size=None,
-    highlight_label_id=True,
+    xr_obj, label_name,
+        n_patches=None, labels_id=None,
+        padding=None, min_patch_size=None, 
+        highlight_label_id=True, 
 ):
     """
-    Create a generator extracting patches around labels (from a prelabeled xr.Dataset).
-
+    Create a generator extracting patches around labels. 
+    
     Only one parameter between n_patches and labels_id can be specified.
     If n_patches=None and labels_id=None are both None, it returns a patch for each label.
     The patch minimum size is defined by min_patch_size, which default to 2 in all dimensions.
-    If the naive label patch size is smaller than min_patch_size, the patch is enlarged to have
+    If the naive label patch size is smaller than min_patch_size, the patch is enlarged to have 
     size equal to min_patch_size.
-
+        
     The output patches are not guaranteed to have equal size !
-
+         
     Parameters
     ----------
-    xr_obj : xr.Dataset
+    xr_obj : xr.Dataset 
         xr.Dataset with a label array named label_bame.
     label_name : TYPE
         Name of the variable/coordinate representing the label array.
     n_patches : int, optional
         Number of patches to extract. The default is None.
-    labels_id : list, optional
-        List of labels for which to extract the patch.
+    labels_id : list, optional 
+        List of labels for which to extract the patch. 
         If None, it extracts the patch by label order (1, 2, 3, ...)
         The default is None.
     min_patch_size : (int, tuple), optional
         The minimum size of the patch to extract.
         If None (default) it set a minimum size of 2 in all dimensions.
     padding : (int, tuple), optional
-        The padding to apply in each direction.
+        The padding to apply in each direction. 
         If None, it applies 0 padding in every dimension.
         The default is None.
-    highlight_label_id : (bool), optional
-        If True, the laben_name array of each patch is modified to contain only
+    highlight_label_id : (bool), optional 
+        If True, the laben_name array of each patch is modified to contain only 
         the label_id used to select the patch.
 
     Yields
     ------
     (xr.Dataset or xr.DataArray)
         A xarray object patch.
 
     """
-    # Get label array information
+    # Get label array information 
     label_arr = xr_obj[label_name].data
     dims = xr_obj[label_name].dims
     shape = label_arr.shape
-
-    # Check input arguments
-    if n_patches is not None and labels_id is not None:
-        raise ValueError("Specify either n_patches or labels_id.")
+      
+    # Check input arguments 
+    if n_patches is not None and labels_id is not None: 
+        raise ValueError("Specify either n_patches or labels_id.")  
     label_arr = _check_label_arr(label_arr)  # ouput is np.array
     labels_id = _check_labels_id(labels_id=labels_id, label_arr=label_arr)
     min_patch_size = _check_patch_size(min_patch_size, array_shape=shape)
     padding = _check_padding(padding, array_shape=shape)
-
+   
     # If no labels, no patch to extract
     n_labels = len(labels_id)
-    if n_labels == 0:
+    if n_labels == 0: 
         raise ValueError("No labels available.")
-        # yield None # TODO: DEFINE CORRECT BEHAVIOUR
-
+        # yield None # TODO: DEFINE CORRECT BEHAVIOUR 
+    
     # If n_patches is None --> n_patches = n_labels, else min(n_patches, n_labels)
     n_patches = min(n_patches, n_labels) if n_patches else n_labels
 
     # Extract patch around the label
     for label_id in labels_id[0:n_patches]:
-        # Extract patch list_slice
-        list_slices = _get_patch_list_slices(
-            label_arr=label_arr, label_id=label_id, padding=padding, min_patch_size=min_patch_size
-        )
+       
+        # Get label bounding box slices 
+        list_slices = _get_labels_bbox_slices(label_arr == label_id)
+        
+        # Apply padding to the slices  
+        list_slices = pad_slices(list_slices, padding=padding, valid_shape=label_arr.shape)
+                
+        # Increase slices to match min_patch_size
+        list_slices = enlarge_slices(list_slices, min_size=min_patch_size, valid_shape=label_arr.shape)
+             
+        # Create subsetting dictionary
+        isel_dict = {dim: slc for dim, slc in zip(dims,list_slices)}
+        
         # Extract xarray patch around label
-        isel_dict = {dim: slc for dim, slc in zip(dims, list_slices)}
         xr_obj_patch = xr_obj.isel(isel_dict)
-
-        # If asked, set label array to 0 except for label_id
-        if highlight_label_id:
-            xr_obj_patch = highlight_label(xr_obj_patch, label_name=label_name, label_id=label_id)
-
+        
+        # Set label array to 0 except for label_id 
+        if highlight_label_id: 
+            patch_label_arr = xr_obj_patch[label_name].data
+            patch_label_arr[patch_label_arr != label_id] = 0
+            xr_obj_patch[label_name].data = patch_label_arr
+        
         # Return the patch around the label
         yield xr_obj_patch
-
+            
 
 def labels_patch_generator(
     xr_obj,
     variable=None,
     min_value_threshold=-np.inf,
     max_value_threshold=np.inf,
     min_area_threshold=1,
     max_area_threshold=np.inf,
     footprint=None,
     sort_by="area",
     sort_decreasing=True,
     # Patch settings
     n_patches=None,
     padding=None,
-    min_patch_size=None,
-):
-    """
-    Create a generator extracting patches around sensible regions of an xr.Dataset.
-
-    The function first derives the labels array, and then it extract patches for n_patches labels.
-    If n_patches=None it returns a patch for each label.
-    The patch minimum size is defined by min_patch_size, which default to 2 in all dimensions.
-    If the naive label patch size is smaller than min_patch_size, the patch is enlarged to have
-    size equal to min_patch_size.
-
-    The output patches are not guaranteed to have equal size !
-
-    Parameters
-    ----------
-    xr_obj : (xr.Dataset or xr.DataArray)
-        xarray object.
-    variable : str, optional
-        Dataset variable to exploit to derive the labels.
-        Must be specified only if the input object is an xr.Dataset.
-    min_value_threshold : float, optional
-        The minimum value to define the interior of a label.
-        The default is -np.inf.
-    max_value_threshold : float, optional
-        The maximum value to define the interior of a label.
-        The default is np.inf.
-    min_area_threshold : float, optional
-        The minimum number of connected pixels to be defined as a label.
-        The default is 1.
-    max_area_threshold : float, optional
-        The maximum number of connected pixels to be defined as a label.
-        The default is np.inf.
-    footprint : (int, np.ndarray or None), optional
-        This argument enables to dilate the mask derived after applying
-        min_value_threshold and max_value_threshold.
-        If footprint = 0 or None, no dilation occur.
-        If footprint is a positive integer, it create a disk(footprint)
-        If footprint is a 2D array, it must represent the neighborhood expressed
-        as a 2-D array of 1’s and 0’s.
-        The default is None (no dilation).
-    sort_by : (callable or str), optional
-        A function or statistics to define the order of the labels.
-        Valid string statistics are "area", "maximum", "mininum", "mean",
-        "median", "sum", "standard_deviation", "variance".
-        The default is "area".
-    sort_decreasing : bool, optional
-        If True, sort labels by decreasing 'sort_by' value.
-        The default is True.
-    n_patches : int, optional
-        Number of patches to extract. The default is None (all).
-    padding : (int, tuple), optional
-        The padding to apply in each direction.
-        If None, it applies 0 padding in every dimension.
-        The default is None.
-    min_patch_size : (int, tuple), optional
-        The minimum size of the patch to extract.
-        If None (default) it set a minimum size of 2 in all dimensions.
-
-    Yields
-    ------
-    (xr.Dataset or xr.DataArray)
-        A xarray object patch.
-
-    """
-    # Retrieve labeled xarray object
-    xr_obj = label_xarray_object(
-        xr_obj,
-        variable=variable,
-        min_value_threshold=min_value_threshold,
-        max_value_threshold=max_value_threshold,
-        min_area_threshold=min_area_threshold,
-        max_area_threshold=max_area_threshold,
-        footprint=footprint,
-        sort_by=sort_by,
-        sort_decreasing=sort_decreasing,
-        label_name="label",
-    )
-
-    # Define the patch generator
+    min_patch_size=None, 
+):  
+    # Retrieve labeled xarray object 
+    xr_obj = label_xarray_object(xr_obj, 
+                                 variable=variable,
+                                 min_value_threshold=min_value_threshold,
+                                 max_value_threshold=max_value_threshold,
+                                 min_area_threshold=min_area_threshold,
+                                 max_area_threshold=max_area_threshold,
+                                 footprint=footprint,
+                                 sort_by=sort_by,
+                                 sort_decreasing=sort_decreasing,
+                                 label_name="label",
+                                 )
+    
+    # Define the patch generator 
     patch_gen = get_labeled_object_patches(
-        xr_obj,
-        label_name="label",
-        n_patches=n_patches,
+        xr_obj, 
+        label_name="label", 
+        n_patches=n_patches, 
         padding=padding,
-        min_patch_size=min_patch_size,
+        min_patch_size=min_patch_size
     )
-
+    
     return patch_gen
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gpm_api-0.2.2/gpm_api/patch/utils.py` & `gpm_api-0.2.3/gpm_api/patch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Wed Oct 19 16:51:11 2022
 
 @author: ghiggi
 """
+import pandas as pd
+import numpy as np
 import itertools
 
-import numpy as np
-import pandas as pd
 from scipy.ndimage import find_objects
 from scipy.ndimage.measurements import center_of_mass
 
 from gpm_api.patch.labels import get_areas_labels
 from gpm_api.utils.slices import (
     get_slice_size,
+    get_idx_bounds_from_slice,
+    get_slice_from_idx_bounds,
+    pad_slices,
 )
-
 ####--------------------------------------------------------------------------.
 # Shapely bounds: (xmin, ymin, xmax, ymax)
 # Matlotlib extent: (xmin, xmax, ymin, ymax)
 # Cartopy extent: (xmin, xmax, ymin, ymax)
 # GPM-API extent: (xmin, xmax, ymin, ymax)
-
+    
 ####--------------------------------------------------------------------------.
 
-
 def get_row_col_slice_centroid(row_slice, col_slice):
     row = int((row_slice.start + row_slice.stop - 1) / 2)
     col = int((col_slice.start + col_slice.stop - 1) / 2)
     return row, col
 
 
 ####--------------------------------------------------------------------------.
-#### Patch splitter
-
+#### Patch splitter 
 
 def split_large_object_slices(object_slices, patch_size):
     if len(patch_size) == 1:
         patch_size = [patch_size] * len(object_slices)
     if np.any(np.array(patch_size) <= 2):
         raise ValueError("Minimum patch_size should be 2.")
     if len(patch_size) != len(object_slices):
@@ -167,15 +168,17 @@
     # ---------------------------------.
     # Loop over each label, and extract patches
     list_patch_slices = []
     # i = 0
     # object_slice = objects_slices[i]
     for i, object_slice in enumerate(objects_slices):
         # If slices larger than patch_size, split into multiple slices and loop over it
-        conform_object_slices = split_large_object_slices(object_slice, patch_size=patch_size)
+        conform_object_slices = split_large_object_slices(
+            object_slice, patch_size=patch_size
+        )
         # r_slice, c_slice = conform_object_slices[0]
         for r_slice, c_slice in conform_object_slices:
             # print(i)
             # ---------------------------------.
             # Define patch label
             tmp_label = labels[r_slice, c_slice]
 
@@ -217,57 +220,60 @@
                 row = r_slice.start + row[0]
                 col = c_slice.start + col[0]
             elif centered_on == "min":
                 row, col = np.where(tmp_intensity == np.nanmin(tmp_intensity))
                 row = r_slice.start + row[0]
                 col = c_slice.start + col[0]
             elif centered_on == "centroid":
-                row, col = get_row_col_slice_centroid(row_slice=r_slice, col_slice=c_slice)
+                row, col = get_row_col_slice_centroid(
+                    row_slice=r_slice, col_slice=c_slice
+                )
             elif centered_on == "center_of_mass":
                 row, col = center_of_mass(tmp_label_mask)
                 row = int(row)
                 col = int(col)
                 row = r_slice.start + row
                 col = c_slice.start + col
             else:
                 raise NotImplementedError("")
 
             # ---------------------------------.
             # Retrieve actual patch
-            row_slice, col_slice = get_patch_slices_around(row, col, patch_size, image_shape)
+            row_slice, col_slice = get_patch_slices_around(
+                row, col, patch_size, image_shape
+            )
             # assert get_slice_size(col_slice) == 128
             # print(get_slice_size(col_slice))
             # Append to list
             list_patch_slices.append((row_slice, col_slice))
 
     # ---------------------------------.
     # Postprocessing list_patch_slices
     # TODO: with shapely?
     # - distance between centroids ---> group ...
 
     # ---------------------------------.
     # Compute patch statistics
     if callable(patch_stats_fun):
         patch_statistics = [
-            patch_stats_fun(intensity[r_slice, c_slice]) for r_slice, c_slice in list_patch_slices
+            patch_stats_fun(intensity[r_slice, c_slice])
+            for r_slice, c_slice in list_patch_slices
         ]
     else:
         patch_statistics = None
     # ---------------------------------.
     # Return object
     return list_patch_slices, patch_statistics
 
-
 ####--------------------------------------------------------------------------.
 #########################
 #### Patch Stats Info ###
 #########################
 # TODO: Inside get_label_stats
-# - Add label mask
-
+# - Add label mask 
 
 def patch_stats_fun(patch: np.ndarray):
     width = patch.shape[1]
     height = patch.shape[0]
     patch_area = width * height
     stats_dict = {
         "Max": np.nanmax(patch),
@@ -323,15 +329,17 @@
             centered_on=centered_on,
             patch_stats_fun=patch_stats_fun,
         )
         # Found upper left index
         list_patch_upper_left_idx = [
             [slc.start for slc in list_slc] for list_slc in list_patch_slices
         ]
-        upper_left_str = [str(row) + "-" + str(col) for row, col in list_patch_upper_left_idx]
+        upper_left_str = [
+            str(row) + "-" + str(col) for row, col in list_patch_upper_left_idx
+        ]
 
         # Define data.frame
         df = pd.DataFrame(patch_statistics)
         df["upper_left_idx"] = upper_left_str
     else:
         df = pd.DataFrame()
```

### Comparing `gpm_api-0.2.2/gpm_api/scripts/download_daily_gpm_data.py` & `gpm_api-0.2.3/gpm_api/scripts/download_monthly_gpm_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,79 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
-Created on Mon Mar 13 11:48:22 2023
+Created on Mon Mar 13 12:11:27 2023
 
 @author: ghiggi
 """
 import sys
-import warnings
-
 import click
-
-from gpm_api.io import GPM_VERSION  # CURRENT GPM VERSION
+import warnings
+from gpm_api.io import GPM_VERSION # CURRENT GPM VERSION
 
 warnings.filterwarnings("ignore")
 sys.tracebacklimit = 0  # avoid full traceback error if occur
 
 # -------------------------------------------------------------------------.
 # Click Command Line Interface decorator
 @click.command()
-@click.argument("product", type=str)
-@click.argument("year", type=int)
-@click.argument("month", type=int)
-@click.argument("day", type=int)
-@click.option("--product_type", type=str, show_default=True, default="RS")
-@click.option("--version", type=int, show_default=True, default=GPM_VERSION)
-@click.option("--n_threads", type=int, default=2)
-@click.option("--transfer_tool", type=str, default="curl")
-@click.option("--progress_bar", type=bool, default=False)
-@click.option("--force_download", type=bool, default=False)
-@click.option("--check_integrity", type=bool, default=True)
-@click.option("--remove_corrupted", type=bool, default=True)
-@click.option("--verbose", type=bool, default=True)
-@click.option("--retry", type=int, default=1)
-@click.option("--base_dir", type=str, default=None)
-@click.option("--username", type=str, default=None)
-@click.option("--password", type=str, default=None)
-def download_daily_gpm_data(
+@click.argument('product', type=str)
+@click.argument('year', type=int)
+@click.argument('month', type=int)
+@click.option('--product_type', type=str, show_default=True, default="RS")
+@click.option('--version', type=int, show_default=True, default=GPM_VERSION)
+@click.option('--n_threads', type=int, default=10)
+@click.option('--transfer_tool', type=str, default="curl")
+@click.option('--progress_bar', type=bool, default=False)
+@click.option('--force_download', type=bool, default=False)
+@click.option('--check_integrity', type=bool, default=True)
+@click.option('--remove_corrupted', type=bool, default=True)
+@click.option('--verbose', type=bool, default=True)
+@click.option('--retry', type=int, default=1)
+@click.option('--base_dir', type=str, default=None)
+@click.option('--username', type=str, default=None)
+@click.option('--password', type=str, default=None)
+def download_monthly_gpm_data(
     product,
     year,
     month,
-    day,
     product_type="RS",
     version=GPM_VERSION,
-    n_threads=2,
+    n_threads=10,
     transfer_tool="curl",
     progress_bar=False,
     force_download=False,
     check_integrity=True,
     remove_corrupted=True,
     verbose=True,
-    retry=1,
+    retry=1, 
     base_dir=None,
     username=None,
     password=None,
 ):
-    """Download the GPM product for a specific date."""
-    from gpm_api.utils.archive import download_daily_data
-
-    _ = download_daily_data(
+    """Download the GPM product for a specific month."""
+    from gpm_api.utils.archive import download_monthly_data
+    
+    _ = download_monthly_data(
         product=product,
         year=year,
         month=month,
-        day=day,
         product_type=product_type,
         version=version,
         n_threads=n_threads,
         transfer_tool=transfer_tool,
         progress_bar=progress_bar,
         force_download=force_download,
         check_integrity=check_integrity,
         remove_corrupted=remove_corrupted,
         verbose=verbose,
         retry=retry,
         base_dir=base_dir,
         username=username,
         password=password,
     )
-
-    return
+ 
+    return None
 
 
 if __name__ == "__main__":
-    download_daily_gpm_data()
+    download_monthly_gpm_data()
```

### Comparing `gpm_api-0.2.2/gpm_api/scripts/download_monthly_gpm_data.py` & `gpm_api-0.2.3/gpm_api/scripts/download_daily_gpm_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
-Created on Mon Mar 13 12:11:27 2023
+Created on Mon Mar 13 11:48:22 2023
 
 @author: ghiggi
 """
 import sys
-import warnings
-
 import click
-
-from gpm_api.io import GPM_VERSION  # CURRENT GPM VERSION
+import warnings
+from gpm_api.io import GPM_VERSION # CURRENT GPM VERSION
 
 warnings.filterwarnings("ignore")
 sys.tracebacklimit = 0  # avoid full traceback error if occur
 
 # -------------------------------------------------------------------------.
 # Click Command Line Interface decorator
 @click.command()
-@click.argument("product", type=str)
-@click.argument("year", type=int)
-@click.argument("month", type=int)
-@click.option("--product_type", type=str, show_default=True, default="RS")
-@click.option("--version", type=int, show_default=True, default=GPM_VERSION)
-@click.option("--n_threads", type=int, default=10)
-@click.option("--transfer_tool", type=str, default="curl")
-@click.option("--progress_bar", type=bool, default=False)
-@click.option("--force_download", type=bool, default=False)
-@click.option("--check_integrity", type=bool, default=True)
-@click.option("--remove_corrupted", type=bool, default=True)
-@click.option("--verbose", type=bool, default=True)
-@click.option("--retry", type=int, default=1)
-@click.option("--base_dir", type=str, default=None)
-@click.option("--username", type=str, default=None)
-@click.option("--password", type=str, default=None)
-def download_monthly_gpm_data(
+@click.argument('product', type=str)
+@click.argument('year', type=int)
+@click.argument('month', type=int)
+@click.argument('day', type=int)
+@click.option('--product_type', type=str, show_default=True, default="RS")
+@click.option('--version', type=int, show_default=True, default=GPM_VERSION)
+@click.option('--n_threads', type=int, default=2)
+@click.option('--transfer_tool', type=str, default="curl")
+@click.option('--progress_bar', type=bool, default=False)
+@click.option('--force_download', type=bool, default=False)
+@click.option('--check_integrity', type=bool, default=True)
+@click.option('--remove_corrupted', type=bool, default=True)
+@click.option('--verbose', type=bool, default=True)
+@click.option('--retry', type=int, default=1)
+@click.option('--base_dir', type=str, default=None)
+@click.option('--username', type=str, default=None)
+@click.option('--password', type=str, default=None)
+def download_daily_gpm_data(
     product,
     year,
     month,
+    day,
     product_type="RS",
     version=GPM_VERSION,
-    n_threads=10,
+    n_threads=2,
     transfer_tool="curl",
     progress_bar=False,
     force_download=False,
     check_integrity=True,
     remove_corrupted=True,
     verbose=True,
-    retry=1,
+    retry=1, 
     base_dir=None,
     username=None,
     password=None,
 ):
-    """Download the GPM product for a specific month."""
-    from gpm_api.utils.archive import download_monthly_data
-
-    _ = download_monthly_data(
+    """Download the GPM product for a specific date."""
+    from gpm_api.utils.archive import download_daily_data
+    
+    _ = download_daily_data(
         product=product,
         year=year,
         month=month,
+        day=day,
         product_type=product_type,
         version=version,
         n_threads=n_threads,
         transfer_tool=transfer_tool,
         progress_bar=progress_bar,
         force_download=force_download,
         check_integrity=check_integrity,
         remove_corrupted=remove_corrupted,
         verbose=verbose,
         retry=retry,
         base_dir=base_dir,
         username=username,
         password=password,
     )
-
-    return
+ 
+    return None
 
 
 if __name__ == "__main__":
-    download_monthly_gpm_data()
+    download_daily_gpm_data()
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/info.py` & `gpm_api-0.2.3/gpm_api/tests/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue Nov  1 15:14:46 2022
 
 @author: ghiggi
 """
-### NASA pattern
-# product level:
-# - 1A, 2A, 2B,
+### NASA pattern 
+# product level: 
+# - 1A, 2A, 2B, 
 # - 3A-MO, 3B-DAY, 3A-DAY-ASC, 3A-DAY-DESC, 3B-ORBIT, 3B-MO. 3B-HHR-{E/L}
 # - 2A-CS-<SITE> (CS=COINCIDENCE)
 
-# satellite:
+# satellite: 
 # - TRMM, GPM, SSMIS, ..
 # - MS (multi-sensor) --> IMERG
 
-### JAXA pattern
+### JAXA pattern 
 # mission_id (mission + satellite_id)
-# sensor: KUR, KAR, CMB
+# sensor: KUR, KAR, CMB 
 # product_type: R(NRT) or S (RS)
 
-### Example file names
-# # IMERG
+### Example file names 
+# # IMERG 
 # fname = "3B-HHR.MS.MRG.3IMERG.20140422-S043000-E045959.0270.V06B.HDF5"
-
+ 
 # # 2B
 # fname = "2B.GPM.DPRGMI.2HCSHv7-0.20140422-S013047-E030320.000831.V07A.HDF5"
 # fname = "2B.GPM.DPRGMI.CORRA2022.20140422-S230649-E003923.000845.V07A.HDF5"
 # fname = "2B.TRMM.PRTMI.2HCSHv7-0.20140422-S110725-E123947.093603.V07A.HDF5"
 
 # # 2A
 # fname = "2A.MT1.SAPHIR.PRPS2019v2-02.20140422-S000858-E015053.013038.V06A.HDF5"
 # fname = "2A.GPM.DPR.V9-20211125.20201028-S075448-E092720.037875.V07A.HDF5"
-# # 1C
+# # 1C 
 # fname = "1C.GPM.GMI.XCAL2016-C.20140422-S013047-E030320.000831.V07A.HDF5"
 # # 1B
 # fname = "GPMCOR_KUR_2010280754_0927_037875_1BS_DAB_07A.h5"
 # fname = "GPMCOR_KAR_2010280754_0927_037875_1BS_DAB_07A.h5"
 # fname = "1B.TRMM.PR.V9-20210630.20140422-S002044-E015306.093596.V07A.HDF5"
 # # 1A
 # fname = "1A.GPM.GMI.COUNT2021.20140422-S230649-E003923.000845.V07A.HDF5"
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/io/test_00_24_granules.py` & `gpm_api-0.2.3/gpm_api/tests/io/test_find_filters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,108 +1,66 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Mon Aug 17 18:23:58 2020
+Created on Thu Oct 13 15:22:34 2022
 
 @author: ghiggi
 """
-import datetime
-
-from gpm_api.io.find import (
-    find_daily_GPM_disk_filepaths,
-    find_daily_GPM_PPS_filepaths,
-    find_GPM_files,
+import datetime 
+import gpm_api
+from gpm_api.io.products import GPM_products
+from gpm_api.io.pps import find_pps_daily_filepaths
+from gpm_api.io.checks import (
+    check_version,
+    check_product,
+    check_product_type,
+    check_time,
+    check_date,
+    is_empty,
+)
+from gpm_api.io.filter import (
+    filter_by_time,
+    filter_by_product,
 )
 
-##----------------------------------------------------------------------------.
-base_dir = "/home/ghiggi/tmp"
+
+#-------------------------------------------------------------------------.
+base_dir = '/home/ghiggi/tmp'
 username = "gionata.ghiggi@epfl.ch"
-product = "2A-DPR"
-start_hhmmss = "000000"
-end_hhmmss = "020000"
-version = 6
-
-##----------------------------------------------------------------------------.
-## Still BUGGY for the following case
-# - Need to take only the previous day
-start_hhmmss = "000000"
-end_hhmmss = "001000"
-# - Need to take only a single granule in current day
-start_hhmmss = "020028"
-end_hhmmss = "020030"
-# - Need to take last granule
-start_hhmmss = "235000"
-end_hhmmss = "240000"
-
-# start_hhmmss and end_hhmmss in datetime.time format
-start_hhmmss = datetime.time.fromisoformat("00:00:00")
-end_hhmmss = datetime.time.fromisoformat("23:59:00")
-##----------------------------------------------------------------------------.
-### Retrieve RS filepaths
-date = datetime.date.fromisoformat("2014-08-09")
-product_type = "RS"
-
-(server_paths, disk_paths) = find_daily_GPM_PPS_filepaths(
-    username=username,
-    base_dir=base_dir,
-    product=product,
-    date=date,
-    start_hhmmss=start_hhmmss,
-    end_hhmmss=end_hhmmss,
-    product_type=product_type,
-    version=version,
-    flag_first_date=True,
-)
-print(server_paths)
-print(disk_paths)
+version = 7
+product_type = 'RS'
+products  = GPM_products(product_type)
 
-find_daily_GPM_disk_filepaths(
-    base_dir=base_dir,
-    product=product,
-    date=date,
-    start_hhmmss=start_hhmmss,
-    end_hhmmss=end_hhmmss,
-    product_type=product_type,
-    version=version,
-    flag_first_date=True,
-)
-##----------------------------------------------------------------------------.
-### Retrieve NRT filepaths
-date = datetime.date.fromisoformat("2020-08-16")
-product_type = "NRT"
-
-(server_paths, disk_paths) = find_daily_GPM_PPS_filepaths(
-    username=username,
-    base_dir=base_dir,
-    product=product,
-    product_type=product_type,
-    version=version,
-    date=date,
-    start_hhmmss=start_hhmmss,
-    end_hhmmss=end_hhmmss,
-    flag_first_date=True,
-)
-print(server_paths)
-print(disk_paths)
+date = datetime.date.fromisoformat("2020-08-17")
 
-find_daily_GPM_disk_filepaths(
-    base_dir=base_dir,
-    product=product,
-    date=date,
-    start_hhmmss=start_hhmmss,
-    end_hhmmss=end_hhmmss,
-    product_type=product_type,
-    version=version,
-    flag_first_date=True,
-)
+start_time = datetime.datetime.strptime("2020-08-17 00:00:00", '%Y-%m-%d %H:%M:%S')
+end_time = datetime.datetime.strptime("2020-08-17 04:00:00", '%Y-%m-%d %H:%M:%S')
 
-### find_GPM_files()
-start_time = datetime.datetime.fromisoformat("2020-08-15 00:00:00")
-end_time = datetime.datetime.fromisoformat("2020-08-17 00:00:00")
-find_GPM_files(
-    base_dir=base_dir,
-    product=product,
-    start_time=start_time,
-    end_time=end_time,
-    product_type=product_type,
-    version=version,
-)
+product = "2A-DPR"
+flag_first_date=False
+verbose = True
+force_download = False
+
+#-------------------------------------------------------------------------.
+date = check_date(date)
+check_product_type(product_type = product_type)
+check_product(product = product, product_type = product_type)
+start_hhmmss = datetime.datetime.strftime(start_time,"%H%M%S")
+end_hhmmss = datetime.datetime.strftime(end_time,"%H%M%S")
+
+#-------------------------------------------------------------------------.
+## Retrieve the list of files available on NASA PPS server
+(pps_fpaths, disk_fpaths) = find_pps_daily_filepaths(username = username,
+                                                    base_dir = base_dir, 
+                                                    product = product, 
+                                                    product_type = product_type,
+                                                    version = version,
+                                                    date = date, 
+                                                    start_hhmmss = start_hhmmss, 
+                                                    end_hhmmss = end_hhmmss,
+                                                    flag_first_date = flag_first_date,
+                                                    verbose = verbose)
+ 
+
+#-------------------------------------------------------------------------.
+filter_by_time(pps_fpaths, date, start_hhmmss, end_hhmmss)
+filter_by_product(pps_fpaths, product=product)
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/io/test_GPM_products.py` & `gpm_api-0.2.3/gpm_api/tests/io/test_GPM_products.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,65 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Mon Aug 17 14:35:58 2020
 
 @author: ghiggi
 """
+import os
 
 from gpm_api.io.products import (
-    GPM_1B_NRT_products,
-    GPM_1B_RS_products,
-    GPM_1C_NRT_products,
-    GPM_1C_RS_products,
-    GPM_2A_NRT_products,
-    GPM_2A_RS_products,
-    GPM_CMB_2B_NRT_products,
-    GPM_CMB_2B_RS_products,
-    GPM_DPR_1B_NRT_products,
-    GPM_DPR_1B_RS_products,
-    GPM_DPR_2A_ENV_NRT_products,
-    GPM_DPR_2A_ENV_RS_products,
-    GPM_DPR_2A_NRT_products,
-    GPM_DPR_2A_RS_products,
+    
+    GPM_products,
+    GPM_IMERG_products,
+    
+    GPM_NRT_products,
+    GPM_RS_products, 
+    
     GPM_DPR_NRT_products,
-    GPM_DPR_RS_products,
+    GPM_PMW_NRT_products,
     GPM_IMERG_NRT_products,
-    GPM_IMERG_products,
+    GPM_CMB_NRT_products,
+
+    GPM_DPR_RS_products,
+    GPM_PMW_RS_products,
+    GPM_CMB_RS_products,
     GPM_IMERG_RS_products,
-    GPM_NRT_products,
-    GPM_PMW_1B_NRT_products,
-    GPM_PMW_1B_RS_products,
+    
+    GPM_DPR_1B_NRT_products,
     GPM_PMW_1C_NRT_products,
-    GPM_PMW_1C_RS_products,
+    GPM_DPR_2A_NRT_products,
+    GPM_DPR_2A_ENV_NRT_products,
+    GPM_PMW_1B_NRT_products,
     GPM_PMW_2A_GPROF_NRT_products,
-    GPM_PMW_2A_GPROF_RS_products,
     GPM_PMW_2A_PRPS_NRT_products,
-    GPM_PMW_2A_PRPS_RS_products,
-    GPM_PMW_NRT_products,
-    GPM_PMW_RS_products,
-    GPM_products,
-    GPM_RS_products,
-)
+    GPM_CMB_2B_NRT_products,  
+    GPM_IMERG_NRT_products,   
 
+    GPM_DPR_1B_RS_products,
+    GPM_DPR_2A_RS_products, 
+    GPM_DPR_2A_ENV_RS_products,
+    GPM_PMW_1A_RS_products, 
+    GPM_PMW_1B_RS_products,
+    GPM_PMW_1C_RS_products, 
+    GPM_PMW_2A_PRPS_RS_products, 
+    GPM_PMW_2A_GPROF_RS_products,
+    GPM_CMB_2B_RS_products,
+    GPM_IMERG_RS_products,
+   
+    GPM_1B_NRT_products,
+    GPM_1C_NRT_products,
+    GPM_2A_NRT_products,
+   
+    GPM_1B_RS_products,
+    GPM_1C_RS_products, 
+    GPM_2A_RS_products, 
+ 
+)
+ 
 GPM_DPR_1B_RS_products()
 GPM_DPR_1B_NRT_products()
 GPM_DPR_2A_RS_products()
 GPM_DPR_2A_NRT_products()
 GPM_DPR_2A_ENV_RS_products()
 GPM_DPR_2A_ENV_NRT_products()
 GPM_DPR_RS_products()
@@ -59,19 +74,19 @@
 GPM_PMW_2A_PRPS_RS_products()
 GPM_PMW_2A_PRPS_NRT_products()
 GPM_PMW_RS_products()
 GPM_PMW_NRT_products()
 
 GPM_CMB_2B_NRT_products()
 GPM_CMB_2B_RS_products()
-
+ 
 GPM_IMERG_NRT_products()
 GPM_IMERG_RS_products()
 GPM_IMERG_products()
-
+ 
 GPM_1B_RS_products()
 GPM_1B_NRT_products()
 GPM_1C_RS_products()
 GPM_1C_NRT_products()
 GPM_2A_RS_products()
 GPM_2A_NRT_products()
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/io/test_downloads.py` & `gpm_api-0.2.3/gpm_api/tests/io/test_downloads.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Mon Aug 17 11:54:23 2020
 
 @author: ghiggi
 """
+import numpy as np 
 import datetime
-
-import numpy as np
-
 import gpm_api
-from gpm_api.io.products import GPM_NRT_products, GPM_RS_products
+from gpm_api.io.products import GPM_RS_products, GPM_NRT_products, GPM_products
 
 ##----------------------------------------------------------------------------.
-### Donwload data
-base_dir = "/home/ghiggi/tmp"
+### Donwload data 
+base_dir = '/home/ghiggi/tmp'
 username = "gionata.ghiggi@epfl.ch"
 
 
 ##-----------------------------------------------------------------------------.
 ## Retrieve RS data
 version = 7
-product_type = "RS"
-products = GPM_RS_products()  # GPM_products(product_type)
+product_type = 'RS'
+products  = GPM_RS_products() # GPM_products(product_type)
 
-# Only GPM
-start_time = datetime.datetime.strptime("2020-08-09 15:00:00", "%Y-%m-%d %H:%M:%S")
-end_time = datetime.datetime.strptime("2020-08-09 17:00:00", "%Y-%m-%d %H:%M:%S")
+# Only GPM 
+start_time = datetime.datetime.strptime("2020-08-09 15:00:00", '%Y-%m-%d %H:%M:%S')
+end_time = datetime.datetime.strptime("2020-08-09 17:00:00", '%Y-%m-%d %H:%M:%S')
 
 # Both GPM-TRMM
-start_time = datetime.datetime.strptime("2014-08-09 00:00:00", "%Y-%m-%d %H:%M:%S")
-end_time = datetime.datetime.strptime("2014-08-09 03:00:00", "%Y-%m-%d %H:%M:%S")
+start_time = datetime.datetime.strptime("2014-08-09 00:00:00", '%Y-%m-%d %H:%M:%S')
+end_time = datetime.datetime.strptime("2014-08-09 03:00:00", '%Y-%m-%d %H:%M:%S')
 
 for product in products:
     print("Product:", product)
-    gpm_api.download(
-        base_dir=base_dir,
-        username=username,
-        product=product,
-        product_type=product_type,
-        version=version,
-        start_time=start_time,
-        end_time=end_time,
-        verbose=True,
-    )
-
+    gpm_api.download(base_dir = base_dir, 
+                     username = username,
+                     product = product, 
+                     product_type = product_type,
+                     version = version,
+                     start_time = start_time,
+                     end_time = end_time,
+                     verbose = True)
+    
 ##-----------------------------------------------------------------------------.
-## Retrieve NRT data
+## Retrieve NRT data 
 version = 6
-product_type = "NRT"
-products = GPM_NRT_products()  # GPM_products(product_type)
+product_type = 'NRT'
+products  = GPM_NRT_products()  # GPM_products(product_type)
 
 date = datetime.date.fromisoformat("2020-08-17")
 
-start_time = datetime.datetime.strptime("2020-08-17 00:00:00", "%Y-%m-%d %H:%M:%S")
-end_time = datetime.datetime.strptime("2020-08-17 04:00:00", "%Y-%m-%d %H:%M:%S")
+start_time = datetime.datetime.strptime("2020-08-17 00:00:00", '%Y-%m-%d %H:%M:%S')
+end_time = datetime.datetime.strptime("2020-08-17 04:00:00", '%Y-%m-%d %H:%M:%S')
 
 for product in products:
     print("Product:", product)
-    gpm_api.download(
-        base_dir=base_dir,
-        username=username,
-        product=product,
-        product_type=product_type,
-        start_time=start_time,
-        end_time=end_time,
-    )
-
+    gpm_api.download(base_dir = base_dir, 
+                     username = username,
+                     product = product, 
+                     product_type = product_type,
+                     start_time = start_time,
+                     end_time = end_time)
+    
 ##-----------------------------------------------------------------------------.
 ## Download data for a specific day
-date = np.datetime64("2017-01-01").astype(datetime.datetime)
+date = np.datetime64('2017-01-01').astype(datetime.datetime)
 version = 6
-product_type = "RS"
-product = "2A-Ku"
-base_dir = "/home/ghiggi/tmp"
-start_hhmmss = datetime.datetime.strptime("01:00:00", "%H:%M:%S")
-end_hhmmss = datetime.datetime.strptime("03:00:00", "%H:%M:%S")
-
-gpm_api.download(
-    base_dir=base_dir,
-    username=username,
-    version=version,
-    product=product,
-    product_type=product_type,
-    date=date,
-    start_hhmmss=start_hhmmss,
-    end_hhmmss=end_hhmmss,
-)
-# -----------------------------------------------------------------------------.
+product_type = 'RS'
+product = '2A-Ku'
+base_dir = '/home/ghiggi/tmp'
+start_hhmmss = datetime.datetime.strptime("01:00:00","%H:%M:%S")
+end_hhmmss =  datetime.datetime.strptime("03:00:00","%H:%M:%S")
+
+gpm_api.download(base_dir=base_dir, 
+                 username = username,
+                 version = version,
+                 product=product,
+                 product_type = product_type,
+                 date=date, 
+                 start_hhmmss=start_hhmmss,
+                 end_hhmmss=end_hhmmss)
+#-----------------------------------------------------------------------------.
+
+
+
+
+
+
+
+
+
+
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_archive.py` & `gpm_api-0.2.3/gpm_api/tests/test_archive.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,68 +2,69 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jan 19 16:19:22 2023
 
 @author: ghiggi
 """
 import datetime
-
 from gpm_api.utils.archive import (
-    check_archive_completness,
-    check_file_integrity,
     check_no_duplicated_files,
+    check_file_integrity,
+    check_archive_completness,
 )
 
 base_dir = "/ltenas8/data/GPM"
 product_type = "RS"
 product = "2A-DPR"
 version = 7
 start_time = datetime.datetime(2022, 2, 1)
 end_time = datetime.datetime(2022, 3, 1)
-download = True
-username = None
-transfer_tool = "wget"
-n_threads = 4
-verbose = True
-
+download=True
+username=None
+transfer_tool="wget"
+n_threads=4
+verbose=True
+ 
 check_no_duplicated_files(
-    base_dir=base_dir,
-    product=product,
+    base_dir=base_dir, 
+    product=product, 
     start_time=start_time,
-    end_time=end_time,
+    end_time=end_time, 
     version=version,
     product_type=product_type,
-    verbose=True,
+    verbose=True, 
 )
 
 check_file_integrity(
-    base_dir=base_dir,
-    product=product,
+    base_dir=base_dir, 
+    product=product, 
     start_time=start_time,
-    end_time=end_time,
+    end_time=end_time, 
     version=version,
     product_type=product_type,
     remove_corrupted=True,
-    verbose=True,
+    verbose=True, 
 )
 
 check_archive_completness(
-    base_dir=base_dir,
-    product=product,
+    base_dir=base_dir, 
+    product=product, 
     start_time=start_time,
-    end_time=end_time,
+    end_time=end_time, 
     version=version,
     product_type=product_type,
     download=True,
     username="gionata.ghiggi@epfl.ch",
     transfer_tool=transfer_tool,
     n_threads=n_threads,
     verbose=verbose,
 )
-
+   
 # TODO: SIMPLIFY periods by unique dates?
-# --> call download_daily_data instead in check_archive_completness
-list_missing_periods = [
-    ([datetime.datetime(2022, 2, 2, 22, 17, 44)], [datetime.datetime(2022, 2, 23, 1, 5, 7)]),
-    ([datetime.datetime(2022, 2, 26, 7, 45, 58)], [datetime.datetime(2022, 2, 26, 9, 18, 33)]),
-    ([datetime.datetime(2022, 2, 26, 20, 6, 31)], [datetime.datetime(2022, 2, 27, 0, 44, 15)]),
-]
+# --> call download_daily_data instead in check_archive_completness      
+list_missing_periods = [([datetime.datetime(2022, 2, 2, 22, 17, 44)],
+                         [datetime.datetime(2022, 2, 23, 1, 5, 7)]),
+                        ([datetime.datetime(2022, 2, 26, 7, 45, 58)],
+                         [datetime.datetime(2022, 2, 26, 9, 18, 33)]),
+                        ([datetime.datetime(2022, 2, 26, 20, 6, 31)],
+                         [datetime.datetime(2022, 2, 27, 0, 44, 15)])]
+
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_crs_cf.py` & `gpm_api-0.2.3/gpm_api/tests/test_crs_cf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,101 +1,103 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Wed Mar  8 11:09:49 2023
 
 @author: ghiggi
 """
-import numpy as np
-import pyproj
+import pyproj 
 import xarray as xr
+import numpy as np 
 
 
 def create_dummy_swath_ds():
-    # Define dataset
+    # Define dataset 
     variable = "variable"
     shape = (3, 5)
     data = np.zeros(shape)
     lat = np.linspace(0, 10, shape[0])
     lon = np.linspace(20, 40, shape[1])
     lons, lats = np.meshgrid(lon, lat)
-    coords = {"longitude": (("y", "x"), lons), "latitude": (("y", "x"), lats)}
+    coords = {"longitude": (("y","x"), lons), 
+              "latitude": (("y","x"), lats)}
     dims = ("y", "x")
     ds = xr.DataArray(data=data, coords=coords, dims=dims, name=variable).to_dataset()
-    # Define pyproj CRS
+    # Define pyproj CRS 
     crs = pyproj.CRS(proj="longlat", ellps="WGS84")
-    return ds, crs
+    return ds, crs 
 
 
 def create_dummy_proj_wgs84_ds():
-    # Define dataset
+    # Define dataset 
     variable = "variable"
     shape = (3, 5)
     data = np.zeros(shape)
     lat = np.linspace(0, 10, shape[0])
     lon = np.linspace(20, 40, shape[1])
-    coords = {"longitude": lon, "latitude": lat}
+    coords = {"longitude": lon, 
+              "latitude": lat}
     dims = ("latitude", "longitude")
     ds = xr.DataArray(data=data, coords=coords, dims=dims, name=variable).to_dataset()
-    # Define pyproj CRS
+    # Define pyproj CRS 
     crs = pyproj.CRS(proj="longlat", ellps="WGS84")
-    return ds, crs
+    return ds, crs 
 
 
 def create_dummy_proj_geo_radian_ds():
     # Define pyproj CRS (GOES-16)
-    proj_str = "+proj=geos +sweep=x +lon_0=-75 +h=35786023 +x_0=0 +y_0=0 +ellps=GRS80 +units=m +no_defs +type=crs"
+    proj_str = '+proj=geos +sweep=x +lon_0=-75 +h=35786023 +x_0=0 +y_0=0 +ellps=GRS80 +units=m +no_defs +type=crs'
     crs = pyproj.CRS(proj_str)
-    # Define dataset
+    # Define dataset 
     variable = "variable"
     shape = (3, 5)
     data = np.zeros(shape)
     coords = {
-        "y": np.arange(shape[0]),  # radians [0-3]
-        "x": np.arange(shape[1]),  # radians [0-5]
+          'y': np.arange(shape[0]), # radians [0-3]
+          'x': np.arange(shape[1]), # radians [0-5]
     }
-    dims = ("y", "x")
+    dims = ('y', 'x')
     ds = xr.DataArray(data=data, dims=dims, coords=coords, name=variable).to_dataset()
     # Set x,y unit to radian
     ds["x"].attrs["units"] = "radian"
     ds["y"].attrs["units"] = "radian"
-    # Return info
-    return ds, crs
-
+    # Return info 
+    return ds, crs 
+      
 
 def create_dummy_proj_geo_metre_ds():
     # Define pyproj CRS (GOES-16)
-    proj_str = "+proj=geos +sweep=x +lon_0=-75 +h=35786023 +x_0=0 +y_0=0 +ellps=GRS80 +units=m +no_defs +type=crs"
+    proj_str = '+proj=geos +sweep=x +lon_0=-75 +h=35786023 +x_0=0 +y_0=0 +ellps=GRS80 +units=m +no_defs +type=crs'
     crs = pyproj.CRS(proj_str)
     # Retrieve satellite height
     satellite_height = crs.to_dict()["h"]
-    # Define dataset
+    # Define dataset 
     variable = "variable"
     shape = (3, 5)
     data = np.zeros(shape)
     coords = {
-        "y": np.arange(shape[0]) * satellite_height,  # meter
-        "x": np.arange(shape[1]) * satellite_height,  # meter
+          'y': np.arange(shape[0])*satellite_height,  # meter
+          'x': np.arange(shape[1])*satellite_height,  # meter
     }
-    dims = ("y", "x")
+    dims = ('y', 'x')
     ds = xr.DataArray(data=data, dims=dims, coords=coords, name=variable).to_dataset()
     # Set x,y unit to metre
     ds["x"].attrs["units"] = "metre"
     ds["y"].attrs["units"] = "metre"
     return ds, crs
 
 
-def create_dummy_proj_polar_ds():
-    # Define pyproj CRS
-    proj_str = "+proj=laea +lat_0=-90 +lon_0=0 +a=6371228.0 +units=m"
+def create_dummy_proj_polar_ds(): 
+    # Define pyproj CRS 
+    proj_str = '+proj=laea +lat_0=-90 +lon_0=0 +a=6371228.0 +units=m'
     crs = pyproj.CRS(proj_str)
-    # Define dataset
+    # Define dataset 
     variable = "variable"
     shape = (3, 5)
     data = np.zeros(shape)
     coords = {
-        "y": np.arange(shape[0]),  # radians [0-3]
-        "x": np.arange(shape[1]),  # radians [0-5]
+          'y': np.arange(shape[0]), # radians [0-3]
+          'x': np.arange(shape[1]), # radians [0-5]
     }
-    dims = ("y", "x")
+    dims = ('y', 'x')
     ds = xr.DataArray(data=data, dims=dims, coords=coords, name=variable).to_dataset()
-    return ds, crs
+    return ds, crs
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_dataset.py` & `gpm_api-0.2.3/gpm_api/tests/test_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 """
 Created on Sat Dec 10 15:06:51 2022
 
 @author: ghiggi
 """
 from gpm_api.dataset.reader import open_granule, open_dataset
 
-scan_mode = None
-groups = None
-variables = None
-decode_cf = False
-chunks = "auto"
-prefix_group = True
+scan_mode=None
+groups=None
+variables=None
+decode_cf=False
+chunks="auto"
+prefix_group=True
 
 filepath = "/home/ghiggi/GPM/RS/V06/IMERG/IMERG-FR/2019/07/13/3B-HHR.MS.MRG.3IMERG.20190713-S123000-E125959.0750.V06B.HDF5"
 
 
 # IMERG-EARLY
-# 3B-HHR-E.MS.MRG.3IMERG.20221201-S020000-E022959.0120.V06C.RT-H5
-# # IMERG-LATE
-# 3B-HHR-L.MS.MRG.3IMERG.20221201-S023000-E025959.0150.V06C.RT-H5
-# # IMERG FINAL
-# 3B-HHR.MS.MRG.3IMERG.20190713-S123000-E125959.0750.V06B.HDF5
+3B-HHR-E.MS.MRG.3IMERG.20221201-S020000-E022959.0120.V06C.RT-H5
+# IMERG-LATE
+3B-HHR-L.MS.MRG.3IMERG.20221201-S023000-E025959.0150.V06C.RT-H5
+# IMERG FINAL 
+3B-HHR.MS.MRG.3IMERG.20190713-S123000-E125959.0750.V06B.HDF5"
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_dataset_regularity.py` & `gpm_api-0.2.3/gpm_api/tests/test_dataset_regularity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jan  4 19:36:49 2023
 
 @author: ghiggi
 """
+import os
 import datetime
-
 import numpy as np
-
 import gpm_api
+from dask.diagnostics import ProgressBar
 
 base_dir = "/home/ghiggi"
 
 #### Define analysis time period
 start_time = datetime.datetime.strptime("2020-08-01 12:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2020-08-10 12:00:00", "%Y-%m-%d %H:%M:%S")
 
@@ -35,47 +35,51 @@
 )
 
 ds = ds.compute()
 
 ds.isel(along_track=slice(0, 10000)).gpm_api.plot_map(variable=variable)
 
 ###---------------------------------------------------------------------------.
-from gpm_api.utils.checks import get_contiguous_scan_slices, get_discontiguous_scan_slices
+from gpm_api.utils.checks import get_regular_time_slices
+from gpm_api.utils.checks import get_nonregular_time_slices
+from gpm_api.utils.checks import get_contiguous_scan_slices
+from gpm_api.utils.checks import get_discontiguous_scan_slices
 
 ds.gpm_api.is_regular
 ds.gpm_api.has_regular_timesteps
 ds.gpm_api.has_contiguous_scans
 ds.gpm_api.get_regular_time_slices()
 ds.gpm_api.get_contiguous_scan_slices()
 
-#### Operational checks
+#### Operational checks 
 gpm_api.check_regular_timesteps(ds)
 gpm_api.check_contiguous_scans(ds)
 gpm_api.check_valid_geolocation(ds)
 
 ###---------------------------------------------------------------------------.
-# Mock discontinguous and test plotting
+# Mock discontinguous and test plotting 
 indices = np.arange(0, 1000)
 ds.isel(along_track=indices).gpm_api.plot_map(variable=variable)
 indices = np.append(indices[0:200], indices[800:1000])
 ds.isel(along_track=indices).gpm_api.get_contiguous_scan_slices()
 ds.isel(along_track=indices).gpm_api.plot_map(variable=variable)
 
 ###---------------------------------------------------------------------------.
 # Investigate PMW scan discontinuities
 list_slices = get_discontiguous_scan_slices(ds)
-ds.isel(along_track=list_slices[0])["gpm_id"]  # at granule change
+ds.isel(along_track=list_slices[0])['gpm_id'] # at granule change 
 ds.isel(along_track=list_slices[0]).gpm_api.plot_map(variable=variable)
 
 slice_problem_occurence = list_slices[0]
 print(slice_problem_occurence)
-da = ds[variable].isel(along_track=slice_problem_occurence)  # size 2
-get_contiguous_scan_slices(da)  # not possible to discern if only 2 scans
+da = ds[variable].isel(along_track=slice_problem_occurence) # size 2
+get_contiguous_scan_slices(da) # not possible to discern if only 2 scans
 p = da.gpm_api.plot_map_mesh(edgecolors="r")
 
-slice_enlarged = slice(slice_problem_occurence.start - 1, slice_problem_occurence.stop + 1)
+slice_enlarged = slice(slice_problem_occurence.start-1, slice_problem_occurence.stop+1)
 print(slice_enlarged)
-da = ds[variable].isel(along_track=slice_enlarged)  # size 4
-get_contiguous_scan_slices(da)  # 0-1 ... and 2-3
+da = ds[variable].isel(along_track=slice_enlarged) # size 4
+get_contiguous_scan_slices(da) # 0-1 ... and 2-3
 da.gpm_api.plot_map_mesh(ax=p.axes)
 
 ###---------------------------------------------------------------------------.
+
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_dataset_valid_geolocation.py` & `gpm_api-0.2.3/gpm_api/tests/test_dataset_valid_geolocation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jan  5 00:36:59 2023
 
 @author: ghiggi
 """
+import os
 import datetime
-
 import numpy as np
-
 import gpm_api
+from dask.diagnostics import ProgressBar
 
 ###----------------------------------------------------------------------------.
 base_dir = "/home/ghiggi"
 start_time = datetime.datetime.strptime("2020-08-01 12:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2020-08-10 12:00:00", "%Y-%m-%d %H:%M:%S")
 product = "2A-SSMIS-F16"
 product_type = "RS"
-variable = "surfacePrecipitation"
+variable = "surfacePrecipitation" 
 
 ds = gpm_api.open_dataset(
     base_dir=base_dir,
     product=product,
-    product_type=product_type,
+    product_type = product_type,
     start_time=start_time,
     end_time=end_time,
     # Optional
     version=7,
     variables=variable,
-    # decode_cf=True,
+    # decode_cf=True, 
     chunks="auto",
     prefix_group=False,
 )
 
 ds = ds.compute()
 ds1 = ds
 
@@ -40,27 +40,27 @@
 
 ds = ds.isel(along_track=slice(0, 10000))
 
 ds[variable].gpm_api.plot_map()
 
 # -----------------------------------------------------------------------------.
 ### TODO: add checks when missing coordinates
-# 3. Implement missing coordinates checks
-# 4. Test get_contiguous_scan_slices when missing coordinates
-# 4. Test plotting for missing coordinates ---> mask !
+# 3. Implement missing coordinates checks 
+# 4. Test get_contiguous_scan_slices when missing coordinates   
+# 4. Test plotting for missing coordinates ---> mask ! 
 #   --> No unvalid coordinates
-#   --> Mask for plotting
-#   --> Do not mask for crop
+#   --> Mask for plotting 
+#   --> Do not mask for crop 
 
-# --> When mask --- when decoding cf ... or custom afterwards !
-# --> Mask variables only?
-# --> xarray does not allow masked coordinates
+# --> When mask --- when decoding cf ... or custom afterwards ! 
+# --> Mask variables only? 
+# --> xarray does not allow masked coordinates 
 gpm_api.check_valid_geolocation()
 
-# Coordinate -9999
+# Coordinate -9999 
 
 idx_nan = np.where(ds["lat"].data == -9999)
 
 ds = ds.where(ds["lat"] != -9999, np.nan)
 ds = ds.where(ds["lon"] != -9999, np.nan)
 
 xr.where(ds.lon == -9999)
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_disk.py` & `gpm_api-0.2.3/gpm_api/tests/test_disk.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,46 +2,43 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Dec  9 15:46:47 2022
 
 @author: ghiggi
 """
 import datetime
-
 from gpm_api.io.disk import _find_daily_filepaths, find_filepaths
 
 filepaths = "/home/ghiggi/GPM/RS/V07/RADAR/2A-DPR/2020/07/05/"
-
+             
 base_dir = "/home/ghiggi/GPM"
 product = "2A-DPR"
-date = datetime.date(2020, 7, 5)  # OK
+date = datetime.date(2020, 7, 5) # OK
 # date = datetime.date(2020, 7, 3) # NO
-version = 7
-start_time = None
-end_time = None
-product_type = "RS"
-verbose = True
-
-filepaths = _find_daily_filepaths(
-    base_dir=base_dir,
-    product=product,
-    product_type=product_type,
-    date=date,
-    version=version,
-    start_time=start_time,
-    end_time=end_time,
-    verbose=verbose,
-)
+version=7
+start_time=None
+end_time=None
+product_type='RS'
+verbose=True
+
+filepaths = _find_daily_filepaths(base_dir=base_dir,
+                                  product=product, 
+                                  product_type=product_type,
+                                  date=date,  
+                                  version=version,
+                                  start_time=start_time, 
+                                  end_time=end_time,
+                                  verbose=verbose)
 
 
 start_time = datetime.datetime(2020, 7, 5, 0, 2, 0)
 end_time = datetime.datetime(2020, 7, 5, 0, 3, 0)
 
-filepaths = find_filepaths(
-    base_dir=base_dir,
-    product=product,
-    product_type=product_type,
-    version=version,
-    start_time=start_time,
-    end_time=end_time,
-    verbose=verbose,
-)
+filepaths = find_filepaths(base_dir=base_dir,
+                           product=product,  
+                           product_type=product_type,
+                           version=version,
+                           start_time=start_time, 
+                           end_time=end_time,
+                           verbose=verbose)
+
+
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_download.py` & `gpm_api-0.2.3/gpm_api/tests/test_download.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,102 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Fri Dec  9 18:08:16 2022
 
 @author: ghiggi
 """
+import numpy as np 
 import datetime
-import time
+import time 
+from gpm_api.io.download import download_data, wget_cmd, curl_cmd, run
 
-import numpy as np
-
-from gpm_api.io.download import curl_cmd, download_data, run, wget_cmd
 
 ####-------------------------------------------------------------------------.
-#### Test gpm_api.download function
+#### Test gpm_api.download function  
 base_dir = "/home/ghiggi/GPM"
 product = "2A-DPR"
-product_type = "RS"
-username = "gionata.ghiggi@epfl.ch"
+product_type='RS'
+username="gionata.ghiggi@epfl.ch"
 start_time = datetime.datetime(2020, 7, 5, 0, 2, 0)
 end_time = datetime.datetime(2020, 7, 6, 0, 4, 0)
-version = 7
+version=7
 
-verbose = True
+verbose=True
 progress_bar = True
 force_download = False
 check_integrity = True
-remove_corrupted = False  # True
-n_threads = 4
-transfer_tool = "curl"  # works
-transfer_tool = "wget"  # buggy ... especially with lot of threads
-
-l_corrupted = download_data(
-    base_dir=base_dir,
-    username=username,
-    product=product,
-    start_time=start_time,
-    end_time=end_time,
-    product_type=product_type,
-    version=version,
-    n_threads=n_threads,
-    transfer_tool=transfer_tool,
-    progress_bar=progress_bar,
-    force_download=force_download,
-    check_integrity=check_integrity,
-    remove_corrupted=remove_corrupted,
-    verbose=verbose,
-)
+remove_corrupted = False # True 
+n_threads = 4  
+transfer_tool = "curl" # works 
+transfer_tool = "wget" # buggy ... especially with lot of threads
+
+l_corrupted = download_data(base_dir=base_dir, 
+                            username=username, 
+                            product=product, 
+                            start_time=start_time,
+                            end_time=end_time,
+                            product_type=product_type,
+                            version=version,
+                            n_threads=n_threads,
+                            transfer_tool=transfer_tool,
+                            progress_bar=progress_bar, 
+                            force_download=force_download,
+                            check_integrity=check_integrity, 
+                            remove_corrupted=remove_corrupted, 
+                            verbose=verbose)
 
 ####-------------------------------------------------------------------------.
-#### Test single file download with curl and wget
+#### Test single file download with curl and wget 
 server_path = "ftps://arthurhouftps.pps.eosdis.nasa.gov/gpmdata/2020/07/05/radar/2A.GPM.DPR.V9-20211125.20200705-S170044-E183317.036092.V07A.HDF5"
 disk_path1 = "/tmp/dummy1.hdf"
 disk_path2 = "/tmp/dummy2.hdf"
 username = "gionata.ghiggi@epfl.ch"
 password = username
 
-### WGET
+### WGET 
 t_i = time.time()
 cmd = wget_cmd(server_path, disk_path1, username, password)
 print(cmd)
 run([cmd], n_threads=10, progress_bar=True, verbose=True)
 t_f = time.time()
 t_elapsed = np.round(t_f - t_i, 2)
-print(t_elapsed, "seconds")  # 96.6 seconds
+print(t_elapsed, "seconds") # 96.6 seconds  
 
-### CURL cmd
+### CURL cmd 
 t_i = time.time()
 cmd = curl_cmd(server_path, disk_path2, username, password)
-print(cmd)
+print(cmd) 
 run([cmd], n_threads=10, progress_bar=True, verbose=True)
 t_f = time.time()
 t_elapsed = np.round(t_f - t_i, 2)
-print(t_elapsed, "seconds")  # 102.6 seconds
+print(t_elapsed, "seconds") # 102.6 seconds  
 
 
 #### ------------------------------------------------------------------------
-#### Test download with ftplib
+#### Test download with ftplib 
+from gpm_api.io.pps import find_pps_filepaths
 from gpm_api.io.download import (
-    convert_pps_to_disk_filepaths,
+    convert_pps_to_disk_filepaths, 
     filter_download_list,
     ftplib_download,
 )
-from gpm_api.io.pps import find_pps_filepaths
+
 
 username = "gionata.ghiggi@epfl.ch"
 password = "gionata.ghiggi@epfl.ch"
-n_threads = 4
+n_threads = 4 
 
 pps_filepaths = find_pps_filepaths(
     username=username,
     product=product,
     product_type=product_type,
     version=version,
     start_time=start_time,
-    end_time=end_time,
+    end_time=end_time, 
     verbose=verbose,
 )
 
 disk_filepaths = convert_pps_to_disk_filepaths(
     pps_filepaths=pps_filepaths,
     base_dir=base_dir,
     product=product,
@@ -111,34 +109,32 @@
     server_paths=pps_filepaths,
     force_download=force_download,
 )
 
 pps_filepaths = pps_filepaths[0:4]
 disk_filepaths = disk_filepaths[0:4]
 
-ftplib_download(
-    server_paths=pps_filepaths,
-    disk_paths=disk_filepaths,
-    username=username,
-    password=password,
-    n_threads=n_threads,
-)
+ftplib_download(server_paths=pps_filepaths,
+                disk_paths=disk_filepaths, 
+                username=username,
+                password=password, 
+                n_threads=n_threads)
 
 ####-------------------------------------------------------------------------.
-#### Test multiple download at once
-from gpm_api.io.download import convert_pps_to_disk_filepaths, filter_download_list
+#### Test multiple download at once 
 from gpm_api.io.pps import find_pps_filepaths
+from gpm_api.io.download import convert_pps_to_disk_filepaths, filter_download_list
 
 pps_filepaths = find_pps_filepaths(
     username=username,
     product=product,
     product_type=product_type,
     version=version,
     start_time=start_time,
-    end_time=end_time,
+    end_time=end_time, 
     verbose=verbose,
 )
 
 disk_filepaths = convert_pps_to_disk_filepaths(
     pps_filepaths=pps_filepaths,
     base_dir=base_dir,
     product=product,
@@ -147,30 +143,30 @@
 )
 
 pps_filepaths, disk_filepaths = filter_download_list(
     disk_paths=disk_filepaths,
     server_paths=pps_filepaths,
     force_download=force_download,
 )
-
-#### WGET
-import tempfile
-
-# Open temporary file
+ 
+#### WGET  
+import tempfile 
+# Open temporary file 
 temp_files = tempfile.NamedTemporaryFile(mode="w+", suffix=".txt")
-# Create download file list to be read by wget or curl
+# Create download file list to be read by wget or curl 
 for pps_path, disk_path in zip(pps_filepaths[0:2], disk_filepaths[0:2]):
     temp_files.write(f"{pps_path} {disk_path}\n")
 temp_files.seek(0)
 
 # Print the path to the temporary file
 print(temp_files.name)
+ 
 
-
-password = username
+ 
+password = username 
 cmd = "".join(
     [
         "wget ",
         "-4 ",
         "--ftp-user=",
         username,
         " ",
@@ -184,43 +180,42 @@
         "-c ",  # continue from where it left
         "--read-timeout=",
         "10",
         " ",  # if no data arriving for 10 seconds, retry
         "--tries=",
         "5",
         " ",  # retry 5 times (0 forever)
-        "--show-progress ",
+        "--show-progress ", 
         # "-P ",
-        # "4",
-        # " ",
-        "-i ",
+        # "4", 
+        # " ", 
+        "-i ", 
         temp_files.name,
     ]
 )
-
+ 
 # cmd
 
 # wget -4 --ftp-user=gionata.ghiggi@epfl.ch --ftp-password=gionata.ghiggi@epfl.ch --show-progress -P 1 -i /tmp/tmptj56j27u.txt
-
+ 
 # Remove the temporary file
-temp_file.close()
+temp_file.close() 
 
 ###----------------------------
 #### - CURL
-import tempfile
-
-# Open temporary file
+import tempfile 
+# Open temporary file 
 temp_files = tempfile.NamedTemporaryFile(mode="w+", suffix=".txt")
-# Create download file list to be read by wget or curl
+# Create download file list to be read by wget or curl 
 for pps_path, disk_path in zip(pps_filepaths[0:2], disk_filepaths[0:2]):
-    pps_path = pps_path.replace("ftps", "ftp", 1)  # REQUIRED BY CURL
+    pps_path = pps_path.replace("ftps", "ftp", 1) # REQUIRED BY CURL 
     temp_files.write(f"url = {pps_path}\noutput = {disk_path}\n")
 temp_files.seek(0)
-
-password = username
+ 
+password = username 
 cmd = "".join(
     [
         "curl ",
         "--verbose ",
         "--ipv4 ",
         "--insecure ",
         "--user ",
@@ -230,91 +225,87 @@
         " ",
         "--ftp-ssl ",
         # Custom settings
         "--header 'Connection: close' ",
         "--connect-timeout 20 ",
         "--retry 5 ",
         "--retry-delay 10 ",
-        # "-m 4 ", # number of parallel files  # this cause stuffs to not work
+        # "-m 4 ", # number of parallel files  # this cause stuffs to not work 
         "-n ",
-        "-K ",
-        temp_files.name,
+        "-K ", 
+        temp_files.name, 
     ]
 )
 
 print(cmd)
 
 #### ------------------------------------------------------------------------
-#### Test download monthly data
+#### Test download monthly data 
 from gpm_api.utils.archive import download_monthly_data
-
 base_dir = "/home/ghiggi/GPM"
 product = "2A-DPR"
-product_type = "RS"
-username = "gionata.ghiggi@epfl.ch"
+product_type='RS'
+username="gionata.ghiggi@epfl.ch"
 year = 2020
 month = 7
 version = 7
-verbose = True
+verbose=True
 progress_bar = True
 force_download = False
 check_integrity = True
-remove_corrupted = False  # True
-n_threads = 4
-transfer_tool = "curl"  # works
-transfer_tool = "wget"  # buggy ... especially with lot of threads
-
-l_corrupted = download_monthly_data(
-    base_dir=base_dir,
-    username=username,
-    product=product,
-    year=year,
-    month=month,
-    product_type=product_type,
-    version=version,
-    n_threads=n_threads,
-    transfer_tool=transfer_tool,
-    progress_bar=progress_bar,
-    force_download=force_download,
-    check_integrity=check_integrity,
-    remove_corrupted=remove_corrupted,
-    verbose=verbose,
-)
+remove_corrupted = False # True 
+n_threads = 4  
+transfer_tool = "curl" # works 
+transfer_tool = "wget" # buggy ... especially with lot of threads
+
+l_corrupted = download_monthly_data(base_dir=base_dir, 
+                                    username=username, 
+                                    product=product, 
+                                    year=year,
+                                    month=month,
+                                    product_type=product_type,
+                                    version=version,
+                                    n_threads=n_threads,
+                                    transfer_tool=transfer_tool,
+                                    progress_bar=progress_bar, 
+                                    force_download=force_download,
+                                    check_integrity=check_integrity, 
+                                    remove_corrupted=remove_corrupted, 
+                                    verbose=verbose)
 
 
 #### ------------------------------------------------------------------------
-#### Test download GPM IMERG
-import datetime
-
-import gpm_api
-
-base_dir = "/home/ghiggi/GPM"
-start_time = datetime.datetime.strptime("2019-07-13 11:00:00", "%Y-%m-%d %H:%M:%S")
-end_time = datetime.datetime.strptime("2019-07-13 13:00:00", "%Y-%m-%d %H:%M:%S")
-product = "IMERG-FR"  # 'IMERG-ER' 'IMERG-LR'
-product_type = "RS"
+#### Test download GPM IMERG 
+import gpm_api 
+import datetime 
+
+base_dir = '/home/ghiggi/GPM'
+start_time = datetime.datetime.strptime("2019-07-13 11:00:00", '%Y-%m-%d %H:%M:%S')
+end_time = datetime.datetime.strptime("2019-07-13 13:00:00", '%Y-%m-%d %H:%M:%S')
+product = 'IMERG-FR'  # 'IMERG-ER' 'IMERG-LR'
+product_type = 'RS'
 version = 6
-username = "gionata.ghiggi@epfl.ch"
+username = "gionata.ghiggi@epfl.ch" 
 n_threads = 1
-force_download = False
-verbose = True
-progress_bar = True
-check_integrity = True
-transfer_tool = "curl"
-remove_corrupted = True
-
+force_download = False                
+verbose=True
+progress_bar=True
+check_integrity=True
+transfer_tool="curl"
+remove_corrupted=True
 
+    
 # Download the data
-gpm_api.download(
-    base_dir=base_dir,
-    username=username,
-    product=product,
-    product_type=product_type,
-    version=version,
-    start_time=start_time,
-    end_time=end_time,
-    force_download=force_download,
-    verbose=verbose,
-    progress_bar=progress_bar,
-    check_integrity=check_integrity,
-    n_threads=n_threads,
-)
+gpm_api.download(base_dir = base_dir, 
+                 username = username,
+                 product = product, 
+                 product_type = product_type,
+                 version = version, 
+                 start_time = start_time,
+                 end_time = end_time, 
+                 force_download = force_download,                 
+                 verbose=verbose, 
+                 progress_bar=progress_bar,
+                 check_integrity=check_integrity, 
+                 n_threads=n_threads)
+
+
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_filter.py` & `gpm_api-0.2.3/gpm_api/tests/test_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,46 +4,52 @@
 Created on Fri Dec  9 13:14:43 2022
 
 @author: ghiggi
 """
 from gpm_api.io.filter import (
     _filter_filepath,
     filter_filepaths,
+    filter_by_product,
+    filter_by_time, 
+    filter_by_version,
 )
 
-filepaths = [
-    "/home/ghiggi/GPM/RS/V07/RADAR/2A-DPR/2020/07/05/2A.GPM.DPR.V9-20211125.20200705-S000234-E013507.036081.V07A.HDF5",
-    "/home/ghiggi/GPM/RS/V07/RADAR/2A-DPR/2020/07/05/2A.GPM.DPR.V9-20211125.20200705-S000234-E013507.036081.V07A.HDF5",
-]
+filepaths = ["/home/ghiggi/GPM/RS/V07/RADAR/2A-DPR/2020/07/05/2A.GPM.DPR.V9-20211125.20200705-S000234-E013507.036081.V07A.HDF5", 
+            "/home/ghiggi/GPM/RS/V07/RADAR/2A-DPR/2020/07/05/2A.GPM.DPR.V9-20211125.20200705-S000234-E013507.036081.V07A.HDF5"]
 filepath = filepaths[0]
 
 
 product = "2A-DPR"
-version = 7
-start_time = None
-end_time = None
-product_type = "RS"
-
-filter_filepaths(
-    filepaths, product=product, product_type=product_type, start_time=None, end_time=None
-)
+version=7
+start_time=None
+end_time=None
+product_type='RS'
+
+filter_filepaths(filepaths,
+                 product=product,
+                 product_type=product_type,
+                 start_time=None,
+                 end_time=None)
+
+_filter_filepath(filepath,
+                 product=None, 
+                 version=5,
+                 start_time=None, 
+                 end_time=None)
 
-_filter_filepath(filepath, product=None, version=5, start_time=None, end_time=None)
 
-
-# Test imerg filtering
+# Test imerg filtering 
 # - First should be discarded
 # - Second should be mantained
 import datetime
-
-start_time = datetime.datetime.strptime("2019-07-12 11:00:00", "%Y-%m-%d %H:%M:%S")
-end_time = datetime.datetime.strptime("2019-07-12 13:30:00", "%Y-%m-%d %H:%M:%S")
+start_time = datetime.datetime.strptime("2019-07-12 11:00:00", '%Y-%m-%d %H:%M:%S')
+end_time = datetime.datetime.strptime("2019-07-12 13:30:00", '%Y-%m-%d %H:%M:%S')
 product_type = "RS"
 version = 6
-filepaths = [
-    "ftps://arthurhouftps.pps.eosdis.nasa.gov/gpmallversions/V06/2019/07/12/imerg/3B-HHR.MS.MRG.3IMERG.20190712-S100000-E102959.0600.V06B.HDF5",
-    "ftps://arthurhouftps.pps.eosdis.nasa.gov/gpmallversions/V06/2019/07/12/imerg/3B-HHR.MS.MRG.3IMERG.20190712-S130000-E132959.0780.V06B.HDF5",
-]
+filepaths = ['ftps://arthurhouftps.pps.eosdis.nasa.gov/gpmallversions/V06/2019/07/12/imerg/3B-HHR.MS.MRG.3IMERG.20190712-S100000-E102959.0600.V06B.HDF5',
+             'ftps://arthurhouftps.pps.eosdis.nasa.gov/gpmallversions/V06/2019/07/12/imerg/3B-HHR.MS.MRG.3IMERG.20190712-S130000-E132959.0780.V06B.HDF5']
 
-filter_filepaths(
-    filepaths, product=product, product_type=product_type, start_time=start_time, end_time=end_time
-)
+filter_filepaths(filepaths,
+                 product=product,
+                 product_type=product_type,
+                 start_time=start_time,
+                 end_time=end_time)
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_image_labels.py` & `gpm_api-0.2.3/gpm_api/tests/test_image_labels.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jan 11 15:41:22 2023
 
 @author: ghiggi
 """
+import gpm_api
 import datetime
-
 import numpy as np
 import xarray as xr
 
-import gpm_api
 
 base_dir = "/home/ghiggi/GPM"
 start_time = datetime.datetime.strptime("2019-07-13 11:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2019-07-13 13:00:00", "%Y-%m-%d %H:%M:%S")
 product = "IMERG-FR"  # 'IMERG-ER' 'IMERG-LR'
 product_type = "RS"
 version = 6
@@ -53,113 +52,110 @@
 
 # Select variable
 variable = "precipitationCal"
 
 da = ds[variable].isel(time=0)
 
 ####---------------------------------------------------------------------------.
-import numpy as np
-
+import numpy as np 
 from gpm_api.patch.labels import xr_get_areas_labels
 
-# Args labels
-min_value_threshold = 1
-max_value_threshold = np.inf
-min_area_threshold = 5
-max_area_threshold = np.inf
-footprint = None
-sort_by = "area"
-sort_decreasing = True
+# Args labels 
+min_value_threshold=1
+max_value_threshold=np.inf
+min_area_threshold=5
+max_area_threshold=np.inf
+footprint=None
+sort_by="area"
+sort_decreasing=True
 
 data_array = da
-
+ 
 da_labels, n_labels, values = xr_get_areas_labels(
     data_array=data_array,
     min_value_threshold=min_value_threshold,
     max_value_threshold=max_value_threshold,
     min_area_threshold=min_area_threshold,
     max_area_threshold=max_area_threshold,
     footprint=footprint,
     sort_by=sort_by,
     sort_decreasing=sort_decreasing,
 )
 
-da_labels.plot.imshow()  # 0 are plotted
+da_labels.plot.imshow() # 0 are plotted 
 
 ####---------------------------------------------------------------------------.
-#### Check equality
+#### Check equality 
 from gpm_api.patch.labels import label_xarray_object
-
-# Retrieve labeled xarray object
-xr_obj = label_xarray_object(
-    da,
-    min_value_threshold=min_value_threshold,
-    max_value_threshold=max_value_threshold,
-    min_area_threshold=min_area_threshold,
-    max_area_threshold=max_area_threshold,
-    footprint=footprint,
-    sort_by=sort_by,
-    sort_decreasing=sort_decreasing,
-    label_name="label",
-)
+# Retrieve labeled xarray object 
+xr_obj = label_xarray_object(da, 
+                             min_value_threshold=min_value_threshold,
+                             max_value_threshold=max_value_threshold,
+                             min_area_threshold=min_area_threshold,
+                             max_area_threshold=max_area_threshold,
+                             footprint=footprint,
+                             sort_by=sort_by,
+                             sort_decreasing=sort_decreasing,
+                             label_name="label",
+                             )
 xr_obj1 = da.gpm_api.label_object(
     min_value_threshold=min_value_threshold,
     max_value_threshold=max_value_threshold,
     min_area_threshold=min_area_threshold,
     max_area_threshold=max_area_threshold,
     footprint=footprint,
     sort_by=sort_by,
     sort_decreasing=sort_decreasing,
     label_name="label",
-)
-
-da_labels.plot.imshow()  # 0 are plotted
-
-xr_obj["label"].plot.imshow()  # 0 became nan --> Are not plotted
+    )
+ 
+da_labels.plot.imshow() # 0 are plotted 
+ 
+xr_obj["label"].plot.imshow() # 0 became nan --> Are not plotted 
 xr_obj1["label"].plot.imshow()
 xr.testing.assert_equal(xr_obj["label"], xr_obj1["label"])
 np.testing.assert_equal(xr_obj["label"].data, da_labels.where(da_labels > 0).data)
-
+ 
 ####---------------------------------------------------------------------------.
-#### Visualize labels patches
+#### Visualize labels patches 
 
 from gpm_api.visualization.labels import plot_label_patches
 
-# Args labels
-min_value_threshold = 1
-max_value_threshold = np.inf
-min_area_threshold = 5
-max_area_threshold = np.inf
-footprint = None
-footprint = 15
-sort_by = "area"
-sort_decreasing = True
+# Args labels 
+min_value_threshold=1
+max_value_threshold=np.inf
+min_area_threshold=5
+max_area_threshold=np.inf
+footprint=None
+footprint=15
+sort_by="area"
+sort_decreasing=True
 
 xr_obj = da.gpm_api.label_object(
     min_value_threshold=min_value_threshold,
     max_value_threshold=max_value_threshold,
     min_area_threshold=min_area_threshold,
     max_area_threshold=max_area_threshold,
     footprint=footprint,
     sort_by=sort_by,
     sort_decreasing=sort_decreasing,
     label_name="label",
-)
-
+    )
+ 
 # xr_obj["label"].plot.imshow()
 
 # Plot the patches around the labels
-n_patches = 10
+n_patches=10
 label_name = "label"
-add_colorbar = True
-interpolation = "nearest"
-cmap = "Paired"
-fig_kwargs = {}
-
-plot_label_patches(
-    xr_obj,
-    label_name=label_name,
-    n_patches=n_patches,
-    add_colorbar=add_colorbar,
-    interpolation=interpolation,
-    cmap=cmap,
-)
+add_colorbar=True
+interpolation="nearest"
+cmap="Paired"
+fig_kwargs={}
+
+plot_label_patches(xr_obj, 
+                   label_name=label_name,
+                   n_patches=n_patches, 
+                   add_colorbar=add_colorbar,
+                   interpolation=interpolation, 
+                   cmap=cmap)
+
+
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_image_labels_patch.py` & `gpm_api-0.2.3/gpm_api/tests/test_image_labels_patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jan 12 11:04:56 2023
 
 @author: ghiggi
 """
-import datetime
-
+import xarray as xr
 import gpm_api
+import datetime
 
 base_dir = "/home/ghiggi/GPM"
 start_time = datetime.datetime.strptime("2019-07-13 11:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2019-07-13 13:00:00", "%Y-%m-%d %H:%M:%S")
 product = "IMERG-FR"  # 'IMERG-ER' 'IMERG-LR'
 product_type = "RS"
 version = 6
@@ -63,69 +63,65 @@
 #     n_patches=10,
 #     padding=0,
 #     min_patch_size=(20, 20),
 # )
 # list_patch = list(patch_gen)
 
 
-# ----------------------------------------------------------------------------.
+#----------------------------------------------------------------------------.
 # DEBUG
-import numpy as np
-
+import numpy as np 
 from gpm_api.patch.labels import label_xarray_object
 from gpm_api.patch.labels_patch import get_labeled_object_patches
 from gpm_api.visualization.labels import plot_label
 
-# Args labels
-min_value_threshold = 1
-max_value_threshold = np.inf
-min_area_threshold = 5
-max_area_threshold = np.inf
-footprint = None
-sort_by = "area"
-sort_decreasing = True
-label_name = "label"
-
-# Retrieve labeled xarray object
-xr_obj = label_xarray_object(
-    da,
-    min_value_threshold=min_value_threshold,
-    max_value_threshold=max_value_threshold,
-    min_area_threshold=min_area_threshold,
-    max_area_threshold=max_area_threshold,
-    footprint=footprint,
-    sort_by=sort_by,
-    sort_decreasing=sort_decreasing,
-    label_name=label_name,
-)
+# Args labels 
+min_value_threshold=1
+max_value_threshold=np.inf
+min_area_threshold=5
+max_area_threshold=np.inf
+footprint=None
+sort_by="area"
+sort_decreasing=True
+label_name="label"
+
+# Retrieve labeled xarray object 
+xr_obj = label_xarray_object(da, 
+                             min_value_threshold=min_value_threshold,
+                             max_value_threshold=max_value_threshold,
+                             min_area_threshold=min_area_threshold,
+                             max_area_threshold=max_area_threshold,
+                             footprint=footprint,
+                             sort_by=sort_by,
+                             sort_decreasing=sort_decreasing,
+                             label_name=label_name,
+                             )
 
 # Build a generator returning patches around rainy areas
-n_patches = 20
+n_patches=20
 labels_id = None
 padding = None
-min_patch_size = (100, 100)
+min_patch_size=(100, 100)
 highlight_label_id = False
 
 
 da_patch_gen = get_labeled_object_patches(
-    xr_obj,
-    label_name=label_name,
-    n_patches=n_patches,
+    xr_obj, label_name=label_name, n_patches=n_patches, 
     min_patch_size=min_patch_size,
-    highlight_label_id=highlight_label_id,
+    highlight_label_id=highlight_label_id, 
 )
 
 list_patch = list(da_patch_gen)
 
 da_patch = list_patch[7]
 da_patch.gpm_api.plot_image()
 da_patch[label_name].plot.imshow()
 plot_label(da_patch[label_name])
 
 for da_patch in list_patch:
     da_patch.gpm_api.plot_image()
-
+    
 for da_patch in list_patch:
     print(da_patch.shape)
 
 for da_patch in list_patch:
-    plot_label(da_patch[label_name])
+    plot_label(da_patch[label_name])
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_io.py` & `gpm_api-0.2.3/gpm_api/tests/test_io.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Dec  8 17:18:30 2022
 
 @author: ghiggi
 """
-import datetime
+import datetime 
 
 start_time = datetime.datetime(2020, 7, 11, 0, 25, 25)
 end_time = datetime.datetime(2020, 7, 11, 0, 26, 27)
 date = datetime.datetime(2020, 7, 11, 0, 0)
 
-start_hhmmss = datetime.datetime.strftime(start_time, "%H%M%S")
-end_hhmmss = datetime.datetime.strftime(end_time, "%H%M%S")
-
-
+start_hhmmss = datetime.datetime.strftime(start_time,"%H%M%S")
+end_hhmmss = datetime.datetime.strftime(end_time,"%H%M%S")
+    
+    
 find_daily_filepaths
 
 
-### GPM-REFACTOR FILTERING
-### USE TROLL SIFT
+### GPM-REFACTOR FILTERING 
+### USE TROLL SIFT 
 
-# MUST ALWAYS LOOK IN THE DAY BEFORE because 00-01-02 could be in previous day
+# MUST ALWAYS LOOK IN THE DAY BEFORE because 00-01-02 could be in previous day
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_plot_multiorbit_gmi.py` & `gpm_api-0.2.3/gpm_api/tests/test_plot_multiorbit_gmi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue Jan  3 19:21:30 2023
 
 @author: ghiggi
 """
+import os
 import datetime
-
 import numpy as np
-
 import gpm_api
+from dask.diagnostics import ProgressBar
 
 base_dir = "/home/ghiggi"
 
 #### Define analysis time period
 start_time = datetime.datetime.strptime("2020-08-01 12:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2020-08-10 12:00:00", "%Y-%m-%d %H:%M:%S")
 
@@ -33,66 +33,67 @@
     chunks="auto",
     prefix_group=False,
 )
 
 ds = ds.isel(along_track=slice(0, 30000))
 ds = ds.compute()
 
-ds[variable]
+ds[variable] 
 
 ds.gpm_api.plot_map(variable=variable)
 
 # -----------------------------------------------------------------------------.
-# Custom plots
-import cartopy.crs as ccrs
+# Custom plots 
 import matplotlib.pyplot as plt
-
+import cartopy.crs as ccrs
 from gpm_api.visualization.plot import plot_cartopy_background
-
 dpi = 100
 figsize = (12, 10)
 crs_proj = ccrs.Robinson()
 fig, ax = plt.subplots(subplot_kw={"projection": crs_proj}, figsize=figsize, dpi=dpi)
 plot_cartopy_background(ax)
 ds.gpm_api.plot_map(variable=variable, ax=ax)
 
 # Polar projection
 crs_proj = ccrs.Orthographic(180, -90)
 fig, ax = plt.subplots(subplot_kw={"projection": crs_proj}, figsize=figsize, dpi=dpi)
 plot_cartopy_background(ax)
 p = ds.gpm_api.plot_map(variable=variable, ax=ax)
 p.axes.get_extent()
-
+   
 # -----------------------------------------------------------------------------.
 ### DEV CODE
-# - SIMPLIFICATION: IT DISCARD CELLS CROSSING THE ANTIMERIDIAN
+# - SIMPLIFICATION: IT DISCARD CELLS CROSSING THE ANTIMERIDIAN 
 # - BUG IN CARTOPY: DOES NOT ALLOW BAD COLOR TO BE NOT TRANSPARENT !!!
-import cartopy.crs as ccrs
 import matplotlib.pyplot as plt
-
+import cartopy.crs as ccrs
 from gpm_api.utils.utils_cmap import get_colormap_setting
 from gpm_api.visualization.plot import get_antimeridian_mask
-
 plot_kwargs, cbar_kwargs, ticklabels = get_colormap_setting("pysteps_mm/hr")
 
 lons = ds["lon"].data
-lats = ds["lat"].data
+lats = ds["lat"].data 
 arr = ds["surfacePrecipitation"].data
 
 mask = get_antimeridian_mask(lons, buffer=True)
 if np.any(mask):
     arr = np.ma.masked_where(mask, arr)
-    # Sanitize cmap bad color to avoid cartopy bug
-    if "cmap" in plot_kwargs:
-        cmap = plot_kwargs["cmap"]
+    # Sanitize cmap bad color to avoid cartopy bug 
+    if "cmap" in plot_kwargs: 
+        cmap = plot_kwargs['cmap']
         bad = cmap.get_bad()
-        bad[3] = 0  # enforce to 0 (transparent)
+        bad[3] = 0 # enforce to 0 (transparent) 
         cmap.set_bad(bad)
-        plot_kwargs["cmap"] = cmap
-
+        plot_kwargs['cmap'] = cmap
+        
 # - with centroids
-proj = ccrs.PlateCarree()
+proj = ccrs.PlateCarree() 
 ax = plt.axes(projection=proj)
-p = ax.pcolormesh(lons, lats, arr, transform=ccrs.PlateCarree(), **plot_kwargs)
+p = ax.pcolormesh(lons,
+                  lats,
+                  arr,
+                  transform = ccrs.PlateCarree(),
+                  **plot_kwargs
+)
 ax.coastlines()
 
-# -----------------------------------------------------------------------------.
+# -----------------------------------------------------------------------------.
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_plot_multiorbit_pmw_polar.py` & `gpm_api-0.2.3/gpm_api/tests/test_plot_multiorbit_pmw_polar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jan  5 00:19:05 2023
 
 @author: ghiggi
 """
+import os
 import datetime
-
+import numpy as np
 import gpm_api
+from dask.diagnostics import ProgressBar
 
 base_dir = "/home/ghiggi"
 
 #### Define analysis time period
 start_time = datetime.datetime.strptime("2020-08-01 12:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2020-08-02 12:00:00", "%Y-%m-%d %H:%M:%S")
 # end_time = datetime.datetime.strptime("2020-08-10 12:00:00", "%Y-%m-%d %H:%M:%S")
 
-product = "2A-MHS-METOPB"
-product = "2A-SSMIS-F17"
+product = "2A-MHS-METOPB"   
+product = "2A-SSMIS-F17"    
 
 
 product_type = "RS"
 variable = "surfacePrecipitation"
 
 ds = gpm_api.open_dataset(
     base_dir=base_dir,
@@ -33,45 +35,43 @@
     variables=variable,
     product_type=product_type,
     chunks="auto",
     decode_cf=True,
     prefix_group=False,
 )
 
-# gpm_api.check_regular_timesteps(ds) # BAD INDICATOR !
+# gpm_api.check_regular_timesteps(ds) # BAD INDICATOR ! 
 # gpm_api.check_contiguous_scans(ds)
 # ds.gpm_api.get_contiguous_scan_slices()
 
 
 ds = ds.compute()
 ds1 = ds
 
 ds = ds1
 # ds1.gpm_api.get_contiguous_scan_slices()
 
 ds = ds.isel(along_track=slice(0, 20000))
 
-ds = ds.isel(along_track=slice(0, 5000))  # ENOUGH FOR DEVELOPMENT
+ds = ds.isel(along_track=slice(0, 5000)) # ENOUGH FOR DEVELOPMENT
 
-ds[variable]
+ds[variable] 
 
 ds.gpm_api.plot_map(variable=variable)
 
 ds.gpm_api.plot_map(variable=variable, cmap="Spectral", add_swath_lines=False)
 
 # -----------------------------------------------------------------------------.
-# Custom plots
-import cartopy.crs as ccrs
+# Custom plots 
 import matplotlib.pyplot as plt
-
+import cartopy.crs as ccrs
 from gpm_api.visualization.plot import plot_cartopy_background
-
 dpi = 100
 figsize = (12, 10)
 
 # Polar projection
 crs_proj = ccrs.Orthographic(180, -90)
 fig, ax = plt.subplots(subplot_kw={"projection": crs_proj}, figsize=figsize, dpi=dpi)
 plot_cartopy_background(ax)
 p = ds.gpm_api.plot_map(variable=variable, ax=ax, add_swath_lines=True, cmap="Spectral")
-
+ 
 # -----------------------------------------------------------------------------.
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_plot_orbit_pmw_custom_kwargs.py` & `gpm_api-0.2.3/gpm_api/tests/test_plot_orbit_pmw_custom_kwargs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jan  5 00:49:33 2023
 
 @author: ghiggi
 """
+import os
 import datetime
-
+import numpy as np
 import gpm_api
+from dask.diagnostics import ProgressBar
 
 base_dir = "/home/ghiggi"
 
 #### Define analysis time period
 start_time = datetime.datetime.strptime("2020-08-01 12:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2020-08-10 12:00:00", "%Y-%m-%d %H:%M:%S")
 
@@ -27,63 +29,60 @@
     base_dir=base_dir,
     product=product,
     start_time=start_time,
     end_time=end_time,
     # Optional
     version=7,
     variables=variable,
-    # scan_mode="S1",
+    # scan_mode="S1", 
     product_type=product_type,
     chunks="auto",
     prefix_group=False,
 )
 
-ds1 = ds
+ds1 = ds 
 ds1 = ds1.compute()
 
 
 # -----------------------------------------------------------------------------.
-ds = ds1
+ds = ds1 
 
 # ds = ds.isel(along_track=slice(0, 1000))
 
 # ds = ds.isel(along_track=slice(0, 5000))
 # -----------------------------------------------------------------------------.
 
 
 da = ds[variable].isel(channel=8)
-print(da.attrs["LongName"])
+print(da.attrs['LongName'])
 
 da.gpm_api.plot_map()
 da.gpm_api.plot_map(add_swath_lines=False)
 da.gpm_api.plot_map(add_colorbar=False)
 da.gpm_api.plot_map(cmap="Spectral")
 
 da.gpm_api.plot_map(cmap="Spectral", vmin=160, vmax=300)
 
 from gpm_api.visualization.orbit import plot_orbit_map
-
 plot_orbit_map(da)
 
 # -----------------------------------------------------------------------------.
-# Custom plots
-import cartopy.crs as ccrs
-import matplotlib.pyplot as plt
-
+# Custom plots 
 import gpm_api
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
 from gpm_api.visualization.plot import plot_cartopy_background
-
 dpi = 100
 figsize = (12, 10)
 crs_proj = ccrs.Robinson()
 fig, ax = plt.subplots(subplot_kw={"projection": crs_proj}, figsize=figsize, dpi=dpi)
 plot_cartopy_background(ax)
 da.gpm_api.plot_map(ax=ax, cmap="Spectral")
 
 # Polar projection
 crs_proj = ccrs.Orthographic(180, -90)
 fig, ax = plt.subplots(subplot_kw={"projection": crs_proj}, figsize=figsize, dpi=dpi)
 plot_cartopy_background(ax)
 p = da.gpm_api.plot_map(ax=ax, cmap="Spectral")
 # p.axes.get_extent()
-
-# -----------------------------------------------------------------------------.
+    
+# -----------------------------------------------------------------------------.
```

### Comparing `gpm_api-0.2.2/gpm_api/tests/test_unvalid_coordinates.py` & `gpm_api-0.2.3/gpm_api/tests/test_unvalid_coordinates.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,69 +2,77 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Mar  1 11:23:49 2023
 
 @author: ghiggi
 """
 import os
-
 os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"
+import dask
 import gpm_api
+import datetime
+import pandas as pd
+import xarray as xr
+import matplotlib.pyplot as plt 
 
 # import warnings
 # warnings.filterwarnings("ignore")
 
 #### Load GPM Swath
 gpm_base_dir = "/ltenas8/data/GPM"
 product_type = "RS"
 product = "2A-DPR"
-variables = ["precipRateNearSurface", "dataQuality", "SCorientation"]
-version = 7
+variables = ["precipRateNearSurface",
+             "dataQuality", 
+             "SCorientation"]
+version = 7      
 scan_mode = "FS"
 base_dir = gpm_base_dir
-chunks = "auto"  # otherwise concatenating datasets is very slow !
-groups = None
-decode_cf = False
-prefix_group = False
-verbose = False
-
-# ------------------------------
-### GPM DPR
-# After 2019 change scan
-filepath = "/ltenas8/data/GPM/RS/V07/RADAR/2A-DPR/2020/08/19/2A.GPM.DPR.V9-20211125.20200819-S092131-E105404.036787.V07A.HDF5"
+chunks="auto" # otherwise concatenating datasets is very slow !
+groups=None
+decode_cf=False
+prefix_group=False
+verbose=False
+    
+#------------------------------
+### GPM DPR 
+# After 2019 change scan 
+filepath = '/ltenas8/data/GPM/RS/V07/RADAR/2A-DPR/2020/08/19/2A.GPM.DPR.V9-20211125.20200819-S092131-E105404.036787.V07A.HDF5'
 ds_gpm = gpm_api.open_granule(
     filepath,
     scan_mode=scan_mode,
     variables=variables,
     # groups=groups, # TODO
     decode_cf=False,
     prefix_group=prefix_group,
     chunks=chunks,
 )
 
-
+ 
 ds_gpm["precipRateNearSurface"].gpm_api.plot_map()
 
 xr_obj = ds_gpm
-xr_obj.gpm_api.get_slices_valid_geolocation()  # till 7434
+xr_obj.gpm_api.get_slices_valid_geolocation() # till 7434
 xr_obj.gpm_api.get_slices_contiguous_scans()  # till 7435
 xr_obj.gpm_api.is_regular
 xr_obj.isel(along_track=7434)["lon"]
 xr_obj.isel(along_track=7435)["lon"]
 ds_gpm.isel(along_track=slice(0, 7435, None))["precipRateNearSurface"].gpm_api.plot_map()
 ds_gpm.isel(along_track=slice(0, 7435, None)).gpm_api.is_regular
 
 from gpm_api.utils.checks import (
     check_valid_geolocation,
-    get_slices_non_contiguous_scans,
-    get_slices_non_wobbling_swath,
+    get_slices_non_contiguous_scans, 
+    get_slices_non_wobbling_swath
 )
 
 check_valid_geolocation(xr_obj)
-
-xr_obj.gpm_api.get_slices_contiguous_scans(min_size=2)
-xr_obj.gpm_api.get_slices_contiguous_scans(
-    min_size=1
-)  # seems buggy but is because can not verify if last element is contiguous
+ 
+xr_obj.gpm_api.get_slices_contiguous_scans(min_size=2)   
+xr_obj.gpm_api.get_slices_contiguous_scans(min_size=1)  #seems buggy but is because can not verify if last element is contiguous
 get_slices_non_contiguous_scans(xr_obj)
 
 get_slices_non_wobbling_swath(xr_obj, threshold=100)
+ 
+
+ 
+
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/archive.py` & `gpm_api-0.2.3/gpm_api/utils/archive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Tue Nov  1 11:24:29 2022
 
 @author: ghiggi
 """
-import datetime
 import os
+import h5py
+import gpm_api
 import time
-import warnings
-
 import dask
-import h5py
+import datetime
+import warnings
 import numpy as np
 from dateutil.relativedelta import relativedelta
-
-from gpm_api.configs import get_gpm_base_dir, get_gpm_password, get_gpm_username
-from gpm_api.io import GPM_VERSION  # CURRENT GPM VERSION
+from gpm_api.utils.warnings import GPM_Warning
+from gpm_api.io.pps import find_pps_filepaths
+from gpm_api.io.disk import find_filepaths
+from gpm_api.io.info import (
+    get_start_time_from_filepaths, 
+    get_end_time_from_filepaths, 
+    get_granule_from_filepaths
+)
 from gpm_api.io.checks import (
-    check_base_dir,
     check_product,
+    check_base_dir,
     check_start_end_time,
 )
-from gpm_api.io.disk import find_filepaths
-from gpm_api.io.info import (
-    get_end_time_from_filepaths,
-    get_granule_from_filepaths,
-    get_start_time_from_filepaths,
-)
-from gpm_api.io.pps import find_pps_filepaths
-from gpm_api.utils.warnings import GPM_Warning
-
+from gpm_api.io import GPM_VERSION # CURRENT GPM VERSION
 
 ####--------------------------------------------------------------------------.
 ###########################
 #### Archiving utility ####
 ###########################
 def print_elapsed_time(fn):
     def decorator(*args, **kwargs):
@@ -43,15 +41,14 @@
         execution_time = end_time - start_time
         timedelta_str = str(datetime.timedelta(seconds=execution_time))
         print(f"Elapsed time: {timedelta_str} .", end="\n")
         return results
 
     return decorator
 
-
 ####--------------------------------------------------------------------------.
 #########################
 #### Data corruption ####
 #########################
 def get_corrupted_filepaths(filepaths):
     l_corrupted = []
     for filepath in filepaths:
@@ -60,66 +57,61 @@
             hdf = h5py.File(filepath, "r")  # h5py._hl.files.File
             hdf.close()
         except OSError:
             l_corrupted.append(filepath)
     return l_corrupted
 
 
-def remove_corrupted_filepaths(filepaths, verbose=True):
+def remove_corrupted_filepaths(filepaths, verbose=True): 
     for filepath in filepaths:
         if verbose:
             print(f"{filepath} is corrupted and is being removed.")
         os.remove(filepath)
-
+        
 
 def check_file_integrity(
+    base_dir,
     product,
     start_time,
     end_time,
     version=GPM_VERSION,
     product_type="RS",
     remove_corrupted=True,
     verbose=True,
-    base_dir=None,
 ):
     """
     Check GPM granule file integrity over a given period.
-
+    
     If remove_corrupted=True, it removes the corrupted files.
 
     Parameters
     ----------
+    base_dir : str
+       The base directory where GPM data are stored.
     product : str
         GPM product acronym.
     start_time : datetime.datetime
         Start time.
     end_time : datetime.datetime
         End time.
     product_type : str, optional
         GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
     version : int, optional
         GPM version of the data to retrieve if product_type = 'RS'.
         GPM data readers currently support version 4, 5, 6 and 7.
     remove_corrupted : bool, optional
         Whether to remove the corrupted files.
         The default is True.
-    base_dir : str, optional
-        The path to the GPM base directory. If None, it use the one specified
-        in the GPM-API config file.
-        The default is None.
 
     Returns
     -------
     filepaths, list
         List of file paths which are corrupted.
 
     """
-    # Retrieve GPM-API configs
-    base_dir = get_gpm_base_dir(base_dir)
-
     ##--------------------------------------------------------------------.
     # Check base_dir
     base_dir = check_base_dir(base_dir)
     ## Check valid product and variables
     check_product(product, product_type=product_type)
     # Check valid start/end time
     start_time, end_time = check_start_end_time(start_time, end_time)
@@ -134,25 +126,27 @@
         start_time=start_time,
         end_time=end_time,
         verbose=False,
     )
     ##---------------------------------------------------------------------.
     # Check that files have been downloaded  on disk
     if len(filepaths) == 0:
-        raise ValueError("No files found on disk. Please download them before.")
+        raise ValueError(
+            "Requested files are not found on disk. Please download them before."
+        )
 
     ##---------------------------------------------------------------------.
     # Loop over files and list file that can't be opened
     l_corrupted = get_corrupted_filepaths(filepaths)
-
+    
     ##---------------------------------------------------------------------.
     # Report corrupted and remove if asked
     if remove_corrupted:
         remove_corrupted_filepaths(filepaths=l_corrupted, verbose=verbose)
-    else:
+    else: 
         for filepath in l_corrupted:
             print(f"{filepath} is corrupted.")
 
     ##---------------------------------------------------------------------.
     return l_corrupted
 
 
@@ -241,15 +235,16 @@
 
     ####----------------------------------
     #### Find accurate start_time
     print("- Searching for first granule")
     first_start_time = min(l_start_time)
     # Loop every month
     start_times = [
-        first_start_time - datetime.timedelta(days=31 * m) for m in range(1, step_months + 1)
+        first_start_time - datetime.timedelta(days=31 * m)
+        for m in range(1, step_months + 1)
     ]
     start_times = sorted(start_times)
     for start_time in start_times:
         end_time = start_time + datetime.timedelta(days=1)
         filepaths = find_pps_filepaths(
             username=username,
             product=product,
@@ -284,15 +279,16 @@
 
     ####----------------------------------
     #### Find accurate end_time
     print("- Searching for last granule")
     last_start_time = max(l_start_time)
     # Loop every month
     start_times = [
-        last_start_time + datetime.timedelta(days=31 * m) for m in range(1, step_months + 1)
+        last_start_time + datetime.timedelta(days=31 * m)
+        for m in range(1, step_months + 1)
     ]
     start_times = sorted(start_times)[::-1]
     for start_time in start_times:
         print(start_time)
         end_time = start_time + datetime.timedelta(days=1)
         filepaths = find_pps_filepaths(
             username=username,
@@ -336,15 +332,14 @@
 
 
 ####--------------------------------------------------------------------------.
 #######################
 #### Data download ####
 #######################
 
-
 @print_elapsed_time
 def download_daily_data(
     product,
     year,
     month,
     day,
     product_type="RS",
@@ -352,21 +347,21 @@
     n_threads=10,
     transfer_tool="curl",
     progress_bar=False,
     force_download=False,
     check_integrity=True,
     remove_corrupted=True,
     verbose=True,
-    retry=1,
+    retry=1, 
     base_dir=None,
     username=None,
     password=None,
 ):
     from gpm_api.io.download import download_data
-
+    
     start_time = datetime.date(year, month, day)
     end_time = start_time + relativedelta(days=1)
 
     l_corrupted = download_data(
         product=product,
         start_time=start_time,
         end_time=end_time,
@@ -397,21 +392,21 @@
     n_threads=10,
     transfer_tool="curl",
     progress_bar=False,
     force_download=False,
     check_integrity=True,
     remove_corrupted=True,
     verbose=True,
-    retry=1,
+    retry=1, 
     base_dir=None,
     username=None,
     password=None,
 ):
     from gpm_api.io.download import download_data
-
+    
     start_time = datetime.date(year, month, 1)
     end_time = start_time + relativedelta(months=1)
 
     l_corrupted = download_data(
         product=product,
         start_time=start_time,
         end_time=end_time,
@@ -441,15 +436,15 @@
 def check_no_duplicated_files(
     base_dir,
     product,
     start_time,
     end_time,
     version=GPM_VERSION,
     product_type="RS",
-    verbose=True,
+    verbose=True, 
 ):
     """Check that there are not duplicated files based on granule number."""
     ##--------------------------------------------------------------------.
     # Find filepaths
     filepaths = find_filepaths(
         base_dir=base_dir,
         version=version,
@@ -458,243 +453,230 @@
         start_time=start_time,
         end_time=end_time,
         verbose=verbose,
     )
     ##---------------------------------------------------------------------.
     # Check that files have been downloaded  on disk
     if len(filepaths) == 0:
-        raise ValueError("No files found on disk. Please download them before.")
-    ##---------------------------------------------------------------------.
+        raise ValueError(
+            "Requested files are not found on disk. Please download them before."
+        )
+    ##---------------------------------------------------------------------. 
     # Retrieve granule id from filename
     filepaths = np.array(filepaths)
     granule_ids = get_granule_from_filepaths(filepaths)
-
-    # Count granule ids occurence
+    
+    # Count granule ids occurence 
     ids, counts = np.unique(granule_ids, return_counts=True)
-
-    # Get duplicated indices
+    
+    # Get duplicated indices 
     idx_ids_duplicated = np.where(counts > 1)[0].flatten()
     n_duplicated = len(idx_ids_duplicated)
     if n_duplicated > 0:
         duplicated_ids = ids[idx_ids_duplicated]
         for granule_id in duplicated_ids:
             idx_paths_duplicated = np.where(granule_id == granule_ids)[0].flatten()
             tmp_paths_duplicated = filepaths[idx_paths_duplicated].tolist()
             print(f"Granule {granule_id} has duplicated filepaths:")
             for path in tmp_paths_duplicated:
                 print(f"- {path}")
         raise ValueError("There are {n_duplicated} duplicated granules.")
-
-
-def check_time_period_coverage(filepaths, start_time, end_time, raise_error=False):
+        
+        
+def check_time_period_coverage(filepaths, start_time, end_time, raise_error=False): 
     """Check time period start_time, end_time is covered.
-
+    
     If raise_error=True, raise error if time period is not covered.
     If raise_error=False, it raise a GPM warning.
-
+    
     """
     from gpm_api.io.info import (
-        get_end_time_from_filepaths,
         get_start_time_from_filepaths,
+        get_end_time_from_filepaths,
     )
-
     # Check valid start/end time
     start_time, end_time = check_start_end_time(start_time, end_time)
-
-    # Get first and last timestep from filepaths
+    
+    # Get first and last timestep from filepaths 
     filepaths = sorted(filepaths)
     first_start = get_start_time_from_filepaths(filepaths[0])[0]
     last_end = get_end_time_from_filepaths(filepaths[-1])[0]
     # Check time period is covered
     msg = ""
     if first_start > start_time:
         msg = f"The first file start_time ({first_start}) occurs after the specified start_time ({start_time})"
-
+        
     if last_end < end_time:
-        msg1 = (
-            f"The last file end_time ({last_end}) occurs before the specified end_time ({end_time})"
-        )
-        msg = msg + "; and t" + msg1[1:] if msg != "" else msg1
-    if msg != "":
+        msg1 = f"The last file end_time ({last_end}) occurs before the specified end_time ({end_time})"
+        if msg != "":
+           msg = msg + "; and t" + msg1[1:]
+        else: 
+            msg = msg1
+    if msg != "": 
         if raise_error:
             raise ValueError(msg)
-        else:
+        else: 
             warnings.warn(msg, GPM_Warning)
-
+        
 
 def get_time_period_with_missing_files(filepaths):
     """
-    It returns the time period where the are missing granules.
-
+    It returns the time period where the are missing granules. 
+    
     It assumes the input filepaths are for a single GPM product.
 
     Parameters
     ----------
     filepaths : list
         List of GPM file paths.
 
     Returns
     -------
     list_missing : list
         List of tuple (start_time, end_time).
 
     """
+    from gpm_api.utils.checks import _is_contiguous_granule
+    from gpm_api.utils.slices import get_list_slices_from_bool_arr
     from gpm_api.io.info import (
-        get_end_time_from_filepaths,
         get_granule_from_filepaths,
         get_start_time_from_filepaths,
+        get_end_time_from_filepaths,
     )
-    from gpm_api.utils.checks import _is_contiguous_granule
-    from gpm_api.utils.slices import get_list_slices_from_bool_arr
-
     # Retrieve granule id from filename
     granule_ids = get_granule_from_filepaths(filepaths)
-
-    # Sort filepaths by granule number
+    
+    # Sort filepaths by granule number 
     indices = np.argsort(granule_ids)
     filepaths = np.array(filepaths)[indices]
     granule_ids = np.array(granule_ids)[indices]
-
-    # Check if next file granule number is +1
+    
+    # Check if next file granule number is +1 
     is_not_missing = _is_contiguous_granule(granule_ids)
-
-    # If there are missing files
+    
+    # If there are missing files 
     list_missing = []
     if np.any(~is_not_missing):
         # Retrieve slices with unmissing granules
-        # - Do not skip consecutive False
+        # - Do not skip consecutive False  
         # --> is_not_missing=np.array([False, False, True, True, False, False])
         # --> list_slices = [slice(0, 1, None), slice(1, 2, None), slice(2, 5, None), slice(5, 6, None)]
         list_slices = get_list_slices_from_bool_arr(
-            is_not_missing, include_false=True, skip_consecutive_false=False
-        )
+            is_not_missing, include_false=True, skip_consecutive_false=False)   
         # Retrieve start and end_time where there are missing files
         for slc in list_slices[0:-1]:
-            missing_start = get_end_time_from_filepaths(filepaths[slc.stop - 1])[0]
+            missing_start = get_end_time_from_filepaths(filepaths[slc.stop-1])[0]
             missing_end = get_start_time_from_filepaths(filepaths[slc.stop])[0]
             list_missing.append((missing_start, missing_end))
     return list_missing
 
 
 def check_archive_completness(
+    base_dir,
     product,
     start_time,
     end_time,
     version=GPM_VERSION,
     product_type="RS",
     download=True,
+    username=None,
     transfer_tool="wget",
     n_threads=4,
     verbose=True,
-    base_dir=None,
-    username=None,
-    password=None,
 ):
     """
     Check that the GPM product archive is not missing granules over a given period.
-
+    
     This function does not require connection to the PPS to search for the missing files.
-    However, the start and end period are based on the first and last file found on disk !
-
+    However, the start and end period are based on the first and last file found on disk ! 
+ 
     If download=True, it attempt to download the missing granules.
 
     Parameters
     ----------
+    base_dir : str
+       The base directory where GPM data are stored.
     product : str
         GPM product acronym.
     start_time : datetime.datetime
         Start time.
     end_time : datetime.datetime
         End time.
     product_type : str, optional
         GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
     version : int, optional
         GPM version of the data to retrieve if product_type = 'RS'.
         GPM data readers currently support version 4, 5, 6 and 7.
     download : bool, optional
         Whether to download the missing files.
         The default is True.
+    username: str
+        Email address with which you registered on NASA PPS.
     n_threads : int, optional
         Number of parallel downloads. The default is set to 10.
     transfer_tool : str, optional
         Wheter to use curl or wget for data download. The default is "wget".
     verbose : bool, optional
         Whether to print processing details. The default is False.
-    base_dir : str, optional
-        The path to the GPM base directory. If None, it use the one specified
-        in the GPM-API config file.
-        The default is None.
-    username: str, optional
-        Email address with which you registered on the NASA PPS.
-        If None, it uses the one specified in the GPM-API config file.
-        The default is None.
-    password: str, optional
-        Email address with which you registered on the NASA PPS.
-        If None, it uses the one specified in the GPM-API config file.
-        The default is None.
     """
     ##--------------------------------------------------------------------.
     from gpm_api.io.download import download_data
-
-    # -------------------------------------------------------------------------.
-    # Retrieve GPM-API configs
-    base_dir = get_gpm_base_dir(base_dir)
-    username = get_gpm_username(username)
-    password = get_gpm_password(password)
-
+    
+    if download: 
+        if username is None: 
+            raise ValueError("If download=True, provide the username.")
+            
     # Check valid start/end time
     start_time, end_time = check_start_end_time(start_time, end_time)
-
+    
     ##--------------------------------------------------------------------.
     # Find filepaths
     filepaths = find_filepaths(
         base_dir=base_dir,
         version=version,
         product=product,
         product_type=product_type,
         start_time=start_time,
         end_time=end_time,
         verbose=verbose,
     )
     ##---------------------------------------------------------------------.
     # Check that files have been downloaded on disk
     if len(filepaths) == 0:
-        raise ValueError("No files found on disk. Please download them before.")
-
+        raise ValueError(
+            "Requested files are not found on disk. Please download them before."
+        )
+    
     ##---------------------------------------------------------------------.
-    # Check that the specified time period is covered
+    # Check that the specified time period is covered 
     check_time_period_coverage(filepaths, start_time, end_time, raise_error=False)
 
     ##---------------------------------------------------------------------.
     # Loop over files and retrieve time period with missing granules
     list_missing_periods = get_time_period_with_missing_files(filepaths)
-
+    
     # If there are missing data,
-    if len(list_missing_periods) > 0:
-        if download:  # and download=True
+    if len(list_missing_periods) > 0: 
+        if download: # and download=True
             # Attempt to download the missing data
-            for s_time, e_time in list_missing_periods:
-                download_data(
-                    base_dir=base_dir,
-                    username=username,
-                    version=version,
-                    product=product,
-                    product_type=product_type,
-                    start_time=s_time,
-                    end_time=e_time,
-                    n_threads=n_threads,
-                    transfer_tool=transfer_tool,
-                    check_integrity=True,
-                    remove_corrupted=True,
-                    retry=2,
-                    verbose=verbose,
-                )
-        else:
+            for s_time, e_time in list_missing_periods: 
+                download_data(base_dir=base_dir,
+                              username=username,
+                              version=version,
+                              product=product,
+                              product_type=product_type,
+                              start_time=s_time,
+                              end_time=e_time,
+                              n_threads=n_threads,
+                              transfer_tool=transfer_tool,
+                              check_integrity=True,
+                              remove_corrupted=True,
+                              retry=2, 
+                              verbose=verbose,
+                              )
+        else: 
             # Otherwise print time periods with missing data and raise error
-            for s_time, e_time in list_missing_periods:
+            for s_time, e_time in list_missing_periods: 
                 print(f"- Missing data between {s_time} and {e_time}")
-            raise ValueError(
-                "The GPM {product} archive is not complete between {start_time} and {end_time}."
-            )
-
+            raise ValueError("The GPM {product} archive is not complete between {start_time} and {end_time}.")
 
 ####--------------------------------------------------------------------------.
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/area.py` & `gpm_api-0.2.3/gpm_api/utils/area.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,209 +1,227 @@
 #!/usr/bin/env python3
-# Utility to compute corners and cell vertices from centroid 2D coordinates.
-# In future, the code in this file will be added to pyresample !
-import dask.array
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Jan  9 16:42:33 2023
+
+@author: ghiggi
+"""
+"""Utility to compute corners and cell vertices from centroid 2D coordinates. 
+   In future, the code in this file will be added to pyresample !
+"""
+import pyproj 
 import numpy as np
-import pyproj
+import dask.array 
 from dask.array import map_blocks
 
-### SwathDefinition --> geographic coordinates --> computation in ECEF (xyz)
-### AreaDefinition --> proj coordinates --> computation in projection space !
+
+### SwathDefinition --> geographic coordinates --> computation in ECEF (xyz) 
+### AreaDefinition --> proj coordinates --> computation in projection space !   
 
 
 def _infer_interval_breaks(coord, axis=0):
     """Infer the outer and inner midpoints of 2D coordinate arrays.
-
-    An [N,M] array
-
+    
+    An [N,M] array 
+    
     The outer points are defined by taking half-distance of the closest centroid.
     The implementation is inspired from xarray.plot.utils._infer_interval_breaks
-
+    
     Parameters
     ----------
     coord : np.array
         Coordinate array of shape [N,M].
     axis : int, optional
         Axis over which to infer the midpoint.
         axis = 0 infer midpoints along the vertical direction.
         axis = 1 infer midpoints along the horizontal direction.
         The default is 0.
 
     Returns
     -------
-    breaks : np.array
+    breaks : np.array  
         If axis = 0, it returns an array of shape [N+1, M]
         If axis = 0, it returns an array of shape [N, M+1]
     """
     # Determine the half-distance between coordinates
     coord = np.asarray(coord)
     deltas = 0.5 * np.diff(coord, axis=axis)
-    # Infer outer position of first and last
+    # Infer outer position of first and last 
     first = np.take(coord, [0], axis=axis) - np.take(deltas, [0], axis=axis)
     last = np.take(coord, [-1], axis=axis) + np.take(deltas, [-1], axis=axis)
     # Infer position of internal points
-    trim_last = tuple(slice(None, -1) if n == axis else slice(None) for n in range(coord.ndim))
+    trim_last = tuple(
+        slice(None, -1) if n == axis else slice(None) for n in range(coord.ndim)
+    )
     offsets = coord[trim_last] + deltas
     # Compute the breaks
     breaks = np.concatenate([first, offsets, last], axis=axis)
     return breaks
 
-
+ 
 def _get_corners_from_centroids(centroids):
-    """Get the coordinate corners 2D array from the centroids 2D array.
-
+    """Get the coordinate corners 2D array from the centroids 2D array. 
+    
     The corners are guessed assuming equal spacing on either side of the coordinate.
     """
     # Identify breaks along columns
     breaks = _infer_interval_breaks(centroids, axis=1)
     # Identify breaks along rows
     corners = _infer_interval_breaks(breaks, axis=0)
     return corners
 
 
+
 def _do_transform(src_proj, dst_proj, lons, lats, alt):
     """Perform pyproj transformation and stack the results.
-
+    
     If using pyproj >= 3.1, it employs thread-safe pyproj.transformer.Transformer.
     If using pyproj < 3.1, it employs pyproj.transform.
     Docs: https://pyproj4.github.io/pyproj/stable/advanced_examples.html#multithreading
-    """
+    """     
     if float(pyproj.__version__[0:3]) >= 3.1:
         from pyproj import Transformer
-
         transformer = Transformer.from_crs(src_proj.crs, dst_proj.crs)
         x, y, z = transformer.transform(lons, lats, alt, radians=False)
     else:
         x, y, z = pyproj.transform(src_proj, dst_proj, lons, lats, alt)
     return np.dstack((x, y, z))
 
 
 def _geocentric_to_geographic(x, y, z, compute=True):
     """Map from geocentric cartesian to geographic coordinate system."""
-    # Ensure dask array
+    # Ensure dask array 
     x = dask.array.asarray(x)
     y = dask.array.asarray(y)
     z = dask.array.asarray(z)
-    # Define geocentric cartesian and geographic projection
-    geocentric_proj = pyproj.Proj(proj="geocent")
-    geographic_proj = pyproj.Proj(proj="latlong")
-
+    # Define geocentric cartesian and geographic projection 
+    geocentric_proj = pyproj.Proj(proj='geocent')
+    geographic_proj = pyproj.Proj(proj='latlong')
+    
     # Conversion from geocentric cartesian to geographic coordinate system
-    res = map_blocks(
-        _do_transform,
-        geocentric_proj,
-        geographic_proj,
-        x,
-        y,
-        z,
-        new_axis=[2],
-        chunks=(x.chunks[0], x.chunks[1], 3),
-    )
-    if compute:
+    res = map_blocks(_do_transform, 
+                     geocentric_proj, 
+                     geographic_proj,
+                     x,   
+                     y,   
+                     z,
+                     new_axis=[2],
+                     chunks=(x.chunks[0], x.chunks[1], 3)
+                     )
+    if compute: 
         res = res.compute()
-    lons = res[:, :, 0]
-    lats = res[:, :, 1]
+    lons = res[:,:, 0]
+    lats = res[:,:, 1]
     return lons, lats
 
 
 def _geographic_to_geocentric(lons, lats, compute=True):
     """Map from geographic to geocentric cartesian coordinate system."""
-    # Ensure dask array
+    # Ensure dask array 
     lons = dask.array.asarray(lons)
     lats = dask.array.asarray(lats)
-    # Define geocentric cartesian and geographic projection
-    geocentric_proj = pyproj.Proj(proj="geocent")
-    geographic_proj = pyproj.Proj(proj="latlong")
-
-    # Conversion from geographic coordinate system to geocentric cartesian
-    res = map_blocks(
-        _do_transform,
-        geographic_proj,
-        geocentric_proj,
-        lons,
-        lats,
-        dask.array.zeros_like(lons),  # altitude
-        new_axis=[2],
-        chunks=(lons.chunks[0], lons.chunks[1], 3),
-    )
-    if compute:
+    # Define geocentric cartesian and geographic projection 
+    geocentric_proj = pyproj.Proj(proj='geocent')
+    geographic_proj = pyproj.Proj(proj='latlong')
+    
+    # Conversion from geographic coordinate system to geocentric cartesian 
+    res = map_blocks(_do_transform, 
+                     geographic_proj, 
+                     geocentric_proj,
+                     lons,
+                     lats, 
+                     dask.array.zeros_like(lons), # altitude
+                     new_axis=[2],
+                     chunks=(lons.chunks[0], lons.chunks[1], 3)
+                     )
+    if compute: 
         res = res.compute()
-    x = res[:, :, 0]
-    y = res[:, :, 1]
-    z = res[:, :, 2]
+    x = res[:,:, 0]
+    y = res[:,:, 1]
+    z = res[:,:, 2]
     return x, y, z
-
+        
 
 def _get_lonlat_corners(lons, lats):
     """Compute the corners of lon lat 2D pixel centroid coordinate arrays.
-
+    
     It take care of cells crossing the antimeridian.
     It compute corners on geocentric cartesian coordinate system (ECEF).
     """
-    # Map lons, lats to x, y, z centroids
+    # Map lons, lats to x, y, z centroids 
     x, y, z = _geographic_to_geocentric(lons, lats)
-    # Compute corners in geocentric cartesian coordinate system
+    # Compute corners in geocentric cartesian coordinate system  
     x_corners = _get_corners_from_centroids(x)
     y_corners = _get_corners_from_centroids(y)
     z_corners = _get_corners_from_centroids(z)
     # Convert back to lons, lats
-    lons_corners, lat_corners = _geocentric_to_geographic(x_corners, y_corners, z_corners)
+    lons_corners, lat_corners = _geocentric_to_geographic(x_corners, 
+                                                           y_corners, 
+                                                           z_corners)
     return lons_corners, lat_corners
-
+  
 
 def _from_corners_to_bounds(corners, order="counterclockwise"):
-    """Convert from corner 2D array (N+1, M+1)  to quadmesh vertices array (N,M, 4).
-
+    """Convert from corner 2D array (N+1,M+1)  to bounds 3D array (N,M, vertices).
+    
     Counterclockwise and clockwise bounds are defined from the top left corner.
-    Counterclockwise: [top_left, bottom_left, bottom_right, top_right]
-    Clockwise: [bottom_left, top_left, top_right, bottom_right]
-
     Inspired from https://github.com/xarray-contrib/cf-xarray/blob/main/cf_xarray/helpers.py#L113
-    """
+   
+ 
+   """
+    # TODO: The order assumptions might not hold for retrograde satellite orbits
+    # --> spherical checks should be performed !!!
+     
+    # TODO: Is this dask efficient? Or map_overlap and take neighbour values? 
+    
     top_left = corners[:-1, :-1]
     top_right = corners[:-1, 1:]
     bottom_right = corners[1:, 1:]
-    bottom_left = corners[1:, :-1]
+    bottom_left = corners[1:, :-1]  
+    
     if order == "clockwise":
-        list_vertices = [bottom_left, top_left, top_right, bottom_right]
-    else:  # counterclockwise
+        list_vertices = [top_left, top_right, bottom_right, bottom_left]
+    else: # counterclockwise
         list_vertices = [top_left, bottom_left, bottom_right, top_right]
     if hasattr(corners, "chunks"):
         bounds = dask.array.stack(list_vertices, axis=2)
-        # Rechunking over the vertices dimension is required !!!
+        # Rechunking over the vertices dimension is required !!! 
         bounds = bounds.rechunk((bounds.chunks[0], bounds.chunks[1], 4))
     else:
         bounds = np.stack(list_vertices, axis=2)
 
     return bounds
 
 
 def get_quadmesh_vertices(x, y, order="counterclockwise"):
     """Convert (x, y) 2D centroid coordinates array to (N*M, 4, 2) QuadMesh vertices.
-
-    The output vertices can be passed directly to a matplotlib.PolyCollection.
+    
+    The output vertices can be passed directly to a matplotlib.PolyCollection. 
     For plotting with cartopy, the polygon order must be "counterclockwise"
-
+    
     Vertices are defined from the top left corner.
     """
     # - Retrieve QuadMesh corners (m+1 x n+1)
     x_corners, y_corners = _get_lonlat_corners(x, y)
-
+    
     # - Retrieve QuadMesh bounds (m*n x 4)
     x_bounds = _from_corners_to_bounds(x_corners, order="counterclockwise")
     y_bounds = _from_corners_to_bounds(y_corners, order="counterclockwise")
-
+    
     # - Retrieve QuadMesh vertices (m*n, 4, 2)
     vertices = np.stack((x_bounds, y_bounds), axis=2)
-    return vertices
+    return vertices 
 
 
 def is_vertex_clockwise(vertex):
     # TODO: use pyresample.future in future
-    # --> Check elementwise?
-    # https://stackoverflow.com/questions/9473570/polygon-vertices-clockwise-or-counterclockwise
+    # --> Check elementwise? 
+    # https://stackoverflow.com/questions/9473570/polygon-vertices-clockwise-or-counterclockwise 
     from pyresample import SwathDefinition
-
-    is_clockwise = SwathDefinition._corner_is_clockwise(
-        vertex[0][0], vertex[0][1], vertex[1][0], vertex[1][1], vertex[2][0], vertex[2][1]
-    )
+    is_clockwise = SwathDefinition._corner_is_clockwise(vertex[0][0], 
+                                                        vertex[0][1], 
+                                                        vertex[1][0], 
+                                                        vertex[1][1], 
+                                                        vertex[2][0], 
+                                                        vertex[2][1])
     return is_clockwise
+
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/checks.py` & `gpm_api-0.2.3/gpm_api/utils/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sat Dec 10 18:41:48 2022
 
 @author: ghiggi
 """
-import functools
-
 import numpy as np
 import pandas as pd
 import xarray as xr
-
-from gpm_api.utils.geospatial import is_grid, is_orbit
+import functools
+from gpm_api.utils.geospatial import is_orbit, is_grid
 from gpm_api.utils.slices import (
+    get_list_slices_from_indices,
     get_list_slices_from_bool_arr,
+    list_slices_union, 
     list_slices_difference,
-    list_slices_filter,
-    list_slices_flatten,
     list_slices_intersection,
     list_slices_sort,
-    list_slices_union,
+    list_slices_filter,
+    list_slices_flatten
 )
 
 ORBIT_TIME_TOLERANCE = np.timedelta64(3, "s")
 
 
 def check_is_xarray(x):
     if not isinstance(x, (xr.DataArray, xr.Dataset)):
@@ -59,34 +59,33 @@
 
 
 ####--------------------------------------------------------------------------.
 ##########################
 #### Regular granules ####
 ##########################
 
-
-def get_missing_granule_numbers(xr_obj):
+def get_missing_granule_numbers(xr_obj): 
     """Return ID numbers of missing granules."""
     granule_ids = np.unique(xr_obj["gpm_granule_id"].data)
-    min_id = min(granule_ids)
+    min_id =  min(granule_ids)
     max_id = max(granule_ids)
-    possible_ids = np.arange(min_id, max_id + 1)
+    possible_ids = np.arange(min_id, max_id+1)
     missing_ids = possible_ids[~np.isin(possible_ids, granule_ids)]
     return missing_ids
 
 
 def _is_contiguous_granule(granule_ids):
     """Return a boolean array indicating if the next scan is not the same/next granule."""
     # Retrieve if next scan is in the same or next granule (True) or False.
     bool_arr = np.diff(granule_ids) <= 1
 
     # Add True to last position
     bool_arr = np.append(bool_arr, True)
     return bool_arr
-
+    
 
 def get_slices_contiguous_granules(xr_obj, min_size=2):
     """
     Return a list of slices ensuring contiguous granules.
 
     Output format: [slice(start,stop), slice(start,stop),...]
 
@@ -101,36 +100,40 @@
 
     Returns
     -------
     list_slices : list
         List of slice object to select contiguous granules.
     """
 
-    if is_grid(xr_obj) or is_orbit(xr_obj):
-        # Get number of scans/timesteps
-        n_scans = xr_obj["gpm_granule_id"].shape[0]
-        # Define behaviour if less than 2 scans/timesteps
+    if is_grid(xr_obj):
+        # TODO: use granule_id when gpm_api modified to include it also for GRID product
+        return get_slices_regular_time(xr_obj, tolerance=None, min_size=min_size)
+    
+    if is_orbit(xr_obj): 
+        # Get number of scans
+        n_scans = xr_obj["along_track"].shape[0]
+        # Define behaviour if less than 2 scan along track
         # - If n_scans 0, slice(0, 0) could return empty array
         # - If n_scans 1, slice(0, 1) could return the single scan
         # --> Here we decide to return an empty list !
-        if n_scans < min_size:
+        if n_scans < 2:
             list_slices = []
             return list_slices
-
-        # Get boolean array indicating if the next scan/timesteps is same or next granule
+        
+        # Get boolean array indicating if the next scan is same or next granule
         bool_arr = _is_contiguous_granule(xr_obj["gpm_granule_id"].data)
-
+        
         # If granules are missing present, get the slices with non-missing granules
         list_slices = get_list_slices_from_bool_arr(
             bool_arr, include_false=True, skip_consecutive_false=True
         )
-
+        
         # Select only slices with at least 2 scans
         list_slices = list_slices_filter(list_slices, min_size=min_size)
-
+        
         # Return list of contiguous scan slices
         return list_slices
     else:
         raise ValueError("Unrecognized GPM xarray object.")
 
 
 def check_missing_granules(xr_obj):
@@ -143,45 +146,50 @@
         xarray object.
 
     """
     missing_ids = get_missing_granule_numbers(xr_obj)
     n_missing = len(missing_ids)
     if n_missing > 0:
         msg = f"There are {n_missing} missing granules. Their IDs are {missing_ids}."
-        raise ValueError(msg)
+        raise ValueError(msg)    
 
 
 def check_contiguous_granules(xr_obj):
     return check_missing_granules(xr_obj)
-
+        
 
 def has_contiguous_granules(xr_obj):
     """Checks GPM object is composed of consecutive granules."""
-    from gpm_api.utils.geospatial import is_grid, is_orbit
+    from gpm_api.utils.geospatial import is_orbit, is_grid
 
     if is_orbit(xr_obj):
-        return bool(np.all(_is_contiguous_granule(xr_obj["gpm_granule_id"].data)))
+        if np.all(_is_contiguous_granule(xr_obj["gpm_granule_id"].data)):
+            return True
+        else:
+            return False
     if is_grid(xr_obj):
         return has_regular_time(xr_obj)
     else:
         raise ValueError("Unrecognized GPM xarray object.")
-
-
+    
+    
 def has_missing_granules(xr_obj):
     """Checks GPM object has missing granules."""
-    from gpm_api.utils.geospatial import is_grid, is_orbit
+    from gpm_api.utils.geospatial import is_orbit, is_grid
 
     if is_orbit(xr_obj):
-        return bool(np.any(~_is_contiguous_granule(xr_obj["gpm_granule_id"].data)))
+        if np.any(~_is_contiguous_granule(xr_obj["gpm_granule_id"].data)):
+            return True
+        else:
+            return False
     if is_grid(xr_obj):
         return ~has_regular_time(xr_obj)
     else:
         raise ValueError("Unrecognized GPM xarray object.")
-
-
+        
 ####--------------------------------------------------------------------------.
 ############################
 #### Regular timesteps  ####
 ############################
 
 
 def _get_timesteps(xr_obj):
@@ -189,15 +197,15 @@
     timesteps = xr_obj["time"].values
     timesteps = timesteps.astype("M8[s]")
     return timesteps
 
 
 def _infer_time_tolerance(xr_obj):
     """Infer time interval tolerance between timesteps."""
-    from gpm_api.utils.geospatial import is_grid, is_orbit
+    from gpm_api.utils.geospatial import is_orbit, is_grid
 
     # For GPM ORBIT objects, use the ORBIT_TIME_TOLERANCE
     if is_orbit(xr_obj):
         tolerance = ORBIT_TIME_TOLERANCE
     # For GPM GRID objects, infer it from the time difference between first two timesteps
     elif is_grid(xr_obj):
         timesteps = _get_timesteps(xr_obj)
@@ -232,18 +240,18 @@
     Parameters
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
     tolerance : np.timedelta, optional
         The timedelta tolerance to define regular vs. non-regular timesteps.
         If None, it uses the first 2 timesteps to derive the tolerance timedelta.
-        The default is None.
+        The default is None. 
     min_size : int
         Minimum size for a slice to be returned.
-
+    
     Returns
     -------
     list_slices : list
         List of slice object to select regular time intervals.
     """
     # Retrieve timestep
     timesteps = _get_timesteps(xr_obj)
@@ -261,18 +269,18 @@
         is_regular = _is_regular_time(xr_obj, tolerance=tolerance)
 
         # If non-regular timesteps are present, get the slices for each regular interval
         # - If consecutive non-regular timestep occurs, returns slices of size 1
         list_slices = get_list_slices_from_bool_arr(
             is_regular, include_false=True, skip_consecutive_false=False
         )
-
+    
     # Select only slices with at least min_size timesteps
     list_slices = list_slices_filter(list_slices, min_size=min_size)
-
+    
     # Return list of slices with regular timesteps
     return list_slices
 
 
 def get_slices_non_regular_time(xr_obj, tolerance=None):
     """
     Return a list of slices where there are supposedly missing timesteps.
@@ -286,15 +294,15 @@
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
     tolerance : np.timedelta, optional
         The timedelta tolerance to define regular vs. non-regular timesteps.
         The default is None.
         If GPM GRID object, it uses the first 2 timesteps to derive the tolerance timedelta.
-        If GPM ORBIT object, it uses the gpm_api.utils.time.ORBIT_TIME_TOLERANCE.
+        If GPM ORBIT object, it uses the gpm_api.utils.time.ORBIT_TIME_TOLERANCE. 
         It is discouraged to use this function for GPM ORBIT objects !
 
     Returns
     -------
     list_slices : list
         List of slice object to select intervals with non-regular timesteps.
     """
@@ -375,30 +383,26 @@
 
 ####--------------------------------------------------------------------------.
 ########################
 #### Regular scans  ####
 ########################
 def _check_cross_track(function):
     """Check that the cross-track dimension is available.
-
+    
     If not available, raise an error."""
-
     @functools.wraps(function)
     def wrapper(*args, **kwargs):
         # Write decorator function logic here
         xr_obj = args[0]
         if "cross_track" not in xr_obj.dims:
-            raise ValueError(
-                "cross-track dimension not available. Not possible to check for scan regularity."
-            )
-        # Call the function
+            raise ValueError("cross-track dimension not available. Not possible to check for scan regularity.")
+        # Call the function 
         result = function(*args, **kwargs)
-        # Return results
+        # Return results 
         return result
-
     return wrapper
 
 
 @_check_cross_track
 def _get_along_track_scan_distance(xr_obj):
     """Compute the distance between along_track centroids."""
     from pyproj import Geod
@@ -417,15 +421,15 @@
     _, _, dist = geod.inv(start_lons, start_lats, end_lons, end_lats)
     return dist
 
 
 @_check_cross_track
 def _is_contiguous_scans(xr_obj):
     """Return a boolean array indicating if the next scan is contiguous.
-
+    
     The last element is set to True since it can not be verified.
     """
     # Compute along track scan distance
     dist = _get_along_track_scan_distance(xr_obj)
     # Convert to km and round
     dist_km = np.round(dist / 1000, 0)
 
@@ -454,38 +458,38 @@
 
 @_check_cross_track
 def get_slices_contiguous_scans(xr_obj, min_size=2):
     """
     Return a list of slices ensuring contiguous scans (and granules).
 
     Output format: [slice(start,stop), slice(start,stop),...]
-
+    
     It checks for contiguous scans only in the middle of the cross-track !
     If a scan geolocation is NaN, it will be considered non-contiguous.
     An input with less than 2 scans (along-track) returns an empty list.
     Consecutive non-contiguous scans are discarded and not included in the outputs.
     The minimum size of the output slices is 2.
-
+    
     Parameters
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
     min_size : int
         Minimum size for a slice to be returned.
 
     Returns
     -------
     list_slices : list
         List of slice object to select contiguous scans.
     """
     check_is_orbit(xr_obj)
-
+    
     # Get number of scans
     n_scans = xr_obj["along_track"].shape[0]
-
+    
     # Define behaviour if less than 2 scan along track
     # - If n_scans 0, slice(0, 0) could return empty array
     # - If n_scans 1, slice(0, 1) could return the single scan
     # --> Here we decide to return an empty list !
     if n_scans < 2:
         list_slices = []
         return list_slices
@@ -496,21 +500,21 @@
     # If non-contiguous scans are present, get the slices with contiguous scans
     # - It discard consecutive non-contiguous scans
     list_slices = get_list_slices_from_bool_arr(
         is_contiguous, include_false=True, skip_consecutive_false=True
     )
     # Select only slices with at least 2 scans
     list_slices = list_slices_filter(list_slices, min_size=min_size)
-
-    # Also retrieve the slices with non missing granule
+    
+    # Also retrieve the slices with non missing granule 
     list_slices1 = get_slices_contiguous_granules(xr_obj)
-
+    
     # Perform list_slices intersection
     list_slices = list_slices_intersection(list_slices, list_slices1)
-
+    
     # Return list of contiguous scan slices
     return list_slices
 
 
 @_check_cross_track
 def get_slices_non_contiguous_scans(xr_obj):
     """
@@ -538,27 +542,27 @@
     # Define behaviour if less than 2 scan along track
     # - If n_scans 0, slice(0, 0) could return empty array
     # - If n_scans 1, slice(0, 1) could return the single scan
     # --> Here we decide to return an empty list !
     if n_scans < 2:
         list_slices = []
         return list_slices
-
+    
     ### CODE to output slices with size 2.
     # # Get boolean array indicating if the next scan is contiguous
     # is_contiguous = _is_contiguous_scans(xr_obj)
 
     # # If non-contiguous scans are present, get the slices when discontinuity occurs
     # if not np.all(is_contiguous):
     #     indices_next_discontinuous = np.argwhere(~is_contiguous).flatten()
     #     list_slices = [slice(i, i + 2) for i in indices_next_discontinuous]
     # else:
     #     list_slices = []
     # return list_slices
-
+    
     list_slices_valid = get_slices_contiguous_scans(xr_obj, min_size=2)
     list_slices_full = [slice(0, len(xr_obj["along_track"]))]
     list_slices = list_slices_difference(list_slices_full, list_slices_valid)
     return list_slices
 
 
 @_check_cross_track
@@ -583,37 +587,35 @@
     None.
     """
     list_discontinuous_slices = get_slices_non_contiguous_scans(xr_obj)
     n_discontinuous = len(list_discontinuous_slices)
     if n_discontinuous > 0:
         # Retrieve discontinous timesteps interval
         timesteps = _get_timesteps(xr_obj)
-        list_discontinuous = [
-            (timesteps[slc][0], timesteps[slc][-1]) for slc in list_discontinuous_slices
-        ]
+        list_discontinuous = [(timesteps[slc][0],timesteps[slc][-1]) for slc in list_discontinuous_slices]
         first_problematic_timestep = list_discontinuous[0][0]
         # Print non-contiguous scans
         if verbose:
             for start, stop in list_discontinuous:
                 print(f"- Missing scans between {start} and {stop}")
         # Raise error and highlight first non-contiguous scan
-        msg = f"There are {n_discontinuous} non-contiguous scans."
-        msg += f"The first occur at {first_problematic_timestep}."
-        raise ValueError(msg)
+        raise ValueError(
+            f"There are {n_discontinuous} swath portions with non-contiguous scans. The first occur at {first_problematic_timestep}."
+        )
 
 
 @_check_cross_track
 def has_contiguous_scans(xr_obj):
     """Return True if all scans are contiguous. False otherwise."""
     list_discontinuous_slices = get_slices_non_contiguous_scans(xr_obj)
     n_discontinuous = len(list_discontinuous_slices)
     if n_discontinuous > 0:
         return False
     else:
-        return True
+        return True 
 
 
 ####--------------------------------------------------------------------------.
 #############################
 #### Regular geolocation ####
 #############################
 
@@ -632,68 +634,67 @@
 
 def get_slices_valid_geolocation(xr_obj, min_size=2):
     """Return a list of along-track slices ensuring valid geolocation.
 
     Output format: [slice(start,stop), slice(start,stop),...]
 
     The minimum size of the output slices is 2.
-
+    
     If at a given cross-track index, there are always wrong geolocation,
     it discards such cross-track index(es) before indentifying the along-track slices.
-
+    
     Parameters
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
     min_size : int
         Minimum size for a slice to be returned.
         The default is 2.
 
     Returns
     -------
     list_slices : list
         List of slice object with valid geolocation.
     """
-    # Check input
+    # Check input 
     if is_grid(xr_obj):
         raise ValueError("For GRID products, geolocation is expected to be valid.")
     if is_orbit(xr_obj):
-        # - Get unvalid coordinates
+        # - Get unvalid coordinates 
         unvalid_coords = _is_non_valid_geolocation(xr_obj)
         # - Identify cross-track index that along-track are always unvalid
         idx_cross_track_not_all_unvalid = np.where(~unvalid_coords.all("along_track"))[0]
-        # - If all unvalid, return empty list
-        if len(idx_cross_track_not_all_unvalid) == 0:
+        # - If all unvalid, return empty list 
+        if len(idx_cross_track_not_all_unvalid) == 0: 
             list_slices = []
             return list_slices
         # - Select only cross-track index that are not all unvalid along-track
         unvalid_coords = unvalid_coords.isel(cross_track=idx_cross_track_not_all_unvalid)
         # - Now identify scans across which there are still unvalid coordinates
-        unvalid_scans = unvalid_coords.any(dim="cross_track")
+        unvalid_scans = unvalid_coords.any(dim="cross_track")  
         valid_scans = ~unvalid_scans
-        # - Now identify valid along-track slices
+        # - Now identify valid along-track slices 
         list_slices = get_list_slices_from_bool_arr(
             valid_scans, include_false=False, skip_consecutive_false=True
         )
         # Select only slices with at least 2 scans
         list_slices = list_slices_filter(list_slices, min_size=min_size)
         return list_slices
-    return None
 
 
 def get_slices_non_valid_geolocation(xr_obj):
     """Return a list of along-track slices with non-valid geolocation.
 
     Output format: [slice(start,stop), slice(start,stop),...]
 
     The minimum size of the output slices is 2.
-
+    
     If at a given cross-track index, there are always wrong geolocation,
     it discards such cross-track index(es) before indentifying the along-track slices.
-
+    
     Parameters
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
     min_size : int
         Minimum size for a slice to be returned.
         The default is 1.
@@ -720,153 +721,151 @@
 
     """
     list_unvalid_slices = get_slices_non_valid_geolocation(xr_obj)
     n_unvalid_scan_slices = len(list_unvalid_slices)
     if n_unvalid_scan_slices > 0:
         # Retrieve timesteps interval with non valid geolocation
         timesteps = _get_timesteps(xr_obj)
-        list_unvalid = [(timesteps[slc][0], timesteps[slc][-1]) for slc in list_unvalid_slices]
+        list_unvalid = [(timesteps[slc][0],timesteps[slc][-1]) for slc in list_unvalid_slices]
         first_problematic_timestep = list_unvalid[0][0]
         # Print non-contiguous scans
         if verbose:
             for start, stop in list_unvalid:
                 print(f"- Missing scans between {start} and {stop}")
         # Raise error and highlight first non-contiguous scan
-        msg = f"There are {n_unvalid_scan_slices} swath portions with non-valid geolocation."
-        msg += f"The first occur at {first_problematic_timestep}."
-        raise ValueError(msg)
-    return
+        raise ValueError(
+            f"There are {n_unvalid_scan_slices} swath portions with non-valid geolocation. The first occur at {first_problematic_timestep}."
+        )
+        
+    return None 
 
 
 def has_valid_geolocation(xr_obj):
     """Checks GPM object has valid geolocation."""
     if is_orbit(xr_obj):
         list_unvalid_slices = get_slices_non_valid_geolocation(xr_obj)
         n_unvalid_scan_slices = len(list_unvalid_slices)
-        return n_unvalid_scan_slices == 0
+        if n_unvalid_scan_slices == 0:
+            return True
+        else:
+            return False
     if is_grid(xr_obj):
         return True
     else:
-        raise ValueError("Unrecognized GPM xarray object.")
+        raise ValueError("Unrecognized GPM xarray object.")    
 
 
 def apply_on_valid_geolocation(function):
-    """A decorator that apply the get_slices_<function> only on portions
+    """A decorator that apply the get_slices_<function> only on portions 
     with valid geolocation."""
 
     @functools.wraps(function)
     def wrapper(*args, **kwargs):
         xr_obj = args[0]
         # Get slices with valid geolocation
         list_slices_valid = get_slices_valid_geolocation(xr_obj)
         # Loop over valid slices and retrieve the final slices
         list_slices = []
         new_args = list(args)
         for slc in list_slices_valid:
-            # Retrieve slice offset
+            # Retrieve slice offset 
             start_offset = slc.start
-            # Retrieve dataset subset
+            # Retrieve dataset subset 
             subset_xr_obj = xr_obj.isel(along_track=slc)
-            # Update args
+            # Update args 
             new_args[0] = subset_xr_obj
-            # Apply function
+            # Apply function 
             subset_slices = function(*args, **kwargs)
-            # Add start offset to subset slices
-            if len(subset_slices) > 0:
-                subset_slices = [
-                    slice(slc.start + start_offset, slc.stop + start_offset)
-                    for slc in subset_slices
-                ]
+            # Add start offset to subset slices 
+            if len(subset_slices) > 0: 
+                subset_slices = [slice(slc.start + start_offset, slc.stop + start_offset) for slc in subset_slices]
                 list_slices.append(subset_slices)
-        # Flatten the list
+        # Flatten the list 
         list_slices = list_slices_flatten(list_slices)
-        # Return list of slices
+        # Return list of slices 
         return list_slices
-
     return wrapper
 
 
 ####--------------------------------------------------------------------------.
 ############################
 #### Non-wobbling orbit ####
 ############################
 
 
 def _replace_0_values(x):
     """Replace 0 values with previous left non-zero occuring values.
 
     If the array start with 0, it take the first non-zero occuring values
     """
-    # Check inputs
+    # Check inputs 
     x = np.array(x)
     dtype = x.dtype
-    if np.all(x == 0):
-        raise ValueError("It's flat swath orbit.")
+    if np.all(x==0):  
+        raise ValueError("It's flat swath orbit.")  
     # Set 0 to NaN
     x = x.astype(float)
-    x[x == 0] = np.nan
+    x[x==0] = np.nan 
     # Infill from left values, and then from right (if x start with 0)
     x = pd.Series(x).fillna(method="ffill").fillna(method="bfill").to_numpy()
-    # Reset original dtype
+    # Reset original dtype 
     x = x.astype(dtype)
     return x
 
-
 def _get_non_wobbling_lats(lats, threshold=100):
     from gpm_api.utils.slices import list_slices_filter, list_slices_simplify
-
     # Get direction (1 ascending , -1 descending)
     directions = np.sign(np.diff(lats))
     directions = np.append(directions[0], directions)  # include startpoint
     directions = _replace_0_values(directions)
-
+       
     # Identify index where next element change
     idxs_change = np.where(np.diff(directions) != 0)[0]
-
+    
     # Retrieve valid slices
-    indices = np.unique(np.concatenate(([0], idxs_change, [len(lats) - 1])))
-    orbit_slices = [slice(indices[i], indices[i + 1] + 1) for i in range(len(indices) - 1)]
+    indices = np.unique(np.concatenate(([0], idxs_change, [len(lats)-1])))
+    orbit_slices = [slice(indices[i], indices[i+1]+1) for i in range(len(indices)-1)]
     list_slices = list_slices_filter(orbit_slices, min_size=threshold)
     list_slices = list_slices_simplify(list_slices)
     return list_slices
 
 
 @apply_on_valid_geolocation
 def get_slices_non_wobbling_swath(xr_obj, threshold=100):
     """Return the along-track slices along which the swath is not wobbling.
-
-    For wobbling, we define the occurence of changes in latitude directions
+    
+    For wobbling, we define the occurence of changes in latitude directions 
     in less than `threshold` scans.
-    The function extract the along-track boundary on both swath sides and
+    The function extract the along-track boundary on both swath sides and 
     identify where the change in orbit direction occurs.
-    """
-
+   """
+    
     from gpm_api.utils.slices import list_slices_intersection
-
+    
     # Assume lats, lons having shape (y, x) with x=along_track direction
     swath_def = xr_obj.gpm_api.pyresample_area
     lats_side0 = swath_def.lats[0, :]
     lats_side2 = swath_def.lats[-1, :]
-    # Get valid slices
+    # Get valid slices 
     list_slices1 = _get_non_wobbling_lats(lats_side0, threshold=100)
     list_slices2 = _get_non_wobbling_lats(lats_side2, threshold=100)
     list_slices = list_slices_intersection(list_slices1, list_slices2)
     return list_slices
 
 
 @apply_on_valid_geolocation
 def get_slices_wobbling_swath(xr_obj, threshold=100):
     """Return the along-track slices along which the swath is wobbling.
-
-    For wobbling, we define the occurence of changes in latitude directions
+    
+    For wobbling, we define the occurence of changes in latitude directions 
     in less than `threshold` scans.
-    The function extract the along-track boundary on both swath sides and
+    The function extract the along-track boundary on both swath sides and 
     identify where the change in orbit direction occurs.
-    """
-    # TODO: this has not been well checked...likely need +1 somewhere ...
+   """
+    # TODO: this has not been well checked...likely need +1 somewhere ... 
     list_slices1 = get_slices_non_wobbling_swath(xr_obj, threshold=threshold)
     list_slices_full = [slice(0, len(xr_obj["along_track"]))]
     list_slices = list_slices_difference(list_slices_full, list_slices1)
     return list_slices
 
 
 ####---------------------------------------------------------------------------
@@ -877,15 +876,15 @@
 
 def is_regular(xr_obj):
     """Checks the GPM object is regular.
 
     For GPM ORBITS, it checks that the scans are contiguous.
     For GPM GRID, it checks that the timesteps are regularly spaced.
     """
-    from gpm_api.utils.geospatial import is_grid, is_orbit
+    from gpm_api.utils.geospatial import is_orbit, is_grid
 
     if is_orbit(xr_obj):
         return has_contiguous_scans(xr_obj)
     elif is_grid(xr_obj):
         return has_regular_time(xr_obj)
     else:
         raise ValueError("Unrecognized GPM xarray object.")
@@ -898,143 +897,148 @@
     For GPM ORBITS, it returns slices to select contiguouse scans with valid geolocation.
     For GPM GRID, it returns slices to select periods with regular timesteps.
 
     The output format is: [slice(start,stop), slice(start,stop),...]
     For more information, read the documentation of:
     - gpm_api.utils.checks.get_slices_contiguous_scans
     - gpm_api.utils.checks.get_slices_regular_time
-
+    
     Parameters
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
     min_size : int
         Minimum size for a slice to be returned.
         If None, default to 1 for GRID objects, 2 for ORBIT objects.
 
     Returns
     -------
     list_slices : list
         List of slice object to select regular portions.
     """
-    from gpm_api.utils.geospatial import is_grid, is_orbit
+    from gpm_api.utils.geospatial import is_orbit, is_grid
 
     if is_orbit(xr_obj):
         min_size = 2 if min_size is None else min_size
         # Get swath portions where there are not missing scans (and granules)
         list_slices_contiguous = get_slices_contiguous_scans(xr_obj, min_size=min_size)
         # Get swath portions where there are valid geolocation
         list_slices_geolocation = get_slices_valid_geolocation(xr_obj, min_size=min_size)
-        # Find swath portions meeting all the requirements
-        list_slices = list_slices_intersection(list_slices_geolocation, list_slices_contiguous)
-
+        # Find swath portions meeting all the requirements 
+        list_slices = list_slices_intersection(list_slices_geolocation, 
+                                               list_slices_contiguous)
+        
         return list_slices
     elif is_grid(xr_obj):
         min_size = 1 if min_size is None else min_size
         return get_slices_regular_time(xr_obj, min_size=min_size)
     else:
         raise ValueError("Unrecognized GPM xarray object.")
 
 
 ####--------------------------------------------------------------------------.
-#### Get slices from GPM object variable values
-
+#### Get slices from GPM object variable values 
 
 def _check_criteria(criteria):
     if criteria not in ["all", "any"]:
         raise ValueError("Invalid value for criteria parameter. Must be 'all' or 'any'.")
 
 
 def _get_slices_variable_equal_value(da, value, dim=None, criteria="all"):
     """Return the slices with contiguous `value` in the `dim` dimension."""
-    # Check dim
-    if isinstance(dim, str):
+    # Check dim 
+    if isinstance(dim, str): 
         dim = [dim]
     dim = set(dim)
-    # Retrieve dims
+    # Retrieve dims 
     dims = set(da.dims)
     # Identify regions where the value occurs
     da_bool = da == value
     # Collapse other dimension than dim
-    dims_apply_over = list(dims.difference(dim))
-    bool_arr = (
-        da_bool.all(dim=dims_apply_over).data
-        if criteria == "all"
-        else da_bool.all(dim=dims_apply_over).data
-    )
+    dims_apply_over=list(dims.difference(dim))
+    if criteria == "all":
+        bool_arr = da_bool.all(dim=dims_apply_over).data
+    else:
+        bool_arr = da_bool.all(dim=dims_apply_over).data
     # Get list of slices with contiguous value
-    list_slices = get_list_slices_from_bool_arr(
-        bool_arr, include_false=False, skip_consecutive_false=True
-    )
+    list_slices = get_list_slices_from_bool_arr(bool_arr, include_false=False, skip_consecutive_false=True)
     return list_slices
 
 
-def get_slices_var_equals(da, dim, values, union=True, criteria="all"):
-    """Return a list of slices along the `dim` dimension where `values` occurs.
-
+def get_slices_var_equals(da,
+                          dim,
+                          values,
+                          union=True,
+                          criteria="all"):
+    """Return a list of slices along the `dim` dimension where `values` occurs. 
+    
     The function is applied recursively to each value in `values`.
-    If the DataArray has additional dimensions, the "criteria" parameter is
+    If the DataArray has additional dimensions, the "criteria" parameter is 
     used to determine whether all values within each slice index must be equal
-    to value (if set to "all") or if at least one value within the slice index
-    must be equal to value (if set to "any").
-
+    to value (if set to "all") or if at least one value within the slice index 
+    must be equal to value (if set to "any"). 
+    
     If `values` are a list of values:
     - if union=True, it return slices corresponding to the sequence of consecutive values.
     - if union=False, it return slices for each value in values.
-
+    
     If union=False [0,0, 1, 1] with values=[0,1] will return [slice(0,2), slice(2,4)]
     If union=True [0,0, 1, 1] with values=[0,1] will return [slice(0,4)]
-
-    `union` matters when multiple values are specified
+    
+    `union` matters when multiple values are specified 
     `criteria` matters when the DataArray has multiple dimensions.
     """
     _check_criteria(criteria)
-    # Get data array and dimensions
+    # Get data array and dimensions 
     da = da.compute()
     # Retrieve the slices where the value(s) occur
-    if isinstance(values, (float, int)):
-        return _get_slices_variable_equal_value(da=da, value=values, dim=dim, criteria=criteria)
-    else:
-        list_of_list_slices = [
-            _get_slices_variable_equal_value(da=da, value=value, dim=dim, criteria=criteria)
-            for value in values
-        ]
-        list_slices = (
-            list_slices_union(*list_of_list_slices)
-            if union
-            else list_slices_sort(*list_of_list_slices)
-        )
-    return list_slices
-
-
-def get_slices_var_between(da, dim, vmin=-np.inf, vmax=np.inf, criteria="all"):
-    """Return a list of slices along the `dim` dimension where values are between the interval.
-
-    If the DataArray has additional dimensions, the "criteria" parameter is
+    if isinstance(values, (float, int)): 
+        return _get_slices_variable_equal_value(da=da, 
+                                                value=values,
+                                                dim=dim,
+                                                criteria=criteria)
+    else: 
+        list_of_list_slices = [_get_slices_variable_equal_value(da=da, 
+                                                                value=value,
+                                                                dim=dim,
+                                                                criteria=criteria) for value in values]
+        if union: 
+             list_slices = list_slices_union(*list_of_list_slices) 
+        else: 
+             list_slices = list_slices_sort(*list_of_list_slices)              
+    return list_slices 
+
+
+def get_slices_var_between(da,
+                           dim,
+                           vmin=-np.inf,
+                           vmax=np.inf,
+                           criteria="all"):
+    """Return a list of slices along the `dim` dimension where values are between the interval. 
+    
+    If the DataArray has additional dimensions, the "criteria" parameter is 
     used to determine whether all values within each slice index must be between
-    the interval (if set to "all") or if at least one value within the slice index
-    must be between the interval (if set to "any").
-
+    the interval (if set to "all") or if at least one value within the slice index 
+    must be between the interval (if set to "any"). 
+  
     """
     _check_criteria(criteria)
-    # Check dim
-    if isinstance(dim, str):
+    # Check dim 
+    if isinstance(dim, str): 
         dim = [dim]
     dim = set(dim)
-    # Get data array and dimensions
+    # Get data array and dimensions 
     da = da.compute()
-    # Retrieve dims
+    # Retrieve dims 
     dims = set(da.dims)
-    # Identify regions where the value are between the thresholds
+    # Identify regions where the value are between the thresholds 
     da_bool = np.logical_and(da >= vmin, da <= vmax)
     # Collapse other dimension than dim
-    dims_apply_over = list(dims.difference(dim))
-    bool_arr = (
-        da_bool.all(dim=dims_apply_over).data
-        if criteria == "all"
-        else da_bool.any(dim=dims_apply_over).data
-    )
+    dims_apply_over=list(dims.difference(dim))
+    if criteria == "all":
+        bool_arr = da_bool.all(dim=dims_apply_over).data
+    else:
+        bool_arr = da_bool.any(dim=dims_apply_over).data
     # Get list of slices with contiguous value
-    list_slices = get_list_slices_from_bool_arr(
-        bool_arr, include_false=False, skip_consecutive_false=True
-    )
+    list_slices = get_list_slices_from_bool_arr(bool_arr, include_false=False, skip_consecutive_false=True)
     return list_slices
+
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/continents.py` & `gpm_api-0.2.3/gpm_api/utils/continents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Mon Jan 16 18:04:41 2023
 
 @author: ghiggi
 """
 import difflib
-
 CONTINENT_EXTENT_DICT = {
     "Africa": [-18.042, 51.292, -40.833, 37.092],
     "Antarctica": [-180, 180, -90, -60],
     "Arctic": [-180, 180, 60, 90],
     "Asia": [35, 180, 5, 80],
     "Australia": [105, 180, -55, 12],
     "Oceania": [105, 180, -55, 12],
     "Europe": [-30, 40, 34, 72],
     "North America": [-180, -52, 5, 83],
-    "South America": [-85, -30, -60, 15],
+    "South America": [-85, -30, -60, 15]
 }
 
-
 def get_continent_extent(name):
     # TODO: we could create a dictionary class which
     # - optionally is key unsensitive for get method !!!
     # - provide suggestions ...
     # --> Could be reused also when searching for GPM products, ...
     # -------------------------------------------------------------------------.
     # Check country format
     if not isinstance(name, str):
         raise TypeError("Please provide the continent name as a string.")
-
+    
     # Create same dictionary with lower case keys
-    continent_lower_extent_dict = {s.lower(): v for s, v in CONTINENT_EXTENT_DICT.items()}
+    continent_lower_extent_dict = {
+        s.lower(): v for s, v in CONTINENT_EXTENT_DICT.items()
+    }
     # Get list of valid continents
     valid_continent = list(CONTINENT_EXTENT_DICT.keys())
     valid_continent_lower = list(continent_lower_extent_dict)
     if name.lower() in valid_continent_lower:
         extent = continent_lower_extent_dict[name.lower()]
         # TODO:
         # - add 0.5° degree buffer
         # - ensure extent is correct
         return extent
     else:
-        possible_match = difflib.get_close_matches(name, valid_continent, n=1, cutoff=0.6)
+        possible_match = difflib.get_close_matches(
+            name, valid_continent, n=1, cutoff=0.6
+        )
         if len(possible_match) == 0:
             raise ValueError("Provide a valid continent name.")
         else:
             possible_match = possible_match[0]
             raise ValueError(
                 f"No matching continent. Maybe are you looking for '{possible_match}'?"
             )
+            
+
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/countries.py` & `gpm_api-0.2.3/gpm_api/utils/countries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sat Dec 10 16:10:52 2022
 
 @author: ghiggi
 """
-import difflib
 import os
-
 import yaml
+import difflib
 
 
 def extend_lonlat_extent(extent, x):
     """
     Extend the lat/lon extent by x degrees in every direction.
 
     Parameters
@@ -30,25 +30,25 @@
     """
     xmin, xmax, ymin, ymax = extent
     xmin = max(xmin - x, -180)
     xmax = min(xmax + x, 180)
     ymin = max(ymin - x, -90)
     ymax = min(ymax + x, 90)
     new_extent = (xmin, xmax, ymin, ymax)
-    return new_extent
+    return new_extent 
 
 
 def get_country_extent_dictionary():
     # TODO: improve relative path
     file_dir = os.path.realpath(__file__)
     base_dir = "/" + os.path.join(*file_dir.split("/")[0:-2])
     # Define file with extents dictionary
     countries_extent_fpath = os.path.join(base_dir, "etc/country_extent.yaml")
     # Read the data from the YAML file
-    with open(countries_extent_fpath) as infile:
+    with open(countries_extent_fpath, "r") as infile:
         countries_extent_dict = yaml.load(infile, Loader=yaml.FullLoader)
     return countries_extent_dict
 
 
 def get_country_extent(name):
     # TODO: we could create a dictionary class which
     # - optionally is key unsensitive for get method !!!
@@ -57,22 +57,28 @@
     # -------------------------------------------------------------------------.
     # Check country format
     if not isinstance(name, str):
         raise TypeError("Please provide the country name as a string.")
     # Get country extent dictionary
     countries_extent_dict = get_country_extent_dictionary()
     # Create same dictionary with lower case keys
-    countries_lower_extent_dict = {s.lower(): v for s, v in countries_extent_dict.items()}
+    countries_lower_extent_dict = {
+        s.lower(): v for s, v in countries_extent_dict.items()
+    }
     # Get list of valid countries
     valid_countries = list(countries_extent_dict.keys())
     valid_countries_lower = list(countries_lower_extent_dict)
     if name.lower() in valid_countries_lower:
         extent = countries_lower_extent_dict[name.lower()]
         extent = extend_lonlat_extent(extent, 0.2)
         return extent
     else:
-        possible_match = difflib.get_close_matches(name, valid_countries, n=1, cutoff=0.6)
+        possible_match = difflib.get_close_matches(
+            name, valid_countries, n=1, cutoff=0.6
+        )
         if len(possible_match) == 0:
             raise ValueError("Provide a valid country name.")
         else:
             possible_match = possible_match[0]
-            raise ValueError(f"No matching country. Maybe are you looking for '{possible_match}'?")
+            raise ValueError(
+                f"No matching country. Maybe are you looking for '{possible_match}'?"
+            )
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/geospatial.py` & `gpm_api-0.2.3/gpm_api/utils/geospatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Wed Aug 17 09:30:29 2022
 
 @author: ghiggi
 """
 import numpy as np
 import xarray as xr
-
 from gpm_api.utils.slices import get_list_slices_from_indices
 
-#### TODO:
+#### TODO: 
 # - croup_around(point, distance)
-# - get_extent_around(point, distance)
+# - get_extent_around(point, distance) 
 
 
 def unwrap_longitude_degree(x, period=360):
     """Unwrap longitude array."""
     x = np.asarray(x)
     mod = period / 2
     return (x + mod) % (2 * mod) - mod
@@ -63,23 +63,23 @@
 
     """
 
     from gpm_api.utils.continents import get_continent_extent
 
     extent = get_continent_extent(name)
     return crop(xr_obj=xr_obj, extent=extent)
-
-
+  
+    
 def get_crop_slices_by_extent(xr_obj, extent):
     """Compute the xarray object slices which are within the specified extent.
-
-
+    
+    
     If the input is a GPM Orbit, it returns a list of along-track slices
     If the input is a GPM Grid, it returns a dictionary of the lon/lat slices.
-
+    
     Parameters
     ----------
     xr_obj : xr.DataArray or xr.Dataset
         xarray object.
     extent : list or tuple
         The extent over which to crop the xarray object.
         `extent` must follow the matplotlib and cartopy conventions:
@@ -93,37 +93,37 @@
         idx_row, idx_col = np.where(
             (lon >= extent[0]) & (lon <= extent[1]) & (lat >= extent[2]) & (lat <= extent[3])
         )
         if idx_col.size == 0:
             raise ValueError("No data inside the provided bounding box.")
         # Retrieve list of along_track slices
         list_slices = get_list_slices_from_indices(idx_col)
-        return list_slices
+        return list_slices        
     elif is_grid(xr_obj):
         lon = xr_obj["lon"].data
         lat = xr_obj["lat"].data
         idx_col = np.where((lon >= extent[0]) & (lon <= extent[1]))[0]
         idx_row = np.where((lat >= extent[2]) & (lat <= extent[3]))[0]
         # If no data in the bounding box in current granule, return empty list
         if idx_row.size == 0 or idx_col.size == 0:
             raise ValueError("No data inside the provided bounding box.")
         lat_slices = get_list_slices_from_indices(idx_row)[0]
         lon_slices = get_list_slices_from_indices(idx_col)[0]
         slices_dict = {"lon": lon_slices, "lat": lat_slices}
-        return slices_dict
+        return slices_dict 
     else:
         raise NotImplementedError("")
 
-
+    
 def get_crop_slices_by_continent(xr_obj, name):
     """Compute the xarray object slices which are within the specified continent.
-
+    
     If the input is a GPM Orbit, it returns a list of along-track slices
     If the input is a GPM Grid, it returns a dictionary of the lon/lat slices.
-
+    
     Parameters
     ----------
     xr_obj : xr.DataArray or xr.Dataset
         xarray object.
     name : str
         Continent name.
     """
@@ -131,18 +131,18 @@
 
     extent = get_continent_extent(name)
     return get_crop_slices_by_extent(xr_obj=xr_obj, extent=extent)
 
 
 def get_crop_slices_by_country(xr_obj, name):
     """Compute the xarray object slices which are within the specified country.
-
+    
     If the input is a GPM Orbit, it returns a list of along-track slices
     If the input is a GPM Grid, it returns a dictionary of the lon/lat slices.
-
+    
     Parameters
     ----------
     xr_obj : xr.DataArray or xr.Dataset
         xarray object.
     name : str
         Country name.
     """
@@ -168,23 +168,21 @@
     Returns
     -------
     xr_obj : xr.DataArray or xr.Dataset
         Cropped xarray object.
 
     """
     # TODO: Check extent
-
+    
     if is_orbit(xr_obj):
         # - Subset only along_track
         list_slices = get_crop_slices_by_extent(xr_obj, extent)
-        if len(list_slices) > 1:
-            raise ValueError(
-                "The orbit is crossing the extent multiple times. Use get_crop_slices_by_extent !."
-            )
-        xr_obj_subset = xr_obj.isel(along_track=list_slices[0])
+        if len(list_slices) > 1: 
+            raise ValueError("The orbit is crossing the extent multiple times. Use get_crop_slices_by_extent !.")
+        xr_obj_subset =  xr_obj.isel(along_track=list_slices[0])
 
     elif is_grid(xr_obj):
         slice_dict = get_crop_slices_by_extent(xr_obj, extent)
         xr_obj_subset = xr_obj.isel(slice_dict)
     else:
         orbit_dims = ("cross_track", "along_track")
         grid_dims = ("lon", "lat")
@@ -198,21 +196,27 @@
 ####---------------------------------------------------------------------------.
 #### TODO MOVE TO utils.checks !!!
 
 
 def is_orbit(xr_obj):
     # TODO: --> MOVED TO gpm_api.dataset
     """Check whether the GPM xarray object is an orbit."""
-    return "along_track" in list(xr_obj.dims)
+    if "along_track" in list(xr_obj.dims):
+        return True
+    else:
+        return False
 
 
 def is_grid(xr_obj):
     # TODO: --> MOVED TO gpm_api.dataset
     """Check whether the GPM xarray object is a grid."""
-    return bool("longitude" in list(xr_obj.dims) or "lon" in list(xr_obj.dims))
+    if "longitude" in list(xr_obj.dims) or "lon" in list(xr_obj.dims):
+        return True
+    else:
+        return False
 
 
 def is_spatial_2d(xr_obj):
     """Check whether the GPM xarray object is a 2D fields.
 
     It returns True if the object has only two spatial dimensions.
     The xarray object is squeezed before testing, so that (i.e. time)
@@ -236,32 +240,32 @@
 
 
 #### TODO MOVE TO pyresample accessor !!!
 
 
 def get_pyresample_area(xr_obj):
     """It returns the corresponding pyresample area."""
-    from pyresample import SwathDefinition
-
+    from pyresample import SwathDefinition, AreaDefinition
+    
     # TODO: Implement as pyresample accessor
     # --> ds.pyresample.area
     # ds.crs.to_pyresample_area
     # ds.crs.to_pyresample_swath
 
     # If Orbit Granule --> Swath Definition
     if is_orbit(xr_obj):
         # Define SwathDefinition with xr.DataArray lat/lons
         # - Otherwise fails https://github.com/pytroll/satpy/issues/1434
-
-        # Ensure correct dimension order
+        
+        # Ensure correct dimension order 
         if "cross_track" in xr_obj.dims:
             xr_obj = xr_obj.transpose("cross_track", "along_track", ...)
-        else:
+        else: 
             raise ValueError("Can not derive SwathDefinition area without cross-track dimension.")
-
+            
         lons = xr_obj["lon"].values
         lats = xr_obj["lat"].values
 
         # TODO: this might be needed
         # - otherwise ValueError 'ndarray is not C-contiguous' when resampling
         # lons = np.ascontiguousarray(lons)
         # lats = np.ascontiguousarray(lats)
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/slices.py` & `gpm_api-0.2.3/gpm_api/utils/slices.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sat Dec 10 18:46:00 2022
 
 @author: ghiggi
 """
-from functools import reduce
-
 import numpy as np
+from functools import reduce
 
 ####---------------------------------------------------------------------------.
-#### Tools for list_slices
+#### Tools for list_slices  
 
 
 def get_list_slices_from_indices(indices):
     """Return a list of slices from a list/array of integer indices.
 
     Example:
         [0,1,2,4,5,8] --> [slices(0,3),slice(4,6), slice(8,9)]
     """
-    if isinstance(indices, (int, float)):
-        indices = [indices]
     # Checks
-    if len(indices) == 0:
+    if len(indices) == 0: 
         list_slices = []
         return list_slices
     indices = np.asarray(indices).astype(int)
     indices = sorted(np.unique(indices))
     if np.any(np.sign(indices) < 0):
-        raise ValueError("get_list_slices_from_indices expects only positive" " integer indices.")
+        raise ValueError("get_list_slices_from_indices expects only positive"
+                         " integer indices.")
     if len(indices) == 1:
         return [slice(indices[0], indices[0] + 1)]
     # Retrieve slices
     # idx_splits = np.where(np.diff(indices) > 1)[0]
     # if len(idx_splits) == 0:
     #     list_slices = [slice(min(indices), max(indices))]
     # else:
@@ -49,38 +48,38 @@
             previous = idx
     list_slices.append(slice(start, previous + 1))
     return list_slices
 
 
 def get_indices_from_list_slices(list_slices, check_non_intersecting=True):
     """Return a numpy array of indices from a list of slices."""
-    if len(list_slices) == 0:
+    if len(list_slices) == 0: 
         return np.array([])
     list_indices = [np.arange(slc.start, slc.stop, slc.step) for slc in list_slices]
     indices, counts = np.unique(np.concatenate(list_indices), return_counts=True)
     if check_non_intersecting and np.any(counts > 1):
         raise ValueError("The list of slices contains intersecting slices!")
     return indices
 
 
 def list_slices_intersection(*args):
     """Return the intersecting slices from multiple list of slices."""
-    list_indices = [get_indices_from_list_slices(l_slc) for l_slc in list(args)]
+    list_indices = [get_indices_from_list_slices(l) for l in list(args)]
     intersect_indices = reduce(np.intersect1d, list_indices)
     return get_list_slices_from_indices(intersect_indices)
 
 
 def list_slices_union(*args):
     """Return the union slices from multiple list of slices."""
-    list_indices = [get_indices_from_list_slices(l_slc) for l_slc in list(args)]
+    list_indices = [get_indices_from_list_slices(l) for l in list(args)]
     union_indices = np.unique(np.concatenate(list_indices))
     return get_list_slices_from_indices(union_indices)
 
 
-def list_slices_difference(list_slices1, list_slices2):
+def list_slices_difference(list_slices1, list_slices2): 
     """Return the list of slices covered by list_slices1 not intersecting list_slices2."""
     list_indices1 = get_indices_from_list_slices(list_slices1)
     list_indices2 = get_indices_from_list_slices(list_slices2)
     diff_indices = np.setdiff1d(list_indices1, list_indices2)
     list_slices = get_list_slices_from_indices(diff_indices)
     return list_slices
 
@@ -104,15 +103,15 @@
 def _list_slices_sort(list_slices):
     """Sort a single list of slices."""
     return sorted(list_slices, key=lambda x: x.start)
 
 
 def list_slices_sort(*args):
     """Sort a single or multiple list of slices by slice.start.
-
+    
     It output a single list of slices!
     """
     list_slices = list_slices_combine(*args)
     list_slices = _list_slices_sort(list_slices)
     return list_slices
 
 
@@ -120,116 +119,125 @@
     """Filter list of slices by size."""
     if min_size is None and max_size is None:
         return list_slices
     # Define min and max size if one is not specified
     min_size = 0 if min_size is None else min_size
     max_size = np.inf if max_size is None else max_size
     # Get list of slice sizes
-    sizes = [get_slice_size(slc) if isinstance(slc, slice) else 0 for slc in list_slices]
+    sizes = [
+        get_slice_size(slc) if isinstance(slc, slice) else 0 for slc in list_slices
+    ]
     # Retrieve valid slices
-    valid_bool = np.logical_and(np.array(sizes) >= min_size, np.array(sizes) <= max_size)
+    valid_bool = np.logical_and(
+        np.array(sizes) >= min_size, np.array(sizes) <= max_size
+    )
     list_slices = np.array(list_slices)[valid_bool].tolist()
     return list_slices
 
 
 def list_slices_flatten(list_slices):
     """Flatten out list of slices with 2 nested level.
-
+    
     Examples:
     [[slice(1, 7934, None)], [slice(1, 2, None)]] --> [slice(1, 7934, None), slice(1, 2, None)]
     [slice(1, 7934, None), slice(1, 2, None)] --> [slice(1, 7934, None), slice(1, 2, None)]
     """
     flat_list = []
     for sublist in list_slices:
         if isinstance(sublist, list):
             for item in sublist:
                 flat_list.append(item)
-        else:
+        else: 
             flat_list.append(sublist)
-    return flat_list
+    return flat_list 
+   
 
-
-def get_list_slices_from_bool_arr(bool_arr, include_false=True, skip_consecutive_false=True):
+def get_list_slices_from_bool_arr(
+    bool_arr, include_false=True, skip_consecutive_false=True
+):
     """Return the slices corresponding to sequences of True in the input arrays.
 
     If include_false=True, the last element of each slice sequence (except the last) will be False
     If include_false=False, no element in each slice sequence will be False
     If skip_consecutive_false=True (default), the first element of each slice must be a True.
     If skip_consecutive_false=False, it returns also slices of size 1 which selects just the False value.
     Note: if include_false = False, skip_consecutive_false is automatically True.
-
+    
     Examples:
-    If include_false=True and skip_consecutive_false=False:
+    If include_false=True and skip_consecutive_false=False: 
        --> [False, False] --> [slice(0,1), slice(1,2)]
-    If include_false=True and skip_consecutive_false=True:
+    If include_false=True and skip_consecutive_false=True: 
        --> [False, False] --> []
        --> [False, False, True] --> [slice(2,3)]
        --> [False, False, True, False] --> [slice(2,4)]
     If include_false=False:
         --> [False, False, True, False] --> [slice(2,3)]
-
+        
     """
     # Check the arguments
     if not include_false:
         skip_consecutive_false = True
     bool_arr = np.array(bool_arr)
     # If all True
     if np.all(bool_arr):
         list_slices = [slice(0, len(bool_arr))]
     # If all False
     elif np.all(~bool_arr):
-        list_slices = (
-            [] if skip_consecutive_false else [slice(i, i + 1) for i in range(0, len(bool_arr))]
-        )
+        if skip_consecutive_false:
+            list_slices = []
+        else:
+            list_slices = [slice(i, i + 1) for i in range(0, len(bool_arr))]
     # If True and False
     else:
         # Retrieve indices where False start to occur
         false_indices = np.argwhere(~bool_arr).flatten()
         # Prepend -1 so first start start at 0, if no False at idx 0
         false_indices = np.append(-1, false_indices)
         list_slices = []
         for i in range(1, len(false_indices)):
             idx_before = false_indices[i - 1]
             idx = false_indices[i]
-            if skip_consecutive_false and idx - idx_before == 1:
-                continue
+            if skip_consecutive_false:
+                if idx - idx_before == 1:
+                    continue
             # Define start
             start = idx_before + 1
             # Define stop
-            stop = idx + 1 if include_false else idx
+            if include_false:
+                stop = idx + 1
+            else:
+                stop = idx
             # Define slice
             slc = slice(start, stop)
             list_slices.append(slc)
 
         # Includes the last slice (if the last bool_arr element is not False)
         if idx < len(bool_arr) - 1:
             start = idx + 1
             stop = len(bool_arr)
             slc = slice(start, stop)
             list_slices.append(slc)
 
     # Return list of slices
     return list_slices
 
-
 # tests for _get_list_slices_from_bool_arr
 # bool_arr = np.array([True, False, True, True, True])
 # bool_arr = np.array([True, True, True, False, True])
 # bool_arr = np.array([True, True, True, True, False])
 # bool_arr = np.array([True, False, False, True, True])
 # bool_arr = np.array([True, True, True, False, False])
 # bool_arr = np.array([False, True, True, True, False])
 # bool_arr = np.array([False, False, True, True, True])
 # bool_arr = np.array([False])
 
 
 ####----------------------------------------------------------------------------.
 #### Tools for slice manipulation
 
-
 def ensure_is_slice(slc):
     if isinstance(slc, slice):
         return slc
     else:
         if isinstance(slc, int):
             slc = slice(slc, slc + 1)
         elif isinstance(slc, (list, tuple)) and len(slc) == 1:
@@ -240,45 +248,45 @@
             # TODO: check if continuous
             raise ValueError("Impossibile to convert to a slice object.")
     return slc
 
 
 def get_slice_size(slc):
     """Get size of the slice.
-
-    Note: The actual slice size must not be representative of the true slice if
+    
+    Note: The actual slice size must not be representative of the true slice if 
     slice.stop is larger than the length of object to be sliced.
     """
     if not isinstance(slc, slice):
         raise TypeError("Expecting slice object")
     size = slc.stop - slc.start
     return size
 
 
 def get_idx_bounds_from_slice(slc):
     """Get start and end indices of the slice.
-
+    
     Note: For index based selection, use idx_start:idx_end+1 !
-    """
+    """    
     if not isinstance(slc, slice):
         raise TypeError("Expecting slice object")
     idx_start = slice.start
     idx_end = slice.stop - 1
     return idx_start, idx_end
 
 
 def get_slice_from_idx_bounds(idx_start, idx_end):
     """Return the slice required to include the idx bounds."""
-    return slice(idx_start, idx_end + 1)
-
+    return slice(idx_start, idx_end+1)
+   
 
-def pad_slice(slc, padding, min_start=0, max_stop=np.inf):
+def pad_slice(slc, padding, min_start=0, max_stop=np.inf): 
     """
     Increase/decrease the slice with the padding argument.
-
+    
     Parameters
     ----------
     slc : slice
         Slice objects.
     padding : int
         Padding to be applied to the slice.
     min_start : int, optional
@@ -289,199 +297,155 @@
         The maximum value for the stop of the new slice.
 
     Returns
     -------
     list_slices : TYPE
         The list of slices after applying padding.
     """
-
+    
     new_slice = slice(max(slc.start - padding, 0), min(slc.stop + padding, max_stop))
     return new_slice
 
 
 def pad_slices(list_slices, padding, valid_shape):
     """
     Increase/decrease the list of slices with the padding argument.
-
+    
     Parameters
     ----------
     list_slices : list
         List of slice objects.
     padding : (int or tuple)
         Padding to be applied on each slice.
     valid_shape : tuple
-        The shape of the array which the slices should be valid on.
+        The shape of the array which the slices should be valid on. 
 
     Returns
     -------
     list_slices : TYPE
         The list of slices after applying padding.
     """
-    # Check the inputs
+    # Check the inputs 
     if isinstance(padding, int):
         padding = [padding] * len(list_slices)
     if isinstance(valid_shape, int):
         valid_shape = [valid_shape] * len(list_slices)
     if isinstance(padding, (list, tuple)) and len(padding) != len(valid_shape):
-        raise ValueError(
-            "Invalid padding. The length of padding should be the same as the length of valid_shape."
-        )
-    # Apply padding
-    list_slices = [
-        pad_slice(s, padding=p, min_start=0, max_stop=valid_shape[i])
-        for i, (s, p) in enumerate(zip(list_slices, padding))
-    ]
+        raise ValueError("Invalid padding. The length of padding should be the same as the length of valid_shape.")
+    # Apply padding 
+    list_slices = [pad_slice(s, padding=p, min_start=0, max_stop=valid_shape[i]) for i, (s, p) in enumerate(zip(list_slices, padding))]
     return list_slices
 
 
 # min_size = 10
 # min_start = 0
-# max_stop = 20
+# max_stop = 20 
 # slc = slice(1, 5)   # left bound
 # slc = slice(15, 20) # right bound
 # slc = slice(8, 12) # middle
 
-
 def enlarge_slice(slc, min_size, min_start=0, max_stop=np.inf):
-    """
-    Enlarge a slice object to have at least a size of min_size.
-
-    The function enforces the left and right bounds of the slice by max_stop and min_start.
-    If the original slice size is larger than min_size, the original slice will be returned.
-
-    Parameters
-    ----------
-    slc : slice
-        The original slice object to be enlarged.
-    min_size : min_size
-        The desired minimum size of the new slice.
-    min_start : int, optional
-       The default is np.inf.
-       The minimum value for the start of the new slice.
-       The default is 0.
-    max_stop : int
-        The maximum value for the stop of the new slice.
-
-    Returns
-    -------
-    slice
-        The new slice object with a size of at least min_size and respecting the left and right bounds.
-
-    """
-    # Get slice size
-    slice_size = get_slice_size(slc)
-
-    # If min_size is larger than allowable size, raise error
-    if min_size > (max_stop - min_start):
-        raise ValueError(
-            f"'min_size' {min_size} is too large to generate a slice between {min_start} and {max_stop}."
-        )
-
-    # If slice size larger than min_size, return the slice
-    if slice_size >= min_size:
-        return slc
-
-    # Calculate the number of points to add on both sides
-    n_indices_to_add = min_size - slice_size
-    add_to_left = add_to_right = n_indices_to_add // 2
-
-    # If n_indices_to_add is odd, add + 1 on the left
-    if n_indices_to_add % 2 == 1:
-        add_to_left += 1
-
-    # Adjust adding for left and right bounds
-    naive_start = slc.start - add_to_left
-    naive_stop = slc.stop + add_to_right
-    if naive_start <= min_start:
-        exceeding_left_size = min_start - naive_start
-        add_to_right += exceeding_left_size
-        add_to_left -= exceeding_left_size
-    if naive_stop >= max_stop:
-        exceeding_right_size = naive_stop - max_stop
-        add_to_right -= exceeding_right_size
-        add_to_left += exceeding_right_size
-
-    # Define new slice
-    start = slc.start - add_to_left
-    stop = slc.stop + add_to_right
-    new_slice = slice(start, stop)
-
-    # Check
-    assert get_slice_size(new_slice) == min_size
-
-    # Return new slice
-    return new_slice
-
+     """
+     Enlarge a slice object to have at least a size of min_size. 
+     
+     The function enforces the left and right bounds of the slice by max_stop and min_start.
+     If the original slice size is larger than min_size, the original slice will be returned.
+                 
+     Parameters
+     ----------
+     slc : slice
+         The original slice object to be enlarged.
+     min_size : min_size
+         The desired minimum size of the new slice.
+     min_start : int, optional
+        The default is np.inf.
+        The minimum value for the start of the new slice.
+        The default is 0.
+     max_stop : int
+         The maximum value for the stop of the new slice.
+
+     Returns
+     -------
+     slice
+         The new slice object with a size of at least min_size and respecting the left and right bounds.
+
+     """
+     # Get slice size 
+     slice_size = get_slice_size(slc)
+     
+     # If slice size larger than min_size, return the slice 
+     if slice_size >= min_size:
+         return slc
+          
+     # Calculate the number of points to add on both sides
+     n_indices_to_add = min_size - slice_size
+     add_to_left = add_to_right = n_indices_to_add // 2
+     
+     # If n_indices_to_add is odd, add + 1 on the left 
+     if n_indices_to_add % 2 == 1:
+         add_to_left += 1
+     
+     # Adjust adding for left and right bounds 
+     naive_start = slc.start - add_to_left 
+     naive_stop = slc.stop + add_to_right
+     if naive_start <= min_start:
+         exceeding_left_size = min_start - naive_start
+         add_to_right += exceeding_left_size
+         add_to_left -= exceeding_left_size
+     if naive_stop >= max_stop:
+         exceeding_right_size = naive_stop - max_stop
+         add_to_right -= exceeding_right_size
+         add_to_left += exceeding_right_size
+     
+     # Define new slice 
+     start = slc.start - add_to_left
+     stop = slc.stop + add_to_right
+     new_slice = slice(start, stop) 
+     
+     # Check 
+     assert  get_slice_size(new_slice) == min_size
+     
+     # Return new slice 
+     return new_slice
+ 
 
 def enlarge_slices(list_slices, min_size, valid_shape):
     """
-    Enlarge a list of slice object to have at least a size of min_size.
-
+    Enlarge a list of slice object to have at least a size of min_size. 
+     
     The function enforces the left and right bounds of the slice to be between 0 and valid_shape.
     If the original slice size is larger than min_size, the original slice will be returned.
-
+    
     Parameters
     ----------
     list_slices : list
         List of slice objects.
     min_size : (int or tuple)
         Minimum size of the output slice.
     valid_shape : tuple
-        The shape of the array which the slices should be valid on.
+        The shape of the array which the slices should be valid on. 
 
     Returns
     -------
     list_slices : list
         The list of slices after enlarging it (if necessary).
     """
-    # Check the inputs
+    # Check the inputs 
     if isinstance(min_size, int):
         min_size = [min_size] * len(list_slices)
     if isinstance(valid_shape, int):
         valid_shape = [valid_shape] * len(list_slices)
     if isinstance(min_size, (list, tuple)) and len(min_size) != len(min_size):
-        raise ValueError(
-            "Invalid min_size. The length of min_size should be the same as the length of valid_shape."
-        )
-    # Enlarge the slice
-    list_slices = [
-        enlarge_slice(slc, min_size=s, min_start=0, max_stop=valid_shape[i])
-        for i, (slc, s) in enumerate(zip(list_slices, min_size))
-    ]
+        raise ValueError("Invalid min_size. The length of min_size should be the same as the length of valid_shape.")
+    # Enlarge the slice  
+    list_slices = [enlarge_slice(slc, min_size=s, min_start=0, max_stop=valid_shape[i]) for i, (slc, s) in enumerate(zip(list_slices, min_size))]
     return list_slices
 
-
 ###----------------------------------------------------------------------------.
-#### Tools for slice creation
+ 
 
 
-def get_slice_around_index(index, size, min_start=0, max_stop=np.inf):
-    """
-    Get a slice object of `size` around `index` value.
 
-    If size is larger than (max_stop-min_start), raise an error.
 
-    Parameters
-    ----------
-    index : int
-        The index value around which to retrieve the slice.
-    min_size : min_size
-        The desired size of the slice around the index.
-    min_start : int, optional
-       The default is np.inf.
-       The minimum value for the start of the new slice.
-       The default is 0.
-    max_stop : int
-        The maximum value for the stop of the new slice.
 
-    Returns
-    -------
-    slice
-        The new slice object with a size of at least min_size and respecting the left and right bounds.
 
-    """
 
-    index_slc = slice(index, index + 1)
-    slc = enlarge_slice(index_slc, min_size=size, min_start=min_start, max_stop=max_stop)
-    if slc == index_slc:
-        raise ValueError("'size' {size} is to large to be between {min_start} and {max_stop}.")
-    return slc
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/time.py` & `gpm_api-0.2.3/gpm_api/utils/time.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Mon Oct 31 13:24:41 2022
 
 @author: ghiggi
 """
 import numpy as np
 import pandas as pd
-
 from gpm_api.io.checks import (
-    check_start_end_time,
     check_time,
+    check_start_end_time,
 )
 
+
 ####--------------------------------------------------------------------------.
 ############################
 #### Subsetting by time ####
 ############################
 
 
 def subset_by_time(xr_obj, start_time=None, end_time=None):
@@ -101,15 +102,17 @@
 
 
 def has_nat(timesteps):
     """Return True if any of the timesteps is NaT."""
     return np.any(is_nat(timesteps))
 
 
-def interpolate_nat(timesteps, method="linear", limit=5, limit_direction=None, limit_area=None):
+def interpolate_nat(
+    timesteps, method="linear", limit=5, limit_direction=None, limit_area=None
+):
     """
     Fill NaT values using an interpolation method.
 
     Notes:
     - Depending on the interpolation method (i.e. linear) the infilled values
       could have ns resolution.
 
@@ -195,15 +198,17 @@
     timesteps = xr_obj["time"].values
 
     # In case only 1 timestep, return the object (also Grid case)
     if len(timesteps) == 1:
         return xr_obj
 
     # Interpolate if maximum 10 timesteps are missing
-    timesteps = interpolate_nat(timesteps, method="linear", limit=limit, limit_area="inside")
+    timesteps = interpolate_nat(
+        timesteps, method="linear", limit=limit, limit_area="inside"
+    )
 
     # Check if there are still residual NaT
     if np.any(is_nat(timesteps)):
         raise ValueError("More than 10 consecutive timesteps are NaT.")
 
     # Update timesteps xarray object
     xr_obj["time"].data = timesteps
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/utils_HDF5.py` & `gpm_api-0.2.3/gpm_api/utils/utils_HDF5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Tue Jul 21 19:54:34 2020
 
 @author: ghiggi
 """
+import numpy
 import ast
-
 import h5py
-import numpy
 
 # -----------------------------------------------------------------------------.
 from gpm_api.utils.utils_string import (
-    str_collapse,
+    str_replace,
+    str_islist,
     str_detect,
-    str_isfloat,
     str_isinteger,
-    str_islist,
+    str_isfloat,
+    str_remove,
+    str_collapse,
     str_remove_empty,
-    str_replace,
 )
 
-
 # -----------------------------------------------------------------------------.
 def initialize_dict_with(keys):
     # dict(zip(keys, [None]*len(keys)))
     # {key: None for key in keys}
     return dict.fromkeys(keys)
 
 
 def numpy_numeric_format():
     return (
-        float,  # numpy.float deprecated since 1.20 and remove in 1.24
+        float, # numpy.float deprecated since 1.20 and remove in 1.24
         numpy.float32,
         numpy.float64,
         numpy.integer,
         numpy.int16,
         numpy.int32,
     )
 
@@ -73,15 +73,17 @@
             attr_dict[item] = attr
         # If attr is a string
         elif isinstance(attr, str):
             attr_dict[item] = parser(attr)
         # If a compressed string [with lot of attributes separeted by \n ...
         elif isinstance(attr, numpy.bytes_):
             # Decode
-            attr_str = attr.decode("UTF-8", errors="ignore").split("\n")  # Always create a list
+            attr_str = attr.decode("UTF-8", errors="ignore").split(
+                "\n"
+            )  # Always create a list
             # Clean the string
             attr_str = str_replace(attr_str, ";", "")
             attr_str = str_replace(attr_str, "\t", "")
             # attr_str = str_replace(attr_str,"=$","='-9999'")
             # Return a sub-dictionary if multiple arguments
             if isinstance(attr_str, list) and len(attr_str) > 1:
                 # Remove empty list element
@@ -89,15 +91,16 @@
                 # If = not present, collapse the string
                 if not all(str_detect(attr_str, "=")):
                     attr_dict[item] = str_collapse(attr_str)
                     continue
                 # If = is present in each list element --> Return a subdictionary
                 else:
                     tmp_dict = dict(
-                        (k.strip(), v.strip()) for k, v in (s.split("=", 1) for s in attr_str)
+                        (k.strip(), v.strip())
+                        for k, v in (s.split("=", 1) for s in attr_str)
                     )
                     # Process dictionary values
                     for k, v in tmp_dict.items():
                         tmp_dict[k] = parser(v)
                     # Attach dictionary
                     attr_dict[item] = tmp_dict
             # Return as string otherwise
@@ -143,31 +146,33 @@
             if len(attr_keys) >= 1:
                 for attr_key in attr_keys:
                     tmp_attr = hdf.attrs[attr_key]
                     # Decode if compressed
                     if isinstance(tmp_attr, numpy.bytes_):
                         tmp_attr = tmp_attr.decode("UTF-8")
                         tmp_attr = "\n" + tmp_attr
-                        tmp_attr = str_replace(tmp_attr, "\n", str("\n" + sep + "\t" + "\t" + "\t"))
+                        tmp_attr = str_replace(
+                            tmp_attr, "\n", str("\n" + sep + "\t" + "\t" + "\t")
+                        )
                         print(sep + "\t", "-->", attr_key, ":", tmp_attr)
                     else:
                         print(sep + "\t", "-->", attr_key, ":", tmp_attr)
         # Print keys of sub-group and sub-dataset
-        for key in hdf:
+        for key in hdf.keys():
             print(sep, "-", key, ":", hdf[key])
             print_hdf5(
                 hdf[key],
                 sep=sep + "\t",
                 dataset_attrs=dataset_attrs,
                 group_attrs=group_attrs,
             )
     elif isinstance(hdf, h5py.Dataset):
         # Option to print dataset attributes
         if dataset_attrs:
-            for attr_key in hdf.attrs:
+            for attr_key in hdf.attrs.keys():
                 print(sep + "\t", "-", attr_key, ":", hdf.attrs[attr_key])
 
 
 def h5dump(filepath, group="/", dataset_attrs=True, group_attrs=True):
     """
     Print HDF5 file metadata (and then close HDF5 file).
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/utils_cmap.py` & `gpm_api-0.2.3/gpm_api/utils/utils_cmap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Mon Nov 29 16:33:35 2021
 
 @author: ghiggi
 """
 ####--------------------------------------------------------------------------.
 ### TODO
@@ -63,27 +64,25 @@
 # norm = mpl.colors.BoundaryNorm(clevs, cmap.N)
 
 # https://stackoverflow.com/questions/16834861/create-own-colormap-using-matplotlib-and-plot-color-scale
 # Look at pycolorbar existing code
 
 # --------------------------------------------------------------------------.
 import copy
-
+import warnings
 import matplotlib
-import matplotlib as mpl
 import matplotlib.colors
-import matplotlib.pylab as plt
 import numpy as np
+import matplotlib as mpl
+import matplotlib.pylab as plt
+
 
 PRECIP_VALID_TYPES = ("intensity", "depth", "prob")
 PRECIP_VALID_UNITS = ("mm/h", "mm", "dBZ")
 
-####--------------------------------------------------------------------------.
-#### CMAP DICTIONARY
-
 CMAP_DICT = {
     "IMERG_Solid": {
         "type": "hex",
         "color_list": [
             "#45ffff",  # [0.1 - 0.2]
             "#49ddff",  # [0.2 - 0.3]
             "#4dbbff",  # [0.3 - 0.5]
@@ -107,32 +106,14 @@
             "#fffb00",  # [2.0 - 3.0]
             "#ffc400",  # [3.0 - 5.0]
             "#ff9300",  # [5.0 - 10.0]
             "#ff0000",  # [10.0 - 20.0]
             "#c80000",  # [20.0 - 50.0]
         ],
     },
-    "GOES_CloudPhase": {
-        "type": "name",
-        "color_list": [
-            "lightblue",  # Clear Sky
-            "darkblue",  # Liquid
-            "lightgreen",  # SC Liquid
-            "orange",  # Mixed
-            "white",  # Ice
-            "darkgray",  # Unknown
-        ],
-    },
-    "GOES_BinaryCloudMask": {
-        "type": "name",
-        "color_list": [
-            "lightblue",  # Clear Sky
-            "darkgray",  # Cloudy
-        ],
-    },
     "pysteps": {
         "type": "hex",
         "color_list": [
             "#9c7e94",  # redgray or '#e8d7f2' pink
             "#640064",
             "#AF00AF",
             "#DC00DC",
@@ -191,40 +172,36 @@
                 (40, 0, 0),  # 100
             ]
         )
         / 255,  # convert to 0-1
     },
 }
 
-####--------------------------------------------------------------------------.
-#### GPM COLOR DICTIONARY
-
-
 COLOR_DICT = {
     "IMERG_Solid": {
         "over_color": "#8c149c",
-        "under_color": "none",  # "#3a3d48",
+        "under_color": "none", # "#3a3d48",
         "bad_color": "gray",
         "bad_alpha": 0.5,
         "cmap": "IMERG_Solid",
         "cmap_type": "LinearSegmented",
         "levels": [0.1, 0.2, 0.3, 0.5, 1, 2, 3, 5, 10, 20, 50],
         "extend": "max",
-        "label": "Precipitation intensity [$mm \\ hr^{-1}$]",
+        "label": "Precipitation intensity [$mm \ hr^{-1}$]",
     },
     "IMERG_Liquid": {
         "over_color": "#910000",
-        "under_color": "none",  # "#3a3d48",
+        "under_color": "none", # "#3a3d48",
         "bad_color": "gray",
         "bad_alpha": 0.5,
         "cmap": "IMERG_Liquid",
         "cmap_type": "LinearSegmented",
         "levels": [0.1, 0.2, 0.3, 0.5, 1, 2, 3, 5, 10, 20, 50],
         "extend": "max",
-        "label": "Precipitation intensity [$mm \\ hr^{-1}$]",
+        "label": "Precipitation intensity [$mm \ hr^{-1}$]",
     },
     "GPM_Z": {
         "bad_color": "gray",
         "bad_alpha": 0.5,
         "cmap": "Spectral_r",
         # 'cmap_n': 10,
         "cmap_type": "Colormap",
@@ -262,15 +239,15 @@
         "bad_alpha": 0.5,
         "cmap": "plasma",
         # 'cmap_n': 10,
         "cmap_type": "Colormap",
         "vmin": -1,
         "vmax": 6,
         "extend": "both",
-        "label": "$N_w$ [$\\log{(mm^{-1} \\ m^{-3})}$]",
+        "label": "$N_w$ [$\log{(mm^{-1} \ m^{-3})}$]",
     },
     "GPM_LatentHeating": {
         "bad_color": "gray",
         "bad_alpha": 0.5,
         "cmap": "RdBu_r",
         "cmap_type": "Colormap",
         "norm": "SymLogNorm",
@@ -406,15 +383,15 @@
             40,
             63,
             100,
             160,
         ],
         "extend": "max",
         "extendrect": False,
-        "label": "Precipitation intensity [$mm \\ hr^{-1}$]",
+        "label": "Precipitation intensity [$mm \ hr^{-1}$]",
     },
     "pysteps_dBZ": {
         "over_color": "darkred",
         "bad_color": "gray",
         "bad_alpha": 0.5,
         "cmap": "pysteps",
         "cmap_type": "LinearSegmented",
@@ -424,266 +401,119 @@
         "over_color": "black",
         "bad_color": "gray",
         "bad_alpha": 0.5,
         "cmap": "STEPS-BE",
         "cmap_type": "LinearSegmented",
         "levels": [0.1, 0.25, 0.4, 0.63, 1, 1.6, 2.5, 4, 6.3, 10, 16, 25, 40, 63, 100],
     },
-    # "STEPS-BE_mm/hr": {
-    #     "over_color": "black",
-    #     "bad_color": "gray",
-    #     "bad_alpha": 0.5,
-    #     "cmap": "STEPS-BE",
-    #     "cmap_type": "LinearSegmented",
-    #     "levels": [0.1, 0.25, 0.4, 0.63, 1, 1.6, 2.5, 4, 6.3, 10, 16, 25, 40, 63, 100],
-    # },
+    "STEPS-BE_mm/hr": {
+        "over_color": "black",
+        "bad_color": "gray",
+        "bad_alpha": 0.5,
+        "cmap": "STEPS-BE",
+        "cmap_type": "LinearSegmented",
+        "levels": [0.1, 0.25, 0.4, 0.63, 1, 1.6, 2.5, 4, 6.3, 10, 16, 25, 40, 63, 100],
+    },
     "STEPS-BE_mm/hr": {
         "over_color": "black",
         "bad_color": "gray",
         "bad_alpha": 0.5,
         "cmap": "STEPS-BE",
         "cmap_type": "LinearSegmented",
         "levels": [10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60],
     },
 }
 
 precip_variables = [
-    # DPR
+     # DPR
     "precipRate",
     "precipRateNearSurface",
     "precipRateESurface",
     "precipRateESurface2",
+    "precipRateNearSurface", 
     # CORRA
     "precipTotRate",
     "nearSurfPrecipTotRate",
-    "estimSurfPrecipTotRate",
+    "estimSurfPrecipTotRate", 
     "OEestimSurfPrecipTotRate",
-    # 2A PMW
+    # 2A PMW 
     "surfacePrecipitation",
     # 2A-GPM-SLH
     "nearSurfacePrecipRate",
     # 2B-GPM-CSH
     "surfacePrecipRate",
-    # IMERG
+    # IMERG 
     "precipitationCal",
-    "precipitationUncal",
+    "precipitationUncal", 
     "IRprecipitation",
-    # GEO RRQPE
-    "RRQPE",
-]
+    ]
 
 for var in precip_variables:
     COLOR_DICT[var] = COLOR_DICT["pysteps_mm/hr"]
 
-COLOR_DICT["Tb"] = COLOR_DICT["Brightness_Temperature"]
-COLOR_DICT["Tc"] = COLOR_DICT["Brightness_Temperature"]
-
-####--------------------------------------------------------------------------.
-#### GOES DICTIONARY
-
-
-GOES_DICT = {
-    "COD": {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "viridis",
-        "cmap_type": "Colormap",
-        "vmin": 0,
-        "vmax": 50,
-        "extend": "max",
-        "extendfrac": 0.05,
-        "label": "Cloud Optical Depth at 640 nm [-]",
-    },
-    "CPS": {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "turbo_r",
-        "cmap_type": "Colormap",
-        "vmin": 0,
-        "vmax": 50,
-        "extend": "max",
-        "extendfrac": 0.05,
-        "label": "Cloud Particle Size [um]",
-    },
-    "CTH": {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "viridis",
-        "cmap_type": "Colormap",
-        "vmin": 0,
-        "vmax": 15000,
-        "extend": "max",
-        "extendfrac": 0.05,
-        "label": "Cloud Top Height [m]",
-    },
-    "CTT": {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "RdYlBu_r",
-        "cmap_type": "Colormap",
-        "vmin": 200,
-        "vmax": 300,
-        "extend": "both",
-        "extendfrac": 0.05,
-        "label": "Cloud Top Temperature [K]",
-    },
-    "CTP": {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "RdYlBu_r",
-        "cmap_type": "Colormap",
-        "vmin": 100,
-        "vmax": 1000,
-        "extend": "both",
-        "extendfrac": 0.05,
-        "label": "Cloud Top Pressure [hPa]",
-    },
-    "Phase": {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "GOES_CloudPhase",
-        "cmap_type": "Categorical",
-        "labels": ["Clear Sky", "Liquid", "SC Liquid", "Mixed", "Ice", "Unknown"],
-    },
-    "CM": {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "GOES_BinaryCloudMask",
-        "cmap_type": "Categorical",
-        "labels": ["Clear Sky", "Cloudy"],
-    },
-}
-COLOR_DICT.update(GOES_DICT)
-
-# ABI Reflectance channels (C01-C06)
-reflectance_channels = ["C" + str(i).zfill(2) for i in range(1, 7)]
-
-for channel in reflectance_channels:
-    GOES_DICT[channel] = {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "gray",
-        "cmap_type": "Colormap",
-        "vmin": 0,
-        "vmax": 100,
-        "extend": "neither",
-        "extendfrac": 0.05,
-        "label": "Reflectance [%]",
-    }
-
+COLOR_DICT['Tb'] = COLOR_DICT["Brightness_Temperature"]
+COLOR_DICT['Tc'] = COLOR_DICT["Brightness_Temperature"]
 
-# ABI BT channels (C07-C17)
-bt_channels = ["C" + str(i).zfill(2) for i in range(7, 17)]
-for channel in bt_channels:
-    GOES_DICT[channel] = {
-        "bad_color": "gray",
-        "bad_alpha": 0.5,
-        "cmap": "RdYlBu_r",
-        "cmap_type": "Colormap",
-        "vmin": 200,
-        "vmax": 300,
-        "extend": "both",
-        "extendfrac": 0.05,
-        "label": "Brightness Temperature [K]",
-    }
-
-
-# DQF channels colormaps
-default_dqf = {
-    "under_color": "none",
-    "bad_color": "gray",
-    "bad_alpha": 0.5,
-    "cmap": "viridis",
-    "cmap_type": "Colormap",
-    "vmin": 1,  # 0 is transparent with under_color="none"
-    "extend": "neither",
-    "extendfrac": 0.05,
-    "label": "Data Quality Flag",
-}
-for dqf_name in ["DQF_C" + str(i).zfill(2) for i in range(1, 17)]:
-    GOES_DICT[dqf_name] = default_dqf.copy()
-    GOES_DICT[dqf_name]["vmax"] = 4
-
-# DQF CLOUDS colormaps
-for dqf_name in ["DQF_" + var for var in ["COD", "CPS"]]:
-    GOES_DICT[dqf_name] = default_dqf.copy()
-    GOES_DICT[dqf_name]["vmax"] = 16
-
-for dqf_name in ["DQF_" + var for var in ["CTT", "CTH", "CTP"]]:
-    GOES_DICT[dqf_name] = default_dqf.copy()
-    GOES_DICT[dqf_name]["vmax"] = 6
-
-for dqf_name in ["DQF_" + var for var in ["Phase"]]:
-    GOES_DICT[dqf_name] = default_dqf.copy()
-    GOES_DICT[dqf_name]["vmax"] = 5
-
-for dqf_name in ["DQF_" + var for var in ["RRQPE"]]:
-    GOES_DICT[dqf_name] = default_dqf.copy()
-    GOES_DICT[dqf_name]["vmax"] = 64
-
-for dqf_name in ["DQF_" + var for var in ["CM"]]:
-    GOES_DICT[dqf_name] = default_dqf.copy()
-    GOES_DICT[dqf_name]["vmax"] = 2
-
-####--------------------------------------------------------------------------.
-#### Final color dictionary
-
-COLOR_DICT.update(GOES_DICT)
-
-# Reflectivity
-# "2A-DPR":
+# Reflectivity 
+# "2A-DPR": 
 #     "zFactorFinalESurface",
 #     "zFactorFinalNearSurface",
 #     "zFactorFinal",
 
-# 2A-DPR
+# 2A-DPR 
 # "airTemperature",
 # "landSurfaceType",
 
-# # '2A-ENV-DPR':
-# "cloudLiquidWater",
-# "waterVapor",
+# # '2A-ENV-DPR': 
+# "cloudLiquidWater", 
+# "waterVapor", 
 # "airPressure"],
 
 # # 2A-GMI
 # "rainWaterPath",
 # "cloudWaterPath",
 # "iceWaterPath",
 
 # # '2B-GPM-CORRA': [
 # "precipTotWaterCont",
-# "cloudIceWaterCont",
+# "cloudIceWaterCont", 
 # "cloudLiqWaterCont",
-# "OEcolumnCloudLiqWater",
+# "OEcolumnCloudLiqWater", 
 # "OEcloudLiqWaterCont",
 # "OEcolumnWaterVapor"
 
 # # 1B
-# "Tb",
-# # 1C
-# "Tc",
+# "Tb", 
+# # 1C 
+# "Tc", 
 # # '2B-GPM-CORRA'
 # "OEsimulatedBrightTemp",
 
 # Latent Heat
 # '2B-GPM-CSH': ["latentHeating"],
 # '2A-GPM-SLH': ["latentHeating"],
 
 
-# -----------------------------------------------------------------------------.
+
+
+
+#-----------------------------------------------------------------------------.
 
 
 def _dynamic_formatting_floats(float_array, colorscale="pysteps"):
     """Function to format the floats defining the class limits of the colorbar."""
     float_array = np.array(float_array, dtype=float)
 
     labels = []
     for label in float_array:
         if 0.1 <= label < 1:
-            formatting = ",.2f" if colorscale == "pysteps" else ",.1f"
+            if colorscale == "pysteps":
+                formatting = ",.2f"
+            else:
+                formatting = ",.1f"
         elif 0.01 <= label < 0.1:
             formatting = ",.2f"
         elif 0.001 <= label < 0.01:
             formatting = ",.3f"
         elif 0.0001 <= label < 0.001:
             formatting = ",.4f"
         elif label >= 1 and label.is_integer():
@@ -695,15 +525,15 @@
             labels.append(format(label, formatting))
         else:
             labels.append(str(int(label)))
 
     return labels
 
 
-# --------------------------------------------------------------------------.
+#...--------------------------------------------------------------------------.
 
 
 def get_colormap_setting(cbar_settings_name):
     # TODO: --> Accept other kwargs, check it,  and modify at the end ...
     if not isinstance(cbar_settings_name, (str, type(None))):
         raise TypeError("Expecting the colorscale name.")
 
@@ -716,121 +546,91 @@
         if cbar_settings_name is None:
             print("Returning default colorbar settings.")
         else:
             color_dict["cmap"] = cbar_settings_name
 
         # raise ValueError("{cbar_settings_name} cbar_settings  does not exist.")
 
-    # --------------------------------------------------------------------------.
-    # Get cmap info
+    #--------------------------------------------------------------------------.
+    # Get cmap
     cmap_type = color_dict["cmap_type"]
     cmap_name = color_dict["cmap"]
+    # Get colorbar levels (if available)
     clevs = color_dict.get("levels", None)
-    vmin = color_dict.get("vmin", None)
-    vmax = color_dict.get("vmax", None)
-
-    # Initialize cbar_kwargs
-    cbar_kwargs = {}
-
     # ------------------------------------------------------------------------.
     if cmap_type == "LinearSegmented":
         # TODO: Check level is a list > 2, length + 1 than color_list
 
         # Get color list
         color_list = CMAP_DICT[cmap_name]["color_list"]
 
         # Get colormap
-        cmap = mpl.colors.LinearSegmentedColormap.from_list("cmap", color_list, len(clevs) - 1)
-
-    # ------------------------------------------------------------------------.
-    elif cmap_type == "Categorical":
-        # Get color list
-        color_list = CMAP_DICT[cmap_name]["color_list"]
-
-        # Get class labels
-        labels = color_dict.get("labels", None)
-
-        # Check validity
-        if labels is None:
-            raise ValueError(f"If cmap_type is {cmap_type}, 'labels' list is required.")
-        if not isinstance(labels, list):
-            raise ValueError("'labels' must be a list.")
-        if len(color_list) != len(labels):
-            raise ValueError("'labels' must have same length as the 'color_list'.")
-
-        # Define colormap and colorbar settings
-        nlabels = len(labels)
-        cmap = mpl.colors.ListedColormap(color_list)
-
-        # Define norms
-        norm_bins = np.arange(-1, nlabels) + 0.5
-        norm = mpl.colors.BoundaryNorm(norm_bins, nlabels)
-
-        # Update cbar_kwargs
-        fmt = mpl.ticker.FuncFormatter(lambda x, pos: labels[norm(x)])
-        tickz = norm_bins[:-1] + 0.5
-        cbar_kwargs["format"] = fmt
-        cbar_kwargs["ticks"] = tickz
+        cmap = mpl.colors.LinearSegmentedColormap.from_list(
+            "cmap", color_list, len(clevs) - 1
+        )
 
     # ------------------------------------------------------------------------.
     # TODO: implement other cmap options
     elif cmap_type == "Colormap":
         # Get colormap
         cmap_n = color_dict.get("cmap_n", None)
         cmap = copy.copy(plt.get_cmap(cmap_name, cmap_n))
         vmin = color_dict.get("vmin", None)
         vmax = color_dict.get("vmax", None)
         norm = None
-
     # matplotlib.colors.NoNorm
     else:
         ticks = None
         # vmin and vmax to be defined
         raise NotImplementedError
 
-    # -------------------------------------------------------------------------.
+    #-------------------------------------------------------------------------.
     # Set norm if specified
     if color_dict.get("norm", None):
         if color_dict["norm"] == "SymLogNorm":
             norm = mpl.colors.SymLogNorm(
                 linthresh=color_dict["linthresh"],
                 vmin=vmin,
                 vmax=vmax,
                 base=color_dict.get("base", 10),
             )
         else:
             raise NotImplementedError()
 
-    # -------------------------------------------------------------------------.
+    #-------------------------------------------------------------------------.
     # Define BoundaryNorm
     if clevs is not None:
         norm = mpl.colors.BoundaryNorm(clevs, cmap.N)
-        vmin = None  # cartopy and matplotlib complain if not None when norm is provided !
+        vmin = (
+            None  # cartopy and matplotlib complain if not None when norm is provided !
+        )
         vmax = None
         ticks = clevs
     else:
         ticks = None
         # vmin and vmax to be defined
 
-    # -------------------------------------------------------------------------.
+    #-------------------------------------------------------------------------.
     # Define ticklabels
     # - Generate color level strings with correct amount of decimal places
     if clevs is not None:
         ticklabels = _dynamic_formatting_floats(ticks)
         # clevs_str = [f"{tick:.1f}" for tick in ticks] # for 0.1 probability
     else:
         ticklabels = None
 
-    # -------------------------------------------------------------------------.
+    #-------------------------------------------------------------------------.
     # Set over, under and alpha
     # If not specified, do not set ---> Will fill with the first/last color value
     # If 'none' --> It will be depicted in white
     if color_dict.get("over_color", None):
-        cmap.set_over(color=color_dict.get("over_color"), alpha=color_dict.get("over_alpha", None))
-    if color_dict.get("under_color", None):
+        cmap.set_over(
+            color=color_dict.get("over_color"), alpha=color_dict.get("over_alpha", None)
+        )
+    if color_dict.get("over_color", None):
         cmap.set_under(
             color=color_dict.get("under_color"),
             alpha=color_dict.get("under_alpha", None),
         )
     # ------------------------------------------------------------------------.
     # Set bad color
     # - If not 0, can cause cartopy bug
@@ -838,27 +638,25 @@
     cmap.set_bad(
         color=color_dict.get("bad_color", "none"),
         alpha=color_dict.get("bad_alpha", None),
     )
 
     # ------------------------------------------------------------------------.
     #### Set cbar kwargs
-    default_cbar_kwargs = {
+    cbar_kwargs = {
         "ticks": color_dict.get("ticks", ticks),
         "spacing": color_dict.get("spacing", "uniform"),  # or proportional
         "extend": color_dict.get("extend", "neither"),
         "extendfrac": color_dict.get("extendfrac", "auto"),
         "extendrect": color_dict.get("extendrect", False),
         "label": color_dict.get("label", None),
         "drawedges": color_dict.get("drawedges", False),
         "ticklocation": color_dict.get("ticklocation", "auto"),
         "shrink": color_dict.get("ticklocation", 1),
     }
-    default_cbar_kwargs.update(cbar_kwargs)
-
     # format
     # 'orientation':'horizontal'
     # 'aspect':40,
     # filled=True
 
     # ticklocation{'auto', 'left', 'right', 'top', 'bottom'}
     # extend{'neither', 'both', 'min', 'max'}
@@ -881,72 +679,95 @@
     plot_kwargs = {
         "cmap": cmap,
         "norm": norm,
         "vmin": vmin,
         "vmax": vmax,
     }
     # ------------------------------------------------------------------------.
-    return plot_kwargs, default_cbar_kwargs, ticklabels
+    return plot_kwargs, cbar_kwargs, ticklabels
 
 
-def get_colorbar_settings(name, plot_kwargs={}, cbar_kwargs={}):
-    try:
-        default_plot_kwargs, default_cbar_kwargs, default_ticklabels = get_colormap_setting(name)
-        default_cbar_kwargs["ticklabels"] = None
-    except:
-        default_plot_kwargs = {}
-        default_cbar_kwargs = {}
-
-    # If the default is a categorical colormap
-    # --> TODO: Set all to none
-
-    # If the default is a segmented colormap (with ticks and ticklabels)
-    if default_cbar_kwargs.get("ticks", None) is not None:
-        # If specifying a custom vmin, vmax, norm or cmap args, remove  the defaults
-        # - The discrete colorbar makes no sense anymore
-        if np.any(np.isin(["vmin", "vmax", "norm", "cmap"], list(plot_kwargs.keys()))):
-            default_cbar_kwargs.pop("ticks", None)
-            default_cbar_kwargs.pop("ticklabels", None)
-            default_plot_kwargs.pop("cmap", None)
-            default_plot_kwargs.pop("norm", None)
-            default_plot_kwargs.pop("vmin", None)
-            default_plot_kwargs.pop("vmax", None)
-
-    # If cmap is a string, retrieve colormap
-    if isinstance(plot_kwargs.get("cmap", None), str):
-        plot_kwargs["cmap"] = plt.get_cmap(plot_kwargs["cmap"])
-
-    # Update defaults with custom kwargs
-    default_plot_kwargs.update(plot_kwargs)
-    default_cbar_kwargs.update(cbar_kwargs)
-
-    # Return the kwargs
-    plot_kwargs = default_plot_kwargs
-    cbar_kwargs = default_cbar_kwargs
-
-    # Set default cmap if not available
-    if plot_kwargs.get("cmap", None) is None:
-        plot_kwargs["cmap"] = plt.get_cmap("viridis")
-
-    # Remove vmin, vmax
-    # --> vmin and vmax is not accepted by PolyCollection
-    # --> create norm or modify norm accordingly
-    norm = plot_kwargs.get("norm", None)
-    if norm is None:
-        norm = mpl.colors.Normalize(
-            vmin=plot_kwargs.pop("vmin", None), vmax=plot_kwargs.pop("vmax", None)
+####---------------------------------------------------------------------------.
+def get_colormap(ptype, units="mm/hr", colorscale="pysteps"):
+    """Function to generate a colormap (cmap) and norm.
+    Parameters
+    ----------
+    ptype : {'intensity', 'depth', 'prob'}, optional
+        Type of the map to plot: 'intensity' = precipitation intensity field,
+        'depth' = precipitation depth (accumulation) field,
+        'prob' = exceedance probability field.
+    units : {'mm/hr', 'mm', 'dBZ'}, optional
+        Units of the input array. If ptype is 'prob', this specifies the unit of
+        the intensity threshold.
+    colorscale : {'pysteps', 'STEPS-BE', 'BOM-RF3'}, optional
+        Which colorscale to use. Applicable if units is 'mm/hr', 'mm' or 'dBZ'.
+
+    Returns
+    -------
+    cmap : Colormap instance
+        colormap
+    norm : matplotlibcolors.Normalize object
+        Colors norm
+    clevs: list(float)
+        List of precipitation values defining the color limits.
+    clevs_str: list(str)
+        List of precipitation values defining the color limits (with correct
+        number of decimals).
+    """
+    if ptype in ["intensity", "depth"]:
+        cbar_settings_name = colorscale + "_" + units
+        plot_kwargs, cbar_kwargs, ticklabels = get_colormap_setting(cbar_settings_name)
+        cbar_kwargs["extend"] = "max"
+
+    elif ptype == "prob":
+        plot_kwargs, cbar_kwargs, ticklabels = get_colormap_setting(
+            "Precip_Probability"
         )
-        plot_kwargs["norm"] = norm
+        cbar_kwargs["extend"] = "neither"
     else:
-        if "vmin" in plot_kwargs:
-            if plot_kwargs["vmin"] is None:
-                _ = plot_kwargs.pop("vmin")
-            else:
-                plot_kwargs["norm"].vmin = plot_kwargs.pop("vmin")
+        plot_kwargs = {
+            "cmap": plt.cm.get_cmap("jet"),
+            "norm": mpl.colors.Normalize(),
+        }
+        cbar_kwargs = {}
+        ticklabels = None
+
+    return plot_kwargs, cbar_kwargs, ticklabels
+
+
+####---------------------------------------------------------------------------.
+#################
+### Examples ####
+#################
+# get colormap and color levels
+# colorscale = "STEPS-BE"
+# colorscale = "BOM-RF3"
+# colorscale= "IMERG_liquid"
+# colorscale= "IMERG_solid"
+# colorscale = "pysteps"
+
+
+# plot_kwargs, cbar_kwargs, ticklabels = get_colormap_setting("IMERG_Liquid")
+# plot_kwargs, cbar_kwargs, ticklabels = get_colormap_setting("pysteps_mm/hr")
+
+
+# plot_kwargs, cbar_kwargs,  ticklabels = get_colormap(ptype="default",
+#                                                      units="mm/hr",
+#                                                      colorscale="pysteps")
+
+
+# plot_kwargs, cbar_kwargs,  ticklabels = get_colormap(ptype="intensity",
+#                                                      units="mm/hr",
+#                                                      colorscale="pysteps")
+
+
+# plot_kwargs, cbar_kwargs,  ticklabels = get_colormap(ptype="prob",
+#                                                      units="mm/hr",
+#                                                      colorscale="pysteps")
 
-        if "vmax" in plot_kwargs:
-            if plot_kwargs["vmax"] is None:
-                _ = plot_kwargs.pop("vmax")
-            else:
-                plot_kwargs["norm"].vmax = plot_kwargs.pop("vmax")
 
-    return (plot_kwargs, cbar_kwargs)
+# p = da_precip_subset.plot.imshow(x="along_track", y="cross_track",
+#                                  interpolation="bilinear", # "nearest", "bicubic"
+#                                    cbar_kwargs=cbar_kwargs,
+#                                    **plot_kwargs)
+# cbar = p.colorbar
+# cbar.ax.set_yticklabels(ticklabels)
```

### Comparing `gpm_api-0.2.2/gpm_api/utils/utils_string.py` & `gpm_api-0.2.3/gpm_api/utils/utils_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Tue Jul 21 20:07:02 2020
 
 @author: ghiggi
 """
 # -----------------------------------------------------------------------------.
 ### Utils for parsing strings ####
 # https://www.rdocumentation.org/packages/stringr/versions/1.4.0
-import ast
 import re
-
+import ast
 import numpy as np
 
 
 def rep(x, times=1, each=False, length=0):
     """
     Implementation of functionality of rep() and rep_len() from R.
     Attributes:
@@ -136,37 +136,37 @@
 def str_subset(l_string, pattern):
     if isinstance(l_string, list):
         return [string for string in l_string if re.search(pattern, string)]
     else:
         if re.search(pattern, l_string):
             return l_string
         else:
-            return None
+            return
 
 
 def str_remove(l_string, pattern):
     """Remove strings matching the pattern."""
     if isinstance(l_string, list):
         return [string for string in l_string if not re.search(pattern, string)]
     else:
         if not re.search(pattern, l_string):
             return l_string
         else:
-            return None
+            return
 
 
 def str_remove_empty(l_string):
     """Remove empty strings ''."""
     if isinstance(l_string, list):
         return [string for string in l_string if len(string) >= 1]
     else:
         if len(l_string) >= 1:
             return l_string
         else:
-            return None
+            return
 
 
 def str_locate(l_string, pattern):
     """Provide the index of strings matching the pattern"""
     if isinstance(l_string, list):
         return [i for i, string in enumerate(l_string) if re.search(pattern, string)]
     else:
@@ -190,15 +190,17 @@
         return len(pattern.findall(l_string)) >= 1
     else:
         return False
 
 
 def str_extract(l_string, pattern, simplify=True):
     if isinstance(l_string, list):
-        return [str_simplify(re.findall(pattern, string), simplify) for string in l_string]
+        return [
+            str_simplify(re.findall(pattern, string), simplify) for string in l_string
+        ]
     else:
         return str_simplify(re.findall(pattern, l_string), simplify)
 
 
 def str_replace(l_string, pattern, replacement):
     if isinstance(l_string, list):
         return [re.sub(pattern, replacement, string) for string in l_string]
```

### Comparing `gpm_api-0.2.2/gpm_api/visualization/OLD_comparison.py` & `gpm_api-0.2.3/gpm_api/visualization/OLD_comparison.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Fri Sep  9 12:14:03 2022
 
 @author: ghiggi
 """
-import cartopy.crs as ccrs
-import matplotlib.pyplot as plt
-
 import gpm_api
+import cartopy
+import numpy as np
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+import cartopy.feature as cfeature
 
 
 def compare_products(
     base_dir,
     start_time,
     end_time,
     bbox,
@@ -77,15 +80,15 @@
     #### First Map
     ax = axs[0]
 
     # Retrieve DataArray
     da = list_da[0]
 
     # - Plot map
-    da.gpm_api.plot(ax=ax, add_colorbar=False)
+    p = da.gpm_api.plot(ax=ax, add_colorbar=False)
 
     # - Set title
     title = da.gpm_api.title(time_idx=0, add_timestep=False)
     ax.set_title(title)
 
     # - Set extent
     ax.set_extent(bbox_extent)
@@ -94,15 +97,15 @@
     #### Second Map
     ax = axs[1]
 
     # Retrieve DataArray
     da = list_da[1]
 
     # - Plot map
-    da.gpm_api.plot(ax=ax, add_colorbar=True)
+    p = da.gpm_api.plot(ax=ax, add_colorbar=True)
 
     # TODO: REMOVE Y AXIS
     # ax.set_yticklabels(None)
     #  ax.axes.get_yaxis().set_visible(False)
 
     # - Set title
     title = da.gpm_api.title(time_idx=0, add_timestep=False)
```

### Comparing `gpm_api-0.2.2/gpm_api/visualization/grid.py` & `gpm_api-0.2.3/gpm_api/visualization/grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sat Dec 10 19:13:34 2022
 
 @author: ghiggi
 """
 import cartopy.crs as ccrs
 import matplotlib.pyplot as plt
-
 from gpm_api.utils.checks import check_is_spatial_2d
-from gpm_api.utils.utils_cmap import get_colorbar_settings
 from gpm_api.visualization.plot import (
+    plot_cartopy_background,
     _plot_cartopy_imshow,
     #  _plot_mpl_imshow,
     _plot_xr_imshow,
     _preprocess_figure_args,
     _preprocess_subplot_kwargs,
-    plot_cartopy_background,
+    get_colorbar_settings,
 )
 
 
 def _plot_grid_map_cartopy(
     da,
     ax=None,
     add_colorbar=True,
     interpolation="nearest",
-    fig_kwargs={},
+    fig_kwargs={}, 
     subplot_kwargs={},
     cbar_kwargs={},
     **plot_kwargs,
 ):
     """Plot DataArray 2D field with cartopy."""
     # - Check inputs
     check_is_spatial_2d(da)
@@ -36,26 +36,26 @@
 
     # - Initialize figure
     if ax is None:
         subplot_kwargs = _preprocess_subplot_kwargs(subplot_kwargs)
         fig, ax = plt.subplots(subplot_kw=subplot_kwargs, **fig_kwargs)
         # - Add cartopy background
         ax = plot_cartopy_background(ax)
-
+  
     # - If not specified, retrieve/update plot_kwargs and cbar_kwargs as function of variable name
     variable = da.name
-    plot_kwargs, cbar_kwargs = get_colorbar_settings(
-        name=variable, plot_kwargs=plot_kwargs, cbar_kwargs=cbar_kwargs
-    )
-
-    # - Specify colorbar label
-    if "label" not in cbar_kwargs:
-        unit = da.attrs.get("units", "-")
-        cbar_kwargs["label"] = f"{variable} [{unit}]"
-
+    plot_kwargs, cbar_kwargs = get_colorbar_settings(name=variable,
+                                                     plot_kwargs=plot_kwargs, 
+                                                     cbar_kwargs=cbar_kwargs)
+    
+    # - Specify colorbar label 
+    if "label" not in cbar_kwargs: 
+        unit = da.attrs.get('units', "-")
+        cbar_kwargs['label'] = f"{variable} [{unit}]"
+        
     # - Add variable field with matplotlib
     p = _plot_cartopy_imshow(
         ax=ax,
         da=da,
         x="lon",
         y="lat",
         interpolation=interpolation,
@@ -68,127 +68,125 @@
 
 
 def _plot_grid_map_facetgrid(
     da,
     ax=None,
     add_colorbar=True,
     interpolation="nearest",
-    fig_kwargs={},
+    fig_kwargs={}, 
     subplot_kwargs={},
     cbar_kwargs={},
     **plot_kwargs,
 ):
     """Plot DataArray 2D field with xarray."""
     # - Check inputs
-    if ax is not None:
+    if ax is not None: 
         raise ValueError("When plotting with FacetGrid, do not specify the 'ax'.")
     _preprocess_figure_args(ax=ax, fig_kwargs=fig_kwargs, subplot_kwargs=subplot_kwargs)
     subplot_kwargs = _preprocess_subplot_kwargs(subplot_kwargs)
     # - Add info required to plot on cartopy axes within FacetGrid
-    plot_kwargs.update({"subplot_kws": subplot_kwargs})
-    plot_kwargs.update({"transform": ccrs.PlateCarree()})
+    plot_kwargs.update({"subplot_kws": subplot_kwargs})  
+    plot_kwargs.update({"transform": ccrs.PlateCarree()}) 
 
-    # - Plot with FacetGrid
-    p = plot_grid_image(
-        da=da,
-        ax=None,
-        add_colorbar=add_colorbar,
-        interpolation=interpolation,
-        fig_kwargs={},
-        cbar_kwargs={},
-        **plot_kwargs,
+    # - Plot with FacetGrid   
+    p = plot_grid_image(da=da,
+                        ax=None,
+                        add_colorbar=add_colorbar,
+                        interpolation=interpolation, 
+                        fig_kwargs={}, 
+                        cbar_kwargs={},
+                        **plot_kwargs,
     )
-
-    # - Add cartopy background to each subplot
+    
+    # - Add cartopy background to each subplot 
     for ax in p.axs.flatten():
         plot_cartopy_background(ax)
 
     # - Return mappable
     return p
 
 
 def plot_grid_map(
     da,
     ax=None,
     add_colorbar=True,
     interpolation="nearest",
-    fig_kwargs={},
+    fig_kwargs={}, 
     subplot_kwargs={},
     cbar_kwargs={},
     **plot_kwargs,
 ):
     """Plot DataArray 2D field with cartopy."""
     # Plot FacetGrid with xarray imshow
     if "col" in plot_kwargs or "row" in plot_kwargs:
         p = _plot_grid_map_facetgrid(
             da=da,
             ax=ax,
             add_colorbar=add_colorbar,
             interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             subplot_kwargs=subplot_kwargs,
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
-    # Plot with cartopy imshow
-    else:
+    # Plot with cartopy imshow 
+    else: 
         p = _plot_grid_map_cartopy(
             da=da,
             ax=ax,
             add_colorbar=add_colorbar,
             interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             subplot_kwargs=subplot_kwargs,
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
     # - Return mappable
     return p
 
 
 def plot_grid_image(
-    da,
-    ax=None,
+    da, ax=None,
     add_colorbar=True,
-    interpolation="nearest",
-    fig_kwargs={},
+    interpolation="nearest", 
+    fig_kwargs={}, 
     cbar_kwargs={},
     **plot_kwargs,
 ):
     """Plot DataArray 2D image."""
     # Check inputs
     # check_is_spatial_2d(da)
     _preprocess_figure_args(ax=ax, fig_kwargs=fig_kwargs)
-
+    
     # Initialize figure
     if ax is None:
-        # - If col and row are not provided (not FacetedGrid), initialize
+        # - If col and row are not provided (not FacetedGrid), initialize 
         if "col" not in plot_kwargs and "row" not in plot_kwargs:
             fig, ax = plt.subplots(**fig_kwargs)
         # Add fig_kwargs to plot_kwargs for FacetGrid initialization
-        else:
+        else: 
             plot_kwargs.update(fig_kwargs)
 
     # - If not specified, retrieve/update plot_kwargs and cbar_kwargs as function of product name
-    plot_kwargs, cbar_kwargs = get_colorbar_settings(
-        name=da.name, plot_kwargs=plot_kwargs, cbar_kwargs=cbar_kwargs
-    )
+    plot_kwargs, cbar_kwargs = get_colorbar_settings(name=da.name,
+                                                     plot_kwargs=plot_kwargs, 
+                                                     cbar_kwargs=cbar_kwargs)
 
     # # - Plot with matplotlib
     # p = _plot_mpl_imshow(ax=ax,
     #                      da=da,
     #                      x="lon",
     #                      y="lat",
     #                      interpolation=interpolation,
     #                      add_colorbar=add_colorbar,
     #                      plot_kwargs=plot_kwargs,
     #                      cbar_kwargs=cbar_kwargs,
     #                      ticklabels=ticklabels,
     # )
-
+    
     # - Plot with xarray
     p = _plot_xr_imshow(
         ax=ax,
         da=da,
         x="lon",
         y="lat",
         interpolation=interpolation,
```

### Comparing `gpm_api-0.2.2/gpm_api/visualization/labels.py` & `gpm_api-0.2.3/gpm_api/visualization/labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,153 +1,148 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Thu Jan 12 12:04:17 2023
 
 @author: ghiggi
 """
+import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-import numpy as np
-
 from gpm_api.patch.labels import redefine_label_array
-from gpm_api.patch.labels_patch import get_labeled_object_patches, labels_patch_generator
 from gpm_api.utils.checks import check_is_xarray_dataarray
+from gpm_api.patch.labels_patch import get_labeled_object_patches
+from gpm_api.patch.labels_patch import labels_patch_generator
 from gpm_api.visualization.plot import plot_image
 
 # TODO:
-# - gpm_api.plot_label
+# - gpm_api.plot_label 
 
 
 def get_label_colorbar_settings(label_indices, cmap="Paired"):
     """Return plot and cbar kwargs to plot properly a label array."""
     # Cast to int the label_indices
     label_indices = label_indices.astype(int)
-    # Compute number of required colors
+    # Compute number of required colors 
     n_labels = len(label_indices)
-
-    # Get colormap if string
-    if isinstance(cmap, str):
+    
+    # Get colormap if string 
+    if isinstance(cmap, str): 
         cmap = plt.get_cmap(cmap)
-
-    # Extract colors
+        
+    # Extract colors 
     color_list = [cmap(i) for i in range(cmap.N)]
-
+    
     # Create the new colormap
-    cmap_new = mpl.colors.LinearSegmentedColormap.from_list("Label Classes", color_list, n_labels)
+    cmap_new = mpl.colors.LinearSegmentedColormap.from_list(
+        'Label Classes', color_list, n_labels)
 
     # Define the bins and normalize
-    bounds = np.linspace(1, n_labels + 1, n_labels + 1)
+    bounds = np.linspace(1, n_labels+1, n_labels+1)
     norm = mpl.colors.BoundaryNorm(bounds, cmap_new.N)
-
-    # Define the plot kwargs
+    
+    # Define the plot kwargs 
     plot_kwargs = {}
-    plot_kwargs["cmap"] = cmap_new
-    plot_kwargs["norm"] = norm
-
-    # Define colorbar kwargs
+    plot_kwargs['cmap'] = cmap_new 
+    plot_kwargs['norm'] = norm 
+    
+    # Define colorbar kwargs 
     ticks = bounds[:-1] + 0.5
     ticklabels = label_indices
     assert len(ticks) == len(ticklabels)
     cbar_kwargs = {}
-    cbar_kwargs["label"] = "Label IDs"
-    cbar_kwargs["ticks"] = ticks
-    cbar_kwargs["ticklabels"] = ticklabels
+    cbar_kwargs['label'] = "Label IDs"
+    cbar_kwargs['ticks'] = ticks
+    cbar_kwargs['ticklabels'] = ticklabels 
     return plot_kwargs, cbar_kwargs
 
 
-def plot_label(
-    da, add_colorbar="True", interpolation="nearest", cmap="Paired", fig_kwargs={}, **plot_kwargs
-):
-    # Ensure array is numpy downstrema
+def plot_label(da, 
+               add_colorbar="True",
+               interpolation="nearest", 
+               cmap = "Paired",
+               fig_kwargs={},
+               **plot_kwargs):
+    # Ensure array is numpy downstrema 
     arr = da.data
     if hasattr(arr, "chunks"):
-        arr = arr.compute()
+        arr = arr.compute() 
     # Get label_indices and relabel array from 1 to ... for plotting
     label_indices = np.unique(arr)
     label_indices = np.delete(label_indices, np.where(label_indices == 0)[0].flatten())
     relabeled_arr = redefine_label_array(da.data, label_indices=label_indices)
     da_label = da.copy()
     da_label.data = relabeled_arr
     # Replace 0 with nan
     da_label = da_label.where(da_label > 0)
     # Define appropriate colormap
     plot_kwargs, cbar_kwargs = get_label_colorbar_settings(label_indices, cmap="Paired")
-    # Plot image
-    p = plot_image(
-        da_label,
-        interpolation=interpolation,
-        add_colorbar=add_colorbar,
-        cbar_kwargs=cbar_kwargs,
-        fig_kwargs=fig_kwargs,
-        **plot_kwargs,
-    )
+    # Plot image 
+    p = plot_image(da_label, interpolation=interpolation, add_colorbar=add_colorbar,
+                   cbar_kwargs = cbar_kwargs, fig_kwargs=fig_kwargs, **plot_kwargs)
     return p
 
 
-def plot_label_patches(
-    xr_obj,
-    label_name,
-    n_patches=None,
-    labels_id=None,
-    padding=None,
-    min_patch_size=None,
-    add_colorbar=True,
-    interpolation="nearest",
-    cmap="Paired",
-    fig_kwargs={},
-    **plot_kwargs,
-):
-
+def plot_label_patches(xr_obj, 
+                       label_name,
+                       n_patches=None,
+                       labels_id=None,
+                       padding=None, 
+                       min_patch_size=None,
+                       add_colorbar=True,
+                       interpolation="nearest", 
+                       cmap="Paired",
+                       fig_kwargs={},
+                       **plot_kwargs):
+    
     # Check plot_kwargs keys
-    if "cbar_kwargs" in plot_kwargs:
+    if "cbar_kwargs" in plot_kwargs: 
         raise ValueError("'cbar_kwargs' can not be specified when plotting labels.")
-
-    # Define the patch generator
+    
+    # Define the patch generator 
     patch_gen = get_labeled_object_patches(
-        xr_obj,
-        label_name=label_name,
+        xr_obj, 
+        label_name=label_name, 
         n_patches=n_patches,
         labels_id=labels_id,
         padding=padding,
-        min_patch_size=min_patch_size,
+        min_patch_size=min_patch_size, 
     )
     # Plot patches
     # list_da = list(patch_gen)
     # da = list_da[0]
     for da in patch_gen:
-        plot_label(
-            da[label_name],
-            add_colorbar=add_colorbar,
-            interpolation=interpolation,
-            cmap=cmap,
-            fig_kwargs=fig_kwargs,
-            **plot_kwargs,
-        )
+        p = plot_label(da[label_name], 
+                       add_colorbar=add_colorbar,
+                       interpolation=interpolation, 
+                       cmap = cmap,
+                       fig_kwargs=fig_kwargs,
+                       **plot_kwargs)
         plt.show()
-    return
+    return None
 
 
 # TODO: rename with something label_patches
-# - And modify previous function ?
+# - And modify previous function ?  
 # - add variable arguments and accept xarray object !
 def plot_patches(
     data_array,
     min_value_threshold=-np.inf,
     max_value_threshold=np.inf,
     min_area_threshold=1,
     max_area_threshold=np.inf,
     footprint=None,
     sort_by="area",
     sort_decreasing=True,
     n_patches=None,
     min_patch_size=None,
     padding=None,
-    add_colorbar=True,
+    add_colorbar=True, 
     interpolation="nearest",
-    fig_kwargs={},
+    fig_kwargs={}, 
     cbar_kwargs={},
     **plot_kwargs,
 ):
     check_is_xarray_dataarray(data_array)
 
     # Define generator
     gpm_da_patch_gen = labels_patch_generator(
@@ -163,20 +158,16 @@
         min_patch_size=min_patch_size,
         padding=padding,
     )
 
     # Plot patches
     for da in gpm_da_patch_gen:
         try:
-            plot_image(
-                da,
-                interpolation=interpolation,
-                add_colorbar=add_colorbar,
-                fig_kwargs=fig_kwargs,
-                cbar_kwargs=cbar_kwargs,
-                **plot_kwargs,
-            )
+            plot_image(da, interpolation=interpolation, add_colorbar=add_colorbar, 
+                       fig_kwargs=fig_kwargs, 
+                       cbar_kwargs=cbar_kwargs,
+                       **plot_kwargs)
             plt.show()
-        except:
+        except: 
             pass
 
-    return
+    return None
```

### Comparing `gpm_api-0.2.2/gpm_api/visualization/orbit.py` & `gpm_api-0.2.3/gpm_api/visualization/orbit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,69 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sat Dec 10 19:06:20 2022
 
 @author: ghiggi
 """
 import functools
-
+import numpy as np
 import cartopy.crs as ccrs
 import matplotlib.pyplot as plt
-import numpy as np
-
 from gpm_api.utils.checks import (
-    check_contiguous_scans,
     check_is_spatial_2d,
+    check_contiguous_scans,
     get_slices_regular,
 )
-from gpm_api.utils.utils_cmap import get_colorbar_settings
 from gpm_api.visualization.plot import (
+    plot_cartopy_background,
+    _preprocess_figure_args,
+    _preprocess_subplot_kwargs,
     _plot_cartopy_pcolormesh,
     #  _plot_mpl_imshow,
     _plot_xr_imshow,
-    _preprocess_figure_args,
-    _preprocess_subplot_kwargs,
-    plot_cartopy_background,
+    get_colorbar_settings,
 )
 
 
 def plot_swath_lines(ds, ax=None, **kwargs):
     """Plot GPM orbit granule swath lines."""
     # - 0.0485 to account for 2.5 km from pixel center
     # TODO: adapt based on bin length (changing for each sensor) --> FUNCTION
-
-    # - Initialize figure
-    subplot_kwargs = kwargs.get("subplot_kwargs", {})
-    fig_kwargs = kwargs.get("fig_kwargs", {})
-    if ax is None:
-        subplot_kwargs = _preprocess_subplot_kwargs(subplot_kwargs)
-        fig, ax = plt.subplots(subplot_kw=subplot_kwargs, **fig_kwargs)
-        # - Add cartopy background
-        ax = plot_cartopy_background(ax)
-
-    # - Plot swath line
     lon = ds["lon"].transpose("cross_track", "along_track").data
     lat = ds["lat"].transpose("cross_track", "along_track").data
     ax.plot(lon[0, :] + 0.0485, lat[0, :], transform=ccrs.Geodetic(), **kwargs)
     ax.plot(lon[-1, :] - 0.0485, lat[-1, :], transform=ccrs.Geodetic(), **kwargs)
 
     # ax.plot(da['lon'][:, 0] + 0.0485, da['lat'][:,0],'--k')
     # ax.plot(da['lon'][:,-1] - 0.0485, da['lat'][:,-1],'--k')
 
 
 def infill_invalid_coords(xr_obj):
     """Replace invalid coordinates with closer valid location.
-
+    
     It assumes that the invalid pixel variables are already masked to NaN.
     """
-    # TODO: unvalid pixel coordinates should be masked by full transparency !
-
+    # TODO: unvalid pixel coordinates should be masked by full transparency ! 
+    
     from gpm_api.utils.checks import _is_non_valid_geolocation
-
-    # Retrieve array indicated unvalid geolocation
+    # Retrieve array indicated unvalid geolocation 
     mask = _is_non_valid_geolocation(xr_obj).data
-    # Retrieve lon and lat array
+    # Retrieve lon and lat array 
     lon = xr_obj["lon"].data
     lat = xr_obj["lat"].data
-    # Replace unvalid coordinates with closer valid values
+    # Replace unvalid coordinates with closer valid values 
     lon_dummy = lon.copy()
     lon_dummy[mask] = np.interp(np.flatnonzero(mask), np.flatnonzero(~mask), lon[~mask])
     lat_dummy = lat.copy()
     lat_dummy[mask] = np.interp(np.flatnonzero(mask), np.flatnonzero(~mask), lat[~mask])
     xr_obj["lon"].data = lon_dummy
     xr_obj["lat"].data = lat_dummy
     return xr_obj
 
-
 # TODO: plot swath polygon
 # def plot_swath(ds, ax=None):
 
 # da.gpm_api.pyresample_area.boundary
 # da.gpm_api.pyresample_area.outer_boundary.polygon
 # da.gpm_api.pyresample_area.outer_boundary.sides ..
 
@@ -86,95 +72,102 @@
     """Decorator to call the plotting function multiple times only over contiguous scans intervals."""
 
     @functools.wraps(function)
     def wrapper(*args, **kwargs):
         # Assumption: only da and ax are passed as args
 
         # Get data array (first position)
-        da = args[0] if len(args) > 0 else kwargs.get("da")
+        if len(args) > 0:
+            da = args[0]
+        else:
+            da = kwargs.get("da")
         # Get axis
-        ax = args[1] if len(args) > 1 else kwargs.get("ax")
+        if len(args) > 1:
+            ax = args[1]
+        else:
+            ax = kwargs.get("ax")
 
         # - Check data array
         check_is_spatial_2d(da)
 
         # - Get slices with contiguous scans and valid geolocation
         list_slices = get_slices_regular(da)
         if len(list_slices) == 0:
             return ValueError("No regular scans available. Impossible to plot.")
 
         # - Define kwargs
         user_kwargs = kwargs.copy()
         p = None
-
+        
         # - Call the function over each slice
         for i, slc in enumerate(list_slices):
 
             # Retrive contiguous data array
             tmp_da = da.isel(along_track=slc)
-
+            
             # Replace invalid coordinate with closer value
-            # - This might be necessary for some products
-            #   having all the outer swath invalid coordinates
+            # - This might be necessary for some products 
+            #   having all the outer swath invalid coordinates 
             # tmp_da = infill_invalid_coords(tmp_da)
-
+         
             # Define  temporary kwargs
             tmp_kwargs = user_kwargs.copy()
             tmp_kwargs["da"] = tmp_da
             if i == 0:
                 tmp_kwargs["ax"] = ax
             else:
                 tmp_kwargs["ax"] = p.axes
 
             # Set colorbar to False for all except last iteration
             # --> Avoid drawing multiple colorbars
-            if i != len(list_slices) - 1 and "add_colorbar" in user_kwargs:
-                tmp_kwargs["add_colorbar"] = False
+            if i != len(list_slices) - 1:
+                if "add_colorbar" in user_kwargs:
+                    tmp_kwargs["add_colorbar"] = False
 
             # Before function call
             p = function(**tmp_kwargs)
 
         return p
 
     return wrapper
 
 
 @_call_over_contiguous_scans
 def plot_orbit_map(
-    da,
-    ax=None,
-    add_colorbar=True,
-    add_swath_lines=True,
-    fig_kwargs={},
+    da, ax=None,
+    add_colorbar=True, 
+    add_swath_lines=True, 
+    fig_kwargs={}, 
     subplot_kwargs={},
     cbar_kwargs={},
     **plot_kwargs,
 ):
     """Plot GPM orbit granule in a cartographic map."""
     # - Check inputs
     check_is_spatial_2d(da)
     _preprocess_figure_args(ax=ax, fig_kwargs=fig_kwargs, subplot_kwargs=subplot_kwargs)
 
+    
     # - Initialize figure
     if ax is None:
         subplot_kwargs = _preprocess_subplot_kwargs(subplot_kwargs)
         fig, ax = plt.subplots(subplot_kw=subplot_kwargs, **fig_kwargs)
         # - Add cartopy background
         ax = plot_cartopy_background(ax)
 
     # - If not specified, retrieve/update plot_kwargs and cbar_kwargs as function of variable name
     variable = da.name
-    plot_kwargs, cbar_kwargs = get_colorbar_settings(
-        name=variable, plot_kwargs=plot_kwargs, cbar_kwargs=cbar_kwargs
-    )
-    # - Specify colorbar label
-    if "label" not in cbar_kwargs:
-        unit = da.attrs.get("units", "-")
-        cbar_kwargs["label"] = f"{variable} [{unit}]"
-
+    plot_kwargs, cbar_kwargs = get_colorbar_settings(name=variable,
+                                                     plot_kwargs=plot_kwargs, 
+                                                     cbar_kwargs=cbar_kwargs)
+    # - Specify colorbar label 
+    if "label" not in cbar_kwargs: 
+        unit = da.attrs.get('units', "-")
+        cbar_kwargs['label'] = f"{variable} [{unit}]"
+    
     # - Add swath lines
     if add_swath_lines:
         plot_swath_lines(da, ax=ax, linestyle="--", color="black")
 
     # - Add variable field with cartopy
     p = _plot_cartopy_pcolormesh(
         ax=ax,
@@ -187,39 +180,36 @@
     )
     # - Return mappable
     return p
 
 
 @_call_over_contiguous_scans
 def plot_orbit_mesh(
-    da,
-    ax=None,
-    edgecolors="k",
-    linewidth=0.1,
-    fig_kwargs={},
+    da, ax=None, edgecolors="k", linewidth=0.1,
+    fig_kwargs={}, 
     subplot_kwargs={},
     **plot_kwargs,
 ):
     """Plot GPM orbit granule mesh in a cartographic map."""
     # - Check inputs
     check_is_spatial_2d(da)
     _preprocess_figure_args(ax=ax, fig_kwargs=fig_kwargs, subplot_kwargs=subplot_kwargs)
-
+    
     # - Initialize figure
     if ax is None:
         subplot_kwargs = _preprocess_subplot_kwargs(subplot_kwargs)
         fig, ax = plt.subplots(subplot_kw=subplot_kwargs, **fig_kwargs)
         # - Add cartopy background
         ax = plot_cartopy_background(ax)
 
     # - Define plot_kwargs to display only the mesh
     plot_kwargs["facecolor"] = "none"
     plot_kwargs["alpha"] = 1
-    plot_kwargs["edgecolors"] = (edgecolors,)
-    plot_kwargs["linewidth"] = (linewidth,)
+    plot_kwargs["edgecolors"] = edgecolors,
+    plot_kwargs["linewidth"] = linewidth,
     plot_kwargs["antialiased"] = True
     print(plot_kwargs)
     # - Add variable field with cartopy
     p = _plot_cartopy_pcolormesh(
         ax=ax,
         da=da,
         x="lon",
@@ -228,36 +218,35 @@
         add_colorbar=False,
     )
     # - Return mappable
     return p
 
 
 def plot_orbit_image(
-    da,
-    ax=None,
+    da, ax=None, 
     add_colorbar=True,
     interpolation="nearest",
-    fig_kwargs={},
+    fig_kwargs={}, 
     cbar_kwargs={},
     **plot_kwargs,
 ):
     """Plot GPM orbit granule as in image."""
     # - Check inputs
     check_is_spatial_2d(da)
     check_contiguous_scans(da)
     _preprocess_figure_args(ax=ax, fig_kwargs=fig_kwargs)
 
     # - Initialize figure
     if ax is None:
         fig, ax = plt.subplots(**fig_kwargs)
 
     # - If not specified, retrieve/update plot_kwargs and cbar_kwargs as function of product name
-    plot_kwargs, cbar_kwargs = get_colorbar_settings(
-        name=da.name, plot_kwargs=plot_kwargs, cbar_kwargs=cbar_kwargs
-    )
+    plot_kwargs, cbar_kwargs = get_colorbar_settings(name=da.name,
+                                                     plot_kwargs=plot_kwargs, 
+                                                     cbar_kwargs=cbar_kwargs)
 
     # # - Plot with matplotlib
     # p = _plot_mpl_imshow(ax=ax,
     #                      da=da,
     #                      x="along_track",
     #                      y="cross_track",
     #                      interpolation=interpolation,
```

### Comparing `gpm_api-0.2.2/gpm_api/visualization/plot.py` & `gpm_api-0.2.3/gpm_api/visualization/plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,112 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sat Dec 10 18:42:28 2022
 
 @author: ghiggi
 """
+import numpy as np
 import cartopy
 import cartopy.crs as ccrs
+import matplotlib as mpl
 import matplotlib.pyplot as plt
-import numpy as np
+from scipy.ndimage import binary_dilation
 from matplotlib.collections import PolyCollection
 from mpl_toolkits.axes_grid1 import make_axes_locatable
-from scipy.ndimage import binary_dilation
+from gpm_api.utils.utils_cmap import get_colormap_setting
+
 
 ### TODO: Add xarray + cartopy  (xr_carto) (xr_mpl)
 # _plot_cartopy_xr_imshow
 # _plot_cartopy_xr_pcolormesh
 
 
+# TODO: modify ticklabels in all get_colorbar_settings in  grid and orbit 
+# def get_colorbar_settings(name):
+#     # TODO: to customize as function of da.name
+#     plot_kwargs, cbar_kwargs, ticklabels = get_colormap_setting("pysteps_mm/hr")
+#     return (plot_kwargs, cbar_kwargs, ticklabels)
+
 def _preprocess_figure_args(ax, fig_kwargs={}, subplot_kwargs={}):
-    if ax is not None:
+    if ax is not None: 
         if len(subplot_kwargs) >= 1:
             raise ValueError("Provide `subplot_kwargs`only if `ax`is None")
         if len(fig_kwargs) >= 1:
-            raise ValueError("Provide `fig_kwargs` only if `ax`is None")
-
+            raise ValueError("Provide `fig_kwargs` only if `ax`is None") 
+    
     # If ax is not specified, specify the figure defaults
     # if ax is None:
-    # Set default figure size and dpi
-    # fig_kwargs['figsize'] = (12, 10)
-    # fig_kwargs['dpi'] = 100
-
+        # Set default figure size and dpi  
+        # fig_kwargs['figsize'] = (12, 10)
+        # fig_kwargs['dpi'] = 100
 
 def _preprocess_subplot_kwargs(subplot_kwargs):
     subplot_kwargs = subplot_kwargs.copy()
     if "projection" not in subplot_kwargs:
         subplot_kwargs["projection"] = ccrs.PlateCarree()
     return subplot_kwargs
+        
+
+def get_colorbar_settings(name, plot_kwargs={}, cbar_kwargs={}):
+    # TODO: to customize as function of da.name
+    try: 
+        default_plot_kwargs, default_cbar_kwargs, default_ticklabels = get_colormap_setting(name)
+        default_cbar_kwargs['ticklabels'] = None
+    except: 
+        default_plot_kwargs = {}
+        default_cbar_kwargs = {}
+        default_ticklabels = None # to be placed in cbar_kwargs
+        
+    # If the default is a segmented colormap (with ticks and ticklabels)
+    if default_cbar_kwargs.get("ticks", None) is not None:
+        # If specifying a custom vmin, vmax, norm or cmap args, remove  the defaults
+        # - The discrete colorbar makes no sense anymore
+        if np.any(np.isin(["vmin","vmax", "norm", "cmap"], list(plot_kwargs.keys()))):
+            default_cbar_kwargs.pop("ticks", None)
+            default_cbar_kwargs.pop("ticklabels", None)
+            default_plot_kwargs.pop("cmap", None)
+            default_plot_kwargs.pop("norm", None)
+            default_plot_kwargs.pop("vmin", None)
+            default_plot_kwargs.pop("vmax", None)
+    
+    # If cmap is a string, retrieve colormap 
+    if isinstance(plot_kwargs.get("cmap", None), str): 
+        plot_kwargs["cmap"] = plt.get_cmap(plot_kwargs["cmap"])
+                     
+    # Update defaults with custom kwargs 
+    default_plot_kwargs.update(plot_kwargs)
+    default_cbar_kwargs.update(cbar_kwargs)
+    
+    # Return the kwargs 
+    plot_kwargs = default_plot_kwargs
+    cbar_kwargs = default_cbar_kwargs
+    
+    # Remove vmin, vmax
+    # --> vmin and vmax is not accepted by PolyCollection 
+    # --> create norm or modify norm accordigly
+    norm = plot_kwargs.get("norm", None)
+    if norm is None:
+        norm = mpl.colors.Normalize(vmin=plot_kwargs.pop("vmin", None),
+                                    vmax=plot_kwargs.pop("vmax", None))
+        plot_kwargs["norm"] = norm 
+    else: 
+        if "vmin" in plot_kwargs: 
+            if plot_kwargs["vmin"] is None:
+                _ = plot_kwargs.pop("vmin")
+            else: 
+                plot_kwargs["norm"].vmin = plot_kwargs.pop("vmin")
+
+        if "vmax" in plot_kwargs: 
+            if plot_kwargs["vmax"] is None:
+                _ = plot_kwargs.pop("vmax")
+            else: 
+                plot_kwargs["norm"].vmax = plot_kwargs.pop("vmax")
+                
+    return (plot_kwargs, cbar_kwargs)
 
 
 def get_extent(da, x="lon", y="lat"):
     # TODO: compute corners array to estimate the extent
     # - OR increase by 1° in everydirection and then wrap between -180, 180,90,90
     # Get the minimum and maximum longitude and latitude values
     lon_min, lon_max = da[x].min(), da[x].max()
@@ -67,69 +134,66 @@
     mask[row_indices, col_indices] = 1
     # Buffer by 1 in all directions to ensure edges not crossing the antimeridian
     mask = binary_dilation(mask)
     return mask
 
 
 def get_masked_cells_polycollection(x, y, arr, mask, plot_kwargs):
-    from gpm_api.utils.area import _from_corners_to_bounds, _get_lonlat_corners, is_vertex_clockwise
-
+    from gpm_api.utils.area import _get_lonlat_corners, _from_corners_to_bounds, is_vertex_clockwise
+    
     # - Buffer mask by 1 to derive vertices of all masked QuadMesh
     mask = binary_dilation(mask)
-
-    # - Get index of masked quadmesh
+    
+    # - Get index of masked quadmesh 
     row_mask, col_mask = np.where(mask)
-
+    
     # - Retrieve values of masked cells
     array = arr[row_mask, col_mask]
-
+    
     # - Retrieve QuadMesh corners (m+1 x n+1)
     x_corners, y_corners = _get_lonlat_corners(x, y)
-
+    
     # - Retrieve QuadMesh bounds (m*n x 4)
     x_bounds = _from_corners_to_bounds(x_corners)
     y_bounds = _from_corners_to_bounds(y_corners)
-
+    
     # - Retrieve vertices of masked QuadMesh (n_masked, 4, 2)
     x_vertices = x_bounds[row_mask, col_mask]
     y_vertices = y_bounds[row_mask, col_mask]
-
+    
     vertices = np.stack((x_vertices, y_vertices), axis=2)
-
+    
     # Check that are counterclockwise oriented (check first vertex)
     # TODO: this check should be updated to use pyresample.future.spherical
     if is_vertex_clockwise(vertices[0, :, :]):
         vertices = vertices[:, ::-1, :]
-
-    # - Define additional kwargs for PolyCollection
+    
+    # - Define additional kwargs for PolyCollection 
     plot_kwargs = plot_kwargs.copy()
     if "edgecolors" not in plot_kwargs:
-        plot_kwargs["edgecolors"] = "face"  # 'none'
+        plot_kwargs["edgecolors"] = 'face' # 'none'
     if "linewidth" not in plot_kwargs:
         plot_kwargs["linewidth"] = 0
-    plot_kwargs["antialiaseds"] = False  # to better plotting quality
-
-    # - Define PolyCollection
-    coll = PolyCollection(
-        verts=vertices,
-        array=array,
-        transform=ccrs.Geodetic(),
-        **plot_kwargs,
-    )
+    plot_kwargs["antialiaseds"] = False # to better plotting quality  
+    
+    # - Define PolyCollection 
+    coll = PolyCollection(verts=vertices,
+                          array=array,
+                          transform=ccrs.Geodetic(),
+                          **plot_kwargs,
+                          )
     return coll
-
-
 ####--------------------------------------------------------------------------.
 def plot_cartopy_background(ax):
     """Plot cartopy background."""
     # - Add coastlines
     ax.coastlines()
     ax.add_feature(cartopy.feature.LAND, facecolor=[0.9, 0.9, 0.9])
     ax.add_feature(cartopy.feature.OCEAN, alpha=0.6)
-    ax.add_feature(cartopy.feature.BORDERS)  # BORDERS also draws provinces, ...
+    ax.add_feature(cartopy.feature.BORDERS) # BORDERS also draws provinces, ...
     # - Add grid lines
     gl = ax.gridlines(
         crs=ccrs.PlateCarree(),
         draw_labels=True,
         linewidth=1,
         color="gray",
         alpha=0.1,
@@ -153,36 +217,35 @@
     cax = divider.new_horizontal(size="5%", pad=0.1, axes_class=plt.Axes)
     p.figure.add_axes(cax)
     cbar = plt.colorbar(p, cax=cax, ax=ax, **cbar_kwargs)
     if ticklabels is not None:
         _ = cbar.ax.set_yticklabels(ticklabels)
     return cbar
 
-
 ####--------------------------------------------------------------------------.
 def _plot_cartopy_imshow(
     ax,
     da,
     x,
     y,
     interpolation="nearest",
-    add_colorbar=True,
+    add_colorbar=True, 
     plot_kwargs={},
     cbar_kwargs={},
 ):
     """Plot imshow with cartopy."""
     # - Ensure image with correct dimensions orders
     da = da.transpose(y, x)
     arr = da.data.compute()
 
     # - Derive extent
     extent = [-180, 180, -90, 90]  # TODO: Derive from data !!!!
-
-    # TODO: ensure y data is increasing --> origin = "lower"
-    # TODO: ensure y data is decreasing --> origin = "upper"
+    
+    # TODO: ensure y data is increasing --> origin = "lower" 
+    # TODO: ensure y data is decreasing --> origin = "upper" 
 
     # - Add variable field with cartopy
     p = ax.imshow(
         arr,
         transform=ccrs.PlateCarree(),
         extent=extent,
         origin="lower",
@@ -237,39 +300,41 @@
     p = ax.pcolormesh(
         x,
         y,
         arr,
         transform=ccrs.PlateCarree(),
         **plot_kwargs,
     )
-    # - Add PolyCollection of QuadMesh cells crossing the antimeridian
+    # - Add PolyCollection of QuadMesh cells crossing the antimeridian 
     if is_crossing_antimeridian:
-        coll = get_masked_cells_polycollection(x, y, arr.data, mask=mask, plot_kwargs=plot_kwargs)
+        coll = get_masked_cells_polycollection(x, y, arr.data,
+                                               mask=mask,
+                                               plot_kwargs=plot_kwargs)
         p.axes.add_collection(coll)
 
     # - Set the extent
     # --> To be set in projection coordinates of crs !!!
     #     lon/lat conversion to proj required !
     # extent = get_extent(da, x="lon", y="lat")
     # ax.set_extent(extent)
-
+    
     # - Add colorbar
     if add_colorbar:
         # --> TODO: set axis proportion in a meaningful way ...
         _ = plot_colorbar(p=p, ax=ax, cbar_kwargs=cbar_kwargs)
     return p
 
 
 def _plot_mpl_imshow(
     ax,
     da,
     x,
     y,
     interpolation="nearest",
-    add_colorbar=True,
+    add_colorbar=True, 
     plot_kwargs={},
     cbar_kwargs={},
 ):
     """Plot imshow with matplotlib."""
     # - Ensure image with correct dimensions orders
     da = da.transpose(y, x)
     arr = da.data.compute()
@@ -286,20 +351,17 @@
         # --> TODO: set axis proportion in a meaningful way ...
         _ = plot_colorbar(p=p, ax=ax, cbar_kwargs=cbar_kwargs)
     # - Return mappable
     return p
 
 
 def _plot_xr_imshow(
-    ax,
-    da,
-    x,
-    y,
+    ax, da, x, y,
     interpolation="nearest",
-    add_colorbar=True,
+    add_colorbar=True, 
     plot_kwargs={},
     cbar_kwargs={},
 ):
     """Plot imshow with xarray."""
     # --> BUG with colorbar: https://github.com/pydata/xarray/issues/7014
     ticklabels = cbar_kwargs.pop("ticklabels", None)
     p = da.plot.imshow(
@@ -317,123 +379,120 @@
 
 
 ####--------------------------------------------------------------------------.
 def plot_map(
     da,
     ax=None,
     add_colorbar=True,
-    add_swath_lines=True,  # used only for GPM orbit objects
-    interpolation="nearest",  # used only for GPM grid objects
-    fig_kwargs={},
+    add_swath_lines=True,    # used only for GPM orbit objects
+    interpolation="nearest", # used only for GPM grid objects
+    fig_kwargs={}, 
     subplot_kwargs={},
     cbar_kwargs={},
     **plot_kwargs,
 ):
 
-    from gpm_api.utils.geospatial import is_grid, is_orbit
-
+    from gpm_api.utils.geospatial import is_orbit, is_grid
     from .grid import plot_grid_map
     from .orbit import plot_orbit_map
-
     # Plot orbit
     if is_orbit(da):
         p = plot_orbit_map(
             da=da,
             ax=ax,
             add_colorbar=add_colorbar,
-            add_swath_lines=add_swath_lines,
-            fig_kwargs=fig_kwargs,
+            add_swath_lines=add_swath_lines, 
+            fig_kwargs=fig_kwargs, 
             subplot_kwargs=subplot_kwargs,
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
     # Plot grid
     elif is_grid(da):
         p = plot_grid_map(
             da=da,
             ax=ax,
             add_colorbar=add_colorbar,
             interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             subplot_kwargs=subplot_kwargs,
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
     else:
         raise ValueError("Can not plot. It's neither a GPM grid, neither a GPM orbit.")
     # Return mappable
     return p
 
 
 def plot_image(
-    da,
-    ax=None,
-    add_colorbar=True,
+    da, ax=None, 
+    add_colorbar=True, 
     interpolation="nearest",
-    fig_kwargs={},
+    fig_kwargs={}, 
     cbar_kwargs={},
     **plot_kwargs,
 ):
     # figsize, dpi, subplot_kw only used if ax is None
-    from gpm_api.utils.geospatial import is_grid, is_orbit
+    from gpm_api.utils.geospatial import is_orbit, is_grid
     from gpm_api.visualization.grid import plot_grid_image
     from gpm_api.visualization.orbit import plot_orbit_image
 
     # Plot orbit
     if is_orbit(da):
         p = plot_orbit_image(
             da=da,
             ax=ax,
             add_colorbar=add_colorbar,
             interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
     # Plot grid
     elif is_grid(da):
         p = plot_grid_image(
             da=da,
             ax=ax,
             add_colorbar=add_colorbar,
             interpolation=interpolation,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             cbar_kwargs=cbar_kwargs,
             **plot_kwargs,
         )
     else:
         raise ValueError("Can not plot. It's neither a GPM GRID, neither a GPM ORBIT.")
     # Return mappable
     return p
 
 
 def plot_map_mesh(
     da,
     ax=None,
     edgecolors="k",
     linewidth=0.1,
-    fig_kwargs={},
+    fig_kwargs={}, 
     subplot_kwargs={},
     **plot_kwargs,
 ):
     # Interpolation only for grid objects
     # figsize, dpi, subplot_kw only used if ax is None
-    from gpm_api.utils.geospatial import is_grid, is_orbit
+    from gpm_api.utils.geospatial import is_orbit, is_grid
 
     # from .grid import plot_grid_mesh
     from .orbit import plot_orbit_mesh
 
     # Plot orbit
     if is_orbit(da):
         p = plot_orbit_mesh(
             da=da,
             ax=ax,
             edgecolors=edgecolors,
             linewidth=linewidth,
-            fig_kwargs=fig_kwargs,
+            fig_kwargs=fig_kwargs, 
             subplot_kwargs=subplot_kwargs,
             **plot_kwargs,
         )
     # Plot grid
     elif is_grid(da):
         raise NotImplementedError("Not yet implemented.")
         #     p = plot_grid_mesh(
```

### Comparing `gpm_api-0.2.2/gpm_api/visualization/profile.py` & `gpm_api-0.2.3/gpm_api/visualization/profile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sat Dec 10 18:44:25 2022
 
 @author: ghiggi
 """
-import cartopy.crs as ccrs
-import numpy as np
 import pyproj
+import numpy as np
 import xarray as xr
-
+import cartopy.crs as ccrs
 from gpm_api.utils.slices import ensure_is_slice, get_slice_size
 from gpm_api.utils.utils_cmap import get_colormap_setting
 
 
 def optimize_transect_slices(
     obj, transect_slices, trim_threshold, variable=None, left_pad=0, right_pad=0
 ):
     # --------------------------------------------------------------------------.
     # Check variable
     # --> TODO: This can be removed under certain conditions
     # --> When trim_threshold become facultative
     # --> Left and right padding make sense only when trim_threshold is provided
     # TODO: Min_length, max_length arguments
     # --------------------------------------------------------------------------.
-    if isinstance(obj, xr.Dataset) and variable is None:
-        raise ValueError("If providing a xr.Dataset, 'variable' must be specified.")
+    if isinstance(obj, xr.Dataset):
+        if variable is None:
+            raise ValueError("If providing a xr.Dataset, 'variable' must be specified.")
 
     # --------------------------------------------------------------------------.
     # Check profile slice validity
     along_track_slice = ensure_is_slice(transect_slices["along_track"])
     cross_track_slice = ensure_is_slice(transect_slices["cross_track"])
     along_track_size = get_slice_size(along_track_slice)
     cross_track_size = get_slice_size(cross_track_slice)
     if along_track_size == 1 and cross_track_size == 1:
         raise ValueError("Both 'along_track' and 'cross_track' slices have size 1.")
     if along_track_size != 1 and cross_track_size != 1:
-        raise ValueError("Either 'along_track' or 'cross_track' must have a slice of size 1.")
+        raise ValueError(
+            "Either 'along_track' or 'cross_track' must have a slice of size 1."
+        )
     # --------------------------------------------------------------------------.
     # Get object transect
     obj_transect = obj.isel(transect_slices)
 
     # Retrieve transect dimension name
-    transect_dim_name = "cross_track" if along_track_size == 1 else "along_track"
+    if along_track_size == 1:
+        transect_dim_name = "cross_track"
+    else:
+        transect_dim_name = "along_track"
 
     # Transpose transect dimension to first dimension
     obj_transect = obj_transect.transpose(transect_dim_name, ...)
 
     # --------------------------------------------------------------------------.
     # If xr.Dataset, get a DataArray
     if isinstance(obj_transect, xr.Dataset):
@@ -59,19 +65,22 @@
     # --------------------------------------------------------------------------.
     # Identify transect extent including all pixel/profiles with value above threshold
     # - Transect line
     if ndim_transect == 1:
         idx_above_thr = np.where(obj_transect.data > trim_threshold)[0]
     else:  # 2D case (profile) or more ... (i.e. time or ensemble simulations)
         any_axis = tuple(np.arange(1, ndim_transect))
-        idx_above_thr = np.where(np.any(obj_transect.data > trim_threshold, axis=any_axis))[0]
+        idx_above_thr = np.where(
+            np.any(obj_transect.data > trim_threshold, axis=any_axis)
+        )[0]
 
     # --------------------------------------------------------------------------.
     # Check there are residual data along the transect
     if len(idx_above_thr) == 0:
+        trim_variable = obj_transect.name
         raise ValueError(
             "No {trim_variable} value above trim_threshold={trim_threshold}. Try to decrease it."
         )
     valid_idx = np.unique(idx_above_thr[[0, -1]])
 
     # --------------------------------------------------------------------------.
     # Padding the transect extent
@@ -120,32 +129,35 @@
     # - Valid dimensions # --> TODO: check for each Datarray
     dims = set(list(obj.dims))
     required_dims = set(["along_track", "cross_track", "range"])
     if not dims.issuperset(required_dims):
         raise ValueError(f"Requires xarray object with dimensions {required_dims}")
     # - Verifiy valid input combination
     # --> If input xr.Dataset and variable, lat and lon not specified, raise Error
-    if isinstance(obj, xr.Dataset) and lat is None and lon is None and variable is None:
-        raise ValueError(
-            "Need to provide 'variable' if passing a xr.Dataset and not specifying 'lat' / 'lon'."
-        )
+    if isinstance(obj, xr.Dataset):
+        if lat is None and lon is None and variable is None:
+            raise ValueError(
+                "Need to provide 'variable' if passing a xr.Dataset and not specifying 'lat' / 'lon'."
+            )
 
     # -------------------------------------------------------------------------.
     # If lon and lat are provided, derive center idx
     if lon is not None and lat is not None:
         # TODO: Get closest idx
         # idx_along_track
         # idx_cross_track
         raise NotImplementedError()
 
     # Else derive center locating the maximum intensity
     else:
         if isinstance(obj, xr.Dataset):
             if variable is None:
-                raise ValueError("If providing a xr.Dataset, 'variable' must be specified.")
+                raise ValueError(
+                    "If providing a xr.Dataset, 'variable' must be specified."
+                )
             da_variable = obj[variable].compute()
             obj[variable] = da_variable
         else:
             da_variable = obj.compute()
 
         dict_argmax = da_variable.argmax(da_variable.dims)
         idx_along_track = dict_argmax["along_track"]
@@ -173,15 +185,17 @@
     # Return transect slices
     return transect_slices
 
 
 def plot_profile(da_profile, colorscale=None, ylim=None, ax=None):
     x_direction = da_profile["lon"].dims[0]
     # Retrieve title
-    title = da_profile.gpm_api.title(time_idx=0, prefix_product=False, add_timestep=False)
+    title = da_profile.gpm_api.title(
+        time_idx=0, prefix_product=False, add_timestep=False
+    )
     # Retrieve colormap configs
     plot_kwargs, cbar_kwargs, ticklabels = get_colormap_setting(colorscale)
     # Plot
     p = da_profile.plot.pcolormesh(
         x=x_direction, y="height", ax=ax, cbar_kwargs=cbar_kwargs, **plot_kwargs
     )
     p.axes.set_title(title)
```

### Comparing `gpm_api-0.2.2/gpm_api/visualization/title.py` & `gpm_api-0.2.3/gpm_api/visualization/title.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 """
 Created on Sat Dec 10 18:50:02 2022
 
 @author: ghiggi
 """
 import numpy as np
 
@@ -124,15 +125,18 @@
 
     # Get variable name
     variable = da.name
     # Get product name
     product = da.attrs.get("gpm_api_product", "")
 
     # Create title string
-    title_str = product + " " + variable if prefix_product else da.name
+    if prefix_product:
+        title_str = product + " " + variable
+    else:
+        title_str = da.name
 
     # Make title in Capital Case
     title_str = " ".join([word[0].upper() + word[1:] for word in title_str.split(" ")])
 
     # Add time
     if add_timestep and (is_orbit(da) or da["time"].size == 1):
         time_str = get_time_str(
```

### Comparing `gpm_api-0.2.2/gpm_api.egg-info/PKG-INFO` & `gpm_api-0.2.3/gpm_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpm-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python API for the Global Precipitation Mission Data Archive
 Author-email: Gionata Ghiggi <gionata.ghiggi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2023 Gionata Ghiggi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,131 +53,133 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: image
 Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: tests
 License-File: LICENSE
 
 # Welcome to GPM-API
 [![DOI](https://zenodo.org/badge/286664485.svg)](https://zenodo.org/badge/latestdoi/286664485)
 [![PyPI version](https://badge.fury.io/py/gpm_api.svg)](https://badge.fury.io/py/gpm_api)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gpm_api.svg)](https://anaconda.org/conda-forge/gpm_api)
-[![Tests](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml/badge.svg)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml)
+[![Build Status](https://github.com/ghiggi/gpm_api/workflows/Continuous%20Integration/badge.svg?branch=main)](https://github.com/ghiggi/gpm_api/actions)
 [![Coverage Status](https://coveralls.io/repos/github/ghiggi/gpm_api/badge.svg?branch=main)](https://coveralls.io/github/ghiggi/gpm_api?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/gpm_api/badge/?version=latest)](https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/?badge=stable)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![License](https://img.shields.io/github/license/ghiggi/gpm_api)](https://github.com/ghiggi/gpm_api/blob/master/LICENSE)
 
 The GPM-API is still in development. Feel free to try it out and to report issues or to suggest changes.
 
 ## Quick start
-GPM-API provides an easy-to-use python interface to download, read, process and visualize most
-of the products of the Global Precipitation Measurement Mission (GPM) data archive.
+GPM-API provides an easy-to-use python interface to download, read, process and visualize most 
+of the products of the Global Precipitation Measurement Mission (GPM) data archive. 
 
-The list of available products can be retrieved using:
+The list of available products can be retrieved using: 
 
 ```python
 import gpm_api
 
 gpm_api.available_products(product_type="RS")  # research products
 gpm_api.available_products(product_type="NRT") # near-real-time products
 
 ```
 
-Before starting using GPM-API, we highly suggest to save into a configuration file:
-1. your credentials to access the [NASA Precipitation Processing System (PPS) servers][PPS_link]
-2. the directory on the local disk where to save the GPM dataset of interest.
+Before starting using GPM-API, we highly suggest to save into a configuration file: 
+1. your credentials to access the [NASA Precipitation Processing System (PPS) servers][PPS_link] 
+2. the directory on the local disk where to save the GPM dataset of interest. 
 
-To facilitate the creation of the configuration file, you can run the following script:
+To facilitate the creation of the configuration file, you can run the following script: 
 
 ```python
 import gpm_api
 
-username = "<your PPS username>" # likely your mail
-password = "<your PPS password>" # likely your mail
+username = "<your PPS username>" # likely your mail 
+password = "<your PPS password>" # likely your mail 
 gpm_base_dir = "<path/to/directory/GPM"  # path to the directory where to download the data
-gpm_api.define_configs(gpm_username=username,
-                       gpm_password=password,
+gpm_api.define_configs(gpm_username=username, 
+                       gpm_password=password, 
                        gpm_base_dir=gpm_base_dir)
 
 # You can check that the config file has been correctly created with:
 configs = gpm_api.read_configs()
 print(configs)
 
 ```
 
-Now you can either start to download GPM data within python:
+Now you can either start to download GPM data within python: 
 
 ```python
 import gpm_api
-import datetime
+import datetime 
 
 product = "2A-DPR"
 product_type = "RS"
 version = 7
 
 start_time = datetime.datetime(2020,7, 22, 0, 1, 11)
 end_time = datetime.datetime(2020,7, 22, 0, 23, 5)
 
-gpm_api.download(product=product,
+gpm_api.download(product=product, 
                  product_type=product_type,
                  version=version,
                  n_threads=2,
-                 start_time=start_time,
+                 start_time=start_time, 
                  end_time=end_time)
 
 ```
 
 or from the terminal using i.e. `download_daily_gpm_data <product> <year> <month> <day>`:
 
 ```bash
     download_daily_gpm_data 2A-DPR 2022 7 22
 ```
 
-A GPM granule can be opened in python using:
+A GPM granule can be opened in python using: 
 
 ```python
 import gpm_api
 
 ds = gpm_api.open_granule(<path_to_granule>)
 
 ```
 
-while multiple granules over a specific time period can be opened using:
+while multiple granules over a specific time period can be opened using: 
 
 ```python
 import gpm_api
-import datetime
+import datetime 
 
 product = "2A-DPR"
 product_type = "RS"
 version = 7
 
 start_time = datetime.datetime(2020,7, 22, 0, 1, 11)
 end_time = datetime.datetime(2020,7, 22, 0, 23, 5)
-ds = gpm_api.open_dataset(product=product,
+ds = gpm_api.open_dataset(product=product, 
                           product_type=product_type,
                           version=version
-                          start_time=start_time,
+                          start_time=start_time, 
                           end_time=end_time)
 ```
 
 Look at the [Tutorials][tutorial_link] to learn how to analyse and visualize the GPM products !
 
 ## Installation
 
 
 ### pip
 
 GPM-API can be installed via [pip][pip_link] on Linux, Mac, and Windows.
 On Windows you can install [WinPython][winpy_link] to get Python and pip
 running.
-Prior installation of GPM-API, to avoid [GEOS](https://libgeos.org/) library version incompatibilities when
+Prior installation of GPM-API, to avoid [GEOS](https://libgeos.org/) library version incompatibilities when 
 installing the Cartopy package, we highly suggest to install first Cartopy using `conda install cartopy>=0.21.0`.
 
 Then, install the GPM-API package by typing the following command in the command terminal:
 
     pip install gpm_api
 
 To install the latest development version via pip, see the
@@ -209,15 +211,15 @@
 - 2. Introduction to the PMW 2A products [[Notebook][tut2_pmw2a_link]][[Colab][colab2_pmw2a_link]]
 - 2. Introduction to the RADAR 2A products [[Notebook][tut2_radar_2a_link]][[Colab][colab2_radar_2a_link]]
 - 2. Introduction to the CORRA 2B products [[Notebook][tut2_corra_2b_link]][[Colab][colab2_corra_2b_link]]
 - 2. Introduction to the Latent Heating products [[Notebook][tut2_lh_link]][[Colab][colab2_lh_link]]
 - 2. Introduction to the ENVironment products [[Notebook][tut2_env_link]][[Colab][colab2_env_link]]
 - 3. Introduction to image labeling and patch extraction [[Notebook][tut3_label_link]][[Colab][colab3_label_link]]
 - 3. Introduction to image patch extraction [[Notebook][tut3_patch_link]][[Colab][colab3_patch_link]]
-
+ 
 The associated python scripts are also provided in the `tutorial` folder.
 
 ## Citation
 
 If you are using GPM-API in your publication please cite our paper:
 
 TODO: GMD
@@ -242,26 +244,29 @@
 
 - [zarr](https://zarr.readthedocs.io/en/stable/)
 - [dask_image](https://image.dask.org/en/latest/)
 - [skimage](https://scikit-image.org/)
 
 ## License
 
-The content of this repository is released under the terms of the [MIT](LICENSE) license.
+[MIT][license_link] © 2021-2023
+
 
 [PPS_link]: https://gpm.nasa.gov/data/sources/pps-research
 [tutorial_link]: https://github.com/ghiggi/gpm_api/tree/master#tutorials-and-examples
 
 [pip_link]: https://pypi.org/project/gstools
 [conda_link]: https://docs.conda.io/en/latest/miniconda.html
 [conda_forge_link]: https://github.com/conda-forge/gpm_api-feedstock#installing-gpm_api
 [conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
 [pipiflag]: https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html?highlight=i#cmdoption-i
 [winpy_link]: https://winpython.github.io/
 
+[license_link]: https://github.com/ghiggi/gpm_api/blob/main/LICENSE
+ 
 [doc_link]: https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/
 [doc_install_link]: https://gpm_api.readthedocs.io/projects/gpm_api/en/stable/#pip
 
 [tut1_download_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab1_download_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut2_imerg_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
@@ -286,7 +291,9 @@
 [colab2_env_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut3_label_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab3_label_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 
 [tut3_patch_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
 [colab3_patch_link]: https://github.com/ghiggi/gpm_api/tree/master/tutorials
+ 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpm_api-0.2.2/gpm_api.egg-info/SOURCES.txt` & `gpm_api-0.2.3/gpm_api.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+.flake8
 .gitignore
 .pre-commit-config.yaml
+.prospector.yaml
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CITATION.bib
 LICENSE
 MANIFEST.in
 README.md
@@ -16,22 +18,16 @@
 gpm_api.egg-info/SOURCES.txt
 gpm_api.egg-info/dependency_links.txt
 gpm_api.egg-info/entry_points.txt
 gpm_api.egg-info/requires.txt
 gpm_api.egg-info/top_level.txt
 gpm_api/accessor/__init__.py
 gpm_api/accessor/methods.py
-gpm_api/bucket/__init__.py
-gpm_api/bucket/utils.py
-gpm_api/dataset/attrs.py
-gpm_api/dataset/coords.py
 gpm_api/dataset/crs.py
 gpm_api/dataset/decoding.py
-gpm_api/dataset/dimensions.py
-gpm_api/dataset/group.py
 gpm_api/dataset/reader.py
 gpm_api/etc/__init__.py
 gpm_api/etc/country_acronyms.yaml
 gpm_api/etc/country_bounds.yaml
 gpm_api/etc/country_extent.yaml
 gpm_api/io/__init__.py
 gpm_api/io/checks.py
```

### Comparing `gpm_api-0.2.2/pyproject.toml` & `gpm_api-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -28,44 +28,44 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
-    "Topic :: Scientific/Engineering :: GIS",
+    "Topic :: Scientific/Engineering :: GIS", 
     "Topic :: Scientific/Engineering :: Hydrology",
-    "Topic :: Scientific/Engineering :: Image Processing",
+    "Topic :: Scientific/Engineering :: Image Processing", 
 ]
 keywords = ["GPM", "Precipitation", "API", "DPR", "PMW", "IMERG"]
 dependencies = [
     "xarray",
-    "h5py",
+    "h5py", 
     "netcdf4",
-    "dask",
+    "dask", 
     "pyresample",
     "trollsift",
     "cartopy>=0.20.0",  # should be installed with conda to avoid GEOS compatibility issues.
      # "curl", can be installed with conda.  Make it optional in the code.
     "wget",
     "tqdm",
-    "click",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
 
 [project.optional-dependencies]
 image = ["dask-image", "scikit-image"]
-dev = ["pre-commit",
-       "black", "black[jupyter]", "blackdoc", "ruff",
-       "pytest", "pytest-cov", "pytest-mock", "pydantic",
+dev = ["pre-commit", "black", "isort", "flake8", 
+       "pytest", "pytest-cov", 
        "pip-tools", "bumpver", "twine",
        "setuptools>=61.0.0", "wheel",
        "dask-image", "scikit-image",
-       "sphinx", "sphinx-gallery", "sphinx_rtd_theme", "nbsphinx"]
+       "sphinx", "sphinx-gallery", "nbsphinx"]
+doc = ["sphinx", "sphinx-gallery", "nbsphinx"] # sphinx-rtd-theme numpydoc pandodc
+tests = ["pre-commit", "pytest", "pytest-cov"]
 
 [project.urls]
 Homepage = "https://github.com/ghiggi/gpm_api"
 Source = "https://github.com/ghiggi/gpm_api"
 Tracker = "https://github.com/ghiggi/gpm_api/issues"
 Documentation = "https://gpm_api.readthedocs.io"
 changelog = "https://github.com/ghigg/gpm_api/CHANGELOG.md"
@@ -82,78 +82,82 @@
 # where = ["gpm_api"]
 # include = ["io", "..."]
 
 [project.scripts]
 download_daily_gpm_data="gpm_api.scripts.download_daily_gpm_data:download_daily_gpm_data"
 download_monthly_gpm_data="gpm_api.scripts.download_monthly_gpm_data:download_monthly_gpm_data"
 
+[tool.isort]
+profile = "black"
+skip_gitignore = true
+multi_line_output = 3
+line_length = 100
+skip = [".tox", ".venv", "build", "dist"]
+
 [tool.black]
 line-length = 100
 # skip-string-normalization = true
 target-version = [
     "py37",
     "py38",
     "py39",
     "py310",
     "py311",
 ]
 
-[tool.ruff]
-select = ["F",
-	  "E",
-	  "I",
-	  "W",
-	  "UP",
-	  "Q",
-	  # "SIM",
-	  # "PTH",
-	  #"RET",
-	 ]
-ignore = ["E722"]
-line-length = 120
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
-unfixable = []
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    "dev*",
-    "gpm_api/test*",
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-]
+[tool.pylint]
+    [tool.pylint.main]
+    extension-pkg-whitelist = [
+        "numpy",
+        "scipy",
+    ]
+    ignore = "_version.py"
+    load-plugins = [
+        "pylint.extensions.no_self_use",
+    ]
 
+    [tool.pylint.message_control]
+    disable = [
+        "R0801",
+    ]
+
+    [tool.pylint.reports]
+    output-format = "colorized"
+
+    [tool.pylint.design]
+    max-args = 20
+    max-locals = 50
+    max-branches = 30
+    max-statements = 80
+    max-attributes = 25
+    max-public-methods = 75
 
 [tool.coverage]
     [tool.coverage.run]
     source = ["gpm_api"]
     omit = [
         "*dev*",
         "*docs*",
         "*tutorials*",
-        "*/gpm_api/tests*",
+        "*tests*",
         "*/gpm_api/cli*",
+        "*/gpm_api/0_OLD*",
+        # "*/gpm_api/custom_script.py",
     ]
 
     [tool.coverage.report]
     exclude_lines = [
         "pragma: no cover",
         "def __repr__",
         "def __str__",
     ]
+
+
+
+
+
+
+
+ 
+   
+
+
```

