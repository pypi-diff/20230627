# Comparing `tmp/dcnum-0.11.0.tar.gz` & `tmp/dcnum-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.11.0.tar", last modified: Mon Jun 26 15:14:13 2023, max compression
+gzip compressed data, was "dcnum-0.11.1.tar", last modified: Tue Jun 27 08:33:45 2023, max compression
```

## Comparing `dcnum-0.11.0.tar` & `dcnum-0.11.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.142020 dcnum-0.11.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.130020 dcnum-0.11.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-26 15:14:04.000000 dcnum-0.11.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-26 15:14:04.000000 dcnum-0.11.0/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-26 15:14:04.000000 dcnum-0.11.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 15:14:04.000000 dcnum-0.11.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-26 15:14:04.000000 dcnum-0.11.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 15:14:04.000000 dcnum-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 15:14:13.142020 dcnum-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-26 15:14:04.000000 dcnum-0.11.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-26 15:14:04.000000 dcnum-0.11.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-26 15:14:04.000000 dcnum-0.11.0/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 15:14:04.000000 dcnum-0.11.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 15:14:04.000000 dcnum-0.11.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-26 15:14:04.000000 dcnum-0.11.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:14:13.142020 dcnum-0.11.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.142020 dcnum-0.11.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.502594 dcnum-0.11.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.490594 dcnum-0.11.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-27 08:33:36.000000 dcnum-0.11.1/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-27 08:33:36.000000 dcnum-0.11.1/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-27 08:33:36.000000 dcnum-0.11.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 08:33:36.000000 dcnum-0.11.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-27 08:33:36.000000 dcnum-0.11.1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 08:33:36.000000 dcnum-0.11.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-27 08:33:45.502594 dcnum-0.11.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-27 08:33:36.000000 dcnum-0.11.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-27 08:33:36.000000 dcnum-0.11.1/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.494594 dcnum-0.11.1/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 08:33:45.000000 dcnum-0.11.1/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-27 08:33:36.000000 dcnum-0.11.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.498594 dcnum-0.11.1/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-27 08:33:36.000000 dcnum-0.11.1/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-27 08:33:36.000000 dcnum-0.11.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-27 08:33:36.000000 dcnum-0.11.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-27 08:33:36.000000 dcnum-0.11.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:33:45.502594 dcnum-0.11.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.502594 dcnum-0.11.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:33:45.502594 dcnum-0.11.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-27 08:33:36.000000 dcnum-0.11.1/tests/test_write_writer.py
```

### Comparing `dcnum-0.11.0/.github/workflows/check.yml` & `dcnum-0.11.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/.github/workflows/deploy_pypi.yml` & `dcnum-0.11.1/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/.gitignore` & `dcnum-0.11.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/CHANGELOG` & `dcnum-0.11.1/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.11.1
+ - fix: fix GPUSegmenter labeling
 0.11.0
  - feat: introduce GPUSegmenter base class
  - fix: handle bytes-values in HDF5 attributes
  - ref: correctly introduce `requires_background_correction` for segmenters
  - setup: don't requrie cibuildwheel
 0.10.0
  - enh: some minor improvements in efficiency
```

### Comparing `dcnum-0.11.0/LICENSE` & `dcnum-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/PKG-INFO` & `dcnum-0.11.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.0
+Version: 0.11.1
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.0/README.rst` & `dcnum-0.11.1/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.11.1/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/feat_background/base.py` & `dcnum-0.11.1/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.11.1/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.11.1/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.11.1/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.11.1/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.11.1/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/gate.py` & `dcnum-0.11.1/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/feat/queue_event_extractor.py` & `dcnum-0.11.1/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/meta/ppid.py` & `dcnum-0.11.1/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/read/cache.py` & `dcnum-0.11.1/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/read/hdf5_data.py` & `dcnum-0.11.1/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/segm/segm_thresh.py` & `dcnum-0.11.1/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/segm/segmenter.py` & `dcnum-0.11.1/dcnum/segm/segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,17 @@
             #    footprint=morphology.disk(closing_disk),
             #    out=mask)
             #
             element = Segmenter.get_disk(closing_disk)
             labels_uint8 = np.array(labels, dtype=np.uint8)
             labels_dilated = cv2.dilate(labels_uint8, element)
             labels_eroded = cv2.erode(labels_dilated, element)
-            labels, _ = ndi.label(labels_eroded > 0)
+            labels, _ = ndi.label(
+                input=labels_eroded > 0,
+                structure=ndi.generate_binary_structure(2, 2))
 
         if fill_holes:
             # Floodfill only works with uint8 (too small) or int32
             if not labels.dtype == np.int32:
                 labels = np.array(labels, dtype=np.int32)
             #
             # from scipy import ndimage
@@ -202,15 +204,15 @@
     def segment_frame(self, image):
         """Return the integer label image for `index`"""
         segm_wrap = self.segment_frame_wrapper()
         # obtain mask or label
         mol = segm_wrap(image)
         if mol.dtype == bool:
             # convert mask to label
-            labels, num_labels = ndi.label(
+            labels, _ = ndi.label(
                 input=mol,
                 structure=ndi.generate_binary_structure(2, 2))
         else:
             labels = mol
         # optional postprocessing
         if self.mask_postprocessing:
             labels = self.process_mask(labels, **self.kwargs_mask)
```

### Comparing `dcnum-0.11.0/dcnum/segm/segmenter_cpu.py` & `dcnum-0.11.1/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/segm/segmenter_gpu.py` & `dcnum-0.11.1/dcnum/segm/segmenter_gpu.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import abc
 import pathlib
 
 import numpy as np
+import scipy.ndimage as ndi
 
 
 from .segmenter import Segmenter
 
 
 class GPUSegmenter(Segmenter, abc.ABC):
     mask_postprocessing = False
 
-    def __init__(self, model_file, *args, **kwargs):
+    def __init__(self, model_file=None, *args, **kwargs):
         super(GPUSegmenter, self).__init__(*args, **kwargs)
         self.model_path = self._get_model_path(model_file)
 
     @staticmethod
     def _get_model_path(model_file):
         """Custom hook that may be defined by subclasses"""
         return pathlib.Path(model_file)
@@ -24,10 +25,22 @@
                       start: int = None,
                       stop: int = None):
         if stop is None or start is None:
             start = 0
             stop = len(image_data)
 
         image_slice = image_data[start:stop]
-        segm = self.segment_frame_wrapper(self.model_path)
+        segm = self.segment_frame_wrapper()
 
-        return segm(image_slice)
+        labels = segm(image_slice)
+
+        # Make sure we have integer labels
+        if labels.dtype == bool:
+            new_labels = np.zeros_like(labels, dtype=np.uint16)
+            for ii in range(len(labels)):
+                ndi.label(
+                    input=labels[ii],
+                    output=new_labels[ii],
+                    structure=ndi.generate_binary_structure(2, 2))
+            labels = new_labels
+
+        return labels
```

### Comparing `dcnum-0.11.0/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.11.1/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/write/deque_writer_thread.py` & `dcnum-0.11.1/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/write/queue_collector_thread.py` & `dcnum-0.11.1/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum/write/writer.py` & `dcnum-0.11.1/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/dcnum.egg-info/PKG-INFO` & `dcnum-0.11.1/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.0
+Version: 0.11.1
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.0/dcnum.egg-info/SOURCES.txt` & `dcnum-0.11.1/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/docs/conf.py` & `dcnum-0.11.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/docs/extensions/github_changelog.py` & `dcnum-0.11.1/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/pyproject.toml` & `dcnum-0.11.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.11.1/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.11.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/helper_methods.py` & `dcnum-0.11.1/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.11.1/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_feat_brightness.py` & `dcnum-0.11.1/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_feat_haralick.py` & `dcnum-0.11.1/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_feat_moments_based.py` & `dcnum-0.11.1/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_ppid.py` & `dcnum-0.11.1/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_read_concat_hdf5.py` & `dcnum-0.11.1/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_read_hdf5.py` & `dcnum-0.11.1/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_segm_thresh.py` & `dcnum-0.11.1/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_write_deque_writer_thread.py` & `dcnum-0.11.1/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.0/tests/test_write_writer.py` & `dcnum-0.11.1/tests/test_write_writer.py`

 * *Files identical despite different names*

