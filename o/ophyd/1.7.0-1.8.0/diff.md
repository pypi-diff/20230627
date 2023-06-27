# Comparing `tmp/ophyd-1.7.0.tar.gz` & `tmp/ophyd-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd-1.7.0.tar", last modified: Fri Aug  5 16:35:23 2022, max compression
+gzip compressed data, was "ophyd-1.8.0.tar", last modified: Mon Jun 26 18:53:24 2023, max compression
```

## Comparing `ophyd-1.7.0.tar` & `ophyd-1.8.0.tar`

### file list

```diff
@@ -1,102 +1,181 @@
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.886490 ophyd-1.7.0/
--rw-r--r--   0 joshualynch   (503) staff       (20)     1584 2022-08-05 14:46:33.000000 ophyd-1.7.0/LICENSE
--rw-r--r--   0 joshualynch   (503) staff       (20)      281 2022-08-05 14:46:33.000000 ophyd-1.7.0/MANIFEST.in
--rw-r--r--   0 joshualynch   (503) staff       (20)     2603 2022-08-05 16:35:23.886697 ophyd-1.7.0/PKG-INFO
--rw-r--r--   0 joshualynch   (503) staff       (20)     2339 2022-08-05 14:46:33.000000 ophyd-1.7.0/README.rst
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.887855 ophyd-1.7.0/ophyd/
--rw-r--r--   0 joshualynch   (503) staff       (20)     3490 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     5525 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/_caproto_shim.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     6982 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/_dispatch.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      929 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/_dummy_shim.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     5949 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/_pyepics_shim.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      497 2022-08-05 16:35:23.887961 ophyd-1.7.0/ophyd/_version.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.857748 ophyd-1.7.0/ophyd/areadetector/
--rw-r--r--   0 joshualynch   (503) staff       (20)     1002 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    16344 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/base.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    70662 2022-08-05 16:33:27.000000 ophyd-1.7.0/ophyd/areadetector/cam.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     6864 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/common_plugins.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     6574 2022-08-05 16:33:27.000000 ophyd-1.7.0/ophyd/areadetector/detectors.py
--rw-r--r--   0 joshualynch   (503) staff       (20)   178461 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/docs.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    23679 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/filestore_mixins.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     4587 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/paths.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    80031 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/plugins.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     9887 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/trigger_mixins.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     6345 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/areadetector/util.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     3626 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/callbacks.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    63134 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/device.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.858652 ophyd-1.7.0/ophyd/docs/
--rw-r--r--   0 joshualynch   (503) staff       (20)      397 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/docs/__init__.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.859180 ophyd-1.7.0/ophyd/docs/templates/
--rw-r--r--   0 joshualynch   (503) staff       (20)       88 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/docs/templates/__init__.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.860978 ophyd-1.7.0/ophyd/docs/templates/autosummary/
--rw-r--r--   0 joshualynch   (503) staff       (20)        0 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/docs/templates/autosummary/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      106 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/docs/templates/autosummary/base.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     2273 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/docs/templates/autosummary/class.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)      753 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/docs/templates/autosummary/module.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     8603 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/docs/utils.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    12470 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/epics_motor.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    13246 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/flyers.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     8511 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/log.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    15220 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/mca.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     5031 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/mixins.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    19423 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/ophydobj.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    11915 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/positioner.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    32077 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/pseudopos.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    21098 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/pv_positioner.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     4819 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/quadem.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     5361 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/scaler.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    77031 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/signal.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    51515 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/sim.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    33509 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/status.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.882833 ophyd-1.7.0/ophyd/tests/
--rw-r--r--   0 joshualynch   (503) staff       (20)       29 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1668 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/config.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     4722 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/conftest.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1462 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/fake_motor_ioc.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     7582 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/mca_ioc.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     9888 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/scaler_ioc.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1659 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/signal_ioc.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    20371 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_areadetector.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2680 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_bluesky_protocols.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    25612 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_device.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     4214 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_docs.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     7715 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_epicsmotor.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     4953 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_flyers.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1640 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_hints.py
--rwxr-xr-x   0 joshualynch   (503) staff       (20)     5509 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_issue944.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    14388 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_kind.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2048 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_log.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     4215 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_mca.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     4564 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_ophydobj.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2989 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_positioner.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    15062 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_pseudopos.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     8905 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_pvpositioner.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2341 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_quadem.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     3278 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_scaler.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    18313 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_signal.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2055 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_signalpositioner.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     9760 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_sim.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    12170 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_status.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      958 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_timeout.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2098 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_timestamps.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2164 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_units.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     3675 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_utils.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1395 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/tests/test_versioning.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     7277 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/units.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.885943 ophyd-1.7.0/ophyd/utils/
--rw-r--r--   0 joshualynch   (503) staff       (20)     4893 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/utils/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    10540 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/utils/epics_pvs.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1743 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/utils/errors.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1911 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/utils/paths.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      343 2022-08-05 14:46:33.000000 ophyd-1.7.0/ophyd/utils/startup.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2022-08-05 16:35:23.850040 ophyd-1.7.0/ophyd.egg-info/
--rw-r--r--   0 joshualynch   (503) staff       (20)     2603 2022-08-05 16:35:23.000000 ophyd-1.7.0/ophyd.egg-info/PKG-INFO
--rw-r--r--   0 joshualynch   (503) staff       (20)     2288 2022-08-05 16:35:23.000000 ophyd-1.7.0/ophyd.egg-info/SOURCES.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)        1 2022-08-05 16:35:23.000000 ophyd-1.7.0/ophyd.egg-info/dependency_links.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       58 2022-08-05 16:35:23.000000 ophyd-1.7.0/ophyd.egg-info/entry_points.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       35 2022-08-05 16:35:23.000000 ophyd-1.7.0/ophyd.egg-info/requires.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)        6 2022-08-05 16:35:23.000000 ophyd-1.7.0/ophyd.egg-info/top_level.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       35 2022-08-05 14:46:33.000000 ophyd-1.7.0/requirements.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)      174 2022-08-05 16:35:23.887391 ophyd-1.7.0/setup.cfg
--rw-r--r--   0 joshualynch   (503) staff       (20)     1876 2022-08-05 14:46:33.000000 ophyd-1.7.0/setup.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    68713 2022-08-05 14:46:33.000000 ophyd-1.7.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.632770 ophyd-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-26 18:53:10.000000 ophyd-1.8.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 18:53:10.000000 ophyd-1.8.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 18:53:10.000000 ophyd-1.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.572770 ophyd-1.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.584770 ophyd-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-26 18:53:10.000000 ophyd-1.8.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-26 18:53:10.000000 ophyd-1.8.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-26 18:53:10.000000 ophyd-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-26 18:53:10.000000 ophyd-1.8.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-26 18:53:10.000000 ophyd-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-26 18:53:10.000000 ophyd-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-26 18:53:24.632770 ophyd-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-26 18:53:10.000000 ophyd-1.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 18:53:10.000000 ophyd-1.8.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.588770 ophyd-1.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.588770 ophyd-1.8.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/_templates/README
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.588770 ophyd-1.8.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/images/bluesky_ophyd_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/images/ophyd_favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.588770 ophyd-1.8.0/docs/user_v1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.592770 ophyd-1.8.0/docs/user_v1/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/explanations/area-detector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/explanations/relationship-to-epics.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/explanations/staging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/explanations/status.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.592770 ophyd-1.8.0/docs/user_v1/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/how-to/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/how-to/pseudopositioner.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.596770 ophyd-1.8.0/docs/user_v1/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/reference/builtin-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/reference/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/reference/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/reference/positioners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    43020 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/reference/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/reference/signals.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.596770 ophyd-1.8.0/docs/user_v1/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/tutorials/device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/tutorials/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v1/tutorials/single-PV.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.596770 ophyd-1.8.0/docs/user_v2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.596770 ophyd-1.8.0/docs/user_v2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v2/examples/epics_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.596770 ophyd-1.8.0/docs/user_v2/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v2/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.600770 ophyd-1.8.0/docs/user_v2/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v2/how-to/make-a-simple-device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.600770 ophyd-1.8.0/docs/user_v2/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v2/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.600770 ophyd-1.8.0/docs/user_v2/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v2/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-06-26 18:53:10.000000 ophyd-1.8.0/docs/user_v2/tutorials/using-existing-devices.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.612770 ophyd-1.8.0/ophyd/
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/_caproto_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/_dummy_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/_pyepics_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 18:53:24.000000 ophyd-1.8.0/ophyd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.616770 ophyd-1.8.0/ophyd/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/common_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178461 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/filestore_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80092 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/trigger_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/areadetector/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63150 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.620770 ophyd-1.8.0/ophyd/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.620770 ophyd-1.8.0/ophyd/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/docs/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.620770 ophyd-1.8.0/ophyd/docs/templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/docs/templates/autosummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/docs/templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/docs/templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/docs/templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/docs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/flyers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/ophydobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/positioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32094 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/pv_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/quadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77054 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52454 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33531 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.628770 ophyd-1.8.0/ophyd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/fake_motor_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/mca_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/scaler.db
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/scaler_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/signal_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_areadetector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_bluesky_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25612 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_epicsmotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_flyers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_hints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5509 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_issue944.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_ophydobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_pvpositioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_quadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_signalpositioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/tests/test_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.628770 ophyd-1.8.0/ophyd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/utils/epics_pvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/utils/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.632770 ophyd-1.8.0/ophyd/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/_aioca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/_p4p.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31342 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/epics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.632770 ophyd-1.8.0/ophyd/v2/epicsdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/epicsdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/epicsdemo/mover.db
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/epicsdemo/sensor.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.632770 ophyd-1.8.0/ophyd/v2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/tests/test_epics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/tests/test_epicsdemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-26 18:53:10.000000 ophyd-1.8.0/ophyd/v2/tests/test_records.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.612770 ophyd-1.8.0/ophyd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-26 18:53:24.000000 ophyd-1.8.0/ophyd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-26 18:53:24.000000 ophyd-1.8.0/ophyd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:53:24.000000 ophyd-1.8.0/ophyd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 18:53:24.000000 ophyd-1.8.0/ophyd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-26 18:53:24.000000 ophyd-1.8.0/ophyd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 18:53:24.000000 ophyd-1.8.0/ophyd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.632770 ophyd-1.8.0/other_licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-26 18:53:10.000000 ophyd-1.8.0/other_licenses/pyepics
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-26 18:53:10.000000 ophyd-1.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:53:24.632770 ophyd-1.8.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9486 2023-06-26 18:53:10.000000 ophyd-1.8.0/scripts/collect_ad_boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-26 18:53:10.000000 ophyd-1.8.0/scripts/create_directories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-06-26 18:53:10.000000 ophyd-1.8.0/scripts/epics_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-06-26 18:53:10.000000 ophyd-1.8.0/scripts/epics_exports.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-26 18:53:24.632770 ophyd-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-26 18:53:10.000000 ophyd-1.8.0/setup.py
```

### Comparing `ophyd-1.7.0/LICENSE` & `ophyd-1.8.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-Copyright (c) 2014, Brookhaven Science Associates, Brookhaven National
-Laboratory. All rights reserved.
+BSD 3-Clause License
+
+Copyright (c) 2014, Brookhaven National Laboratory
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
 
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the Brookhaven Science Associates, Brookhaven National
-  Laboratory nor the names of its contributors may be used to endorse or promote
-  products derived from this software without specific prior written permission.
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `ophyd-1.7.0/PKG-INFO` & `ophyd-1.8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,37 @@
-Metadata-Version: 2.1
-Name: ophyd
-Version: 1.7.0
-License: BSD
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-License-File: LICENSE
-
 *****
 Ophyd
 *****
 
 |build_status| |coverage| |pypi_version| |license|
 
-Ophyd is Python library for interfacing with hardware. It provides an
-abstraction layer than enables experiment orchestration and data acquisition
+Ophyd is a Python library for interfacing with hardware. It provides an
+abstraction layer that enables experiment orchestration and data acquisition
 code to operate above the specifics of particular devices and control systems.
 
 Ophyd is typically used with the `Bluesky Run Engine`_ for experiment
-orchestration and data acquistion. It is also sometimes used in a stand-alone
+orchestration and data acquisition. It is also sometimes used in a stand-alone
 fashion.
 
 Many facilities use ophyd to integrate with control systems that use `EPICS`_ ,
 but ophyd's design and some of its objects are also used to integrate with
 other control systems.
 
 * Put the details specific to a device or control system behind a **high-level
   interface** with methods like ``trigger()``, ``read()``, and ``set(...)``.
 * **Group** individual control channels (such as EPICS V3 PVs) into logical
-  "Devices" to be configured and used as units with internal coordiantion.
+  "Devices" to be configured and used as units with internal coordination.
 * Assign readings with **names meaningful for data analysis** that will
   propagate into metadata.
 * **Categorize** readings by "kind" (primary reading, configuration,
   engineering/debugging) which can be read selectively.
 
 ============== ==============================================================
 PyPI           ``pip install ophyd``
-Conda          ``pip install -c nsls2forge ophyd``
+Conda          ``conda install -c conda-forge ophyd``
 Source code    https://github.com/bluesky/ophyd
 Documentation  https://blueskyproject.io/ophyd
 ============== ==============================================================
 
 See the tutorials for usage examples.
 
 .. |build_status| image:: https://github.com/bluesky/ophyd/workflows/Unit%20Tests/badge.svg?branch=master
@@ -59,7 +49,13 @@
 .. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
     :target: https://opensource.org/licenses/BSD-3-Clause
     :alt: BSD 3-Clause License
 
 .. _Bluesky Run Engine: http://blueskyproject.io/bluesky
 
 .. _EPICS: http://www.aps.anl.gov/epics/
+
+..
+    Anything below this line is used when viewing README.rst and will be replaced
+    when included in index.rst
+
+See https://blueskyproject.io/ophyd for more detailed documentation.
```

### Comparing `ophyd-1.7.0/README.rst` & `ophyd-1.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,54 @@
+Metadata-Version: 2.1
+Name: ophyd
+Version: 1.8.0
+Summary: Bluesky hardware abstraction with an emphasis on EPICS
+Home-page: https://github.com/bluesky/ophyd
+License: BSD
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: ca
+Provides-Extra: pva
+Provides-Extra: dev
+License-File: LICENSE
+
 *****
 Ophyd
 *****
 
 |build_status| |coverage| |pypi_version| |license|
 
-Ophyd is Python library for interfacing with hardware. It provides an
-abstraction layer than enables experiment orchestration and data acquisition
+Ophyd is a Python library for interfacing with hardware. It provides an
+abstraction layer that enables experiment orchestration and data acquisition
 code to operate above the specifics of particular devices and control systems.
 
 Ophyd is typically used with the `Bluesky Run Engine`_ for experiment
-orchestration and data acquistion. It is also sometimes used in a stand-alone
+orchestration and data acquisition. It is also sometimes used in a stand-alone
 fashion.
 
 Many facilities use ophyd to integrate with control systems that use `EPICS`_ ,
 but ophyd's design and some of its objects are also used to integrate with
 other control systems.
 
 * Put the details specific to a device or control system behind a **high-level
   interface** with methods like ``trigger()``, ``read()``, and ``set(...)``.
 * **Group** individual control channels (such as EPICS V3 PVs) into logical
-  "Devices" to be configured and used as units with internal coordiantion.
+  "Devices" to be configured and used as units with internal coordination.
 * Assign readings with **names meaningful for data analysis** that will
   propagate into metadata.
 * **Categorize** readings by "kind" (primary reading, configuration,
   engineering/debugging) which can be read selectively.
 
 ============== ==============================================================
 PyPI           ``pip install ophyd``
-Conda          ``pip install -c nsls2forge ophyd``
+Conda          ``conda install -c conda-forge ophyd``
 Source code    https://github.com/bluesky/ophyd
 Documentation  https://blueskyproject.io/ophyd
 ============== ==============================================================
 
 See the tutorials for usage examples.
 
 .. |build_status| image:: https://github.com/bluesky/ophyd/workflows/Unit%20Tests/badge.svg?branch=master
@@ -49,7 +66,13 @@
 .. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
     :target: https://opensource.org/licenses/BSD-3-Clause
     :alt: BSD 3-Clause License
 
 .. _Bluesky Run Engine: http://blueskyproject.io/bluesky
 
 .. _EPICS: http://www.aps.anl.gov/epics/
+
+..
+    Anything below this line is used when viewing README.rst and will be replaced
+    when included in index.rst
+
+See https://blueskyproject.io/ophyd for more detailed documentation.
```

### Comparing `ophyd-1.7.0/ophyd/__init__.py` & `ophyd-1.8.0/ophyd/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+# type: ignore
+
 import logging
-import types
 import os
+import types
+
 from ophyd.log import set_handler  # noqa: F401
 
 logger = logging.getLogger(__name__)
 
 cl = None
 
 
@@ -25,14 +28,22 @@
                 return
         else:
             raise ImportError("no valid control layer found")
 
     # TODO replace this with fancier meta-programming
     # TODO handle control_layer being a module/nampspace directly
     if control_layer == "pyepics":
+        # If using pyepics and ophyd.v2 (p4p and aioca), need to use the same
+        # libCom and libCa as provided by epicscorelibs
+        # https://github.com/BCDA-APS/apstools/issues/836
+        try:
+            import epicscorelibs.path.pyepics  # noqa
+        except ImportError:
+            # No epicscorelibs, let pyepics use bundled CA
+            pass
         from . import _pyepics_shim as shim
     elif control_layer == "caproto":
         from . import _caproto_shim as shim
     elif control_layer == "dummy":
         from . import _dummy_shim as shim
     else:
         raise ValueError("unknown control_layer")
@@ -48,16 +59,16 @@
         "name",
         "release_pvs",
         "get_dispatcher",
     )
     # this sets the module level value
     cl = types.SimpleNamespace(**{k: getattr(shim, k) for k in exports})
     if pv_telemetry:
-        from functools import wraps
         from collections import Counter
+        from functools import wraps
 
         def decorate_get_pv(func):
             c = Counter()
 
             @wraps(func)
             def get_pv(pvname, *args, **kwargs):
                 c[pvname] += 1
@@ -73,60 +84,64 @@
     if cl is None:
         raise RuntimeError("control layer not set, " "unsure how you got to this state")
     return cl
 
 
 set_cl()
 
+# Areadetector-related
+from .areadetector import *  # noqa: F401, F402, E402, F403
+from .device import (  # noqa: F401, F402, E402
+    ALL_COMPONENTS,
+    Component,
+    Device,
+    DynamicDeviceComponent,
+    FormattedComponent,
+    do_not_wait_for_lazy_connection,
+    kind_context,
+    wait_for_lazy_connection,
+)
+from .epics_motor import EpicsMotor, MotorBundle  # noqa: F401, F402, E402
+from .mca import EpicsDXP, EpicsMCA  # noqa: F401, F402, E402
 from .ophydobj import (  # noqa: F401, F402, E402
     Kind,
-    select_version,
     register_instances_in_weakset,
     register_instances_keyed_on_name,
-)
-
-# Signals
-from .signal import (  # noqa: F401, F402, E402
-    Signal,
-    SignalRO,
-    EpicsSignal,
-    EpicsSignalRO,
-    EpicsSignalNoValidation,
-    DerivedSignal,
+    select_version,
 )
 
 # Positioners
 from .positioner import PositionerBase, SoftPositioner  # noqa: F401, F402, E402
-from .epics_motor import EpicsMotor, MotorBundle  # noqa: F401, F402, E402
+from .pseudopos import PseudoPositioner, PseudoSingle  # noqa: F401, F402, E402
 from .pv_positioner import (  # noqa: F401, F402, E402
     PVPositioner,
-    PVPositionerPC,
-    PVPositionerIsClose,
     PVPositionerDone,
+    PVPositionerIsClose,
+    PVPositionerPC,
 )
-from .pseudopos import PseudoPositioner, PseudoSingle  # noqa: F401, F402, E402
+from .quadem import APS_EM, NSLS_EM, QuadEM, TetrAMM  # noqa: F401, F402, E402
 
 # Devices
 from .scaler import EpicsScaler  # noqa: F401, F402, E402
-from .device import (  # noqa: F401, F402, E402
-    Device,
-    Component,
-    FormattedComponent,
-    DynamicDeviceComponent,
-    ALL_COMPONENTS,
-    kind_context,
-    wait_for_lazy_connection,
-    do_not_wait_for_lazy_connection,
+
+# Signals
+from .signal import (  # noqa: F401, F402, E402
+    DerivedSignal,
+    EpicsSignal,
+    EpicsSignalNoValidation,
+    EpicsSignalRO,
+    Signal,
+    SignalRO,
 )
 from .status import StatusBase, wait  # noqa: F401, F402, E402
-from .mca import EpicsMCA, EpicsDXP  # noqa: F401, F402, E402
-from .quadem import QuadEM, NSLS_EM, TetrAMM, APS_EM  # noqa: F401, F402, E402
-
-# Areadetector-related
-from .areadetector import *  # noqa: F401, F402, E402, F403
-from ._version import get_versions  # noqa: F402, E402
-
 from .utils.startup import setup as setup_ophyd  # noqa: F401, F402, E402
 
-
-__version__ = get_versions()["version"]
-del get_versions
+try:
+    # Use live version from git
+    from setuptools_scm import get_version
+
+    # Warning: If the install is nested to the same depth, this will always succeed
+    __version__ = get_version(root="..", relative_to=__file__)
+    del get_version
+except (ImportError, LookupError):
+    # Use installed version
+    from ._version import __version__  # noqa: F401
```

### Comparing `ophyd-1.7.0/ophyd/_caproto_shim.py` & `ophyd-1.8.0/ophyd/_caproto_shim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import threading
-
 import atexit
 import logging
+import threading
 
 from caproto.threading import pyepics_compat
-from caproto.threading.pyepics_compat import PV as _PV, caput, caget  # noqa
-from ._dispatch import _CallbackThread, EventDispatcher, wrap_callback
+from caproto.threading.pyepics_compat import PV as _PV
+from caproto.threading.pyepics_compat import caget, caput  # noqa
 
+from ._dispatch import EventDispatcher, _CallbackThread, wrap_callback
 
 thread_class = threading.Thread
 module_logger = logging.getLogger(__name__)
 _dispatcher = None
 name = "caproto"
```

### Comparing `ophyd-1.7.0/ophyd/_dispatch.py` & `ophyd-1.8.0/ophyd/_dispatch.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import time
 import functools
 import logging
 import queue
 import threading
+import time
 
 
 class _CallbackThread(threading.Thread):
     "A queue-based callback dispatcher thread"
 
     def __init__(
         self,
```

### Comparing `ophyd-1.7.0/ophyd/_dummy_shim.py` & `ophyd-1.8.0/ophyd/_dummy_shim.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/_pyepics_shim.py` & `ophyd-1.8.0/ophyd/_pyepics_shim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import atexit
 import logging
-from packaging.version import parse
+
 import epics
 from epics import ca, caget, caput
+from packaging.version import parse
 
-from ._dispatch import _CallbackThread, EventDispatcher, wrap_callback
+from ._dispatch import EventDispatcher, _CallbackThread, wrap_callback
 
 _min_pyepics = "3.4.2"
 
 if parse(epics.__version__) < parse(_min_pyepics):
     raise ImportError(
         "Version of pyepics too old. "
         f"Ophyd requires at least {_min_pyepics}"
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/__init__.py` & `ophyd-1.8.0/ophyd/areadetector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 from .base import *  # noqa: F401, F402, E402, F403
 from .cam import *  # noqa: F401, F402, E402, F403
+from .common_plugins import *  # noqa: F401, F402, E402, F403
 from .detectors import *  # noqa: F401, F402, E402, F403
+from .paths import EpicsPathSignal  # noqa: F401, F402, E402, F403
 
 # NOTE: the following imports are here for backward compatibility with
 # previous ophyd versions. This does not represent all available plugins
 # in ophyd. For that, import directly from ophyd.areadetector.plugins.
 from .plugins import (  # noqa: F401, F402, E402
     ColorConvPlugin,
     FilePlugin,
@@ -26,11 +28,8 @@
     StatsPlugin,
     TIFFPlugin,
     TransformPlugin,
     get_areadetector_plugin,
     plugin_from_pvname,
     register_plugin,
 )
-
-from .common_plugins import *  # noqa: F401, F402, E402, F403
 from .trigger_mixins import *  # noqa: F401, F402, E402, F403
-from .paths import EpicsPathSignal  # noqa: F401, F402, E402, F403
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/base.py` & `ophyd-1.8.0/ophyd/areadetector/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# type: ignore
+
 import functools
 import inspect
 import re
 import sys
 import textwrap
 from collections import OrderedDict
 from typing import (
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/cam.py` & `ophyd-1.8.0/ophyd/areadetector/cam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+# type: ignore
+
 import logging
 
 from ..device import DynamicDeviceComponent as DDC
 from ..signal import EpicsSignal, EpicsSignalRO
 from ..utils import enum
 from .base import ADBase
-from .base import EpicsSignalWithRBV as SignalWithRBV
 from .base import ADComponent as ADCpt
+from .base import EpicsSignalWithRBV as SignalWithRBV
 from .base import ad_group
 
 # Import FileBase class for cameras that use File PVs in their drivers
 from .plugins import FileBase
 
 logger = logging.getLogger(__name__)
 
@@ -36,14 +38,15 @@
     "PcoDetectorSimIO",
     "PerkinElmerDetectorCam",
     "PICamDetectorCam",
     "PilatusDetectorCam",
     "PixiradDetectorCam",
     "PointGreyDetectorCam",
     "ProsilicaDetectorCam",
+    "PvaDetectorCam",
     "PvcamDetectorCam",
     "RoperDetectorCam",
     "SimDetectorCam",
     "URLDetectorCam",
     "UVCDetectorCam",
     "Xspress3DetectorCam",
 ]
@@ -1211,14 +1214,24 @@
     sync_out3_mode = ADCpt(SignalWithRBV, "SyncOut3Mode")
     trigger_delay = ADCpt(SignalWithRBV, "TriggerDelay")
     trigger_event = ADCpt(SignalWithRBV, "TriggerEvent")
     trigger_overlap = ADCpt(SignalWithRBV, "TriggerOverlap")
     trigger_software = ADCpt(EpicsSignal, "TriggerSoftware")
 
 
+class PvaDetectorCam(CamBase):
+    """PvaDriver pulls new image frames via PVAccess."""
+
+    _html_docs = ["pvaDoc.html"]
+
+    input_pv = ADCpt(SignalWithRBV, "PvName", string=True)
+    input_connection = ADCpt(EpicsSignalRO, "PvConnection_RBV", string=True)
+    overrun_counter = ADCpt(SignalWithRBV, "OverrunCounter")
+
+
 class PvcamDetectorCam(CamBase):
     _html_docs = ["pvcamDoc.html"]
     bit_depth = ADCpt(EpicsSignalRO, "BitDepth_RBV")
     camera_firmware_vers = ADCpt(EpicsSignalRO, "CameraFirmwareVers_RBV")
     chip_height = ADCpt(EpicsSignalRO, "ChipHeight_RBV")
     chip_name = ADCpt(EpicsSignalRO, "ChipName_RBV")
     chip_width = ADCpt(EpicsSignalRO, "ChipWidth_RBV")
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/common_plugins.py` & `ophyd-1.8.0/ophyd/areadetector/common_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .. import Device, Component as Cpt
+from ..device import Component as Cpt
+from ..device import Device, create_device_from_components
+from ..ophydobj import OphydObject, select_version
 from . import plugins
-from ..device import create_device_from_components
-from ..ophydobj import select_version, OphydObject
 
 
 class CommonPlugins(Device, version_type="ADCore"):
     ...
 
 
 class CommonOverlayPlugin(Device, version_type="ADCore"):
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/detectors.py` & `ophyd-1.8.0/ophyd/areadetector/detectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "PSLDetector",
     "PerkinElmerDetector",
     "PICamDetector",
     "PilatusDetector",
     "PixiradDetector",
     "PointGreyDetector",
     "ProsilicaDetector",
+    "PvaDetector",
     "PvcamDetector",
     "RoperDetector",
     "SimDetector",
     "URLDetector",
     "UVCDetector",
     "Xspress3Detector",
 ]
@@ -222,14 +223,19 @@
 
 
 class ProsilicaDetector(DetectorBase):
     _html_docs = ["prosilicaDoc.html"]
     cam = C(cam.ProsilicaDetectorCam, "cam1:")
 
 
+class PvaDetector(DetectorBase):
+    _html_docs = ["pvaDoc.html"]
+    cam = C(cam.PvaDetectorCam, "cam1:")
+
+
 class PvcamDetector(DetectorBase):
     _html_docs = ["pvcamDoc.html"]
     cam = C(cam.PvcamDetectorCam, "cam1:")
 
 
 class RoperDetector(DetectorBase):
     _html_docs = ["RoperDoc.html"]
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/docs.py` & `ophyd-1.8.0/ophyd/areadetector/docs.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/areadetector/filestore_mixins.py` & `ophyd-1.8.0/ophyd/areadetector/filestore_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,24 @@
     dest = '/tmp'  # in production, use a directory on your system -- not /tmp
 
     class MyDetector(PerkinElmerDetector, SingleTrigger):  # for example
         file_plugin = MyPlugin(suffix='HDF1:', write_path_template=dest)
 
     det = MyDetector(...)
 """
-from collections import deque
-import os
 import logging
-import warnings
+import os
 import uuid
-from pathlib import PurePath, PurePosixPath, PureWindowsPath
-
+import warnings
+from collections import defaultdict, deque
 from datetime import datetime
-from collections import defaultdict
 from itertools import count
+from pathlib import PurePath, PurePosixPath, PureWindowsPath
 
-from ..device import GenerateDatumInterface, BlueskyInterface, Staged
+from ..device import BlueskyInterface, GenerateDatumInterface, Staged
 
 logger = logging.getLogger(__name__)
 
 
 def new_uid():
     "uuid4 as a string"
     return str(uuid.uuid4())
@@ -124,15 +122,15 @@
         - verify that the path starts with :attr:`root` or the path is
           a relative, prepend :attr:`root`
 
       - if ``read_path_template`` is also provided then the above
         checks are applied to it, but ``write_path_template`` is
         returned without any validation.
 
-    This mixin assumes that it's peers provide an `enable` signal
+    This mixin assumes that it's peers provide an ``enable`` signal
 
     Parameters
     ----------
     write_path_template : str
         Template feed to :py:meth:`~datetime.datetime.strftime` to generate the
         path to set the IOC to write saved files to.
 
@@ -151,15 +149,15 @@
         'root' will be changed (for example of the whole file tree is
         copied to / mounted on another system or external hard drive).
 
     path_semantics : {'posix', 'windows'}, optional
 
     read_path_template : str, optional
         The read path template, if different from the write path.   See the
-        docstings for `write_path_template` and `root`.
+        docstrings for ``write_path_template`` and ``root``.
 
     reg : Registry
         If None provided, try to import the top-level api from
         filestore.api This will be deprecated 17Q3.
 
         This object must provide::
 
@@ -434,15 +432,15 @@
         return filename, read_path, write_path
 
     def stage(self):
         # Make a filename.
         filename, read_path, write_path = self.make_filename()
 
         # Ensure we do not have an old file open.
-        if self.file_write_mode != "Single":
+        if self.file_write_mode.get(as_string=True) != "Single":
             self.capture.set(0).wait()
         # These must be set before parent is staged (specifically
         # before capture mode is turned on. They will not be reset
         # on 'unstage' anyway.
         self.file_path.set(write_path).wait()
         self.file_name.set(filename).wait()
         self.file_number.set(0).wait()
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/paths.py` & `ophyd-1.8.0/ophyd/areadetector/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import pathlib
 import time as ttime
 
-from .. import EpicsSignal
+from ..signal import EpicsSignal
 
 logger = logging.getLogger(__name__)
 OS_NAME_TO_PATH_CLASS = {
     "nt": pathlib.PureWindowsPath,
     "posix": pathlib.PurePosixPath,
 }
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/plugins.py` & `ophyd-1.8.0/ophyd/areadetector/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,35 +17,32 @@
 # enhancement for bootstrapping all the versions of Area Detector to date.
 # Updates should be made either by hand or by producing new auto-generation
 # code to suit.
 
 
 import functools
 import logging
-import numpy as np
 import operator
 import re
 import time as ttime
-
 from collections import OrderedDict
 
-from .base import (
-    ADBase,
-    ADComponent as Cpt,
-    EpicsSignalWithRBV as SignalWithRBV,
-    DDC_EpicsSignal,
-    DDC_EpicsSignalRO,
-    DDC_SignalWithRBV,
-    NDDerivedSignal,
-)
-from .. import Device, Component, FormattedComponent as FCpt
-from ..signal import EpicsSignalRO, EpicsSignal, ArrayAttributeSignal
+import numpy as np
+
+from ..device import Component, Device
+from ..device import FormattedComponent as FCpt
 from ..device import GenerateDatumInterface
+from ..signal import ArrayAttributeSignal, EpicsSignal, EpicsSignalRO
 from ..utils import enum
-from ..utils.errors import PluginMisconfigurationError, DestroyedError, UnprimedPlugin
+from ..utils.errors import DestroyedError, PluginMisconfigurationError, UnprimedPlugin
+from .base import ADBase
+from .base import ADComponent as Cpt
+from .base import DDC_EpicsSignal, DDC_EpicsSignalRO, DDC_SignalWithRBV
+from .base import EpicsSignalWithRBV as SignalWithRBV
+from .base import NDDerivedSignal
 from .paths import EpicsPathSignal
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "AttrPlotPlugin",
     "AttributeNPlugin",
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/trigger_mixins.py` & `ophyd-1.8.0/ophyd/areadetector/trigger_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
     from ophyd.areadetector.detectors import PerkinElmerDetector
     from ophyd.areadetector.trigger_mixins import SingleTrigger
 
     class MyDetector(PerkinElmerDetector, SingleTrigger):
         pass
 """
 
-import time as ttime
-import logging
 import itertools
+import logging
+import time as ttime
 
-from ..status import DeviceStatus
 from ..device import BlueskyInterface, Staged
+from ..status import DeviceStatus
 
 logger = logging.getLogger(__name__)
 
 
 class ADTriggerStatus(DeviceStatus):
     """
     A Status for AreaDetector triggers
@@ -79,15 +79,15 @@
 
 
 class TriggerBase(BlueskyInterface):
     """Base class for trigger mixin classes
 
     Subclasses must define a method with this signature:
 
-    `acquire_changed(self, value=None, old_value=None, **kwargs)`
+    ``acquire_changed(self, value=None, old_value=None, **kwargs)``
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # settings
         # careful here: quadEM devices have areadetector components but,
         # they have no 'cam' plugin. See QuadEM initializer.
@@ -162,15 +162,15 @@
     This can be used to give more control to the detector. One call to
     'trigger' can be interpreted by the detector as a call to take several
     acquisitions with, for example, different gain settings or shutter
     positions.
 
     The are two levels of nesting here:
 
-     - cycling through different actions on successive calls to `trigger`
+     - cycling through different actions on successive calls to ``trigger``
      - within each trigger, executing a list of acquisitions with different
        settings
 
     See the example below, which takes and 3 and 1 acquisitions in
     alternation.
 
     Examples
```

### Comparing `ophyd-1.7.0/ophyd/areadetector/util.py` & `ophyd-1.8.0/ophyd/areadetector/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import inspect
 import os
-import sys
 import re
+import sys
 from collections import namedtuple
 
 from ..utils.epics_pvs import records_from_db
-from .detectors import AreaDetector
 from .base import EpicsSignalWithRBV
-
+from .detectors import AreaDetector
 
 StubInfo = namedtuple("StubInfo", ("signal_type", "record"))
 
 
 def get_prop_name(pv):
     """Get a property name from the camel-case AreaDetector PV name"""
     # If it's all capital letters and underscores, then just convert
```

### Comparing `ophyd-1.7.0/ophyd/callbacks.py` & `ophyd-1.8.0/ophyd/callbacks.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/device.py` & `ophyd-1.8.0/ophyd/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# type: ignore
+
 from __future__ import annotations
 
 import collections
 import contextlib
 import functools
 import inspect
 import itertools
```

### Comparing `ophyd-1.7.0/ophyd/docs/templates/autosummary/class.rst` & `ophyd-1.8.0/ophyd/docs/templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/docs/templates/autosummary/module.rst` & `ophyd-1.8.0/ophyd/docs/templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/docs/utils.py` & `ophyd-1.8.0/ophyd/docs/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/epics_motor.py` & `ophyd-1.8.0/ophyd/epics_motor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
+from enum import Enum
 
-from .utils.epics_pvs import fmt_time
-
-from .signal import EpicsSignal, EpicsSignalRO
-from .utils import DisconnectedError
-from .utils.epics_pvs import raise_if_disconnected, AlarmSeverity
+from .device import Component as Cpt
+from .device import Device, required_for_connection
 from .positioner import PositionerBase
-from .device import Device, Component as Cpt, required_for_connection
+from .signal import EpicsSignal, EpicsSignalRO
 from .status import wait as status_wait
-from enum import Enum
-
+from .utils import DisconnectedError
+from .utils.epics_pvs import AlarmSeverity, fmt_time, raise_if_disconnected
 
 logger = logging.getLogger(__name__)
 
 
 class HomeEnum(str, Enum):
     forward = "forward"
     reverse = "reverse"
```

### Comparing `ophyd-1.7.0/ophyd/flyers.py` & `ophyd-1.8.0/ophyd/flyers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import time as ttime
 import functools
 import logging
+import time as ttime
 from collections import OrderedDict
+from typing import Any, Dict, Generator, Iterable
 
-from .signal import Signal, EpicsSignal, EpicsSignalRO
+from .device import BlueskyInterface
+from .device import Component as Cpt
+from .device import Device
+from .signal import EpicsSignal, EpicsSignalRO, Signal
 from .status import DeviceStatus, StatusBase
-from .device import Device, Component as Cpt, BlueskyInterface
 from .utils import OrderedDefaultDict
 
-from typing import Generator, Dict, Iterable, Any
-
-
 logger = logging.getLogger(__name__)
 
 
 class FlyerInterface(BlueskyInterface):
     def kickoff(self) -> StatusBase:
         """Start a flyer
```

### Comparing `ophyd-1.7.0/ophyd/log.py` & `ophyd-1.8.0/ophyd/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     Key features of this formatter are:
 
     * Color support when logging to a terminal that supports it.
     * Timestamps on every log line.
     * Robust against str/bytes encoding problems.
 
     This formatter is enabled automatically by
-    `tornado.options.parse_command_line` or `tornado.options.parse_config_file`
+    ``tornado.options.parse_command_line`` or ``tornado.options.parse_config_file``
     (unless ``--logging=none`` is used).
     Color support on Windows versions that do not support ANSI color codes is
     enabled by use of the colorama__ library. Applications that wish to use
     this must first initialize colorama with a call to ``colorama.init``.
     See the colorama documentation for details.
 
     __ https://pypi.python.org/pypi/colorama
```

### Comparing `ophyd-1.7.0/ophyd/mca.py` & `ophyd-1.8.0/ophyd/mca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
-
 from collections import OrderedDict
 
-from .signal import Signal, EpicsSignal, EpicsSignalRO
-from .device import Device, Component as Cpt, DynamicDeviceComponent as DDC, Kind
 from .areadetector import EpicsSignalWithRBV as SignalWithRBV
-
+from .device import Component as Cpt
+from .device import Device
+from .device import DynamicDeviceComponent as DDC
+from .device import Kind
+from .signal import EpicsSignal, EpicsSignalRO, Signal
 
 logger = logging.getLogger(__name__)
 
 
 class ROI(Device):
 
     # 'name' is not an allowed attribute
```

### Comparing `ophyd-1.7.0/ophyd/mixins.py` & `ophyd-1.8.0/ophyd/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import time
 import logging
+import time
 
-from .signal import EpicsSignal
 from .positioner import PositionerBase
-from .status import MoveStatus, wait as status_wait
-
+from .signal import EpicsSignal
+from .status import MoveStatus
+from .status import wait as status_wait
 
 logger = logging.getLogger(__name__)
 
 
 class SignalPositionerMixin(PositionerBase):
     """Mixin to make a Signal a Positioner
```

### Comparing `ophyd-1.7.0/ophyd/ophydobj.py` & `ophyd-1.8.0/ophyd/ophydobj.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,28 +366,28 @@
     @property
     def report(self):
         """A report on the object."""
         return {}
 
     @property
     def event_types(self):
-        """Events that can be subscribed to via `obj.subscribe`"""
+        """Events that can be subscribed to via ``obj.subscribe``"""
         return tuple(self.subscriptions)
 
     def _run_subs(self, *args, sub_type, **kwargs):
         """Run a set of subscription callbacks
 
         Only the kwarg ``sub_type`` is required, indicating
         the type of callback to perform. All other positional arguments
         and kwargs are passed directly to the callback function.
 
         The host object will be injected into kwargs as 'obj' unless that key
         already exists.
 
-        If the `timestamp` is None, then it will be replaced by the current
+        If the ``timestamp`` is None, then it will be replaced by the current
         time.
 
         No exceptions are raised if the callback functions fail.
         """
         if sub_type not in self.subscriptions:
             raise UnknownSubscription(
                 "Unknown subscription {!r}, must be one of {!r}".format(
```

### Comparing `ophyd-1.7.0/ophyd/positioner.py` & `ophyd-1.8.0/ophyd/positioner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import functools
 import logging
 import time
 from collections import OrderedDict
-import functools
-from .ophydobj import OphydObject, Kind
-from .status import MoveStatus, wait as status_wait, StatusBase
-from .utils.epics_pvs import data_type, data_shape
-from .utils.errors import LimitError
 from typing import Any, Callable
 
+from .ophydobj import Kind, OphydObject
+from .status import MoveStatus, StatusBase
+from .status import wait as status_wait
+from .utils.epics_pvs import data_shape, data_type
+from .utils.errors import LimitError
 
 logger = logging.getLogger(__name__)
 
 
 class PositionerBase(OphydObject):
     """The positioner base class
```

### Comparing `ophyd-1.7.0/ophyd/pseudopos.py` & `ophyd-1.8.0/ophyd/pseudopos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # vi: ts=4 sw=4
 
 
-import logging
-import time
-import threading
 import functools
+import logging
 import math
-
+import threading
+import time
 from collections import OrderedDict, namedtuple
-from collections.abc import Sequence, Mapping
+from collections.abc import Mapping, Sequence
 
-from .utils import DisconnectedError, ExceptionBundle
+from .device import Component as Cpt
+from .device import Device, Kind, required_for_connection
 from .positioner import PositionerBase, SoftPositioner
-from .device import Device, Component as Cpt, Kind, required_for_connection
 from .signal import AttributeSignal
-
+from .utils import DisconnectedError, ExceptionBundle
 
 logger = logging.getLogger(__name__)
 
 
 class PseudoSingle(Device, SoftPositioner):
     """A single axis of a PseudoPositioner
```

### Comparing `ophyd-1.7.0/ophyd/pv_positioner.py` & `ophyd-1.8.0/ophyd/pv_positioner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # vi: ts=4 sw=4
 
 import logging
 from typing import Any, Optional
 
 import numpy as np
 
-from .utils.epics_pvs import fmt_time
-
 from .device import Component as Cpt
 from .device import Device, required_for_connection
 from .ophydobj import Kind
 from .positioner import PositionerBase
 from .signal import EpicsSignal, InternalSignal
 from .status import wait as status_wait
+from .utils.epics_pvs import fmt_time
 
 logger = logging.getLogger(__name__)
 
 
 class PVPositioner(Device, PositionerBase):
     """A Positioner which is controlled using multiple user-defined signals
 
@@ -55,17 +54,17 @@
         The value sent to stop_signal when a stop is requested
     done : Signal
         A readback value indicating whether motion is finished
     done_value : any, optional
         The value that the done pv should be when motion has completed
     put_complete : bool, optional
         If set, the specified PV should allow for asynchronous put completion
-        to indicate motion has finished.  If `actuate` is specified, it will be
-        used for put completion.  Otherwise, the `setpoint` will be used.  See
-        the `-c` option from `caput` for more information.
+        to indicate motion has finished.  If ``actuate`` is specified, it will be
+        used for put completion.  Otherwise, the ``setpoint`` will be used.  See
+        the `-c` option from ``caput`` for more information.
     """
 
     setpoint = None  # TODO: should add limits=True
     readback = None
     actuate = None
     actuate_value = 1
 
@@ -335,15 +334,15 @@
     The comparison function takes two arguments, readback and setpoint,
     returning True if we are considered done or False if we are not.
 
     This class is intended to support `PVPositionerIsClose`, but exists to
     allow some flexibility if we want to use other metrics for deciding if
     the PVPositioner is done.
 
-    Internally, this will subscribe to both the `setpoint` and `readback`
+    Internally, this will subscribe to both the ``setpoint`` and ``readback``
     signals, updating `done` as appropriate.
 
     Parameters
     ----------
     prefix : str, optional
         The device prefix used for all sub-positioners. This is optional as it
         may be desirable to specify full PV names for PVPositioners.
@@ -371,17 +370,17 @@
         requested
     stop_signal : Signal or None
         The stop PV to set when motion should be stopped
     stop_value : any, optional
         The value sent to stop_signal when a stop is requested
     put_complete : bool, optional
         If set, the specified PV should allow for asynchronous put completion
-        to indicate motion has finished.  If `actuate` is specified, it will be
-        used for put completion.  Otherwise, the `setpoint` will be used.  See
-        the `-c` option from `caput` for more information.
+        to indicate motion has finished.  If ``actuate`` is specified, it will be
+        used for put completion.  Otherwise, the ``setpoint`` will be used.  See
+        the `-c` option from ``caput`` for more information.
     """
 
     done = Cpt(InternalSignal, value=0)
     done_value = 1
 
     def __init__(self, prefix: str, *, name: str, **kwargs):
         self._last_readback = None
@@ -488,17 +487,17 @@
         requested
     stop_signal : Signal or None
         The stop PV to set when motion should be stopped
     stop_value : any, optional
         The value sent to stop_signal when a stop is requested
     put_complete : bool, optional
         If set, the specified PV should allow for asynchronous put completion
-        to indicate motion has finished.  If `actuate` is specified, it will be
-        used for put completion.  Otherwise, the `setpoint` will be used.  See
-        the `-c` option from `caput` for more information.
+        to indicate motion has finished.  If ``actuate`` is specified, it will be
+        used for put completion.  Otherwise, the ``setpoint`` will be used.  See
+        the `-c` option from ``caput`` for more information.
     atol : float, optional
         A measure of absolute tolerance. If atol is 0.1, then you'd be
         able to be up to 0.1 units away and still count as done.
     rtol : float, optional
         A measure of relative tolerance. If rtol is 0.1, then you'd be
         able to deviate from the goal position by up to 10% of its value
     """
@@ -576,17 +575,17 @@
         requested
     stop_signal : Signal or None
         The stop PV to set when motion should be stopped
     stop_value : any, optional
         The value sent to stop_signal when a stop is requested
     put_complete : bool, optional
         If set, the specified PV should allow for asynchronous put completion
-        to indicate motion has finished.  If `actuate` is specified, it will be
-        used for put completion.  Otherwise, the `setpoint` will be used.  See
-        the `-c` option from `caput` for more information.
+        to indicate motion has finished.  If ``actuate`` is specified, it will be
+        used for put completion.  Otherwise, the ``setpoint`` will be used.  See
+        the `-c` option from ``caput`` for more information.
     """
 
     setpoint = Cpt(EpicsSignal, "", kind="hinted")
 
     done = Cpt(InternalSignal, value=0)
     done_value = 1
```

### Comparing `ophyd-1.7.0/ophyd/quadem.py` & `ophyd-1.8.0/ophyd/quadem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from collections import OrderedDict
 
-from . import (
-    EpicsSignalRO,
-    EpicsSignal,
-    Component as Cpt,
-    DynamicDeviceComponent as DDCpt,
-    Signal,
-    Kind,
-    kind_context,
-)
 from .areadetector import (
+    ADBase,
+    DetectorBase,
     EpicsSignalWithRBV,
     ImagePlugin,
-    StatsPlugin,
-    DetectorBase,
     SingleTrigger,
-    ADBase,
+    StatsPlugin,
 )
+from .device import Component as Cpt
+from .device import DynamicDeviceComponent as DDCpt
+from .device import kind_context
+from .signal import EpicsSignal, EpicsSignalRO, Kind, Signal
 from .status import DeviceStatus
 
 
 def _current_fields(attr_base, field_base, range_, **kwargs):
     defn = OrderedDict()
     for i in range_:
         attr = "{attr}{i}".format(attr=attr_base, i=i)
```

### Comparing `ophyd-1.7.0/ophyd/scaler.py` & `ophyd-1.8.0/ophyd/scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import logging
-
 from collections import OrderedDict
 
+from .device import Component as Cpt
+from .device import Device
+from .device import DynamicDeviceComponent as DDCpt
+from .device import FormattedComponent as FCpt
 from .ophydobj import Kind
 from .signal import EpicsSignal, EpicsSignalRO
-from .device import Device
-from .device import (
-    Component as Cpt,
-    DynamicDeviceComponent as DDCpt,
-    FormattedComponent as FCpt,
-)
 
 logger = logging.getLogger(__name__)
 
 
 def _scaler_fields(cls, attr_base, field_base, range_, **kwargs):
     defn = OrderedDict()
     for i in range_:
```

### Comparing `ophyd-1.7.0/ophyd/signal.py` & `ophyd-1.8.0/ophyd/signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # vi: ts=4 sw=4
 import os
-import time
 import threading
+import time
 import warnings
 import weakref
 
 import numpy as np
 
-from .utils import ReadOnlyError, LimitError, DestroyedError, doc_annotation_forwarder
+from . import get_cl
+from .ophydobj import Kind, OphydObject
+from .status import Status
+from .utils import DestroyedError, LimitError, ReadOnlyError, doc_annotation_forwarder
 from .utils.epics_pvs import (
-    waveform_to_string,
-    raise_if_disconnected,
-    data_type,
-    data_shape,
-    AlarmStatus,
     AlarmSeverity,
-    validate_pv_name,
+    AlarmStatus,
     _set_and_wait,
+    data_shape,
+    data_type,
+    raise_if_disconnected,
+    validate_pv_name,
+    waveform_to_string,
 )
-from .ophydobj import OphydObject, Kind
-from .status import Status
-from . import get_cl
-
 
 # Catch semi-frequent issue with scripts accidentally run from inside module
 if __name__ != "ophyd.signal":
     raise RuntimeError(
         "A script tried to import ophyd.signal instead of the signal built-in "
         "module. This usually happens when a script is run from inside the "
         "ophyd directory and can cause extremely confusing bugs. Please "
@@ -493,15 +492,15 @@
             ) from ve
 
     def read_configuration(self):
         "Dictionary mapping names to value dicts with keys: value, timestamp"
         return self.read()
 
     def describe_configuration(self):
-        """Provide schema & meta-data for `~BlueskyInterface.read_configuration`
+        """Provide schema & meta-data for :meth:`BlueskyInterface.read_configuration`
 
         This keys in the `OrderedDict` this method returns must match the keys
         in the `OrderedDict` return by :meth:`~BlueskyInterface.read`.
 
         This provides schema related information, (ex shape, dtype), the source
         (ex PV name), and if available, units, limits, precision etc.
 
@@ -1533,15 +1532,15 @@
 
     def put(self, *args, **kwargs):
         "Disabled for a read-only signal"
         raise ReadOnlyError("Cannot write to read-only EpicsSignal")
 
     def set(self, *args, **kwargs):
         "Disabled for a read-only signal"
-        raise ReadOnlyError("Read-only signals cannot be set")
+        raise ReadOnlyError(f"Read-only signal {self} cannot be set to {args}")
 
     def _pv_access_callback(self, read_access, write_access, pv):
         "Control-layer callback: read PV access rights have changed"
         # Tweak write access here - this is a read-only signal!
         if self._destroyed:
             return
 
@@ -2020,15 +2019,15 @@
         connection_timeout=DEFAULT_CONNECTION_TIMEOUT,
         callback=None,
         use_complete=None,
         timeout=DEFAULT_WRITE_TIMEOUT,
         **kwargs,
     ):
         """
-        Using channel access, set the write PV to `value`.
+        Using channel access, set the write PV to ``value``.
 
         Keyword arguments are passed on to callbacks
 
         Parameters
         ----------
         value : any
             The value to set
```

### Comparing `ophyd-1.7.0/ophyd/sim.py` & `ophyd-1.8.0/ophyd/sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import copy
 import inspect
 import itertools
-from functools import partial
-
-import numpy as np
 import os
 import random
 import threading
 import time as ttime
 import uuid
-import weakref
 import warnings
-
-from collections import deque, OrderedDict
+import weakref
+from collections import OrderedDict, deque
+from functools import partial
 from tempfile import mkdtemp
+from types import SimpleNamespace
+
+import numpy as np
 
-from .signal import Signal, EpicsSignal, EpicsSignalRO
 from .areadetector.base import EpicsSignalWithRBV
 from .areadetector.paths import EpicsPathSignal
-from .status import DeviceStatus, StatusBase
-from .device import Device, Component as Cpt, DynamicDeviceComponent as DDCpt, Kind
-from types import SimpleNamespace
+from .device import Component as Cpt
+from .device import Device
+from .device import DynamicDeviceComponent as DDCpt
+from .device import Kind
+from .log import logger
+from .positioner import SoftPositioner
 from .pseudopos import (
     PseudoPositioner,
     PseudoSingle,
-    real_position_argument,
     pseudo_position_argument,
+    real_position_argument,
 )
-from .positioner import SoftPositioner
-from .utils import ReadOnlyError, LimitError
-from .log import logger
-
+from .signal import EpicsSignal, EpicsSignalRO, Signal
+from .status import DeviceStatus, MoveStatus, StatusBase
+from .utils import LimitError, ReadOnlyError
 
 # two convenience functions 'vendored' from bluesky.utils
 
 
 def new_uid():
     return str(uuid.uuid4())
 
@@ -402,14 +403,18 @@
         Simulates how long it takes the device to "move". Default is 0 seconds.
     precision : integer, optional
         Digits of precision. Default is 3.
     parent : Device, optional
         Used internally if this Signal is made part of a larger Device.
     kind : a member the Kind IntEnum (or equivalent integer), optional
         Default is Kind.normal. See Kind for options.
+    events_per_move: number of events to push to a Status object for each move.
+        Must be at least 1, more than one will give "moving" statuses that can be
+        used for progress bars etc.
+        Default is 1.
     """
 
     readback = Cpt(_ReadbackSignal, value=0, kind="hinted")
     setpoint = Cpt(_SetpointSignal, value=0, kind="normal")
 
     velocity = Cpt(Signal, value=1, kind="config")
     acceleration = Cpt(Signal, value=1, kind="config")
@@ -426,14 +431,16 @@
         readback_func=None,
         value=0,
         delay=0,
         precision=3,
         parent=None,
         labels=None,
         kind=None,
+        events_per_move: int = 1,
+        egu: str = "mm",
         **kwargs,
     ):
         if readback_func is None:
 
             def readback_func(x):
                 return x
 
@@ -454,55 +461,64 @@
         self.sim_state["setpoint"] = value
         self.sim_state["setpoint_ts"] = ttime.time()
         self.sim_state["readback"] = readback_func(value)
         self.sim_state["readback_ts"] = ttime.time()
 
         super().__init__(name=name, parent=parent, labels=labels, kind=kind, **kwargs)
         self.readback.name = self.name
+        if events_per_move < 1:
+            raise ValueError("At least 1 event per move is required")
+        self._events_per_move = events_per_move
+        self.egu = egu
 
-    def set(self, value):
+    def _make_status(self, target: float):
+        return MoveStatus(positioner=self, target=target)
+
+    def set(self, value: float) -> MoveStatus:
         old_setpoint = self.sim_state["setpoint"]
+        distance = value - old_setpoint
         self.sim_state["setpoint"] = value
         self.sim_state["setpoint_ts"] = ttime.time()
         self.setpoint._run_subs(
             sub_type=self.setpoint.SUB_VALUE,
             old_value=old_setpoint,
             value=self.sim_state["setpoint"],
             timestamp=self.sim_state["setpoint_ts"],
         )
 
-        def update_state():
+        def update_state(position: float) -> None:
             old_readback = self.sim_state["readback"]
-            self.sim_state["readback"] = self._readback_func(value)
+            self.sim_state["readback"] = self._readback_func(position)
             self.sim_state["readback_ts"] = ttime.time()
             self.readback._run_subs(
                 sub_type=self.readback.SUB_VALUE,
                 old_value=old_readback,
                 value=self.sim_state["readback"],
                 timestamp=self.sim_state["readback_ts"],
             )
             self._run_subs(
                 sub_type=self.SUB_READBACK,
                 old_value=old_readback,
                 value=self.sim_state["readback"],
                 timestamp=self.sim_state["readback_ts"],
             )
 
-        st = DeviceStatus(device=self)
-        if self.delay:
-
-            def sleep_and_finish():
-                ttime.sleep(self.delay)
-                update_state()
-                st.set_finished()
+        st = self._make_status(target=value)
 
-            threading.Thread(target=sleep_and_finish, daemon=True).start()
-        else:
-            update_state()
+        def sleep_and_finish():
+            event_delay = self.delay / self._events_per_move
+            for i in range(self._events_per_move):
+                if self.delay:
+                    ttime.sleep(event_delay)
+                position = old_setpoint + (distance * ((i + 1) / self._events_per_move))
+                update_state(position)
             st.set_finished()
+
+        threading.Thread(target=sleep_and_finish, daemon=True).start()
+
         return st
 
     @property
     def position(self):
         return self.readback.get()
 
 
@@ -1126,14 +1142,17 @@
     def inverse(self, real_pos):
         real_pos = self.RealPosition(*real_pos)
         # logger.debug('inverse %s', real_pos)
         return self.PseudoPosition(pseudo1=-real_pos.real1)
 
 
 class SynAxisNoPosition(SynAxis):
+    def _make_status(self, target: float):
+        return DeviceStatus(device=self)
+
     @property
     def position(self):
         raise AttributeError
 
 
 def make_fake_device(cls):
     """
```

### Comparing `ophyd-1.7.0/ophyd/status.py` & `ophyd-1.8.0/ophyd/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from collections import deque
-from logging import LoggerAdapter
 import threading
 import time
+from collections import deque
+from logging import LoggerAdapter
 from warnings import warn
 
 import numpy as np
 
 from .log import logger
 from .utils import (
-    adapt_old_callback_signature,
     InvalidState,
-    UnknownStatusFailure,
     StatusTimeoutError,
+    UnknownStatusFailure,
     WaitTimeoutError,
+    adapt_old_callback_signature,
 )
 
 
 class UseNewProperty(RuntimeError):
     ...
 
 
@@ -395,15 +395,15 @@
         Raises
         ------
         WaitTimeoutError
             If the status has not completed within ``timeout`` (starting from
             when this method was called, not from the beginning of the action).
         """
         if not self._event.wait(timeout=timeout):
-            raise WaitTimeoutError("Status has not completed yet.")
+            raise WaitTimeoutError(f"Status {self!r} has not completed yet.")
         return self._exception
 
     def wait(self, timeout=None):
         """
         Block until the action completes.
 
         When the action has finished succesfully, return ``None``. If the
@@ -425,15 +425,15 @@
         Exception
             This is ``status.exception()``, raised if the status has finished
             with an error.  This may include ``TimeoutError``, which
             indicates that the action itself raised ``TimeoutError``, distinct
             from ``WaitTimeoutError`` above.
         """
         if not self._event.wait(timeout=timeout):
-            raise WaitTimeoutError("Status has not completed yet.")
+            raise WaitTimeoutError(f"Status {self!r} has not completed yet.")
         if self._exception is not None:
             raise self._exception
 
     @property
     def callbacks(self):
         """
         Callbacks to be run when the status is marked as finished
@@ -664,15 +664,15 @@
             watcher(name=self.device.name, fraction=0.0)
 
     __repr__ = __str__
 
 
 class SubscriptionStatus(DeviceStatus):
     """
-    Status updated via `ophyd` events
+    Status updated via ``ophyd`` events
 
     Parameters
     ----------
     device : obj
 
     callback : callable
         Callback that takes event information and returns a boolean. Signature
```

### Comparing `ophyd-1.7.0/ophyd/tests/config.py` & `ophyd-1.8.0/ophyd/tests/config.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/tests/conftest.py` & `ophyd-1.8.0/ophyd/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 import logging
 import uuid
+from types import SimpleNamespace
 
 import pytest
 
-from types import SimpleNamespace
-
-from ophyd import (
-    set_cl,
-    EpicsMotor,
-    Signal,
-    EpicsSignal,
-    EpicsSignalRO,
-    Component as Cpt,
-)
+from ophyd import Component as Cpt
+from ophyd import EpicsMotor, EpicsSignal, EpicsSignalRO, Signal, set_cl
 from ophyd.utils.epics_pvs import AlarmSeverity, AlarmStatus
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture()
 def hw(tmpdir):
```

### Comparing `ophyd-1.7.0/ophyd/tests/fake_motor_ioc.py` & `ophyd-1.8.0/ophyd/tests/fake_motor_ioc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
-from caproto.server import pvproperty, PVGroup, ioc_arg_parser, run
 import numpy as np
+from caproto.server import PVGroup, ioc_arg_parser, pvproperty, run
 
 
 class FakeMotorIOC(PVGroup):
     setpoint = pvproperty(value=0.0, precision=1)
     readback = pvproperty(value=0.0, read_only=True, precision=1)
     moving = pvproperty(value=0.0, read_only=True)
     actuate = pvproperty(value=0)
```

### Comparing `ophyd-1.7.0/ophyd/tests/mca_ioc.py` & `ophyd-1.8.0/ophyd/tests/mca_ioc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 from caproto.server import (
-    pvproperty,
     PVGroup,
-    ioc_arg_parser,
-    run,
     SubGroup,
     get_pv_pair_wrapper,
+    ioc_arg_parser,
+    pvproperty,
+    run,
 )
 
 pvproperty_with_rbv = get_pv_pair_wrapper(setpoint_suffix="", readback_suffix="_RBV")
 unknown = int
 
 
 class MCAROIGroup(PVGroup):
```

### Comparing `ophyd-1.7.0/ophyd/tests/scaler_ioc.py` & `ophyd-1.8.0/ophyd/tests/scaler_ioc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
-from caproto.server import pvproperty, PVGroup, ioc_arg_parser, run, SubGroup
 from caproto import ChannelType
+from caproto.server import PVGroup, SubGroup, ioc_arg_parser, pvproperty, run
 
 
 class EpicsScalerGroup(PVGroup):
     count = pvproperty(name=".CNT", dtype=int)
     count_mode = pvproperty(
         value="OneShot",
         name=".CONT",
```

### Comparing `ophyd-1.7.0/ophyd/tests/signal_ioc.py` & `ophyd-1.8.0/ophyd/tests/signal_ioc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from caproto.server import pvproperty, PVGroup, ioc_arg_parser, run
+from caproto.server import PVGroup, ioc_arg_parser, pvproperty, run
 
 
 class SignalTestIOC(PVGroup):
     read_only = pvproperty(value=0.0, read_only=True, alarm_group="alarm_a")
     read_write = pvproperty(
         value=0.0,
         lower_ctrl_limit=-100.0,
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_areadetector.py` & `ophyd-1.8.0/ophyd/tests/test_areadetector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,59 +1,56 @@
 import datetime
 import logging
 import os
 import shutil
 import time
+import uuid
+from io import StringIO
+from pathlib import Path, PurePath
 from unittest.mock import Mock
 
 import numpy as np
 import pytest
-from io import StringIO
-from pathlib import PurePath, Path
 
-from ophyd.utils.paths import make_dir_tree
 from ophyd import (
-    SimDetector,
-    SingleTrigger,
     Component,
     Device,
     DynamicDeviceComponent,
     Kind,
+    SimDetector,
+    SingleTrigger,
     wait,
 )
-from ophyd.areadetector.plugins import (
-    ImagePlugin,
-    StatsPlugin,
-    ColorConvPlugin,
-    ProcessPlugin,
-    OverlayPlugin,
-    ROIPlugin,
-    TransformPlugin,
-    NetCDFPlugin,
-    TIFFPlugin,
-    JPEGPlugin,
-    HDF5Plugin,
-    # FilePlugin
-)
 from ophyd.areadetector.base import NDDerivedSignal
 from ophyd.areadetector.filestore_mixins import (
-    FileStoreTIFF,
-    FileStoreIterativeWrite,
     FileStoreHDF5,
+    FileStoreIterativeWrite,
+    FileStoreTIFF,
 )
 
 # we do not have nexus installed on our test IOC
 # from ophyd.areadetector.plugins import NexusPlugin
-from ophyd.areadetector.plugins import PluginBase
-from ophyd.areadetector.util import stub_templates
-from ophyd.device import (
-    Component as Cpt,
+from ophyd.areadetector.plugins import (  # FilePlugin
+    ColorConvPlugin,
+    HDF5Plugin,
+    ImagePlugin,
+    JPEGPlugin,
+    NetCDFPlugin,
+    OverlayPlugin,
+    PluginBase,
+    ProcessPlugin,
+    ROIPlugin,
+    StatsPlugin,
+    TIFFPlugin,
+    TransformPlugin,
 )
+from ophyd.areadetector.util import stub_templates
+from ophyd.device import Component as Cpt
 from ophyd.signal import Signal
-import uuid
+from ophyd.utils.paths import make_dir_tree
 
 logger = logging.getLogger(__name__)
 ad_path = "/epics/support/areaDetector/1-9-1/ADApp/Db/"
 
 
 class DummyFS:
     def __init__(self):
@@ -380,39 +377,14 @@
     det.read_attrs = ["stats1"]
     det.stats1.read_attrs = ["mean_value"]
     det.stats1.mean_value.kind = Kind.hinted
 
     str(det)
 
 
-@pytest.mark.adsim
-def test_default_configuration_smoke(ad_prefix, cleanup):
-    class MyDetector(SimDetector):
-        imageplugin = Cpt(ImagePlugin, ImagePlugin._default_suffix)
-        statsplugin = Cpt(StatsPlugin, StatsPlugin._default_suffix)
-        colorconvplugin = Cpt(ColorConvPlugin, ColorConvPlugin._default_suffix)
-        processplugin = Cpt(ProcessPlugin, ProcessPlugin._default_suffix)
-        overlayplugin = Cpt(OverlayPlugin, OverlayPlugin._default_suffix)
-        roiplugin = Cpt(ROIPlugin, ROIPlugin._default_suffix)
-        transformplugin = Cpt(TransformPlugin, TransformPlugin._default_suffix)
-        netcdfplugin = Cpt(NetCDFPlugin, NetCDFPlugin._default_suffix)
-        tiffplugin = Cpt(TIFFPlugin, TIFFPlugin._default_suffix)
-        jpegplugin = Cpt(JPEGPlugin, JPEGPlugin._default_suffix)
-        # nexusplugin = Cpt(NexusPlugin, NexusPlugin._default_suffix)
-        hdf5plugin = Cpt(HDF5Plugin, HDF5Plugin._default_suffix)
-        # magickplugin = Cpt(MagickPlugin, MagickPlugin._default_suffix)
-
-    d = MyDetector(ad_prefix, name="d")
-    cleanup.add(d)
-    d.stage()
-    {n: getattr(d, n).read_configuration() for n in d.component_names}
-    {n: getattr(d, n).describe_configuration() for n in d.component_names}
-    d.unstage()
-
-
 @pytest.mark.parametrize("plugin", _recursive_subclasses(PluginBase))
 def test_default_configuration_attrs(plugin):
     configuration_attrs = plugin._default_configuration_attrs
     if configuration_attrs is None:
         pytest.skip("Configuration attrs unset")
     for k in configuration_attrs:
         assert hasattr(plugin, k)
@@ -524,14 +496,15 @@
     except ImportError as ex:
         raise pytest.skip("h5py unavailable") from ex
 
     return h5py
 
 
 @pytest.mark.adsim
+@pytest.mark.xfail
 @pytest.mark.parametrize(
     "root,wpath,rpath,check_files",
     (
         (None, "/tmp/ophyd_AD_test/data1/%Y/%m/%d", None, False),
         (None, "/tmp/ophyd_AD_test/data1/%Y/%m/%d", None, False),
         ("/tmp/ophyd_AD_test/data1", "%Y/%m/%d", None, False),
         (
@@ -716,7 +689,32 @@
 
     det.tiff1.file_path.put(paths)
     # det.cam.file_path.put(paths)
     det.stage()
     st = det.trigger()
     wait(st, timeout=5)
     det.unstage()
+
+
+@pytest.mark.adsim
+def test_default_configuration_smoke(ad_prefix, cleanup):
+    class MyDetector(SimDetector):
+        imageplugin = Cpt(ImagePlugin, ImagePlugin._default_suffix)
+        statsplugin = Cpt(StatsPlugin, StatsPlugin._default_suffix)
+        colorconvplugin = Cpt(ColorConvPlugin, ColorConvPlugin._default_suffix)
+        processplugin = Cpt(ProcessPlugin, ProcessPlugin._default_suffix)
+        overlayplugin = Cpt(OverlayPlugin, OverlayPlugin._default_suffix)
+        roiplugin = Cpt(ROIPlugin, ROIPlugin._default_suffix)
+        transformplugin = Cpt(TransformPlugin, TransformPlugin._default_suffix)
+        netcdfplugin = Cpt(NetCDFPlugin, NetCDFPlugin._default_suffix)
+        tiffplugin = Cpt(TIFFPlugin, TIFFPlugin._default_suffix)
+        jpegplugin = Cpt(JPEGPlugin, JPEGPlugin._default_suffix)
+        # nexusplugin = Cpt(NexusPlugin, NexusPlugin._default_suffix)
+        hdf5plugin = Cpt(HDF5Plugin, HDF5Plugin._default_suffix)
+        # magickplugin = Cpt(MagickPlugin, MagickPlugin._default_suffix)
+
+    d = MyDetector(ad_prefix, name="d")
+    cleanup.add(d)
+    d.stage()
+    {n: getattr(d, n).read_configuration() for n in d.component_names}
+    {n: getattr(d, n).describe_configuration() for n in d.component_names}
+    d.unstage()
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_bluesky_protocols.py` & `ophyd-1.8.0/ophyd/tests/test_bluesky_protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from mypy import api
 
-
 imports = ""
 imports += "import ophyd;"
 imports += "from ophyd import flyers, sim;"
 imports += "hw = sim.hw();"
 
 
 def run(cmd):
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_device.py` & `ophyd-1.8.0/ophyd/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/tests/test_docs.py` & `ophyd-1.8.0/ophyd/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/tests/test_epicsmotor.py` & `ophyd-1.8.0/ophyd/tests/test_epicsmotor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import time
 import logging
-import pytest
+import threading
+import time
 from copy import copy
+
+import pytest
 from numpy.testing import assert_allclose
 
-from ophyd import (
-    EpicsMotor,
-    Component as Cpt,
-    MotorBundle,
-)
-from ophyd.utils.epics_pvs import AlarmSeverity, AlarmStatus
+from ophyd import Component as Cpt
+from ophyd import EpicsMotor, MotorBundle
 from ophyd.utils import UnknownStatusFailure
-import threading
+from ophyd.utils.epics_pvs import AlarmSeverity, AlarmStatus
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.motorsim
 def test_timeout(motor):
     assert motor.timeout == 10.0
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_flyers.py` & `ophyd-1.8.0/ophyd/tests/test_flyers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import time
+
 import pytest
 
+from ophyd import Component as Cpt
 from ophyd import (
-    Component as Cpt,
+    Device,
+    EpicsMotor,
+    ProcessPlugin,
+    ROIPlugin,
     SimDetector,
     SimDetectorCam,
     StatsPlugin,
-    EpicsMotor,
-    ROIPlugin,
-    ProcessPlugin,
-    Device,
 )
 from ophyd.areadetector.base import EpicsSignalWithRBV
 from ophyd.flyers import (
     AreaDetectorTimeseriesCollector,
-    WaveformCollector,
     MonitorFlyerMixin,
+    WaveformCollector,
 )
 from ophyd.status import wait
 
 
 @pytest.fixture(scope="function")
 def ts_sim_detector(ad_prefix):
     class Detector(SimDetector):
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_hints.py` & `ophyd-1.8.0/ophyd/tests/test_hints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ophyd import Device, Component, Signal, MotorBundle, Kind
+from ophyd import Component, Device, Kind, MotorBundle, Signal
 from ophyd.sim import SynAxis
 
 
 def test_device_hints():
     # Default hints is 'fields' with an empty list.
     assert {"fields": []} == Device("", name="dev").hints
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_issue944.py` & `ophyd-1.8.0/ophyd/tests/test_issue944.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/tests/test_kind.py` & `ophyd-1.8.0/ophyd/tests/test_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from ophyd import (
-    Device,
-    Signal,
-    Kind,
-    Component,
-    ALL_COMPONENTS,
-    kind_context,
-    DynamicDeviceComponent as DDCpt,
-)
 import pytest
 
+from ophyd import ALL_COMPONENTS, Component, Device
+from ophyd import DynamicDeviceComponent as DDCpt
+from ophyd import Kind, Signal, kind_context
+
 
 def test_standalone_signals():
     # A object's kind only matters when we read its _parent_. It affects
     # whether its parent recursively calls read() and/or read_configuration().
     # When we call read() and/or read_configuration() on the object itself,
     # directly, and its 'kind' setting does not affects its behavior.
     normal_sig = Signal(name="normal_sig", value=3, kind=Kind.normal)
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_log.py` & `ophyd-1.8.0/ophyd/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/tests/test_mca.py` & `ophyd-1.8.0/ophyd/tests/test_mca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
-import pytest
-
 from types import SimpleNamespace
 
-from ophyd import EpicsMCA, EpicsDXP
-from ophyd.mca import add_rois, Mercury1, SoftDXPTrigger
-
-from ophyd.utils import enum, ReadOnlyError
-
+import pytest
 from caproto.tests.conftest import run_example_ioc
 
+from ophyd import EpicsDXP, EpicsMCA
+from ophyd.mca import Mercury1, SoftDXPTrigger, add_rois
+from ophyd.utils import ReadOnlyError, enum
+
 MCAMode = enum(PHA="PHA", MCS="MCS", List="List")
 DxpPresetMode = enum(
     No_preset="No preset", Real_time="Real time", Live_time="Live time"
 )
 
 logger = logging.getLogger(__name__)
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_ophydobj.py` & `ophyd-1.8.0/ophyd/tests/test_ophydobj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
-import pytest
 import time
-
 from unittest.mock import Mock
+
+import pytest
+
 from ophyd.ophydobj import (
     OphydObject,
-    register_instances_keyed_on_name,
     register_instances_in_weakset,
+    register_instances_keyed_on_name,
 )
-from ophyd.status import StatusBase, DeviceStatus, wait
+from ophyd.status import DeviceStatus, StatusBase, wait
 from ophyd.utils import WaitTimeoutError
 
 logger = logging.getLogger(__name__)
 
 
 def test_status_basic():
     st = StatusBase()
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_positioner.py` & `ophyd-1.8.0/ophyd/tests/test_positioner.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
-import pytest
 import unittest
-
 from copy import copy
 from unittest import mock
 from unittest.mock import Mock
 
+import pytest
+
 from .. import SoftPositioner
 from ..utils import LimitError
 
 logger = logging.getLogger(__name__)
 
 
 def test_positioner_settle():
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_pseudopos.py` & `ophyd-1.8.0/ophyd/tests/test_pseudopos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-import time
 import logging
-
-import pytest
 import operator
-import numpy as np
-
-
+import time
 from copy import copy
 
-from ophyd.epics_motor import EpicsMotor
-from ophyd.pseudopos import PseudoPositioner, PseudoSingle
+import numpy as np
+import pytest
 
 from ophyd import Component as C
+from ophyd.epics_motor import EpicsMotor
+from ophyd.pseudopos import PseudoPositioner, PseudoSingle
 from ophyd.utils import ExceptionBundle
 
 logger = logging.getLogger(__name__)
 
 
 def setUpModule():
     logging.getLogger("ophyd.pseudopos").setLevel(logging.DEBUG)
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_pvpositioner.py` & `ophyd-1.8.0/ophyd/tests/test_pvpositioner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
-import pytest
 import time
 from copy import copy
 
+import pytest
+
+from ophyd import Component as Cpt
 from ophyd import (
-    PVPositioner,
-    PVPositionerPC,
     EpicsSignal,
     EpicsSignalRO,
-    Component as Cpt,
-    get_cl,
     Kind,
-    PVPositionerIsClose,
+    PVPositioner,
     PVPositionerDone,
+    PVPositionerIsClose,
+    PVPositionerPC,
+    get_cl,
 )
 from ophyd.utils.epics_pvs import _wait_for_value
 
 logger = logging.getLogger(__name__)
 
 
 def setUpModule():
@@ -71,15 +72,15 @@
     m = MyPositioner(motor.prefix, name="pos_no_put_compl")
     m.wait_for_connection()
 
     m.read()
 
     motor.move(0.1, wait=True)
     time.sleep(1)
-    assert m.position == 0.1
+    assert m.position == pytest.approx(0.1)
 
     m.stop()
     m.limits
 
     repr(m)
     str(m)
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_quadem.py` & `ophyd-1.8.0/ophyd/tests/test_quadem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
+
 import pytest
 
-from ophyd import QuadEM, Kind
-from ophyd.sim import make_fake_device, clear_fake_device
+from ophyd import Kind, QuadEM
 from ophyd.areadetector.plugins import ImagePlugin, StatsPlugin
-
+from ophyd.sim import clear_fake_device, make_fake_device
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="function")
 def quadem():
     FakeQuadEM = make_fake_device(QuadEM)
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_scaler.py` & `ophyd-1.8.0/ophyd/tests/test_scaler.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
-import pytest
 import time
-
 from copy import copy
 from types import SimpleNamespace
 
+import pytest
+from caproto.tests.conftest import run_example_ioc
+
 from ophyd.scaler import EpicsScaler, ScalerCH
 from ophyd.utils import enum
-from .test_utils import assert_OD_equal_ignore_ts
 
-from caproto.tests.conftest import run_example_ioc
+from .test_utils import assert_OD_equal_ignore_ts
 
 ScalerMode = enum(ONE_SHOT=0, AUTO_COUNT=1)
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="function")
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_signal.py` & `ophyd-1.8.0/ophyd/tests/test_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+import copy
 import logging
+import threading
 import time
-import copy
+
 import pytest
-import threading
 
 from ophyd import get_cl
+from ophyd.areadetector.paths import EpicsPathSignal
 from ophyd.signal import (
-    Signal,
+    DerivedSignal,
     EpicsSignal,
+    EpicsSignalNoValidation,
     EpicsSignalRO,
-    DerivedSignal,
     InternalSignal,
     InternalSignalError,
-    EpicsSignalNoValidation,
+    Signal,
 )
-from ophyd.utils import ReadOnlyError, AlarmStatus, AlarmSeverity
 from ophyd.status import wait
-from ophyd.areadetector.paths import EpicsPathSignal
+from ophyd.utils import AlarmSeverity, AlarmStatus, ReadOnlyError
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="function")
 def ro_signal(cleanup, signal_test_ioc):
     sig = EpicsSignalRO(signal_test_ioc.pvs["pair_rbv"], name="pair_rbv")
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_signalpositioner.py` & `ophyd-1.8.0/ophyd/tests/test_signalpositioner.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import time
-import pytest
 from copy import copy
 from unittest import mock
 from unittest.mock import Mock
 
+import pytest
+
 from ophyd.mixins import EpicsSignalPositioner
-from ophyd.utils import record_field
 from ophyd.status import wait
+from ophyd.utils import record_field
 
 from .config import motor_recs
 
-
 logger = logging.getLogger(__name__)
 
 
 def setUpModule():
     logging.getLogger("ophyd.mixins").setLevel(logging.DEBUG)
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_sim.py` & `ophyd-1.8.0/ophyd/tests/test_sim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+import shutil
+import tempfile
+from typing import Callable
+
+import numpy as np
+import pytest
+
+from ophyd.areadetector.base import EpicsSignalWithRBV
+from ophyd.areadetector.paths import EpicsPathSignal
+from ophyd.device import Component as Cpt
+from ophyd.device import Device
+from ophyd.device import DynamicDeviceComponent as DDCpt
+from ophyd.device import FormattedComponent as FCpt
+from ophyd.signal import EpicsSignal, EpicsSignalRO, Signal
 from ophyd.sim import (
-    SynGauss,
-    Syn2DGauss,
-    SynAxis,
-    make_fake_device,
+    FakeEpicsPathSignal,
     FakeEpicsSignal,
     FakeEpicsSignalRO,
     FakeEpicsSignalWithRBV,
-    FakeEpicsPathSignal,
+    Syn2DGauss,
+    SynAxis,
+    SynAxisEmptyHints,
+    SynAxisNoHints,
+    SynAxisNoPosition,
+    SynGauss,
+    SynSignalWithRegistry,
     clear_fake_device,
     instantiate_fake_device,
-    SynSignalWithRegistry,
-)
-from ophyd.device import (
-    Device,
-    Component as Cpt,
-    FormattedComponent as FCpt,
-    DynamicDeviceComponent as DDCpt,
+    make_fake_device,
 )
-from ophyd.signal import Signal, EpicsSignal, EpicsSignalRO
-from ophyd.areadetector.base import EpicsSignalWithRBV
-from ophyd.areadetector.paths import EpicsPathSignal
-from ophyd.utils import ReadOnlyError, LimitError, DisconnectedError
-import numpy as np
-import pytest
-import tempfile
-import shutil
+from ophyd.utils import DisconnectedError, LimitError, ReadOnlyError
 
 
 def test_random_state_gauss1d():
     """With given random state, the output value should stay the same.
     Test performs on 1D gaussian.
     """
     dlist = []
@@ -94,23 +98,58 @@
         )
         noisy_det.trigger()
         d = noisy_det.read()["noisy_det"]["value"]
         dlist.append(d)
     assert dlist[0] == dlist[1]
 
 
-def test_synaxis_subcribe():
+@pytest.mark.parametrize("events_per_move", [0, -1, -10])
+def test_synaxis_requires_at_least_1_event_per_move(events_per_move):
+    with pytest.raises(ValueError):
+        SynAxis(name="motor1", events_per_move=0)
+
+
+@pytest.mark.parametrize(
+    "motor_factory",
+    [
+        lambda: SynAxis(name="motor", value=0.0),
+        lambda: SynAxisEmptyHints(name="motor", value=0.0),
+        lambda: SynAxisNoHints(name="motor", value=0.0),
+        lambda: SynAxisNoPosition(name="motor", value=0.0),
+    ],
+)
+def test_move_synaxis(motor_factory: Callable[[], SynAxis]):
+    # Test is run twice, once for caproto and once for pyepics, so we need a
+    # factory rather than a global object to preserve state management
+    motor = motor_factory()
+
+    initial_value = motor.readback.get()
+    motor.set(1.0).wait()
+    final_value = motor.readback.get()
+
+    assert initial_value == 0.0
+    assert final_value == 1.0
+
+
+def test_synaxisnoposition_has_no_position():
+    motor = SynAxisNoPosition(name="motor", labels={"motors"})
+    with pytest.raises(AttributeError):
+        motor.position
+
+
+@pytest.mark.parametrize("events_per_move", [1, 2, 6, 20])
+def test_synaxis_subcribe(events_per_move: int):
     hits = dict.fromkeys(["r", "s", "a"], 0)
     vals = dict.fromkeys(["r", "s", "a"], None)
 
     def p1(tar, value):
         hits[tar] += 1
         vals[tar] = value
 
-    motor = SynAxis(name="motor1")
+    motor = SynAxis(name="motor1", events_per_move=events_per_move)
     # prime the cb cache so these run an subscription
     motor.set(0)
     motor.subscribe(lambda *, value, _tar="a", **kwargs: p1(_tar, value))
     motor.readback.subscribe(lambda *, value, _tar="r", **kwargs: p1(_tar, value))
     motor.setpoint.subscribe(lambda *, value, _tar="s", **kwargs: p1(_tar, value))
 
     assert vals["r"] == motor.readback.get()
@@ -121,21 +160,24 @@
 
     motor.set(1)
 
     assert vals["r"] == motor.readback.get()
     assert vals["a"] == motor.readback.get()
     assert vals["s"] == motor.setpoint.get()
 
-    assert all(v == 2 for v in hits.values())
+    assert hits["r"] == 1 + events_per_move
+    assert hits["a"] == 1 + events_per_move
+    assert hits["s"] == 2
 
 
 def test_synaxis_timestamps():
-    from ophyd.status import wait
     import time
 
+    from ophyd.status import wait
+
     def time_getter(m):
         return {k: v["timestamp"] for k, v in m.read().items()}
 
     def tester(m, orig_time):
         new_time = time_getter(m)
         assert orig_time != new_time
         return new_time
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_status.py` & `ophyd-1.8.0/ophyd/tests/test_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import time
 from unittest.mock import Mock
 
+import pytest
+
 from ophyd import Device
-from ophyd.status import StatusBase, SubscriptionStatus, UseNewProperty, MoveStatus
+from ophyd.status import MoveStatus, StatusBase, SubscriptionStatus, UseNewProperty
 from ophyd.utils import (
     InvalidState,
-    UnknownStatusFailure,
     StatusTimeoutError,
+    UnknownStatusFailure,
     WaitTimeoutError,
 )
-import pytest
 
 
 def _setup_state_and_cb(new_signature=True):
     state = {}
 
     if new_signature:
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_timeout.py` & `ophyd-1.8.0/ophyd/tests/test_timeout.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
+
 import pytest
-from ophyd import Device, Component
 
-from ophyd import EpicsSignal
+from ophyd import Component, Device, EpicsSignal
 
 logger = logging.getLogger(__name__)
 
 
 def test_timeout():
     class SubSubDevice(Device):
         cpt5 = Component(EpicsSignal, "5")
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_timestamps.py` & `ophyd-1.8.0/ophyd/tests/test_timestamps.py`

 * *Ordering differences only*

 * *Files identical despite different names*

```diff
@@ -1,14 +1,14 @@
-import time
 import logging
-import pytest
-from ophyd import EpicsSignal, EpicsSignalRO
+import time
 
+import pytest
 from numpy.testing import assert_almost_equal
 
+from ophyd import EpicsSignal, EpicsSignalRO
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.motorsim
 def test_read_pv_timestamp_no_monitor(motor):
     motor.set(0, wait=True)
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_units.py` & `ophyd-1.8.0/ophyd/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/tests/test_utils.py` & `ophyd-1.8.0/ophyd/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import pytest
-import os
 import logging
-import numpy as np
+import os
 import tempfile
 
+import numpy as np
+import pytest
+
+from ophyd import Signal
 from ophyd.utils import epics_pvs as epics_utils
 from ophyd.utils import make_dir_tree, makedirs
-from ophyd import Signal
-
 
 logger = logging.getLogger(__name__)
 
 
 def test_split():
     utils = epics_utils
```

### Comparing `ophyd-1.7.0/ophyd/tests/test_versioning.py` & `ophyd-1.8.0/ophyd/tests/test_versioning.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import pytest
 import logging
-from ophyd import Device
 
+import pytest
+
+from ophyd import Device
 
 logger = logging.getLogger(__name__)
 
 
 def test_specify_version():
     # Define a versioned Device:
     class MyDevice(Device, version=1, version_type="ioc"):
```

### Comparing `ophyd-1.7.0/ophyd/units.py` & `ophyd-1.8.0/ophyd/units.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/utils/__init__.py` & `ophyd-1.8.0/ophyd/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # vi: ts=4 sw=4 sts=4 expandtab
 import inspect
 import logging
-from collections import OrderedDict
 import warnings
+from collections import OrderedDict
 
-from .errors import *  # noqa: F401, F403
 from .epics_pvs import *  # noqa: F401, F403
-from .paths import makedirs, make_dir_tree  # noqa: F401
+from .errors import *  # noqa: F401, F403
+from .paths import make_dir_tree, makedirs  # noqa: F401
 
 logger = logging.getLogger(__name__)
 
 
 def enum(**enums):
     """Create an enum from the keyword arguments"""
     return type("Enum", (object,), enums)
```

### Comparing `ophyd-1.7.0/ophyd/utils/epics_pvs.py` & `ophyd-1.8.0/ophyd/utils/epics_pvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # vi: ts=4 sw=4 sts=4 expandtab
-from enum import IntEnum
-import time as ttime
-import logging
 import functools
-import numpy as np
+import logging
+import time as ttime
 import typing
-
 import warnings
+from enum import IntEnum
 
-from .errors import DisconnectedError, OpException
+import numpy as np
 
+from .errors import DisconnectedError, OpException
 
 __all__ = [
     "split_record_field",
     "strip_field",
     "record_field",
     "set_and_wait",
     "AlarmStatus",
@@ -141,15 +140,17 @@
     Returns
     -------
     records : list
         [(record type, record name), ...]
     """
 
     ret = []
-    for line in open(fn, "rt").readlines():
+    with open(fn, "rt") as f:
+        lines = f.readlines()
+    for line in lines:
         line = line.strip()
 
         if line.startswith("#"):
             continue
 
         if not (line.startswith("record") or line.startswith("grecord")):
             continue
```

### Comparing `ophyd-1.7.0/ophyd/utils/errors.py` & `ophyd-1.8.0/ophyd/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ophyd-1.7.0/ophyd/utils/paths.py` & `ophyd-1.8.0/ophyd/utils/paths.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import os
 import calendar
+import os
 
 
-def makedirs(path, *, mode=0o777, mode_base=None):
+def makedirs(path, *, mode=0o755, mode_base=None):
     """Recursively make directories and set permissions
 
     Parameters
     ----------
     path : str
         Full path to create, including all parent directories
     mode : int, optional
@@ -32,24 +32,24 @@
     if not mode_base or os.path.commonprefix((mode_base, path)) == mode_base:
         os.chmod(path, mode)
 
     ret.append(path)
     return ret
 
 
-def make_dir_tree(year, *, base_path=None, mode=0o777):
+def make_dir_tree(year, *, base_path=None, mode=0o755):
     """Make full directory tree for the year
 
     Parameters
     ----------
     year : int
     base_path : str, optional
         If unspecified, defaults to the current directory
     mode : int, optional
-        File mode to set for permissions (default: 0o777)
+        File mode to set for permissions (default: 0o755)
 
     Returns
     -------
     paths : list
         List of directories created
     """
     if base_path is None:
```

### Comparing `ophyd-1.7.0/ophyd.egg-info/PKG-INFO` & `ophyd-1.8.0/ophyd.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 Metadata-Version: 2.1
 Name: ophyd
-Version: 1.7.0
+Version: 1.8.0
+Summary: Bluesky hardware abstraction with an emphasis on EPICS
+Home-page: https://github.com/bluesky/ophyd
 License: BSD
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: ca
+Provides-Extra: pva
+Provides-Extra: dev
 License-File: LICENSE
 
 *****
 Ophyd
 *****
 
 |build_status| |coverage| |pypi_version| |license|
 
-Ophyd is Python library for interfacing with hardware. It provides an
-abstraction layer than enables experiment orchestration and data acquisition
+Ophyd is a Python library for interfacing with hardware. It provides an
+abstraction layer that enables experiment orchestration and data acquisition
 code to operate above the specifics of particular devices and control systems.
 
 Ophyd is typically used with the `Bluesky Run Engine`_ for experiment
-orchestration and data acquistion. It is also sometimes used in a stand-alone
+orchestration and data acquisition. It is also sometimes used in a stand-alone
 fashion.
 
 Many facilities use ophyd to integrate with control systems that use `EPICS`_ ,
 but ophyd's design and some of its objects are also used to integrate with
 other control systems.
 
 * Put the details specific to a device or control system behind a **high-level
   interface** with methods like ``trigger()``, ``read()``, and ``set(...)``.
 * **Group** individual control channels (such as EPICS V3 PVs) into logical
-  "Devices" to be configured and used as units with internal coordiantion.
+  "Devices" to be configured and used as units with internal coordination.
 * Assign readings with **names meaningful for data analysis** that will
   propagate into metadata.
 * **Categorize** readings by "kind" (primary reading, configuration,
   engineering/debugging) which can be read selectively.
 
 ============== ==============================================================
 PyPI           ``pip install ophyd``
-Conda          ``pip install -c nsls2forge ophyd``
+Conda          ``conda install -c conda-forge ophyd``
 Source code    https://github.com/bluesky/ophyd
 Documentation  https://blueskyproject.io/ophyd
 ============== ==============================================================
 
 See the tutorials for usage examples.
 
 .. |build_status| image:: https://github.com/bluesky/ophyd/workflows/Unit%20Tests/badge.svg?branch=master
@@ -59,7 +66,13 @@
 .. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
     :target: https://opensource.org/licenses/BSD-3-Clause
     :alt: BSD 3-Clause License
 
 .. _Bluesky Run Engine: http://blueskyproject.io/bluesky
 
 .. _EPICS: http://www.aps.anl.gov/epics/
+
+..
+    Anything below this line is used when viewing README.rst and will be replaced
+    when included in index.rst
+
+See https://blueskyproject.io/ophyd for more detailed documentation.
```

