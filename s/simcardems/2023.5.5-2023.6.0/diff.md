# Comparing `tmp/simcardems-2023.5.5.tar.gz` & `tmp/simcardems-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simcardems-2023.5.5.tar", last modified: Mon Jun  5 10:52:52 2023, max compression
+gzip compressed data, was "simcardems-2023.6.0.tar", last modified: Tue Jun 27 12:52:36 2023, max compression
```

## Comparing `simcardems-2023.5.5.tar` & `simcardems-2023.6.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.997527 simcardems-2023.5.5/
--rw-r--r--   0 root         (0) root         (0)    26526 2023-06-05 10:34:58.000000 simcardems-2023.5.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3845 2023-06-05 10:52:51.997527 simcardems-2023.5.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3141 2023-06-05 10:34:58.000000 simcardems-2023.5.5/README.md
--rw-r--r--   0 root         (0) root         (0)     1831 2023-06-05 10:52:51.997527 simcardems-2023.5.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-05 10:34:58.000000 simcardems-2023.5.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.981526 simcardems-2023.5.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems/
--rw-r--r--   0 root         (0) root         (0)     3453 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/__main__.py
--rw-r--r--   0 root         (0) root         (0)    10005 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     5423 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     9241 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/cli.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/config.py
--rw-r--r--   0 root         (0) root         (0)    18669 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/datacollector.py
--rw-r--r--   0 root         (0) root         (0)    10019 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/ep_model.py
--rw-r--r--   0 root         (0) root         (0)    17148 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/geometry.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/gui.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/lvgeometry.py
--rw-r--r--   0 root         (0) root         (0)    11482 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/mechanics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems/models/
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      819 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60760 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    14164 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6993 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    60344 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    12046 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.993527 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/
--rw-r--r--   0 root         (0) root         (0)      559 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    70634 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    12043 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.993527 simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      419 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60636 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
--rw-r--r--   0 root         (0) root         (0)     5730 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/newton_solver.py
--rw-r--r--   0 root         (0) root         (0)    21900 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/postprocess.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/runner.py
--rw-r--r--   0 root         (0) root         (0)     6485 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/save_load_functions.py
--rw-r--r--   0 root         (0) root         (0)     4515 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/slabgeometry.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/time_stepper.py
--rw-r--r--   0 root         (0) root         (0)     5462 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/utils.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/value_extractor.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3845 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2052 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:35:22.000000 simcardems-2023.5.5/src/simcardems.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      337 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.997527 simcardems-2023.5.5/tests/
--rw-r--r--   0 root         (0) root         (0)      523 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_datacollector.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_mechanics_model.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_postprocessing.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_save_load_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.765539 simcardems-2023.6.0/
+-rw-r--r--   0 root         (0) root         (0)    26526 2023-06-27 12:42:52.000000 simcardems-2023.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-06-27 12:52:36.765539 simcardems-2023.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-27 12:42:52.000000 simcardems-2023.6.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-06-27 12:52:36.769539 simcardems-2023.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-27 12:42:52.000000 simcardems-2023.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.757539 simcardems-2023.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.761539 simcardems-2023.6.0/src/simcardems/
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    10005 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     9241 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/config.py
+-rw-r--r--   0 root         (0) root         (0)    21808 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/datacollector.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/ep_model.py
+-rw-r--r--   0 root         (0) root         (0)    17227 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/geometry.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/gui.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/lvgeometry.py
+-rw-r--r--   0 root         (0) root         (0)    11482 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/mechanics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.761539 simcardems-2023.6.0/src/simcardems/models/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.765539 simcardems-2023.6.0/src/simcardems/models/explicit_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60760 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    14203 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.765539 simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6993 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    60344 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12085 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.765539 simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    70634 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12082 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.765539 simcardems-2023.6.0/src/simcardems/models/pureEP_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60636 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/newton_solver.py
+-rw-r--r--   0 root         (0) root         (0)    21900 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)     7218 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6860 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/save_load_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4515 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/slabgeometry.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/time_stepper.py
+-rw-r--r--   0 root         (0) root         (0)     5486 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/value_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-27 12:42:52.000000 simcardems-2023.6.0/src/simcardems/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.761539 simcardems-2023.6.0/src/simcardems.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-06-27 12:52:36.000000 simcardems-2023.6.0/src/simcardems.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-06-27 12:52:36.000000 simcardems-2023.6.0/src/simcardems.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 12:52:36.000000 simcardems-2023.6.0/src/simcardems.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-27 12:52:36.000000 simcardems-2023.6.0/src/simcardems.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 12:43:15.000000 simcardems-2023.6.0/src/simcardems.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      337 2023-06-27 12:52:36.000000 simcardems-2023.6.0/src/simcardems.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-27 12:52:36.000000 simcardems-2023.6.0/src/simcardems.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:52:36.765539 simcardems-2023.6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_datacollector.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_mechanics_model.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_postprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-27 12:42:52.000000 simcardems-2023.6.0/tests/test_save_load_functions.py
```

### Comparing `simcardems-2023.5.5/LICENSE` & `simcardems-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/PKG-INFO` & `simcardems-2023.6.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1
-Name: simcardems
-Version: 2023.5.5
-Summary: Simula Cardiac electromechanics solver
-Home-page: https://github.com/ComputationalPhysiology/simcardems
-Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
-Author-email: henriknf@simula.no
-License: LGPL-2.1
-Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: gui
-License-File: LICENSE
-
 [![CI](https://github.com/ComputationalPhysiology/simcardems/actions/workflows/main.yml/badge.svg)](https://github.com/ComputationalPhysiology/simcardems/actions/workflows/main.yml)
 [![PyPI version](https://badge.fury.io/py/simcardems.svg)](https://badge.fury.io/py/simcardems)
-[![codecov](https://codecov.io/gh/ComputationalPhysiology/simcardems/branch/main/graph/badge.svg?token=V5DOQ1PUVF)](https://codecov.io/gh/ComputationalPhysiology/simcardems)
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/simcardems-coverage.json)](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/simcardems-coverage.json)
 [![github pages](https://github.com/ComputationalPhysiology/simcardems/actions/workflows/github-pages.yml/badge.svg)](https://github.com/ComputationalPhysiology/simcardems/actions/workflows/github-pages.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComputationalPhysiology/simcardems/main.svg)](https://results.pre-commit.ci/latest/github/ComputationalPhysiology/simcardems/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v2.1-blue.svg)](https://www.gnu.org/licenses/lgpl-2.1)
 [![DOI](https://zenodo.org/badge/409220068.svg)](https://zenodo.org/badge/latestdoi/409220068)
 [![status](https://joss.theoj.org/papers/28986461c27b8a76c8ac5a43dc57e8dc/status.svg)](https://joss.theoj.org/papers/28986461c27b8a76c8ac5a43dc57e8dc)
```

### Comparing `simcardems-2023.5.5/setup.cfg` & `simcardems-2023.6.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = Simula Cardiac electromechanics solver
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ComputationalPhysiology/simcardems
 author = Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 author_email = henriknf@simula.no
 license = LGPL-2.1
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 keywords = action potential, cardiac mechanics, electrophysiology, electromechanics
 
 [options]
```

### Comparing `simcardems-2023.5.5/src/simcardems/__init__.py` & `simcardems-2023.6.0/src/simcardems/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,47 +35,29 @@
 from .runner import TimeStepper
 from .version import __version__
 
 
 def set_log_level(level):
     from daiquiri import set_default_log_levels
 
-    loggers = [
-        "simcardems.benchmark.logger"
-        "simcardems.boundary_conditions.logger"
-        "simcardems.cli.logger"
-        "simcardems.config.logger"
-        "simcardems.datacollector.logger"
-        "simcardems.ep_model.logger"
-        "simcardems.geometry.logger"
-        "simcardems.gui.logger"
-        "simcardems.mechanics_model.logger"
-        "simcardems.newton_solver.logger"
-        "simcardems.postprocess.logger"
-        "simcardems.save_load_functions.logger"
-        "simcardems.runner.logger"
-        "simcardems.utils.logger"
-        "simcardems.value_extractor.logger",
-        "simcardems.slabgeometry.logger",
-    ] + models.loggers
     _pulse.set_log_level(level)
     _daiquiri.setup(level=level)
 
     if level < _logging.INFO:
         # Turn on INFO for dolfin
         _dolfin.set_log_level(_logging.INFO)
 
     # If debug level turn on more logging
     if level < _logging.DEBUG:
         _dolfin.set_log_level(_logging.DEBUG)
         for module in ["FFC", "UFL"]:
             _logger = _logging.getLogger(module)
             _logger.setLevel(_logging.INFO)
 
-    set_default_log_levels((logger, level) for logger in loggers)
+    set_default_log_levels([("simcardems", level)])
 
 
 set_log_level(_logging.INFO)
 
 _dolfin.set_log_level(_logging.WARNING)
 for module in ["matplotlib", "h5py", "FFC", "UFL"]:
     _logger = _logging.getLogger(module)
@@ -114,8 +96,9 @@
     "TimeStepper",
     "lvgeometry",
     "newton_solver",
     "MechanicsNewtonSolver_ODE",
     "MechanicsNewtonSolver",
     "config",
     "Config",
+    "models",
 ]
```

### Comparing `simcardems-2023.5.5/src/simcardems/benchmark.py` & `simcardems-2023.6.0/src/simcardems/benchmark.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/boundary_conditions.py` & `simcardems-2023.6.0/src/simcardems/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/cli.py` & `simcardems-2023.6.0/src/simcardems/cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/config.py` & `simcardems-2023.6.0/src/simcardems/config.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/datacollector.py` & `simcardems-2023.6.0/src/simcardems/datacollector.py`

 * *Files 11% similar despite different names*

```diff
@@ -200,48 +200,67 @@
         outdir,
         geo: BaseGeometry,
         outfilename: str = "results.h5",
         reset_state=True,
     ) -> None:
         self.outdir = Path(outdir)
         self._results_file = self.outdir / outfilename
-        self.comm = geo.mesh.mpi_comm()  # FIXME: Is this important?
+        self.comm = geo.mesh.mpi_comm()
+
         self._value_extractor = ValueExtractor(geo)
 
+        file_exist = False
         if reset_state:
-            utils.remove_file(self._results_file)
+            logger.debug("Reset state")
+            utils.remove_file(self._results_file, comm=self.comm)
+
+        else:
+            dolfin.MPI.barrier(self.comm)
+            if self.comm.rank == 0:
+                file_exist = self._results_file.is_file()
+            file_exist = self.comm.bcast(file_exist, root=0)
+            dolfin.MPI.barrier(self.comm)
 
         self._times_stamps = set()
-        if not self._results_file.is_file():
+        logger.debug(f"File {self._results_file} exists: {file_exist}")
+        if not file_exist:
+            logger.debug("Dump geometry")
             geo.dump(self.results_file)
+            logger.debug("Done with dumping geometry")
             from . import __version__
             from packaging.version import parse
 
             version = parse(__version__)
 
-            with h5pyfile(self._results_file, "a") as f:
-                f.create_dataset("version_major", data=version.major)
-                f.create_dataset("version_minor", data=version.minor)
-                f.create_dataset("version_micro", data=version.micro)
+            if self.comm.rank == 0:
+                with h5pyfile(self._results_file, "a", force_serial=True) as f:
+                    f.create_dataset("version_major", data=version.major)
+                    f.create_dataset("version_minor", data=version.minor)
+                    f.create_dataset("version_micro", data=version.micro)
 
         else:
+            logger.debug("Try to read time stamps")
             try:
                 with h5pyfile(self._results_file, "r") as f:
                     self._times_stamps = set(f["ep"]["V"].keys())
             except KeyError:
                 pass
+        logger.debug("Done in datacollector init")
 
         self._functions: Dict[str, Dict[str, dolfin.Function]] = {
             "ep": {},
             "mechanics": {},
         }
         self._reductions: Dict[str, Dict[str, str]] = {
             "ep": {},
             "mechanics": {},
         }
+        # Let us synchronize so that we done have any processors
+        # that starts storing data before all processors get here
+        # dolfin.MPI.barrier(self.comm)
 
     @property
     def valid_reductions(self) -> List[str]:
         return ["full", "average"] + list(self._value_extractor.boundary.nodes())
 
     @property
     def results_file(self):
@@ -289,44 +308,55 @@
         if f"{t_str}" in self._times_stamps:
             logger.info(f"Time stamp {t_str} already exist in file")
             return
 
         self._times_stamps.add(t_str)
 
         # First do the full values
+        logger.debug(
+            f"Store in file : {self.results_file}, exists: {Path(self.results_file).exists()}",
+        )
+
         with dolfin.HDF5File(self.comm, self.results_file, "a") as h5file:
             for group, names in self.names.items():
                 logger.debug(
-                    f"Save full states in HDF5File {self.results_file} for group {group}",
+                    f"1. Save full states in HDF5File {self.results_file} for group {group}",
                 )
                 for name in names:
-                    logger.debug(f"Save {name}")
+                    logger.debug(
+                        f"1. Save {name}: reduction {self._reductions[group][name]}",
+                    )
                     if self._reductions[group][name] == "full":
                         f = self._functions[group][name]
                         h5file.write(f, f"{group}/{name}/{t_str}")
 
         # Next do the other reductions
-        with h5pyfile(self.results_file, "a") as h5file:
+        with h5pyfile(self.results_file, "a", comm=self.comm) as h5file:
             for group, names in self.names.items():
                 logger.debug(
-                    f"Save reduced states in HDF5File {self.results_file} for group {group}",
+                    f"2. Save reduced states in HDF5File {self.results_file} for group {group}",
                 )
                 for name in names:
-                    logger.debug(f"Save {name}")
+                    logger.debug(
+                        f"2. Save {name}, reduction: {self._reductions[group][name]}",
+                    )
                     if self._reductions[group][name] == "full":
                         continue
 
+                    logger.debug("Here")
+
                     f = self._functions[group][name]
                     value = self._value_extractor.eval(
                         f,
                         value=self._reductions[group][name],
                     )
                     if f"{group}/{name}" not in h5file:
                         h5file.create_group(f"{group}/{name}")
                     h5file[f"{group}/{name}"].create_dataset(t_str, data=value)
+        logger.debug("Done storing")
 
     def save_residual(self, residual, index):
         logger.debug("Save residual")
         with h5pyfile(self._results_file, "a") as h5file:
             if "residual" not in h5file:
                 h5file.create_group("residual")
             h5file["residual"].create_dataset(str(index), data=residual)
@@ -354,93 +384,139 @@
         self._h5file = None
         self._h5pyfile = None
         self._h5name = Path(h5name)
         if not self._h5name.is_file():
             raise FileNotFoundError(f"File {h5name} does not exist")
 
         self.geo = load_geometry(self._h5name)
-        self._h5pyfile = h5pyfile(self._h5name, "r").__enter__()
-
-        self.version_major = extract_number_from_h5py(
-            self._h5pyfile.get("version_major"),
-        )
-        self.version_minor = extract_number_from_h5py(
-            self._h5pyfile.get("version_minor"),
-        )
-        self.version_micro = extract_number_from_h5py(
-            self._h5pyfile.get("version_micro"),
-        )
-
-        # Find the remaining functions
-        self.names = {
-            group: [name for name in self._h5pyfile.get(group, {}).keys()]
-            for group in ["ep", "mechanics"]
-        }
-        if not empty_ok and len(self.names["ep"]) + len(self.names["mechanics"]) == 0:
-            raise ValueError("No functions found in results file")
-
-        # Get time stamps
-        all_time_stamps = {
-            "{group}:{name}": sorted(
-                list(self._h5pyfile[group][name].keys()),
-                key=lambda x: float(x),
-            )
-            for group, names in self.names.items()
-            for name in names
-        }
-
-        # An verify that they are all the same
-        self.time_stamps = (
-            None
-            if not all_time_stamps
-            else all_time_stamps[next(iter(all_time_stamps.keys()))]
-        )
-        for name in all_time_stamps.keys():
-            assert self.time_stamps == all_time_stamps[name], name
-
-        if not empty_ok and (self.time_stamps is None or len(self.time_stamps) == 0):
-            raise ValueError("No time stamps found")
-
-        # Get the signatures - FIXME: Add a check that the signature exist.
-        self._signatures: Dict[str, Dict[str, Optional[str]]] = {}
-        for group, names in self.names.items():
-            self._signatures[group] = {}
-            for name in names:
-                try:
-                    self._signatures[group][name] = (
-                        self._h5pyfile[group][name][self.time_stamps[0]]  # type: ignore
-                        .attrs["signature"]
-                        .decode()
-                    )
-                except KeyError:
-                    self._signatures[group][name] = None
-
-        if "residual" in self._h5pyfile:
-            self._residual = [
-                self._h5pyfile["residual"][k][...]
-                for k in self._h5pyfile["residual"].keys()
-            ]
-        else:
-            self._residual = []
+        self._gather_h5py_attributes(empty_ok=empty_ok)
 
         self._h5file = dolfin.HDF5File(
-            self.ep_mesh.mpi_comm(),
+            self.geo.comm(),
             self._h5name.as_posix(),
             "r",
         )
 
         self._create_functions()
         self.value_extractor = ValueExtractor(self.geo)
         self._finalizer_h5file = weakref.finalize(self, close_h5file, self._h5file)
         self._finalizer_h5pyfile = weakref.finalize(
             self,
             close_h5pyfile,
             self._h5pyfile,
         )
 
+    def _bcast_attributes(self) -> None:
+        comm = self.geo.comm()
+        if dolfin.MPI.size(comm) == 1:
+            # There is nothing to do
+            return
+
+        dolfin.MPI.barrier(comm)
+        self.version_major: Optional[int] = comm.bcast(self.version_major, root=0)
+        self.version_minor: Optional[int] = comm.bcast(self.version_minor, root=0)
+        self.version_micro: Optional[int] = comm.bcast(self.version_micro, root=0)
+        self.names: Dict[str, List[str]] = comm.bcast(self.names, root=0)
+        self.time_stamps: Optional[np.ndarray] = comm.bcast(self.time_stamps, root=0)
+        self._signatures: Dict[str, Dict[str, Optional[str]]] = comm.bcast(
+            self._signatures,
+            root=0,
+        )
+        self._residual: List[float] = comm.bcast(self._residual, root=0)
+        dolfin.MPI.barrier(comm)
+
+    def _gather_h5py_attributes(self, empty_ok=False):
+        if dolfin.MPI.rank(self.geo.comm()) == 0:
+            self._h5pyfile = h5pyfile(
+                self._h5name,
+                "r",
+                comm=self.geo.comm(),
+                force_serial=True,
+            ).__enter__()
+
+            self.version_major = extract_number_from_h5py(
+                self._h5pyfile.get("version_major"),
+            )
+            self.version_minor = extract_number_from_h5py(
+                self._h5pyfile.get("version_minor"),
+            )
+            self.version_micro = extract_number_from_h5py(
+                self._h5pyfile.get("version_micro"),
+            )
+
+            # Find the remaining functions
+            self.names = {
+                group: [name for name in self._h5pyfile.get(group, {}).keys()]
+                for group in ["ep", "mechanics"]
+            }
+
+            if (
+                not empty_ok
+                and len(self.names["ep"]) + len(self.names["mechanics"]) == 0
+            ):
+                raise ValueError("No functions found in results file")
+
+            # Get time stamps
+            all_time_stamps = {
+                "{group}:{name}": sorted(
+                    list(self._h5pyfile[group][name].keys()),
+                    key=lambda x: float(x),
+                )
+                for group, names in self.names.items()
+                for name in names
+            }
+
+            # An verify that they are all the same
+            self.time_stamps = (
+                None
+                if not all_time_stamps
+                else all_time_stamps[next(iter(all_time_stamps.keys()))]
+            )
+            for name in all_time_stamps.keys():
+                assert self.time_stamps == all_time_stamps[name], name
+
+            if not empty_ok and (
+                self.time_stamps is None or len(self.time_stamps) == 0
+            ):
+                raise ValueError("No time stamps found")
+
+            # Get the signatures -
+            self._signatures = {}
+            for group, names in self.names.items():
+                self._signatures[group] = {}
+                for name in names:
+                    try:
+                        self._signatures[group][name] = (
+                            self._h5pyfile[group][name][self.time_stamps[0]]  # type: ignore
+                            .attrs["signature"]
+                            .decode()
+                        )
+                    except KeyError:
+                        self._signatures[group][name] = None
+
+            if "residual" in self._h5pyfile:
+                self._residual = [
+                    self._h5pyfile["residual"][k][...]
+                    for k in self._h5pyfile["residual"].keys()
+                ]
+            else:
+                self._residual = []
+        else:
+            # Get these from broadcasting
+            self.version_major = None
+            self.version_minor = None
+            self.version_micro = None
+            self.names = {}
+            self.time_stamps = None
+            self._signatures = {}
+            self._residual = []
+
+        dolfin.MPI.barrier(self.geo.comm())
+        self._bcast_attributes()
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.cleanup()
 
     def cleanup(self):
@@ -473,27 +549,24 @@
         return len(self.time_stamps)
 
     def __repr__(self):
         return f"{self.__class__.__name__}({str(self._h5name)})"
 
     def _create_functions(self):
         self._function_spaces = {}
+        logger.debug(f"Create functions from signatures: {self._signatures}")
 
-        for group, signature_dict in self._signatures.items():
+        for group, signature_dict in sorted(self._signatures.items()):
             mesh = self.ep_mesh if group == "ep" else self.mech_mesh
 
-            self._function_spaces.update(
-                {
-                    group: {
-                        signature: dolfin.FunctionSpace(mesh, eval(signature))
-                        for signature in set(signature_dict.values())
-                        if signature is not None
-                    },
-                },
-            )
+            fs_group = {}
+            for signature in sorted(set(signature_dict.values())):
+                logger.debug(signature)
+                fs_group[signature] = dolfin.FunctionSpace(mesh, eval(signature))
+            self._function_spaces[group] = fs_group
 
         self._functions = {
             group: {
                 name: dolfin.Function(
                     self._function_spaces[group][self._signatures[group][name]],
                 )
                 for name in names
@@ -580,11 +653,18 @@
             raise RuntimeError("No data found in result file")
         if t not in self.time_stamps:
             raise KeyError(f"Invalid time stamps {t}")
 
         try:
             func = self._functions[group_str][name]
         except KeyError:
-            return self._h5pyfile[group_str][name][t][...].item()  # type: ignore
+            comm = self.geo.comm()
+
+            value = None
+            if dolfin.MPI.rank(comm) == 0:
+                value = self._h5pyfile[group_str][name][t][...].item()  # type: ignore
+            value = comm.bcast(value, root=0)
+
+            return value
         else:
             self._h5file.read(func, f"{group_str}/{name}/{t}/")
             return func
```

### Comparing `simcardems-2023.5.5/src/simcardems/ep_model.py` & `simcardems-2023.6.0/src/simcardems/ep_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/geometry.py` & `simcardems-2023.6.0/src/simcardems/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,19 +274,20 @@
         unlink: bool = True,
     ):
         path = Path(fname)
         schema = type(self).default_schema()
 
         kwargs = {k: getattr(self, k) for k in schema if k != "info"}
         kwargs["info"] = self.parameters
+        logger.debug("Instantiating geometry")
         geo = Geometry(**kwargs, schema=schema)
 
         if schema_path is None:
             schema_path = path.with_suffix(".json")
-
+        logger.debug("Save geo")
         geo.save(path, schema_path=schema_path, unlink=unlink)
         logger.info(f"Saved geometry to {fname}")
 
     def _get_microstructure_if_None(
         self,
         mesh: dolfin.Mesh,
         ffun: dolfin.MeshFunction,
```

### Comparing `simcardems-2023.5.5/src/simcardems/gui.py` & `simcardems-2023.6.0/src/simcardems/gui.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/lvgeometry.py` & `simcardems-2023.6.0/src/simcardems/lvgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/mechanics_model.py` & `simcardems-2023.6.0/src/simcardems/mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/__init__.py` & `simcardems-2023.6.0/src/simcardems/models/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/em_model.py` & `simcardems-2023.6.0/src/simcardems/models/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/__init__.py` & `simcardems-2023.6.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/cell_model.py` & `simcardems-2023.6.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/em_model.py` & `simcardems-2023.6.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,15 @@
             h5file.write(self.ep_solver.vs, "/ep/vs")
             h5file.write(self.mech_solver.state, "/mechanics/state")
 
         io.dict_to_h5(
             self.cell_params(),
             path,
             "ep/cell_params",
+            comm=self.geometry.comm(),
         )
 
     @classmethod
     def from_state(
         cls,
         path: Union[str, Path],
         drug_factors_file: Union[str, Path] = "",
```

### Comparing `simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py` & `simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py` & `simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py` & `simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py` & `simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,27 +57,26 @@
         f_mech: dolfin.Function,
         f_ep: dolfin.Function,
     ) -> dolfin.Function:
         """Interpolates function from mechanics to ep mesh"""
 
         x = dolfin.as_backend_type(f_mech.vector()).vec()
         a, temp = self.transfer_matrix.getVecs()
-
         self.transfer_matrix.mult(x, temp)
         f_ep.vector().vec().aypx(0.0, temp)
         f_ep.vector().apply("")
 
         # Remember to free memory allocated by petsc: https://gitlab.com/petsc/petsc/-/issues/1309
         x.destroy()
         a.destroy()
         temp.destroy()
 
     @property
     def coupling_type(self):
-        return "fully_coupled_ORdmm_Land"
+        return "fully_coupled_Tor_Land"
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, type(self)):
             return NotImplemented
 
         if not super().__eq__(__o):
             return False
@@ -287,14 +286,15 @@
             h5file.write(self.ep_solver.vs, "/ep/vs")
             h5file.write(self.mech_solver.state, "/mechanics/state")
 
         io.dict_to_h5(
             self.cell_params(),
             path,
             "ep/cell_params",
+            comm=self.geometry.comm(),
         )
 
     @classmethod
     def from_state(
         cls,
         path: Union[str, Path],
         drug_factors_file: Union[str, Path] = "",
```

### Comparing `simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/__init__.py` & `simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/active_model.py` & `simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py` & `simcardems-2023.6.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/em_model.py` & `simcardems-2023.6.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,27 @@
         f_mech: dolfin.Function,
         f_ep: dolfin.Function,
     ) -> dolfin.Function:
         """Interpolates function from mechanics to ep mesh"""
 
         x = dolfin.as_backend_type(f_mech.vector()).vec()
         a, temp = self.transfer_matrix.getVecs()
+
         self.transfer_matrix.mult(x, temp)
         f_ep.vector().vec().aypx(0.0, temp)
         f_ep.vector().apply("")
 
         # Remember to free memory allocated by petsc: https://gitlab.com/petsc/petsc/-/issues/1309
         x.destroy()
         a.destroy()
         temp.destroy()
 
     @property
     def coupling_type(self):
-        return "fully_coupled_Tor_Land"
+        return "fully_coupled_ORdmm_Land"
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, type(self)):
             return NotImplemented
 
         if not super().__eq__(__o):
             return False
@@ -286,14 +287,15 @@
             h5file.write(self.ep_solver.vs, "/ep/vs")
             h5file.write(self.mech_solver.state, "/mechanics/state")
 
         io.dict_to_h5(
             self.cell_params(),
             path,
             "ep/cell_params",
+            comm=self.geometry.comm(),
         )
 
     @classmethod
     def from_state(
         cls,
         path: Union[str, Path],
         drug_factors_file: Union[str, Path] = "",
```

### Comparing `simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py` & `simcardems-2023.6.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/em_model.py` & `simcardems-2023.6.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         ) as h5file:
             h5file.write(self.ep_solver.vs, "/ep/vs")
 
         io.dict_to_h5(
             self.cell_params(),
             path,
             "ep/cell_params",
+            comm=self.geometry.comm(),
         )
 
     @classmethod
     def from_state(
         cls,
         path: Union[str, Path],
         drug_factors_file: Union[str, Path] = "",
```

### Comparing `simcardems-2023.5.5/src/simcardems/newton_solver.py` & `simcardems-2023.6.0/src/simcardems/newton_solver.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/postprocess.py` & `simcardems-2023.6.0/src/simcardems/postprocess.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/runner.py` & `simcardems-2023.6.0/src/simcardems/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import typing
 from pathlib import Path
 
+import dolfin
 from tqdm import tqdm
 
 from . import save_load_functions as io
 from . import utils
 from .config import Config
 from .models import em_model
 from .time_stepper import TimeStepper
@@ -217,15 +218,15 @@
 
 def create_progressbar(
     time_stepper: typing.Optional[TimeStepper] = None,
     show_progress_bar: bool = Config.show_progress_bar,
 ):
     if time_stepper is None:
         raise ValueError("Please provide a time stepper")
-    if show_progress_bar:
+    if dolfin.MPI.size(dolfin.MPI.comm_world) == 1 and show_progress_bar:
         # Show progressbar
         pbar = tqdm(time_stepper, total=time_stepper.total_steps)
     else:
         # Hide progressbar
         pbar = _tqdm(time_stepper, total=time_stepper.total_steps)
     return pbar
```

### Comparing `simcardems-2023.5.5/src/simcardems/save_load_functions.py` & `simcardems-2023.6.0/src/simcardems/save_load_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,45 +27,53 @@
 def vs_functions_to_dict(vs, state_names):
     return {
         name: utils.sub_function(vs, index) for index, name in enumerate(state_names)
     }
 
 
 @contextlib.contextmanager
-def h5pyfile(h5name, filemode="r"):
+def h5pyfile(h5name, filemode="r", force_serial: bool = False, comm=None):
     import h5py
     from mpi4py import MPI
 
-    if h5py.h5.get_config().mpi and dolfin.MPI.size(dolfin.MPI.comm_world) > 1:
+    if comm is None:
+        comm = dolfin.MPI.comm_world
+
+    if h5py.h5.get_config().mpi and dolfin.MPI.size(comm) > 1 and not force_serial:
         h5file = h5py.File(h5name, filemode, driver="mpio", comm=MPI.COMM_WORLD)
     else:
-        if dolfin.MPI.size(dolfin.MPI.comm_world) > 1:
+        if dolfin.MPI.size(comm) > 1 and not force_serial:
             warnings.warn("h5py is not installed with MPI support")
         h5file = h5py.File(h5name, filemode)
     yield h5file
 
     h5file.close()
 
 
-def dict_to_h5(data, h5name, h5group, use_attrs: bool = True):
-    with h5pyfile(h5name, "a") as h5file:
-        if h5group == "":
-            group = h5file
-        else:
-            group = h5file.create_group(h5group)
-        for k, v in data.items():
-            if use_attrs:
-                group.attrs[k] = v
+def dict_to_h5(data, h5name, h5group, use_attrs: bool = True, comm=None):
+    if comm is None:
+        comm = dolfin.MPI.comm_world
+    if comm.rank == 0:
+        with h5pyfile(h5name, "a", force_serial=True) as h5file:
+            if h5group == "":
+                group = h5file
             else:
-                try:
-                    group.create_dataset(k, data=v)
-                except OSError:
-                    logger.warning(
-                        f"Unable to save key {k} with data {v} in {h5name}/{h5group}",
-                    )
+                group = h5file.create_group(h5group)
+            for k, v in data.items():
+                if use_attrs:
+                    group.attrs[k] = v
+                else:
+                    try:
+                        group.create_dataset(k, data=v)
+                    except OSError:
+                        logger.warning(
+                            f"Unable to save key {k} with data {v} in {h5name}/{h5group}",
+                        )
+    # Synchronize
+    dolfin.MPI.barrier(comm)
 
 
 def decode(x):
     if isinstance(x, bytes):
         return x.decode()
     elif isinstance(x, list):
         return [xi for xi in map(decode, x)]
@@ -150,25 +158,25 @@
 def save_state(
     path,
     config: Config,
     geo: geometry.BaseGeometry,
     state_params: Optional[Dict[str, float]] = None,
 ):
     path = Path(path)
-    utils.remove_file(path)
+    utils.remove_file(path, comm=geo.comm())
 
     logger.info(f"Save state to {path}")
     geo.dump(path)
     logger.debug("Save using dolfin.HDF5File")
 
     logger.debug("Save using h5py")
-    dict_to_h5(serialize_dict(config.as_dict()), path, "config")
+    dict_to_h5(serialize_dict(config.as_dict()), path, "config", comm=geo.comm())
     if state_params is None:
         state_params = {}
-    dict_to_h5(serialize_dict(state_params), path, "state_params")
+    dict_to_h5(serialize_dict(state_params), path, "state_params", comm=geo.comm())
 
 
 def load_state(
     path: Union[str, Path],
     drug_factors_file: Union[str, Path] = "",
     popu_factors_file: Union[str, Path] = "",
     disease_state="healthy",
```

### Comparing `simcardems-2023.5.5/src/simcardems/slabgeometry.py` & `simcardems-2023.6.0/src/simcardems/slabgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/time_stepper.py` & `simcardems-2023.6.0/src/simcardems/time_stepper.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/src/simcardems/utils.py` & `simcardems-2023.6.0/src/simcardems/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 mpi_filt = MPIFilt()
 
 
 def getLogger(name):
     import daiquiri
 
     logger = daiquiri.getLogger(name)
+
     logger.logger.addFilter(mpi_filt)
     return logger
 
 
 logger = getLogger(__name__)
 
 
@@ -137,20 +138,22 @@
     e = x.vector() - x_prev.vector()
     norm = e.norm("l2")
     if x_norm > 0:
         norm /= x_norm
     return norm
 
 
-def remove_file(path):
+def remove_file(path, comm=None):
+    if comm is None:
+        comm = dolfin.MPI.comm_world
     path = Path(path)
-    if dolfin.MPI.rank(dolfin.MPI.comm_world) == 0:
+    if comm.rank == 0:
         if path.is_file():
             path.unlink()
-    dolfin.MPI.barrier(dolfin.MPI.comm_world)
+    dolfin.MPI.barrier(comm)
 
 
 def setup_assigner(vs, index):
     # Set-up separate potential function for post processing
     VS0 = vs.function_space().sub(index)
     V = VS0.collapse()
     v = dolfin.Function(V)
```

### Comparing `simcardems-2023.5.5/src/simcardems/value_extractor.py` & `simcardems-2023.6.0/src/simcardems/value_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 logger = utils.getLogger(__name__)
 
 
 class ValueExtractor:
     def __init__(self, geo: BaseGeometry):
         self.geo = geo
         self.volume = dolfin.assemble(dolfin.Constant(1.0) * dolfin.dx(domain=geo.mesh))
-        logger.debug("Creating ValueExtractor with geo: {geo!r}")
+        logger.debug(f"Creating ValueExtractor with geo: {geo!r}")
 
         if isinstance(self.geo, SlabGeometry):
             self.boundary: Boundary = SlabBoundary(geo.mesh)
         elif isinstance(self.geo, LeftVentricularGeometry):
             self.boundary = LVBoundary(geo.mesh)
         else:
             raise NotImplementedError
+        logger.debug("Done")
 
     def average(self, func: dolfin.Function) -> float:
         if func.value_rank() == 0:
             return dolfin.assemble(func * dolfin.dx) / self.volume
         else:
             # Take the magnitude
             return dolfin.assemble(dolfin.sqrt(func**2) * dolfin.dx) / self.volume
```

### Comparing `simcardems-2023.5.5/src/simcardems.egg-info/PKG-INFO` & `simcardems-2023.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.5.5
+Version: 2023.6.0
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
@@ -15,15 +15,15 @@
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: gui
 License-File: LICENSE
 
 [![CI](https://github.com/ComputationalPhysiology/simcardems/actions/workflows/main.yml/badge.svg)](https://github.com/ComputationalPhysiology/simcardems/actions/workflows/main.yml)
 [![PyPI version](https://badge.fury.io/py/simcardems.svg)](https://badge.fury.io/py/simcardems)
-[![codecov](https://codecov.io/gh/ComputationalPhysiology/simcardems/branch/main/graph/badge.svg?token=V5DOQ1PUVF)](https://codecov.io/gh/ComputationalPhysiology/simcardems)
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/simcardems-coverage.json)](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/simcardems-coverage.json)
 [![github pages](https://github.com/ComputationalPhysiology/simcardems/actions/workflows/github-pages.yml/badge.svg)](https://github.com/ComputationalPhysiology/simcardems/actions/workflows/github-pages.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComputationalPhysiology/simcardems/main.svg)](https://results.pre-commit.ci/latest/github/ComputationalPhysiology/simcardems/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v2.1-blue.svg)](https://www.gnu.org/licenses/lgpl-2.1)
 [![DOI](https://zenodo.org/badge/409220068.svg)](https://zenodo.org/badge/latestdoi/409220068)
 [![status](https://joss.theoj.org/papers/28986461c27b8a76c8ac5a43dc57e8dc/status.svg)](https://joss.theoj.org/papers/28986461c27b8a76c8ac5a43dc57e8dc)
```

### Comparing `simcardems-2023.5.5/src/simcardems.egg-info/SOURCES.txt` & `simcardems-2023.6.0/src/simcardems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/tests/test_boundary_conditions.py` & `simcardems-2023.6.0/tests/test_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/tests/test_cli.py` & `simcardems-2023.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/tests/test_datacollector.py` & `simcardems-2023.6.0/tests/test_datacollector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pathlib import Path
 from unittest import mock
 
 import dolfin
-import h5py
 import pytest
 import simcardems
 
 
 def test_DataCollector_reset_state_when_file_exists(tmp_path, geo):
     simcardems.DataCollector(tmp_path, geo=geo)
 
@@ -24,15 +23,15 @@
     remove_file_mock.assert_not_called()
     assert Path(collector.results_file).is_file()
 
 
 def test_DataCollector_create_file_with_geo(tmp_path, geo):
     collector = simcardems.DataCollector(tmp_path, geo=geo)
     assert Path(collector.results_file).is_file()
-    with h5py.File(collector.results_file, "r") as h5file:
+    with simcardems.save_load_functions.h5pyfile(collector.results_file, "r") as h5file:
         assert "geometry" in h5file
 
 
 def test_DataCollector_register(tmp_path, geo):
     V = dolfin.FunctionSpace(geo.mesh, "CG", 1)
     f = dolfin.Function(V)
```

### Comparing `simcardems-2023.5.5/tests/test_geometry.py` & `simcardems-2023.6.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/tests/test_mechanics_model.py` & `simcardems-2023.6.0/tests/test_mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/tests/test_models.py` & `simcardems-2023.6.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/tests/test_postprocessing.py` & `simcardems-2023.6.0/tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/tests/test_runner.py` & `simcardems-2023.6.0/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.5/tests/test_save_load_functions.py` & `simcardems-2023.6.0/tests/test_save_load_functions.py`

 * *Files identical despite different names*

