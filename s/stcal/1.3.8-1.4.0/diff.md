# Comparing `tmp/stcal-1.3.8.tar.gz` & `tmp/stcal-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stcal-1.3.8.tar", last modified: Wed May 31 17:06:43 2023, max compression
+gzip compressed data, was "stcal-1.4.0.tar", last modified: Tue Jun 27 19:10:26 2023, max compression
```

## Comparing `stcal-1.3.8.tar` & `stcal-1.4.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.497736 stcal-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.417734 stcal-1.3.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/label_pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-31 17:06:32.000000 stcal-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 17:06:32.000000 stcal-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-31 17:06:32.000000 stcal-1.3.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-31 17:06:32.000000 stcal-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-31 17:06:32.000000 stcal-1.3.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-31 17:06:32.000000 stcal-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-31 17:06:43.497736 stcal-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-31 17:06:32.000000 stcal-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-31 17:06:32.000000 stcal-1.3.8/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/docs/stcal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/docs/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/jump/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/jump/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/package_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/docs/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/ramp_fitting/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/ramp_fitting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-31 17:06:32.000000 stcal-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:06:43.497736 stcal-1.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.417734 stcal-1.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/src/stcal/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/dark_current/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dark_current/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dark_current/dark_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dark_current/dark_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dynamicdq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/jump/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/jump/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32158 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/jump/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/jump/twopoint_difference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/linearity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/linearity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/linearity/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)   126980 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/ols_fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/ramp_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/ramp_fit_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    56279 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/saturation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/saturation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/saturation/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/src/stcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:06:42.000000 stcal-1.3.8/src/stcal.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.461735 stcal-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/current_gdqfits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.497736 stcal-1.3.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/data/input_gdq_flarge.fits
--rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/data/large_event_input_dq_cube2.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/data/snowball1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    53269 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_ramp_fitting_gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43187 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_twopoint_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-31 17:06:32.000000 stcal-1.3.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.236657 stcal-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/label_pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-27 19:10:12.000000 stcal-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-27 19:10:12.000000 stcal-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-06-27 19:10:12.000000 stcal-1.4.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-27 19:10:12.000000 stcal-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-27 19:10:12.000000 stcal-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-27 19:10:12.000000 stcal-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-27 19:10:26.236657 stcal-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-27 19:10:12.000000 stcal-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-27 19:10:12.000000 stcal-1.4.0/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/docs/stcal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/docs/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/jump/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/jump/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/package_index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/docs/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/ramp_fitting/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/ramp_fitting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-27 19:10:12.000000 stcal-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:10:26.236657 stcal-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.124656 stcal-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/src/stcal/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/src/stcal/dark_current/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dark_current/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dark_current/dark_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dark_current/dark_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dynamicdq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.136656 stcal-1.4.0/src/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/jump/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/jump/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36348 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/jump/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/jump/twopoint_difference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.136656 stcal-1.4.0/src/stcal/linearity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/linearity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/linearity/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.136656 stcal-1.4.0/src/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127963 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/ols_fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/ramp_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/ramp_fit_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56323 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.136656 stcal-1.4.0/src/stcal/saturation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/saturation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/saturation/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/src/stcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-27 19:10:26.000000 stcal-1.4.0/src/stcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.184657 stcal-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/current_gdqfits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.236657 stcal-1.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/data/input_gdq_flarge.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/data/large_event_input_dq_cube2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/data/snowball1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53011 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_ramp_fitting_gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_twopoint_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-27 19:10:12.000000 stcal-1.4.0/tox.ini
```

### Comparing `stcal-1.3.8/.github/labeler.yml` & `stcal-1.4.0/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/.github/pull_request_template.md` & `stcal-1.4.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/.github/workflows/ci.yml` & `stcal-1.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/.github/workflows/publish-to-pypi.yml` & `stcal-1.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/.gitignore` & `stcal-1.4.0/.gitignore`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -139,8 +139,8 @@
 cython_debug/
 
 # setuptools-scm generated module
 src/stcal/_version.py
 
 # auto-generated API docs
 docs/source/api
-.DS_Store
+.DS_Store
```

### Comparing `stcal-1.3.8/.readthedocs.yaml` & `stcal-1.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/CHANGES.rst` & `stcal-1.4.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,34 @@
-1.4.0 (unreleased)
+1.4.0 (2023-06-27)
 ==================
 
 Bug Fixes
 ---------
 
--
+jump
+~~~~
+
+- Updated the jump detection to switch to using the numpy sigmaclip routine to
+  find the actual rms across integrations when there are at least 101 integrations
+  in the exposure. This still allows cosmic rays and snowballs/showers to be flagged
+  without being affected by slope variations due to either brigher-fatter/charge-spilling
+  or errors in the nonlinearity correction.
+  Also added the counting of the number of cosmic rays and snowballs/showers that
+  is then placed in the FITS header in the JWST routines. [#174]
+
+ramp_fitting
+~~~~~~~~~~~~
+
+- Changing where time division occurs during ramp fitting in order to
+  properly handle special cases where the time is not group time, such
+  as when ZEROFRAME data is used, so the time is frame time. [#173]
+
+- Added another line of code to be included in the section where warnings are turned
+  off. The large number of warnings can cause a hang in the Jupyter notebook when
+  running with multiprocessing. [#174]
 
 Changes to API
 --------------
 
 - 
 
 Other
```

### Comparing `stcal-1.3.8/CODE_OF_CONDUCT.md` & `stcal-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/CONTRIBUTING.md` & `stcal-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/LICENSE` & `stcal-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/PKG-INFO` & `stcal-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.3.8
+Version: 1.4.0
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.3.8/README.md` & `stcal-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/benchmarks/dark_current.py` & `stcal-1.4.0/benchmarks/dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/benchmarks/linearity.py` & `stcal-1.4.0/benchmarks/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/benchmarks/ramp_fitting.py` & `stcal-1.4.0/benchmarks/ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/benchmarks/saturation.py` & `stcal-1.4.0/benchmarks/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/docs/Makefile` & `stcal-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/docs/conf.py` & `stcal-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/docs/stcal/jump/description.rst` & `stcal-1.4.0/docs/stcal/jump/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/docs/stcal/ramp_fitting/description.rst` & `stcal-1.4.0/docs/stcal/ramp_fitting/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/pyproject.toml` & `stcal-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/src/stcal/dark_current/dark_class.py` & `stcal-1.4.0/src/stcal/dark_current/dark_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/src/stcal/dark_current/dark_sub.py` & `stcal-1.4.0/src/stcal/dark_current/dark_sub.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/src/stcal/dqflags.py` & `stcal-1.4.0/src/stcal/dqflags.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/src/stcal/jump/jump.py` & `stcal-1.4.0/src/stcal/jump/jump.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import multiprocessing
 import time
-
 import numpy as np
 import cv2 as cv
+import astropy.stats as stats
 
 from astropy.convolution import Ring2DKernel
 from astropy.convolution import convolve
 
 from . import constants
 from . import twopoint_difference as twopt
 
@@ -30,15 +30,16 @@
                  use_ellipses=False,
                  sat_required_snowball=True,
                  expand_large_events=False,
                  sat_expand=2, min_sat_radius_extend=2.5, find_showers=False,
                  edge_size=25, extend_snr_threshold=1.2, extend_min_area=90,
                  extend_inner_radius=1, extend_outer_radius=2.6,
                  extend_ellipse_expand_ratio=1.2, grps_masked_after_shower=5,
-                 max_extended_radius=200):
+                 max_extended_radius=200, minimum_groups=3,
+                 minimum_sigclip_groups=100, only_use_ints=True):
 
     """
     This is the high-level controlling routine for the jump detection process.
     It loads and sets the various input data and parameters needed by each of
     the individual detection methods and then calls the detection methods in
     turn.
 
@@ -194,14 +195,15 @@
 
     pdq : int, 2D array
         updated pixel dq array
     """
     constants.update_dqflags(dqflags)  # populate dq flags
     sat_flag = dqflags["SATURATED"]
     jump_flag = dqflags["JUMP_DET"]
+    number_extended_events = 0
     # Flag the pixeldq where the gain is <=0 or NaN so they will be ignored
     wh_g = np.where(gain_2d <= 0.)
     if len(wh_g[0] > 0):
         pdq[wh_g] = np.bitwise_or(pdq[wh_g], dqflags["NO_GAIN_VALUE"])
         pdq[wh_g] = np.bitwise_or(pdq[wh_g], dqflags["DO_NOT_USE"])
 
     wh_g = np.where(np.isnan(gain_2d))
@@ -242,36 +244,37 @@
         n_slices = max_available // 4 or 1
     elif max_cores == 'half':
         n_slices = max_available // 2 or 1
     elif max_cores == 'all':
         n_slices = max_available
 
     if n_slices == 1:
-        gdq, row_below_dq, row_above_dq = \
+        gdq, row_below_dq, row_above_dq, total_primary_crs, stddev = \
             twopt.find_crs(data, gdq, readnoise_2d, rejection_thresh,
                            three_grp_thresh, four_grp_thresh, frames_per_group,
                            flag_4_neighbors, max_jump_to_flag_neighbors,
                            min_jump_to_flag_neighbors, dqflags,
                            after_jump_flag_e1=after_jump_flag_e1,
                            after_jump_flag_n1=after_jump_flag_n1,
                            after_jump_flag_e2=after_jump_flag_e2,
-                           after_jump_flag_n2=after_jump_flag_n2)
-
+                           after_jump_flag_n2=after_jump_flag_n2, copy_arrs=False,
+                           minimum_groups=3, minimum_sigclip_groups=minimum_sigclip_groups,
+                           only_use_ints=only_use_ints)
         #  This is the flag that controls the flagging of either snowballs.
         if expand_large_events:
             flag_large_events(gdq, jump_flag, sat_flag, min_sat_area=min_sat_area,
                               min_jump_area=min_jump_area,
                               expand_factor=expand_factor,
                               sat_required_snowball=sat_required_snowball,
                               min_sat_radius_extend=min_sat_radius_extend,
                               edge_size=edge_size, sat_expand=sat_expand,
                               max_extended_radius=max_extended_radius)
         if find_showers:
             gdq, num_showers = find_faint_extended(data, gdq, readnoise_2d,
-                                                   frames_per_group,
+                                                   frames_per_group, minimum_sigclip_groups,
                                                    snr_threshold=extend_snr_threshold,
                                                    min_shower_area=extend_min_area,
                                                    inner=extend_inner_radius,
                                                    outer=extend_outer_radius,
                                                    sat_flag=sat_flag, jump_flag=jump_flag,
                                                    ellipse_expand=extend_ellipse_expand_ratio,
                                                    num_grps_masked=grps_masked_after_shower,
@@ -285,27 +288,28 @@
         #  four_grp_thresh, nframes)
 
         # must copy arrays here, find_crs will make copies but if slices
         # are being passed in for multiprocessing then the original gdq will be
         # modified unless copied beforehand
         gdq = gdq.copy()
         data = data.copy()
-        copy_arrs = False  # we dont need to copy arrays again in find_crs
+        copy_arrs = False  # we don't need to copy arrays again in find_crs
 
         for i in range(n_slices - 1):
             slices.insert(i, (data[:, :, i * yinc:(i + 1) * yinc, :],
                               gdq[:, :, i * yinc:(i + 1) * yinc, :],
                               readnoise_2d[i * yinc:(i + 1) * yinc, :],
                               rejection_thresh, three_grp_thresh, four_grp_thresh,
                               frames_per_group, flag_4_neighbors,
                               max_jump_to_flag_neighbors,
                               min_jump_to_flag_neighbors, dqflags,
                               after_jump_flag_e1, after_jump_flag_n1,
                               after_jump_flag_e2, after_jump_flag_n2,
-                              copy_arrs))
+                              copy_arrs, minimum_groups, minimum_sigclip_groups,
+                              only_use_ints))
 
         # last slice get the rest
         slices.insert(n_slices - 1, (data[:, :, (n_slices - 1) *
                                      yinc:n_rows, :],
                                      gdq[:, :, (n_slices - 1) *
                                      yinc:n_rows, :],
                                      readnoise_2d[(n_slices - 1) *
@@ -313,34 +317,53 @@
                                      rejection_thresh, three_grp_thresh,
                                      four_grp_thresh, frames_per_group,
                                      flag_4_neighbors,
                                      max_jump_to_flag_neighbors,
                                      min_jump_to_flag_neighbors, dqflags,
                                      after_jump_flag_e1, after_jump_flag_n1,
                                      after_jump_flag_e2, after_jump_flag_n2,
-                                     copy_arrs))
+                                     copy_arrs, minimum_groups, minimum_sigclip_groups,
+                                     only_use_ints))
         log.info("Creating %d processes for jump detection " % n_slices)
         pool = multiprocessing.Pool(processes=n_slices)
         # Starts each slice in its own process. Starmap allows more than one
         # parameter to be passed.
         real_result = pool.starmap(twopt.find_crs, slices)
         pool.close()
         pool.join()
         k = 0
 
         # Reconstruct gdq, the row_above_gdq, and the row_below_gdq from the
         # slice result
+        total_primary_crs = 0
+        ngrps = gdq.shape[1]
+        nrows = gdq.shape[2]
+        ncols = gdq.shape[3]
+        if only_use_ints:
+            stddev = np.zeros((ngrps - 1, nrows, ncols),
+                              dtype=np.float32)
+        else:
+            stddev = np.zeros((nrows, ncols),
+                              dtype=np.float32)
         for resultslice in real_result:
-
             if len(real_result) == k + 1:  # last result
                 gdq[:, :, k * yinc:n_rows, :] = resultslice[0]
+                if only_use_ints:
+                    stddev[:, k * yinc:n_rows, :] = resultslice[4]
+                else:
+                    stddev[k * yinc:n_rows, :] = resultslice[4]
             else:
                 gdq[:, :, k * yinc:(k + 1) * yinc, :] = resultslice[0]
+                if only_use_ints:
+                    stddev[:, k * yinc:(k + 1) * yinc, :] = resultslice[4]
+                else:
+                    stddev[k * yinc:(k + 1) * yinc, :] = resultslice[4]
             row_below_gdq[:, :, :] = resultslice[1]
             row_above_gdq[:, :, :] = resultslice[2]
+            total_primary_crs += resultslice[3]
             if k != 0:
                 # For all but the first slice, flag any CR neighbors in the top
                 # row of the previous slice and flag any neighbors in the
                 # bottom row of this slice saved from the top of the previous
                 # slice
                 gdq[:, :, k * yinc - 1, :] = \
                     np.bitwise_or(gdq[:, :, k * yinc - 1, :],
@@ -348,50 +371,53 @@
                 gdq[:, :, k * yinc, :] = \
                     np.bitwise_or(gdq[:, :, k * yinc, :],
                                   previous_row_above_gdq[:, :, :])
 
             # save the neighbors to be flagged that will be in the next slice
             previous_row_above_gdq = row_above_gdq.copy()
             k += 1
-
         #  This is the flag that controls the flagging of either
         #  snowballs or showers.
         if expand_large_events:
-            flag_large_events(gdq, jump_flag, sat_flag,
+            total_snowballs = flag_large_events(gdq, jump_flag, sat_flag,
                               min_sat_area=min_sat_area,
                               min_jump_area=min_jump_area,
                               expand_factor=expand_factor,
                               sat_required_snowball=sat_required_snowball,
                               min_sat_radius_extend=min_sat_radius_extend,
                               edge_size=edge_size, sat_expand=sat_expand,
                               max_extended_radius=max_extended_radius)
+            log.info('Total snowballs = %i' % total_snowballs)
+            number_extended_events = total_snowballs
         if find_showers:
             gdq, num_showers = \
                 find_faint_extended(data, gdq, readnoise_2d,
-                                    frames_per_group,
+                                    frames_per_group, minimum_sigclip_groups,
                                     snr_threshold=extend_snr_threshold,
                                     min_shower_area=extend_min_area,
                                     inner=extend_inner_radius,
                                     outer=extend_outer_radius,
                                     sat_flag=sat_flag,
                                     jump_flag=jump_flag,
                                     ellipse_expand=extend_ellipse_expand_ratio,
                                     num_grps_masked=grps_masked_after_shower,
                                     max_extended_radius=max_extended_radius)
+            log.info('Total showers= %i' % num_showers)
+            number_extended_events = num_showers
     elapsed = time.time() - start
     log.info('Total elapsed time = %g sec' % elapsed)
 
     # Back out the applied gain to the SCI, ERR, and readnoise arrays so they're
     #    back in units of DN
     data /= gain_2d
     err /= gain_2d
     readnoise_2d /= gain_2d
 
     # Return the updated data quality arrays
-    return gdq, pdq
+    return gdq, pdq, total_primary_crs, number_extended_events, stddev
 
 
 def flag_large_events(gdq, jump_flag, sat_flag, min_sat_area=1,
                       min_jump_area=6,
                       expand_factor=2.0,
                       sat_required_snowball=True, min_sat_radius_extend=2.5,
                       sat_expand=2, edge_size=25, max_extended_radius=200):
@@ -438,56 +464,58 @@
     Nothing, gdq array is modified.
 
     """
 
     log.info('Flagging large Snowballs')
 
     n_showers_grp = []
-    for integration in range(gdq.shape[0]):
-        for group in range(1, gdq.shape[1]):
+    total_snowballs = 0
+    nints = gdq.shape[0]
+    ngrps = gdq.shape[1]
+    for integration in range(nints):
+        for group in range(1, ngrps):
             current_gdq = 1.0 * gdq[integration, group, :, :]
             prev_gdq = 1.0 * gdq[integration, group - 1, :, :]
             diff_gdq = 1.0 * current_gdq - prev_gdq
             diff_gdq[diff_gdq != sat_flag] = 0
             new_sat = diff_gdq.astype('uint8')
             # find the ellipse parameters for newly saturated pixels
             sat_ellipses = find_ellipses(new_sat, sat_flag, min_sat_area)
 
             # find the ellipse parameters for jump regions
             jump_ellipses = find_ellipses(gdq[integration, group, :, :],
                                           jump_flag, min_jump_area)
             if sat_required_snowball:
                 low_threshold = edge_size
-                high_threshold = max(0, gdq.shape[2] - edge_size)
+                nrows = gdq.shape[2]
+                high_threshold = max(0, nrows - edge_size)
 
                 gdq, snowballs = make_snowballs(gdq, integration, group,
                                                 jump_ellipses, sat_ellipses,
                                                 low_threshold, high_threshold,
                                                 min_sat_radius_extend,
                                                 sat_expand, sat_flag,
                                                 max_extended_radius)
             else:
                 snowballs = jump_ellipses
             n_showers_grp.append(len(snowballs))
+            total_snowballs += len(snowballs)
             gdq, num_events = extend_ellipses(gdq, integration, group,
                                               snowballs,
                                               sat_flag, jump_flag,
                                               expansion=expand_factor,
                                               max_extended_radius=max_extended_radius)
-        if np.all(np.array(n_showers_grp) == 0):
-            log.info(f'No snowballs found in integration {integration}.')
-        else:
-            log.info(f' In integration {integration}, number of snowballs ' +
-                     f'in each group = {n_showers_grp}')
-
+    return total_snowballs
 
 def extend_saturation(cube, grp, sat_ellipses, sat_flag,
                       min_sat_radius_extend, expansion=2,
                       max_extended_radius=200):
-    image = np.zeros(shape=(cube.shape[1], cube.shape[2], 3), dtype=np.uint8)
+    ncols = cube.shape[2]
+    nrows = cube.shape[1]
+    image = np.zeros(shape=(nrows, ncols, 3), dtype=np.uint8)
     outcube = cube.copy()
     for ellipse in sat_ellipses:
         ceny = ellipse[0][0]
         cenx = ellipse[0][1]
         minor_axis = min(ellipse[1][1], ellipse[1][0])
         if minor_axis > min_sat_radius_extend:
             axis1 = ellipse[1][0] + expansion
@@ -507,15 +535,17 @@
 def extend_ellipses(gdq_cube, intg, grp, ellipses, sat_flag, jump_flag,
                     expansion=1.9, expand_by_ratio=True,
                     num_grps_masked=1, max_extended_radius=200):
     # For a given DQ plane it will use the list of ellipses to create
     #  expanded ellipses of pixels with
     # the jump flag set.
     plane = gdq_cube[intg, grp, :, :]
-    image = np.zeros(shape=(plane.shape[0], plane.shape[1], 3), dtype=np.uint8)
+    ncols = plane.shape[1]
+    nrows = plane.shape[0]
+    image = np.zeros(shape=(nrows, ncols, 3), dtype=np.uint8)
     num_ellipses = len(ellipses)
     for ellipse in ellipses:
         ceny = ellipse[0][0]
         cenx = ellipse[0][1]
         # Expand the ellipse by the expansion factor. The number of pixels
         # added to both axes is
         # the number of pixels added to the minor axis. This prevents very
@@ -536,15 +566,16 @@
         axis1 = min(axis1, max_extended_radius)
         axis2 = min(axis2, max_extended_radius)
         alpha = ellipse[2]
         image = cv.ellipse(image, (round(ceny), round(cenx)), (round(axis1 / 2),
                            round(axis2 / 2)), alpha, 0, 360,
                            (0, 0, jump_flag), -1)
         jump_ellipse = image[:, :, 2]
-        last_grp = min(grp + num_grps_masked, gdq_cube.shape[1])
+        ngrps = gdq_cube.shape[1]
+        last_grp = min(grp + num_grps_masked, ngrps)
         #  This loop will flag the number of groups
         for flg_grp in range(grp, last_grp):
             sat_pix = np.bitwise_and(gdq_cube[intg, flg_grp, :, :], sat_flag)
             saty, satx = np.where(sat_pix == sat_flag)
             jump_ellipse[saty, satx] = 0
             gdq_cube[intg, flg_grp, :, :] = \
                 np.bitwise_or(gdq_cube[intg, flg_grp, :, :], jump_ellipse)
@@ -622,15 +653,16 @@
     if jump[0][0] < low_threshold or jump[0][1] < low_threshold\
             or jump[0][0] > high_threshold or jump[0][1] > high_threshold:
         return True
     else:
         return False
 
 
-def find_faint_extended(indata, gdq, readnoise_2d, nframes, snr_threshold=1.3,
+def find_faint_extended(indata, gdq, readnoise_2d, nframes, minimum_sigclip_groups,
+                        snr_threshold=1.3,
                         min_shower_area=40, inner=1, outer=2, sat_flag=2,
                         jump_flag=4, ellipse_expand=1.1, num_grps_masked=25,
                         max_extended_radius=200):
     """
     Parameters
     ----------
       indata : float, 4D array
@@ -671,54 +703,104 @@
     """
     read_noise_2 = readnoise_2d**2
     data = indata.copy()
     data[gdq == sat_flag] = np.nan
     data[gdq == 1] = np.nan
     data[gdq == jump_flag] = np.nan
     all_ellipses = []
-    for intg in range(data.shape[0]):
-        diff = np.diff(data[intg], axis=0)
-        median_diffs = np.nanmedian(diff, axis=0)
+    first_diffs = np.diff(data, axis=1)
+    first_diffs_masked = np.ma.masked_array(first_diffs, mask=np.isnan(first_diffs))
+    nints = data.shape[0]
+    if nints > minimum_sigclip_groups:
+        mean, median, stddev = stats.sigma_clipped_stats(first_diffs_masked, sigma=5,
+                                                         axis=0)
+    for intg in range(nints):
         # calculate sigma for each pixel
-        sigma = np.sqrt(np.abs(median_diffs) + read_noise_2 / nframes)
-
-        # The difference from the median difference for each group
-        e_jump = diff - median_diffs[np.newaxis, :, :]
-
-        ratio = np.abs(e_jump) / sigma[np.newaxis, :, :]  # SNR ratio of
-        # each diff.
+        if nints <= minimum_sigclip_groups:
+            median_diffs = np.nanmedian(first_diffs_masked[intg], axis=0)
+            sigma = np.sqrt(np.abs(median_diffs) + read_noise_2 / nframes)
+            # The difference from the median difference for each group
+            e_jump = first_diffs_masked[intg] - median_diffs[np.newaxis, :, :]
+            # SNR ratio of each diff.
+            ratio = np.abs(e_jump) / sigma[np.newaxis, :, :]
 
         #  The convolution kernal creation
         ring_2D_kernel = Ring2DKernel(inner, outer)
-        for grp in range(1, ratio.shape[0] + 1):
+        ngrps = data.shape[1]
+        for grp in range(1, ngrps):
+            if nints > minimum_sigclip_groups:
+                median_diffs = median[grp-1]
+                sigma = stddev[grp-1]
+                # The difference from the median difference for each group
+                e_jump = first_diffs_masked[intg] - median_diffs[np.newaxis, :, :]
+                # SNR ratio of each diff.
+                ratio = np.abs(e_jump) / sigma[np.newaxis, :, :]
             masked_ratio = ratio[grp-1].copy()
             jumpy, jumpx = np.where(gdq[intg, grp, :, :] == jump_flag)
             #  mask pix. that are already flagged as jump
             masked_ratio[jumpy, jumpx] = np.nan
 
             saty, satx = np.where(gdq[intg, grp, :, :] == sat_flag)
 
             #  mask pix. that are already flagged as sat.
             masked_ratio[saty, satx] = np.nan
 
             masked_smoothed_ratio = convolve(masked_ratio, ring_2D_kernel)
-            extended_emission = np.zeros(shape=(ratio.shape[1],
-                                                ratio.shape[2]), dtype=np.uint8)
+            nrows = ratio.shape[1]
+            ncols = ratio.shape[2]
+            extended_emission = np.zeros(shape=(nrows,
+                                                ncols), dtype=np.uint8)
             exty, extx = np.where(masked_smoothed_ratio > snr_threshold)
             extended_emission[exty, extx] = 1
             #  find the contours of the extended emission
             contours, hierarchy = cv.findContours(extended_emission,
                                                   cv.RETR_EXTERNAL,
                                                   cv.CHAIN_APPROX_SIMPLE)
             #  get the countours that are above the minimum size
             bigcontours = [con for con in contours if cv.contourArea(con) >
                            min_shower_area]
             #  get the minimum enclosing rectangle which is the same as the
             # minimum enclosing ellipse
             ellipses = [cv.minAreaRect(con) for con in bigcontours]
+
+
+            expand_by_ratio = True
+            expansion = 1.0
+            plane = gdq[intg, grp, :, :]
+            nrows = plane.shape[0]
+            ncols = plane.shape[1]
+            image = np.zeros(shape=(nrows, ncols, 3), dtype=np.uint8)
+            image2 = np.zeros_like(image)
+            cv.drawContours(image2, bigcontours, -1, (0, 0, jump_flag), -1)
+            for ellipse in ellipses:
+                ceny = ellipse[0][0]
+                cenx = ellipse[0][1]
+                # Expand the ellipse by the expansion factor. The number of pixels
+                # added to both axes is
+                # the number of pixels added to the minor axis. This prevents very
+                # large flagged ellipses
+                # with high axis ratio ellipses. The major and minor axis are not
+                # always the same index.
+                # Therefore, we have to test to find which is actually the minor axis.
+                if expand_by_ratio:
+                    if ellipse[1][1] < ellipse[1][0]:
+                        axis1 = ellipse[1][0] + (expansion - 1.0) * ellipse[1][1]
+                        axis2 = ellipse[1][1] * expansion
+                    else:
+                        axis1 = ellipse[1][0] * expansion
+                        axis2 = ellipse[1][1] + (expansion - 1.0) * ellipse[1][0]
+                else:
+                    axis1 = ellipse[1][0] + expansion
+                    axis2 = ellipse[1][1] + expansion
+                axis1 = min(axis1, max_extended_radius)
+                axis2 = min(axis2, max_extended_radius)
+                alpha = ellipse[2]
+                image = cv.ellipse(image, (round(ceny), round(cenx)), (round(axis1 / 2),
+                                                                       round(axis2 / 2)), alpha, 0, 360,
+                                   (0, 0, jump_flag), -1)
             if len(ellipses) > 0:
                 # add all the showers for this integration to the list
                 all_ellipses.append([intg, grp, ellipses])
     if all_ellipses:
         #  Now we actually do the flagging of the pixels inside showers.
         # This is deferred until all showers are detected. because the showers
         # can flag future groups and would confuse the detection algorthim if
@@ -728,13 +810,8 @@
             grp = showers[1]
             ellipses = showers[2]
             gdq, num = extend_ellipses(gdq, intg, grp, ellipses, sat_flag,
                                        jump_flag, expansion=ellipse_expand,
                                        expand_by_ratio=True,
                                        num_grps_masked=num_grps_masked,
                                        max_extended_radius=max_extended_radius)
-    if np.all(all_ellipses == 0):
-        log.info('No showers found in exposure.')
-    else:
-        num_showers = len(all_ellipses)
-        log.info(f' Number of showers flagged = {num_showers}')
     return gdq, len(all_ellipses)
```

### Comparing `stcal-1.3.8/src/stcal/jump/twopoint_difference.py` & `stcal-1.4.0/src/stcal/jump/twopoint_difference.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 import numpy as np
-
+import astropy.stats as stats
+import warnings
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
 
-def find_crs(dataa, group_dq, read_noise, rejection_thresh,
+def find_crs(dataa, group_dq, read_noise, normal_rej_thresh,
              two_diff_rej_thresh, three_diff_rej_thresh, nframes,
              flag_4_neighbors, max_jump_to_flag_neighbors,
              min_jump_to_flag_neighbors, dqflags,
              after_jump_flag_e1=0.0,
              after_jump_flag_n1=0,
              after_jump_flag_e2=0.0,
              after_jump_flag_n2=0,
-             copy_arrs=True):
+             copy_arrs=True, minimum_groups=3, minimum_sigclip_groups=100,
+             only_use_ints=True):
 
     """
     Find CRs/Jumps in each integration within the input data array. The input
     data array is assumed to be in units of electrons, i.e. already multiplied
     by the gain. We also assume that the read noise is in units of electrons.
     We also assume that there are at least three groups in the integrations.
     This was checked by jump_step before this routine is called.
@@ -29,15 +31,15 @@
 
     group_dq : int, 4D array
         group DQ flags
 
     read_noise : float, 2D array
         The read noise of each pixel
 
-    rejection_thresh : float
+    normal_rej_thresh : float
         cosmic ray sigma rejection threshold
 
     two_diff_rej_thresh : float
         cosmic ray sigma rejection threshold for ramps having 3 groups
 
     three_diff_rej_thresh : float
         cosmic ray sigma rejection threshold for ramps having 4 groups
@@ -79,167 +81,249 @@
         Gives the number of groups to flag after jumps with DN values above that
         given by after_jump_flag_dn2
 
     copy_arrs : bool
         Flag for making internal copies of the arrays so the input isn't modified,
         defaults to True.
 
+    minimum_groups : integer
+        The minimum number of groups to perform jump detection.
+
+    minimum_sigclip_groups : integer
+        The minimum number of groups required for the sigma clip routine to be
+        used for jump detection rather than using the expected noise based on
+        the read noise and gain files.
+
+    only_use_ints : boolean
+        If True the sigma clip process will only apply for groups between
+        integrations. This means that a group will only be compared against the
+        same group in other integrations. If False all groups across all integrations
+        will be used to detect outliers.
     Returns
     -------
     gdq : int, 4D array
         group DQ array with reset flags
 
     row_below_gdq : int, 3D array (num_ints, num_groups, num_cols)
         pixels below current row also to be flagged as a CR
 
     row_above_gdq : int, 3D array (num_ints, num_groups, num_cols)
         pixels above current row also to be flagged as a CR
 
     """
-
     # copy data and group DQ array
     if copy_arrs:
-        dataa = dataa.copy()
+        dat = dataa.copy()
         gdq = group_dq.copy()
     else:
+        dat = dataa
         gdq = group_dq
-
     # Get data characteristics
     nints, ngroups, nrows, ncols = dataa.shape
     ndiffs = ngroups - 1
-
     # get readnoise, squared
     read_noise_2 = read_noise**2
-
     # create arrays for output
     row_above_gdq = np.zeros((nints, ngroups, ncols), dtype=np.uint8)
     row_below_gdq = np.zeros((nints, ngroups, ncols), dtype=np.uint8)
 
     # get dq flags for saturated, donotuse, jump
     sat_flag = dqflags["SATURATED"]
     dnu_flag = dqflags["DO_NOT_USE"]
     jump_flag = dqflags["JUMP_DET"]
 
+    # get data, gdq
+    num_flagged_grps = 0
+    # determine the number of groups with all pixels set to DO_NOT_USE
+    ngrps = dat.shape[1]
     for integ in range(nints):
-
-        log.info(f'Working on integration {integ + 1}:')
-
-        # get data, gdq for this integration
-        dat = dataa[integ]
-        gdq_integ = gdq[integ]
-
+        for grp in range(dat.shape[1]):
+            if np.all(np.bitwise_and(gdq[integ, grp, :, :], dnu_flag)):
+                num_flagged_grps += 1
+    if only_use_ints and nints:
+        total_groups = nints
+    else:
+        total_groups = nints * ngrps - num_flagged_grps
+    if (ngrps < minimum_groups and only_use_ints and nints < minimum_sigclip_groups) or \
+            (not only_use_ints and nints * ngrps < minimum_sigclip_groups and
+             ngrps < minimum_groups):
+        log.info("Jump Step was skipped because exposure has less than the minimum number of usable groups")
+        log.info("Data shape {}".format(str(dat.shape)))
+        dummy = np.zeros((dataa.shape[1] - 1, dataa.shape[2], dataa.shape[3]),
+                         dtype=np.float32)
+        return gdq, row_below_gdq, row_above_gdq, 0, dummy
+    else:
         # set 'saturated' or 'do not use' pixels to nan in data
-        dat[np.where(np.bitwise_and(gdq_integ, sat_flag))] = np.nan
-        dat[np.where(np.bitwise_and(gdq_integ, dnu_flag))] = np.nan
+        dat[np.where(np.bitwise_and(gdq, sat_flag))] = np.nan
+        dat[np.where(np.bitwise_and(gdq, dnu_flag))] = np.nan
+        dat[np.where(np.bitwise_and(gdq, dnu_flag + sat_flag))] = np.nan
 
         # calculate the differences between adjacent groups (first diffs)
         # use mask on data, so the results will have sat/donotuse groups masked
-        first_diffs = np.diff(dat, axis=0)
+        first_diffs = np.diff(dat, axis=1)
 
         # calc. the median of first_diffs for each pixel along the group axis
-        median_diffs = calc_med_first_diffs(first_diffs)
-
+        first_diffs_masked = np.ma.masked_array(first_diffs, mask=np.isnan(first_diffs))
+        median_diffs = np.ma.median(first_diffs_masked, axis=(0, 1))
         # calculate sigma for each pixel
         sigma = np.sqrt(np.abs(median_diffs) + read_noise_2 / nframes)
 
         # reset sigma so pxels with 0 readnoise are not flagged as jumps
         sigma[np.where(sigma == 0.)] = np.nan
 
         # compute 'ratio' for each group. this is the value that will be
         # compared to 'threshold' to classify jumps. subtract the median of
         # first_diffs from first_diffs, take the abs. value and divide by sigma.
-        e_jump = first_diffs - median_diffs[np.newaxis, :, :]
-        ratio = np.abs(e_jump) / sigma[np.newaxis, :, :]
+        e_jump_4d = first_diffs - median_diffs[np.newaxis, :, :]
+        ratio_all = np.abs(first_diffs - median_diffs[np.newaxis, np.newaxis, :, :]) / \
+                    sigma[np.newaxis, np.newaxis, :, :]
+        if (only_use_ints and nints >= minimum_sigclip_groups) or \
+           (not only_use_ints and total_groups >= minimum_sigclip_groups):
+            log.info(" Jump Step using sigma clip {} greater than {}, rejection threshold {}".format(
+                str(total_groups), str(minimum_sigclip_groups), str(normal_rej_thresh)))
+            warnings.filterwarnings("ignore", ".*All-NaN slice encountered.*", RuntimeWarning)
+            warnings.filterwarnings("ignore", ".*Mean of empty slice.*", RuntimeWarning)
+            warnings.filterwarnings("ignore", ".*Degrees of freedom <= 0.*", RuntimeWarning)
+
+            if only_use_ints:
+                mean, median, stddev = stats.sigma_clipped_stats(first_diffs_masked, sigma=normal_rej_thresh,
+                                                                 axis=0)
+                clipped_diffs = stats.sigma_clip(first_diffs_masked, sigma=normal_rej_thresh,
+                                                 axis=0, masked=True)
+            else:
+                mean, median, stddev = stats.sigma_clipped_stats(first_diffs_masked, sigma=normal_rej_thresh,
+                                                                 axis=(0, 1))
+                clipped_diffs = stats.sigma_clip(first_diffs_masked, sigma=normal_rej_thresh,
+                                                 axis=(0, 1), masked=True)
+            jump_mask = np.logical_and(clipped_diffs.mask, np.logical_not(first_diffs_masked.mask))
+            jump_mask[np.bitwise_and(jump_mask, gdq[:, 1:, :, :] == sat_flag)] = False
+            jump_mask[np.bitwise_and(jump_mask, gdq[:, 1:, :, :] == dnu_flag)] = False
+            jump_mask[np.bitwise_and(jump_mask, gdq[:, 1:, :, :] == (dnu_flag + sat_flag))] = False
+            gdq[:, 1:, :, :] = np.bitwise_or(gdq[:, 1:, :, :], jump_mask *
+                                             np.uint8(dqflags["JUMP_DET"]))
+            # if grp is all jump set to do not use
+            for integ in range(nints):
+                for grp in range(ngrps):
+                    if np.all(np.bitwise_or(np.bitwise_and(gdq[integ, grp, :, :], jump_flag),
+                                            np.bitwise_and(gdq[integ, grp, :, :], dnu_flag))):
+                        jumpy, jumpx = np.where(gdq[integ, grp, :, :] == jump_flag)
+                        gdq[integ, grp, jumpy, jumpx] = 0
+            warnings.resetwarnings()
+        else:
+            for integ in range(nints):
+
+                # get data, gdq for this integration
+                dat = dataa[integ]
+                gdq_integ = gdq[integ]
+
+                # set 'saturated' or 'do not use' pixels to nan in data
+                dat[np.where(np.bitwise_and(gdq_integ, sat_flag))] = np.nan
+                dat[np.where(np.bitwise_and(gdq_integ, dnu_flag))] = np.nan
+
+                # calculate the differences between adjacent groups (first diffs)
+                # use mask on data, so the results will have sat/donotuse groups masked
+                first_diffs = np.diff(dat, axis=0)
+
+                # calc. the median of first_diffs for each pixel along the group axis
+                median_diffs = calc_med_first_diffs(first_diffs)
+
+                # calculate sigma for each pixel
+                sigma = np.sqrt(np.abs(median_diffs) + read_noise_2 / nframes)
+                # reset sigma so pxels with 0 readnoise are not flagged as jumps
+                sigma[np.where(sigma == 0.)] = np.nan
+
+                # compute 'ratio' for each group. this is the value that will be
+                # compared to 'threshold' to classify jumps. subtract the median of
+                # first_diffs from first_diffs, take the abs. value and divide by sigma.
+                e_jump = first_diffs - median_diffs[np.newaxis, :, :]
+                ratio = np.abs(e_jump) / sigma[np.newaxis, :, :]
+
+                # create a 2d array containing the value of the largest 'ratio' for each group
+                warnings.filterwarnings("ignore", ".*All-NaN slice encountered.*", RuntimeWarning)
+                max_ratio = np.nanmax(ratio, axis=0)
+                warnings.resetwarnings()
+                # now see if the largest ratio of all groups for each pixel exceeds the threshold.
+                # there are different threshold for 4+, 3, and 2 usable groups
+                num_unusable_groups = np.sum(np.isnan(first_diffs), axis=0)
+                row4cr, col4cr = np.where(np.logical_and(ndiffs - num_unusable_groups >= 4,
+                                                         max_ratio > normal_rej_thresh))
+                row3cr, col3cr = np.where(np.logical_and(ndiffs - num_unusable_groups == 3,
+                                                         max_ratio > three_diff_rej_thresh))
+                row2cr, col2cr = np.where(np.logical_and(ndiffs - num_unusable_groups == 2,
+                                                         max_ratio > two_diff_rej_thresh))
+
+                # get the rows, col pairs for all pixels with at least one CR
+                all_crs_row = np.concatenate((row4cr, row3cr, row2cr))
+                all_crs_col = np.concatenate((col4cr, col3cr, col2cr))
+
+                # iterate over all groups of the pix w/ an inital CR to look for subsequent CRs
+                # flag and clip the first CR found. recompute median/sigma/ratio
+                # and repeat the above steps of comparing the max 'ratio' for each pixel
+                # to the threshold to determine if another CR can be flagged and clipped.
+                # repeat this process until no more CRs are found.
+                for j in range(len(all_crs_row)):
+                    # get arrays of abs(diffs), ratio, readnoise for this pixel
+                    pix_first_diffs = first_diffs[:, all_crs_row[j], all_crs_col[j]]
+                    pix_ratio = ratio[:, all_crs_row[j], all_crs_col[j]]
+                    pix_rn2 = read_noise_2[all_crs_row[j], all_crs_col[j]]
 
-        # create a 2d array containing the value of the largest 'ratio' for each group
-        max_ratio = np.nanmax(ratio, axis=0)
+                    # Create a mask to flag CRs. pix_cr_mask = 0 denotes a CR
+                    pix_cr_mask = np.ones(pix_first_diffs.shape, dtype=bool)
 
-        # now see if the largest ratio of all groups for each pixel exceeds the threshold.
-        # there are different threshold for 4+, 3, and 2 usable groups
-        num_unusable_groups = np.sum(np.isnan(first_diffs), axis=0)
-        row4cr, col4cr = np.where(np.logical_and(ndiffs - num_unusable_groups >= 4,
-                                  max_ratio > rejection_thresh))
-        row3cr, col3cr = np.where(np.logical_and(ndiffs - num_unusable_groups == 3,
-                                  max_ratio > three_diff_rej_thresh))
-        row2cr, col2cr = np.where(np.logical_and(ndiffs - num_unusable_groups == 2,
-                                  max_ratio > two_diff_rej_thresh))
-
-        log_str = 'From highest outlier, two-point found {} pixels with at least one CR from {} groups.'
-        log.info(log_str.format(len(row4cr), 'five or more'))
-
-        # get the rows, col pairs for all pixels with at least one CR
-        all_crs_row = np.concatenate((row4cr, row3cr, row2cr))
-        all_crs_col = np.concatenate((col4cr, col3cr, col2cr))
-
-        # iterate over all groups of the pix w/ an inital CR to look for subsequent CRs
-        # flag and clip the first CR found. recompute median/sigma/ratio
-        # and repeat the above steps of comparing the max 'ratio' for each pixel
-        # to the threshold to determine if another CR can be flagged and clipped.
-        # repeat this process until no more CRs are found.
-        for j in range(len(all_crs_row)):
-
-            # get arrays of abs(diffs), ratio, readnoise for this pixel
-            pix_first_diffs = first_diffs[:, all_crs_row[j], all_crs_col[j]]
-            pix_ratio = ratio[:, all_crs_row[j], all_crs_col[j]]
-            pix_rn2 = read_noise_2[all_crs_row[j], all_crs_col[j]]
-
-            # Create a mask to flag CRs. pix_cr_mask = 0 denotes a CR
-            pix_cr_mask = np.ones(pix_first_diffs.shape, dtype=bool)
-
-            # set the largest ratio as a CR
-            pix_cr_mask[np.nanargmax(pix_ratio)] = 0
-            new_CR_found = True
-
-            # loop and check for more CRs, setting the mask as you go and
-            # clipping the group with the CR. stop when no more CRs are found
-            # or there is only one two diffs left (which means there is
-            # actually one left, since the next CR will be masked after
-            # checking that condition)
-
-            while new_CR_found and ((ndiffs - np.sum(np.isnan(pix_first_diffs))) > 2):
-
-                new_CR_found = False
-
-                # set CRs to nans in first diffs to clip them
-                pix_first_diffs[~pix_cr_mask] = np.nan
-
-                # recalculate median, sigma, and ratio
-                new_pix_median_diffs = calc_med_first_diffs(pix_first_diffs)
-
-                new_pix_sigma = np.sqrt(np.abs(new_pix_median_diffs) + pix_rn2 / nframes)
-                new_pix_ratio = np.abs(pix_first_diffs - new_pix_median_diffs) / new_pix_sigma
-
-                # check if largest ratio exceeds threhold appropriate for num remaining groups
-
-                # select appropriate thresh. based on number of remaining groups
-                rej_thresh = rejection_thresh
-                if ndiffs - np.sum(np.isnan(pix_first_diffs)) == 3:
-                    rej_thresh = three_diff_rej_thresh
-                if ndiffs - np.sum(np.isnan(pix_first_diffs)) == 2:
-                    rej_thresh = two_diff_rej_thresh
-                new_pix_max_ratio_idx = np.nanargmax(new_pix_ratio)  # index of largest ratio
-                if new_pix_ratio[new_pix_max_ratio_idx] > rej_thresh:
+                    # set the largest ratio as a CR
+                    pix_cr_mask[np.nanargmax(pix_ratio)] = 0
                     new_CR_found = True
-                    pix_cr_mask[new_pix_max_ratio_idx] = 0
 
-            # Found all CRs for this pix - set flags in input DQ array
-            gdq[integ, 1:, all_crs_row[j], all_crs_col[j]] = \
-                np.bitwise_or(gdq[integ, 1:, all_crs_row[j], all_crs_col[j]],
-                              dqflags["JUMP_DET"] * np.invert(pix_cr_mask))
+                    # loop and check for more CRs, setting the mask as you go and
+                    # clipping the group with the CR. stop when no more CRs are found
+                    # or there is only one two diffs left (which means there is
+                    # actually one left, since the next CR will be masked after
+                    # checking that condition)
+                    while new_CR_found and (ndiffs - np.sum(np.isnan(pix_first_diffs)) > 2):
+
+                        new_CR_found = False
+
+                        # set CRs to nans in first diffs to clip them
+                        pix_first_diffs[~pix_cr_mask] = np.nan
+
+                        # recalculate median, sigma, and ratio
+                        new_pix_median_diffs = calc_med_first_diffs(pix_first_diffs)
+
+                        new_pix_sigma = np.sqrt(np.abs(new_pix_median_diffs) + pix_rn2 / nframes)
+                        new_pix_ratio = np.abs(pix_first_diffs - new_pix_median_diffs) / new_pix_sigma
+
+                        # check if largest ratio exceeds threhold appropriate for num remaining groups
+
+                        # select appropriate thresh. based on number of remaining groups
+                        rej_thresh = normal_rej_thresh
+                        if ndiffs - np.sum(np.isnan(pix_first_diffs)) == 3:
+                            rej_thresh = three_diff_rej_thresh
+                        if ndiffs - np.sum(np.isnan(pix_first_diffs)) == 2:
+                            rej_thresh = two_diff_rej_thresh
+                        new_pix_max_ratio_idx = np.nanargmax(new_pix_ratio)  # index of largest ratio
+                        if new_pix_ratio[new_pix_max_ratio_idx] > rej_thresh:
+                            new_CR_found = True
+                            pix_cr_mask[new_pix_max_ratio_idx] = 0
+                        unusable_diffs = np.sum(np.isnan(pix_first_diffs))
+                    # Found all CRs for this pix - set flags in input DQ array
+                    gdq[integ, 1:, all_crs_row[j], all_crs_col[j]] = \
+                        np.bitwise_or(gdq[integ, 1:, all_crs_row[j], all_crs_col[j]],
+                                      dqflags["JUMP_DET"] * np.invert(pix_cr_mask))
 
+        cr_integ, cr_group, cr_row, cr_col = np.where(np.bitwise_and(gdq, jump_flag))
+        num_primary_crs = len(cr_group)
         if flag_4_neighbors:  # iterate over each 'jump' pixel
-            cr_group, cr_row, cr_col = np.where(np.bitwise_and(gdq[integ], jump_flag))
-
             for j in range(len(cr_group)):
 
-                ratio_this_pix = ratio[cr_group[j] - 1, cr_row[j], cr_col[j]]
+                ratio_this_pix = ratio_all[cr_integ[j], cr_group[j] - 1, cr_row[j], cr_col[j]]
 
                 # Jumps must be in a certain range to have neighbors flagged
-                if ratio_this_pix < max_jump_to_flag_neighbors and \
-                        ratio_this_pix > min_jump_to_flag_neighbors:
+                if (ratio_this_pix < max_jump_to_flag_neighbors) and \
+                        (ratio_this_pix > min_jump_to_flag_neighbors):
+                    integ = cr_integ[j]
                     group = cr_group[j]
                     row = cr_row[j]
                     col = cr_col[j]
 
                     # This section saves flagged neighbors that are above or
                     # below the current range of row. If this method
                     # running in a single process, the row above and below are
@@ -281,38 +365,45 @@
                                     np.bitwise_or(gdq[integ, group, row, col + 1], jump_flag)
 
         # flag n groups after jumps above the specified thresholds to account for
         # the transient seen after ramp jumps
         flag_e_threshold = [after_jump_flag_e1, after_jump_flag_e2]
         flag_groups = [after_jump_flag_n1, after_jump_flag_n2]
 
-        cr_group, cr_row, cr_col = np.where(np.bitwise_and(gdq[integ], jump_flag))
+
         for cthres, cgroup in zip(flag_e_threshold, flag_groups):
             if cgroup > 0:
-                log.info(f"Flagging {cgroup} groups after detected jumps with e >= {np.mean(cthres)}.")
-
+                cr_intg, cr_group, cr_row, cr_col = np.where(np.bitwise_and(gdq, jump_flag))
                 for j in range(len(cr_group)):
+                    intg = cr_intg[j]
                     group = cr_group[j]
                     row = cr_row[j]
                     col = cr_col[j]
-                    if e_jump[group - 1, row, col] >= cthres[row, col]:
+                    if e_jump_4d[intg, group - 1, row, col] >= cthres[row, col]:
                         for kk in range(group, min(group + cgroup + 1, ngroups)):
-                            if (gdq[integ, kk, row, col] & sat_flag) == 0:
-                                if (gdq[integ, kk, row, col] & dnu_flag) == 0:
-                                    gdq[integ, kk, row, col] =\
+                            if (gdq[intg, kk, row, col] & sat_flag) == 0:
+                                if (gdq[intg, kk, row, col] & dnu_flag) == 0:
+                                    gdq[intg, kk, row, col] = \
                                         np.bitwise_or(gdq[integ, kk, row, col], jump_flag)
-
-    return gdq, row_below_gdq, row_above_gdq
+    if 'stddev' in locals():
+        return gdq, row_below_gdq, row_above_gdq, num_primary_crs, stddev
+    else:
+        if only_use_ints:
+            dummy = np.zeros((dataa.shape[1]-1, dataa.shape[2], dataa.shape[3]),
+                             dtype=np.float32)
+        else:
+            dummy = np.zeros((dataa.shape[2], dataa.shape[3]), dtype=np.float32)
+        return gdq, row_below_gdq, row_above_gdq, num_primary_crs, dummy
 
 
 def calc_med_first_diffs(first_diffs):
 
     """ Calculate the median of `first diffs` along the group axis.
 
-        If there 4+ usable groups (e.g not flagged as saturated, donotuse,
+        If there are 4+ usable groups (e.g not flagged as saturated, donotuse,
         or a previously clipped CR), then the group with largest absoulte
         first difference will be clipped and the median of the remianing groups
         will be returned. If there are exactly 3 usable groups, the median of
         those three groups will be returned without any clipping. Finally, if
         there are two usable groups, the group with the smallest absolute
         difference will be returned.
```

### Comparing `stcal-1.3.8/src/stcal/linearity/linearity.py` & `stcal-1.4.0/src/stcal/linearity/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/src/stcal/ramp_fitting/gls_fit.py` & `stcal-1.4.0/src/stcal/ramp_fitting/gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/src/stcal/ramp_fitting/ols_fit.py` & `stcal-1.4.0/src/stcal/ramp_fitting/ols_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,15 +603,20 @@
         one_group[integ] = np.where(one_group_int)
 
         del one_group_int
         del good_0
         del bad_1_
 
     ramp_data.one_groups_locs = one_group
-    # (NFrames + 1) * TFrame / 2
+
+    # Refer to JP-3242 for derivation.
+    # Updated: One Group Time = [(TFrame * NFrames * (NFrames + 1)] / [2 * NFrames]
+    # There is an NFrames term in the numerator and denominator, so when
+    # cancelled we get:
+    # One Group Time = (NFrames + 1) * TFrame / 2
     ramp_data.one_groups_time = (ramp_data.nframes + 1) * ramp_data.frame_time / 2
 
 
 def ols_ramp_fit_single(
         ramp_data, buffsize, save_opt, readnoise_2d, gain_2d, weighting):
     """
     Fit a ramp using ordinary least squares. Calculate the count rate for each
@@ -652,19 +657,20 @@
     """
     tstart = time.time()
 
     if not ramp_data.suppress_one_group_ramps:
         # This must be done before the ZEROFRAME replacements to prevent
         # ZEROFRAME replacement being confused for one good group ramps
         # in the 0th group.
-        if ramp_data.groupgap > 0:
+        if ramp_data.nframes > 1:
             find_0th_one_good_group(ramp_data)
 
         if ramp_data.zeroframe is not None:
-            zframe_locs, cnt = utils.use_zeroframe_for_saturated_ramps(ramp_data)
+            zframe_mat, zframe_locs, cnt = utils.use_zeroframe_for_saturated_ramps(ramp_data)
+            ramp_data.zframe_mat = zframe_mat
             ramp_data.zframe_locs = zframe_locs
             ramp_data.cnt = cnt
 
     # Save original shapes for writing to log file, as these may change for MIRI
     n_int, ngroups, nrows, ncols = ramp_data.data.shape
     orig_ngroups = ngroups
     orig_cubeshape = (ngroups, nrows, ncols)
@@ -827,17 +833,14 @@
     ------
     max_seg : int
         Maximum possible number of segments over all groups and segments
 
     gdq_cube_shape : ndarray
         Group DQ dimensions
 
-    effintim : float
-        effective integration time for a single group
-
     f_max_seg : int
         Actual maximum number of segments over all groups and segments
 
     dq_int : ndarray
         The pixel dq for each integration for each pixel
 
     num_seg_per_int : ndarray
@@ -863,30 +866,20 @@
     data = ramp_data.data
     err = ramp_data.err
     groupdq = ramp_data.groupdq
     inpixeldq = ramp_data.pixeldq
 
     # Get instrument and exposure data
     frame_time = ramp_data.frame_time
-    groupgap = ramp_data.groupgap
-    nframes = ramp_data.nframes
 
     # Get needed sizes and shapes
     n_int, ngroups, nrows, ncols = data.shape
     imshape = (nrows, ncols)
     cubeshape = (ngroups,) + imshape
 
-    # Calculate effective integration time (once EFFINTIM has been populated
-    #   and accessible, will use that instead), and other keywords that will
-    #   needed if the pedestal calculation is requested. Note 'nframes'
-    #   is the number of given by the NFRAMES keyword, and is the number of
-    #   frames averaged on-board for a group, i.e., it does not include the
-    #   groupgap.
-    effintim = (nframes + groupgap) * frame_time
-
     # Get GROUP DQ and ERR arrays from input file
     gdq_cube = groupdq
     gdq_cube_shape = gdq_cube.shape
 
     # Get max number of segments fit in all integrations
     max_seg, num_CRs = calc_num_seg(
         gdq_cube, n_int, ramp_data.flags_jump_det, ramp_data.flags_do_not_use)
@@ -986,23 +979,25 @@
 
                 del data_diff
 
             del data_sect
             del ff_sect
             del gdq_sect
 
+    # END LOOP
+
     if pixeldq_sect is not None:
         del pixeldq_sect
 
     ramp_data.data = data
     ramp_data.err = err
     ramp_data.groupdq = groupdq
     ramp_data.pixeldq = inpixeldq
 
-    return max_seg, gdq_cube_shape, effintim, f_max_seg, dq_int, num_seg_per_int,\
+    return max_seg, gdq_cube_shape, f_max_seg, dq_int, num_seg_per_int,\
         sat_0th_group_int, opt_res, pixeldq, inv_var, med_rates
 
 
 def ramp_fit_compute_variances(ramp_data, gain_2d, readnoise_2d, fit_slopes_ans):
     """
     In this 'Second Pass' over the data, loop over integrations and data
     sections to calculate the variances of the slope using the estimated
@@ -1079,15 +1074,15 @@
     # Get needed sizes and shapes
     n_int, ngroups, nrows, ncols = data.shape
     imshape = (nrows, ncols)
     cubeshape = (ngroups,) + imshape
 
     max_seg = fit_slopes_ans[0]
     num_seg_per_int = fit_slopes_ans[5]
-    med_rates = fit_slopes_ans[10]
+    med_rates = fit_slopes_ans[9]
 
     var_p3, var_r3, var_p4, var_r4, var_both4, var_both3, \
         inv_var_both4, s_inv_var_p3, s_inv_var_r3, s_inv_var_both3, segs_4 = \
         utils.alloc_arrays_2(n_int, imshape, max_seg)
 
     # Loop over data integrations
     for num_int in range(n_int):
@@ -1126,19 +1121,19 @@
             del gdq_sect
 
         # The next 4 statements zero out entries for non-existing segments, and
         #   set the variances for segments having negative slopes (the segment
         #   variance is proportional to the median estimated slope) to
         #   outrageously large values so that they will have negligible
         #   contributions.
-        var_p4[num_int, :, :, :] *= (segs_4[num_int, :, :, :] > 0)
 
         # Suppress, then re-enable harmless arithmetic warnings
         warnings.filterwarnings("ignore", ".*invalid value.*", RuntimeWarning)
         warnings.filterwarnings("ignore", ".*divide by zero.*", RuntimeWarning)
+        var_p4[num_int, :, :, :] *= (segs_4[num_int, :, :, :] > 0)
         var_p4[var_p4 <= 0.] = utils.LARGE_VARIANCE
 
         var_r4[num_int, :, :, :] *= (segs_4[num_int, :, :, :] > 0)
         var_r4[var_r4 <= 0.] = utils.LARGE_VARIANCE
 
         # The sums of inverses of the variances are needed for later
         #   variance calculations.
@@ -1279,16 +1274,16 @@
         log.debug('Missing keyword DRPFRMS1, so setting to default value of 0')
 
     # Get needed sizes and shapes
     n_int, ngroups, nrows, ncols = data.shape
     imshape = (nrows, ncols)
 
     # Unpack intermediate computations from preious steps
-    max_seg, gdq_cube_shape, effintim, f_max_seg, dq_int, num_seg_per_int = fit_slopes_ans[:6]
-    sat_0th_group_int, opt_res, pixeldq, inv_var, med_rates = fit_slopes_ans[6:]
+    max_seg, gdq_cube_shape, f_max_seg, dq_int, num_seg_per_int = fit_slopes_ans[:5]
+    sat_0th_group_int, opt_res, pixeldq, inv_var, med_rates = fit_slopes_ans[5:]
 
     var_p3, var_r3, var_p4, var_r4, var_both4, var_both3 = variances_ans[:6]
     inv_var_both4, s_inv_var_p3, s_inv_var_r3, s_inv_var_both3 = variances_ans[6:]
 
     slope_by_var4 = opt_res.slope_seg.copy() / var_both4
 
     del var_both4
@@ -1371,15 +1366,15 @@
         opt_res.sigslope_seg = opt_res.sigslope_seg[:, :f_max_seg, :, :]
         opt_res.yint_seg = opt_res.yint_seg[:, :f_max_seg, :, :]
         opt_res.sigyint_seg = opt_res.sigyint_seg[:, :f_max_seg, :, :]
         opt_res.weights = (inv_var_both4[:, :f_max_seg, :, :])**2.
         opt_res.var_p_seg = var_p4[:, :f_max_seg, :, :]
         opt_res.var_r_seg = var_r4[:, :f_max_seg, :, :]
 
-        opt_info = opt_res.output_optional(effintim)
+        opt_info = opt_res.output_optional(ramp_data.group_time)
     else:
         opt_info = None
 
     if inv_var_both4 is not None:
         del inv_var_both4
 
     if var_p4 is not None:
@@ -1392,28 +1387,28 @@
         del inv_var
 
     if pixeldq is not None:
         del pixeldq
 
     # Output integration-specific results to separate file
     integ_info = utils.output_integ(
-        ramp_data, slope_int, dq_int, effintim, var_p3, var_r3, var_both3)
+        ramp_data, slope_int, dq_int, var_p3, var_r3, var_both3)
 
     if opt_res is not None:
         del opt_res
 
     if slope_int is not None:
         del slope_int
     del var_p3
     del var_r3
     del var_both3
 
-    # Divide slopes by total (summed over all integrations) effective
-    #   integration time to give count rates.
-    c_rates = slope_dataset2 / effintim
+    # The slopes per pixel are now computed, except for unusable data
+    # due to flagging, which is done below.
+    c_rates = slope_dataset2
 
     # Compress all integration's dq arrays to create 2D PIXELDDQ array for
     #   primary output
     final_pixeldq = utils.dq_compress_final(dq_int, ramp_data)
 
     # For invalid slope calculations set to NaN.  Pixels flagged as SATURATED or
     # DO_NOT_USE have invalid data.
@@ -2780,15 +2775,15 @@
     sig_slope_s = np.zeros(npix, dtype=np.float32)
 
     # Calculate slopes etc. for datasets having either 1 or 2 groups per
     #   integration, and return
     if ngroups == 1:  # process all pixels in 1 group/integration dataset
         slope_s, intercept_s, variance_s, sig_intercept_s, sig_slope_s = \
             fit_1_group(slope_s, intercept_s, variance_s, sig_intercept_s,
-                        sig_slope_s, npix, data, c_mask_2d)
+                        sig_slope_s, npix, data, c_mask_2d, ramp_data)
 
         return slope_s, intercept_s, variance_s, sig_intercept_s, sig_slope_s
 
     if ngroups == 2:  # process all pixels in 2 group/integration dataset
         rn_sect_1d = rn_sect.reshape(npix)
         slope_s, intercept_s, variance_s, sig_intercept_s, sig_slope_s = fit_2_group(
             slope_s, intercept_s, variance_s, sig_intercept_s, sig_slope_s, npix,
@@ -2804,25 +2799,25 @@
     #   0th group is good and the 1st group is bad, determine whether or not to
     #   use the 0th group.
     wh_pix_1r = np.where(c_mask_2d[0, :] & (np.logical_not(c_mask_2d[1, :])))
 
     if len(wh_pix_1r[0]) > 0:
         slope_s, intercept_s, variance_s, sig_intercept_s, sig_slope_s = \
             fit_single_read(slope_s, intercept_s, variance_s, sig_intercept_s,
-                            sig_slope_s, npix, data, wh_pix_1r)
+                            sig_slope_s, npix, data, wh_pix_1r, ramp_data)
 
     del wh_pix_1r
 
     # For datasets having >2 groups/integrations, for any semiramp in which only
     #   the 0th and 1st group are good, set slope, etc
     wh_pix_2r = np.where(c_mask_2d.sum(axis=0) == 2)  # ramps with 2 good groups
 
     slope_s, intercept_s, variance_s, sig_slope_s, sig_intercept_s = \
         fit_double_read(c_mask_2d, wh_pix_2r, data_masked, slope_s, intercept_s,
-                        variance_s, sig_slope_s, sig_intercept_s, rn_sect)
+                        variance_s, sig_slope_s, sig_intercept_s, rn_sect, ramp_data)
 
     del wh_pix_2r
 
     # Select ramps having >2 good groups
     wh_pix_to_use = np.where(c_mask_2d.sum(axis=0) > 2)
 
     good_pix = wh_pix_to_use[0]  # Ramps with >2 good groups
@@ -2840,14 +2835,16 @@
         # get sums from optimal weighting
         sumx, sumxx, sumxy, sumy, nreads_wtd, xvalues = calc_opt_sums(
             ramp_data, rn_sect, gain_sect, data_masked, c_mask_2d, xvalues, good_pix)
 
         slope, intercept, sig_slope, sig_intercept = \
             calc_opt_fit(nreads_wtd, sumxx, sumx, sumxy, sumy)
 
+        slope = slope / ramp_data.group_time
+
         variance = sig_slope**2.  # variance due to fit values
 
     elif weighting.lower() == 'unweighted':  # fit using unweighted weighting
         # get sums from unweighted weighting
         sumx, sumxx, sumxy, sumy = calc_unwtd_sums(data_masked, xvalues)
 
         slope, intercept, sig_slope, sig_intercept, line_fit =\
@@ -2873,15 +2870,15 @@
     sig_intercept_s[good_pix] = sig_intercept
     sig_slope_s[good_pix] = sig_slope
 
     return slope_s, intercept_s, variance_s, sig_intercept_s, sig_slope_s
 
 
 def fit_single_read(slope_s, intercept_s, variance_s, sig_intercept_s,
-                    sig_slope_s, npix, data, wh_pix_1r):
+                    sig_slope_s, npix, data, wh_pix_1r, ramp_data):
     """
     For datasets having >2 groups/integrations, for any semiramp in which the
     0th group is good and the 1st group is either SAT or CR, set slope, etc.
 
     Parameters
     ----------
     slope_s : ndarray
@@ -2904,14 +2901,17 @@
 
     data : float
         array of values for current data section
 
     wh_pix_1r : tuple
         locations of pixels whose only good group is the 0th group
 
+    ramp_data : RampData
+        The ramp data needed for processing, specifically flag values.
+
     Returns
     -------
     slope_s : ndarray
         1-D weighted slope for current iteration's pixels for data section
 
     intercept_s : ndarray
         1-D y-intercepts from fit for data section
@@ -2922,28 +2922,45 @@
     sig_slope_s : ndarray
         1-D sigma of slopes from fit for data section
 
     sig_intercept_s : ndarray
         1-D sigma of y-intercepts from fit for data section
     """
     data0_slice = data[0, :, :].reshape(npix)
-    slope_s[wh_pix_1r] = data0_slice[wh_pix_1r]
+
+    # If the one_groups_time is defined, use it.
+    if ramp_data.one_groups_time is not None:
+        slope_s[wh_pix_1r] = data0_slice[wh_pix_1r] / ramp_data.one_groups_time
+        timing = ramp_data.one_groups_time
+    else:
+        slope_s[wh_pix_1r] = data0_slice[wh_pix_1r] / ramp_data.group_time
+        timing = ramp_data.group_time
+
+    # Adjust slope if ZEROFRAME used.  The slope numerator should be
+    # the frame time if the ZEROFRAME is used.
+    if ramp_data.zframe_mat is not None:
+        adjustment = timing / ramp_data.frame_time
+        good_0th_mat = np.zeros((data0_slice.shape), dtype=np.uint8)
+        good_0th_mat[wh_pix_1r] = 1
+        zframe = ramp_data.zframe_mat[ramp_data.current_integ, :, :].reshape(npix)
+        adj_mat = good_0th_mat & zframe
+        slope_s[adj_mat == 1] *= adjustment
 
     # The following arrays will have values correctly calculated later; for
     #   now they are just place-holders
     variance_s[wh_pix_1r] = utils.LARGE_VARIANCE
     sig_slope_s[wh_pix_1r] = 0.
     intercept_s[wh_pix_1r] = 0.
     sig_intercept_s[wh_pix_1r] = 0.
 
     return slope_s, intercept_s, variance_s, sig_slope_s, sig_intercept_s
 
 
 def fit_double_read(mask_2d, wh_pix_2r, data_masked, slope_s, intercept_s,
-                    variance_s, sig_slope_s, sig_intercept_s, rn_sect):
+                    variance_s, sig_slope_s, sig_intercept_s, rn_sect, ramp_data):
     """
     Process all semi-ramps having exactly 2 good groups. May need to optimize
     later to remove loop over pixels.
 
     Parameters
     ----------
     mask_2d : ndarray
@@ -2969,14 +2986,17 @@
 
     sig_intercept_s : ndarray
         1-D sigma of y-intercepts from fit for data section
 
     rn_sect : ndarray
         2-D read noise values for all pixels in data section
 
+    ramp_data : RampData
+        The ramp data needed for processing, specifically flag values.
+
     Returns
     -------
     slope_s : ndarray
         1-D weighted slope for current iteration's pixels for data section
 
     intercept_s : ndarray
         1-D y-intercepts from fit for data section
@@ -2999,15 +3019,15 @@
 
         read_nums = np.where(mask_2d[:, pixel_ff])
         second_read = read_nums[0][1]
         data_ramp = data_masked[:, pixel_ff] * mask_2d[:, pixel_ff]
         data_semi = data_ramp[mask_2d[:, pixel_ff]]  # picks only the 2
         diff_data = data_semi[1] - data_semi[0]
 
-        slope_s[pixel_ff] = diff_data
+        slope_s[pixel_ff] = diff_data / ramp_data.group_time
         intercept_s[pixel_ff] = \
             data_semi[1] * (1. - second_read) + data_semi[0] * second_read  # by geometry
         variance_s[pixel_ff] = 2.0 * rn * rn
         sig_slope_s[pixel_ff] = np.sqrt(2) * rn
         sig_intercept_s[pixel_ff] = np.sqrt(2) * rn
 
     return slope_s, intercept_s, variance_s, sig_slope_s, sig_intercept_s
@@ -3126,15 +3146,15 @@
 
     warnings.resetwarnings()
 
     return slope, intercept, sig_slope, sig_intercept
 
 
 def fit_1_group(slope_s, intercept_s, variance_s, sig_intercept_s,
-                sig_slope_s, npix, data, mask_2d):
+                sig_slope_s, npix, data, mask_2d, ramp_data):
     """
     This function sets the fitting arrays for datasets having only 1 group
     per integration.
 
     Parameters
     ----------
     slope_s : ndarray
@@ -3157,14 +3177,17 @@
 
     data : float
         array of values for current data section
 
     mask_2d : ndarray
         delineates which channels to fit for each pixel, 2-D bool
 
+    ramp_data : RampData
+        The ramp data needed for processing, specifically flag values.
+
     Returns
     -------
     slope_s : ndarray
         weighted slope for current iteration's pixels for data section, 1-D float
 
     intercept_s : ndarray
         y-intercepts from fit for data section, 1-D float
@@ -3179,14 +3202,15 @@
         sigma of slopes from fit for data section, 1-D float
     """
     # For pixels not saturated, recalculate the slope as the value of the SCI
     #   data in that group, which will later be divided by the group exposure
     #   time to give the count rate. Recalculate other fit quantities to be
     #   benign.
     slope_s = data[0, :, :].reshape(npix)
+    slope_s = slope_s / ramp_data.group_time
 
     # The following arrays will have values correctly calculated later; for
     #    now they are just place-holders
     variance_s = np.zeros(npix, dtype=np.float32) + utils.LARGE_VARIANCE
     sig_slope_s = slope_s * 0.
     intercept_s = slope_s * 0.
     sig_intercept_s = slope_s * 0.
@@ -3404,14 +3428,16 @@
     one_group_locs = np.where(bad_0_good_1)
     if len(one_group_locs[0]) > 0:
         data1 = data_r[1, :]
         slope_s[one_group_locs] = data1[one_group_locs]
         variance_s[one_group_locs] = 1.
     del one_group_locs
 
+    slope_s = slope_s / ramp_data.group_time
+
     return slope_s, intercept_s, variance_s, sig_intercept_s, sig_slope_s
 
 
 def calc_num_seg(gdq, n_int, jump_det, do_not_use):
     """
     Calculate the maximum number of segments that will be fit within an
     integration, calculated over all pixels and all integrations.  This value
```

### Comparing `stcal-1.3.8/src/stcal/ramp_fitting/ramp_fit.py` & `stcal-1.4.0/src/stcal/ramp_fitting/ramp_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/src/stcal/ramp_fitting/ramp_fit_class.py` & `stcal-1.4.0/src/stcal/ramp_fitting/ramp_fit_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self.flags_do_not_use = None
         self.flags_jump_det = None
         self.flags_saturated = None
         self.flags_no_gain_val = None
         self.flags_unreliable_slope = None
 
         # ZEROFRAME
+        self.zframe_mat = None
         self.zframe_locs = None
         self.zframe_cnt = 0
         self.zeroframe = None
 
         # Slice info
         self.start_row = None
         self.num_rows = None
```

### Comparing `stcal-1.3.8/src/stcal/ramp_fitting/utils.py` & `stcal-1.4.0/src/stcal/ramp_fitting/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,30 +246,30 @@
         max_num_crs = end_cr.max()
         if max_num_crs == 0:
             max_num_crs = 1
             self.cr_mag_seg = np.zeros(shape=(n_int, 1, imshape[0], imshape[1]))
         else:
             self.cr_mag_seg = cr_com[:, :max_num_crs, :, :]
 
-    def output_optional(self, effintim):
+    def output_optional(self, group_time):
         """
         These results are the cosmic ray magnitudes in the
         segment-specific results for the count rates, y-intercept,
         uncertainty in the slope, uncertainty in the y-intercept,
         pedestal image, fitting weights, and the uncertainties in
         the slope due to poisson noise only and read noise only, and
         the integration-specific results for the pedestal image.  The
         slopes are divided by the effective integration time here to
         yield the count rates. Any variance values that are a large fraction
         of the default value LARGE_VARIANCE correspond to non-existent segments,
         so will be set to 0 here before output.
 
         Parameters
         ----------
-        effintim : float
+        group_time : float
             effective integration time for a single group
 
         Returns
         -------
         opt_info : tuple
             The tuple of computed optional results arrays for fitting.
         """
@@ -280,16 +280,14 @@
         warnings.filterwarnings("ignore", ".*invalid value.*", RuntimeWarning)
         warnings.filterwarnings("ignore", ".*divide by zero.*", RuntimeWarning)
 
         # Tiny 'weights' values correspond to non-existent segments, so set to 0.
         self.weights[1. / self.weights > LARGE_VARIANCE_THRESHOLD] = 0.
         warnings.resetwarnings()
 
-        self.slope_seg /= effintim
-
         opt_info = (self.slope_seg, self.sigslope_seg, self.var_p_seg,
                     self.var_r_seg, self.yint_seg, self.sigyint_seg,
                     self.ped_int, self.weights, self.cr_mag_seg)
 
         return opt_info
 
     def print_full(self):  # pragma: no cover
@@ -627,16 +625,16 @@
     # overwrite where segs>1
     den_r3[wh_seg_pos] = 1. / (segs_beg_3[wh_seg_pos] ** 3. - segs_beg_3[wh_seg_pos])
     warnings.resetwarnings()
 
     return den_r3, den_p3, num_r3, segs_beg_3
 
 
-def calc_pedestal(ramp_data, num_int, slope_int, firstf_int, dq_first, nframes,
-                  groupgap, dropframes1):
+def calc_pedestal(ramp_data, num_int, slope_int, firstf_int, dq_first,
+                  nframes, groupgap, dropframes1):
     """
     The pedestal is calculated by extrapolating the final slope for each pixel
     from its value at the first sample in the integration to an exposure time
     of zero; this calculation accounts for the values of nframes and groupgap.
     Any pixel that is saturated on the 1st group is given a pedestal value of 0.
 
     Parameters
@@ -667,25 +665,25 @@
 
     Returns
     -------
     ped : ndarray
         pedestal image, 2-D float
     """
     ff_all = firstf_int[num_int, :, :].astype(np.float32)
-    ped = ff_all - slope_int[num_int, ::] * \
-        (((nframes + 1.) / 2. + dropframes1) / (nframes + groupgap))
+    tmp = (((nframes + 1.) / 2. + dropframes1) / (nframes + groupgap))
+    ped = ff_all - slope_int[num_int, ::] * tmp
 
     sat_flag = ramp_data.flags_saturated
     ped[np.bitwise_and(dq_first, sat_flag) == sat_flag] = 0
     ped[np.isnan(ped)] = 0.
 
     return ped
 
 
-def output_integ(ramp_data, slope_int, dq_int, effintim, var_p3, var_r3, var_both3):
+def output_integ(ramp_data, slope_int, dq_int, var_p3, var_r3, var_both3):
     """
     For the OLS algorithm, construct the output integration-specific results.
     Any variance values that are a large fraction of the default value
     LARGE_VARIANCE correspond to non-existent segments, so will be set to 0
     here before output.
 
     Parameters
@@ -698,17 +696,14 @@
 
     slope_int : ndarray
        Data cube of weighted slopes for each integration, 3-D float
 
     dq_int : ndarray
        Data cube of DQ arrays for each integration, 3-D int
 
-    effintim : float
-       Effective integration time per integration
-
     var_p3 : ndarray
         Cube of integration-specific values for the slope variance due to
         Poisson noise only, 3-D float
 
     var_r3 : ndarray
         Cube of integration-specific values for the slope variance due to
         read noise only, 3-D float
@@ -727,15 +722,15 @@
     warnings.filterwarnings("ignore", ".*invalid value.*", RuntimeWarning)
     warnings.filterwarnings("ignore", ".*divide by zero.*", RuntimeWarning)
 
     var_p3[var_p3 > LARGE_VARIANCE_THRESHOLD] = 0.
     var_r3[var_r3 > LARGE_VARIANCE_THRESHOLD] = 0.
     var_both3[var_both3 > LARGE_VARIANCE_THRESHOLD] = 0.
 
-    data = slope_int / effintim
+    data = slope_int
     invalid_data = ramp_data.flags_saturated | ramp_data.flags_do_not_use
     data[np.bitwise_and(dq_int, invalid_data).astype(bool)] = np.nan
 
     err = np.sqrt(var_both3)
     dq = dq_int
     var_poisson = var_p3
 
@@ -831,14 +826,15 @@
     b[bi_z:bf_z, :, :] = a[ai_z:af_z, :, :]
 
     return b
 
 
 def get_efftim_ped(ramp_data):
     """
+    XXX - Work to remove this function.
     Calculate the effective integration time for a single group, and return the
     number of frames per group, and the number of frames dropped between groups.
 
     Parameters
     ----------
     ramp_data: RampClass
         Object for input data.
@@ -1588,14 +1584,15 @@
     sat_flag = ramp_data.flags_saturated
     good_flag = 0
     dq = ramp_data.groupdq
 
     zframe_locs = [None] * nints
 
     cnt = 0
+    zframe_mat = np.zeros((nints, nrows, ncols), dtype=np.uint8)
     for integ in range(nints):
         intdq = dq[integ, :, :, :]
 
         # Find ramps with a good zeroeth group, but saturated in
         # the remainder of the ramp.
         wh_sat = groups_saturated_in_integration(intdq, sat_flag, ngroups)
 
@@ -1610,19 +1607,20 @@
             # that is non-zero.  If it is non-zero, replace group zero in the
             # ramp with the data in ZEROFRAME.
             if ramp_data.zeroframe[integ, row, col] != 0:
                 row_list.append(row)
                 col_list.append(col)
                 ramp_data.data[integ, 0, row, col] = ramp_data.zeroframe[integ, row, col]
                 ramp_data.groupdq[integ, 0, row, col] = good_flag
+                zframe_mat[integ, row, col] = 1
                 cnt = cnt + 1
 
         zframe_locs[integ] = (np.array(row_list, dtype=int), np.array(col_list, dtype=int))
 
-    return zframe_locs, cnt
+    return zframe_mat, zframe_locs, cnt
 
 
 def groups_saturated_in_integration(intdq, sat_flag, num_sat_groups):
     """
     Find the ramps in an integration that have num_sat_groups saturated.
 
     Parameters
```

### Comparing `stcal-1.3.8/src/stcal/saturation/saturation.py` & `stcal-1.4.0/src/stcal/saturation/saturation.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         updated group dq array
 
     pdq : int, 2D array
         updated pixel dq array
     """
 
     nints, ngroups, nrows, ncols = data.shape
-
     saturated = dqflags['SATURATED']
     ad_floor = dqflags['AD_FLOOR']
     no_sat_check = dqflags['NO_SAT_CHECK']
 
     # For pixels flagged in reference file as NO_SAT_CHECK,
     # set the saturation check threshold above the A-to-D converter limit,
     # so that they don't get flagged as saturated.
```

### Comparing `stcal-1.3.8/src/stcal.egg-info/PKG-INFO` & `stcal-1.4.0/src/stcal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.3.8
+Version: 1.4.0
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.3.8/src/stcal.egg-info/SOURCES.txt` & `stcal-1.4.0/src/stcal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/current_gdqfits` & `stcal-1.4.0/tests/current_gdqfits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/data/input_gdq_flarge.fits` & `stcal-1.4.0/tests/data/input_gdq_flarge.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/data/large_event_input_dq_cube2.fits` & `stcal-1.4.0/tests/data/large_event_input_dq_cube2.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/data/snowball1.fits` & `stcal-1.4.0/tests/data/snowball1.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/test_dark_current.py` & `stcal-1.4.0/tests/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/test_dq.py` & `stcal-1.4.0/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/test_jump.py` & `stcal-1.4.0/tests/test_jump.py`

 * *Files 12% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     data = np.zeros(shape=(nint, ngrps, nrows, ncols), dtype=np.float32)
     gdq = np.zeros_like(data, dtype=np.uint8)
     gain = 4
     readnoise = np.ones(shape=(nrows, ncols), dtype=np.float32) * 6.0 * gain
     rng = np.random.default_rng(12345)
     data[0, 1:, 14:20, 15:20] = 6 * gain * 1.7
     data = data + rng.normal(size=(nint, ngrps, nrows, ncols)) * readnoise
-    gdq, num_showers = find_faint_extended(data, gdq, readnoise, 1,
+    gdq, num_showers = find_faint_extended(data, gdq, readnoise, 1, 100,
                                            snr_threshold=1.3,
                                            min_shower_area=20, inner=1,
                                            outer=2, sat_flag=2, jump_flag=4,
                                            ellipse_expand=1.1, num_grps_masked=3)
     #  Check that all the expected samples in group 2 are flagged as jump and
     #  that they are not flagged outside
     assert (np.all(gdq[0, 1, 22, 14:23] == 0))
@@ -189,14 +189,48 @@
     assert (np.all(gdq[0, 2, 12, 14:23] == 0))
     assert (np.all(gdq[0, 2, 12:22, 24] == 0))
     assert (np.all(gdq[0, 2, 12:22, 13] == 0))
 
     #  Check that the flags are not applied in the 3rd group after the event
     assert (np.all(gdq[0, 4, 12:22, 14:23]) == 0)
 
+# No shower is found because the event is identical in all ints
+def test_find_faint_extended_sigclip():
+    nint, ngrps, ncols, nrows = 101, 6, 30, 30
+    data = np.zeros(shape=(nint, ngrps, nrows, ncols), dtype=np.float32)
+    gdq = np.zeros_like(data, dtype=np.uint8)
+    gain = 4
+    readnoise = np.ones(shape=(nrows, ncols), dtype=np.float32) * 6.0 * gain
+    rng = np.random.default_rng(12345)
+    data[0, 1:, 14:20, 15:20] = 6 * gain * 1.7
+    data = data + rng.normal(size=(nint, ngrps, nrows, ncols)) * readnoise
+    gdq, num_showers = find_faint_extended(data, gdq, readnoise, 1, 100,
+                                           snr_threshold=1.3,
+                                           min_shower_area=20, inner=1,
+                                           outer=2, sat_flag=2, jump_flag=4,
+                                           ellipse_expand=1.1, num_grps_masked=3)
+    #  Check that all the expected samples in group 2 are flagged as jump and
+    #  that they are not flagged outside
+    assert (np.all(gdq[0, 1, 22, 14:23] == 0))
+    assert (np.all(gdq[0, 1, 21, 16:20] == 0))
+    assert (np.all(gdq[0, 1, 20, 15:22] == 0))
+    assert (np.all(gdq[0, 1, 19, 15:23] == 0))
+    assert (np.all(gdq[0, 1, 18, 14:23] == 0))
+    assert (np.all(gdq[0, 1, 17, 14:23] == 0))
+    assert (np.all(gdq[0, 1, 16, 14:23] == 0))
+    assert (np.all(gdq[0, 1, 15, 14:22] == 0))
+    assert (np.all(gdq[0, 1, 14, 16:22] == 0))
+    assert (np.all(gdq[0, 1, 13, 17:21] == 0))
+    assert (np.all(gdq[0, 1, 12, 14:23] == 0))
+    assert (np.all(gdq[0, 1, 12:23, 24] == 0))
+    assert (np.all(gdq[0, 1, 12:23, 13] == 0))
+
+    #  Check that the flags are not applied in the 3rd group after the event
+    assert (np.all(gdq[0, 4, 12:22, 14:23]) == 0)
+
 
 def test_inside_ellipse5():
     ellipse = ((0, 0), (1, 2), -10)
     point = (1, 0.6)
     result = point_inside_ellipse(point, ellipse)
     assert not result
```

### Comparing `stcal-1.3.8/tests/test_linearity.py` & `stcal-1.4.0/tests/test_linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/test_ramp_fitting.py` & `stcal-1.4.0/tests/test_ramp_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 from stcal.ramp_fitting.ramp_fit import ramp_fit_data
 from stcal.ramp_fitting.ramp_fit_class import RampData
 
 
 DELIM = "-" * 70
 
 # single group intergrations fail in the GLS fitting
@@ -470,16 +469,17 @@
 
     In the second integration all pixels have all good groups.
     """
     # Define the data.
     ngroups, nrows, ncols = 5, 1, 3
     dims = (nints, ngroups, nrows, ncols)
     rnoise, gain = 10, 1
-    nframes, group_time, frame_time = 1, 5.0, 1
+    nframes, frame_time, groupgap = 1, 1, 0
     var = rnoise, gain
+    group_time = (nframes + groupgap) * frame_time
     tm = nframes, group_time, frame_time
 
     # Using the above create the classes and arrays.
     ramp_data, rnoise2d, gain2d = setup_inputs(dims, var, tm)
 
     arr = np.array([k + 1 for k in range(ngroups)], dtype=float)
 
@@ -524,90 +524,90 @@
     slopes, cube, dims = run_one_group_ramp_suppression(1, True)
     nints, ngroups, nrows, ncols = dims
     tol = 1e-5
 
     # Check slopes information
     sdata, sdq, svp, svr, serr = slopes
 
-    check = np.array([[np.nan, np.nan, 1.0000002]])
+    check = np.array([[np.nan, np.nan, 1.0000001]])
     np.testing.assert_allclose(sdata, check, tol)
 
     check = np.array([[DNU | SAT, DNU, GOOD]])
     np.testing.assert_allclose(sdq, check, tol)
 
-    check = np.array([[0., 0., 0.01]])
+    check = np.array([[0., 0., 0.25]])
     np.testing.assert_allclose(svp, check, tol)
 
-    check = np.array([[0., 0., 0.19999999]])
+    check = np.array([[0., 0., 4.999999]])
     np.testing.assert_allclose(svr, check, tol)
 
-    check = np.array([[0., 0., 0.45825756]])
+    check = np.array([[0., 0., 2.2912877]])
     np.testing.assert_allclose(serr, check, tol)
 
     # Check slopes information
     cdata, cdq, cvp, cvr, cerr = cube
 
     check = np.array([[[np.nan, np.nan, 1.0000001]]])
     np.testing.assert_allclose(cdata, check, tol)
 
     check = np.array([[[DNU | SAT, DNU, GOOD]]])
     np.testing.assert_allclose(cdq, check, tol)
 
-    check = np.array([[[0., 0., 0.01]]])
+    check = np.array([[[0., 0., 0.25]]])
     np.testing.assert_allclose(cvp, check, tol)
 
-    check = np.array([[[0., 0., 0.19999999]]])
+    check = np.array([[[0., 0., 4.999999]]])
     np.testing.assert_allclose(cvr, check, tol)
 
-    check = np.array([[[0., 0., 0.4582576]]])
+    check = np.array([[[0., 0., 2.291288]]])
     np.testing.assert_allclose(cerr, check, tol)
 
 
 def test_one_group_ramp_not_suppressed_one_integration():
     """
     Tests one group ramp fitting where suppression turned off.
     """
     slopes, cube, dims = run_one_group_ramp_suppression(1, False)
     nints, ngroups, nrows, ncols = dims
     tol = 1e-5
 
     # Check slopes information
     sdata, sdq, svp, svr, serr = slopes
 
-    check = np.array([[np.nan, 1., 1.0000002]])
+    check = np.array([[np.nan, 1., 1.0000001]])
     np.testing.assert_allclose(sdata, check, tol)
 
     check = np.array([[DNU | SAT, GOOD, GOOD]])
     np.testing.assert_allclose(sdq, check, tol)
 
-    check = np.array([[0., 0.04, 0.01]])
+    check = np.array([[0., 1., 0.25]])
     np.testing.assert_allclose(svp, check, tol)
 
-    check = np.array([[0., 3.9999995, 0.19999999]])
+    check = np.array([[0., 100., 5.0000005]])
     np.testing.assert_allclose(svr, check, tol)
 
-    check = np.array([[0., 2.009975, 0.45825756]])
+    check = np.array([[0., 10.049875, 2.291288]])
     np.testing.assert_allclose(serr, check, tol)
 
     # Check slopes information
     cdata, cdq, cvp, cvr, cerr = cube
 
     check = np.array([[[np.nan, 1., 1.0000001]]])
     np.testing.assert_allclose(cdata, check, tol)
 
     check = np.array([[[DNU | SAT, GOOD, GOOD]]])
     np.testing.assert_allclose(cdq, check, tol)
 
-    check = np.array([[[0., 0.04, 0.01]]])
+    check = np.array([[[0., 1, 0.25]]])
     np.testing.assert_allclose(cvp, check, tol)
 
-    check = np.array([[[0., 3.9999995, 0.19999999]]])
+    check = np.array([[[0., 100., 5.0000005]]])
     np.testing.assert_allclose(cvr, check, tol)
 
-    check = np.array([[[0., 2.0099752, 0.4582576]]])
+    check = np.array([[[0., 10.049875, 2.291288]]])
     np.testing.assert_allclose(cerr, check, tol)
 
 
 def test_one_group_ramp_suppressed_two_integrations():
     """
     Test one good group ramp and two integrations with
     suppression suppression turned on.
@@ -615,50 +615,50 @@
     slopes, cube, dims = run_one_group_ramp_suppression(2, True)
     nints, ngroups, nrows, ncols = dims
     tol = 1e-5
 
     # Check slopes information
     sdata, sdq, svp, svr, serr = slopes
 
-    check = np.array([[1.0000001, 1.0000001, 1.0000002]])
+    check = np.array([[1.0000001, 1.0000001, 1.0000001]])
     np.testing.assert_allclose(sdata, check, tol)
 
     check = np.array([[GOOD, GOOD, GOOD]])
     np.testing.assert_allclose(sdq, check, tol)
 
-    check = np.array([[0.005, 0.01, 0.005]])
+    check = np.array([[0.125, 0.25, 0.125]])
     np.testing.assert_allclose(svp, check, tol)
 
-    check = np.array([[0.19999999, 0.19999999, 0.09999999]])
+    check = np.array([[4.999998 , 4.999998 , 2.4999995]])
     np.testing.assert_allclose(svr, check, tol)
 
-    check = np.array([[0.45276925, 0.45825756, 0.32403702]])
+    check = np.array([[2.263846 , 2.2912874, 1.620185]])
     np.testing.assert_allclose(serr, check, tol)
 
     # Check slopes information
     cdata, cdq, cvp, cvr, cerr = cube
 
-    check = np.array([[[np.nan,    np.nan,    1.0000001]],
+    check = np.array([[[np.nan,     np.nan,     1.0000001]],
                       [[1.0000001, 1.0000001, 1.0000001]]])
     np.testing.assert_allclose(cdata, check, tol)
 
     check = np.array([[[DNU | SAT, DNU, GOOD]],
                       [[GOOD, GOOD, GOOD]]])
     np.testing.assert_allclose(cdq, check, tol)
 
-    check = np.array([[[0.,    0.,    0.01]],
-                      [[0.005, 0.01, 0.01]]])
+    check = np.array([[[0.,    0.,    0.25]],
+                      [[0.125, 0.25, 0.25]]])
     np.testing.assert_allclose(cvp, check, tol)
 
-    check = np.array([[[0.,         0.,         0.19999999]],
-                      [[0.19999999, 0.19999999, 0.19999999]]])
+    check = np.array([[[0.,             0., 4.999999]],
+                      [[4.999999, 4.999999, 4.999999]]])
     np.testing.assert_allclose(cvr, check, tol)
 
-    check = np.array([[[0.,         0.,         0.4582576]],
-                      [[0.45276922, 0.4582576, 0.4582576]]])
+    check = np.array([[[0.,             0., 2.291288]],
+                      [[2.2638464, 2.291288, 2.291288]]])
     np.testing.assert_allclose(cerr, check, tol)
 
 
 def test_one_group_ramp_not_suppressed_two_integrations():
     """
     Test one good group ramp and two integrations with
     suppression suppression turned off.
@@ -666,50 +666,50 @@
     slopes, cube, dims = run_one_group_ramp_suppression(2, False)
     nints, ngroups, nrows, ncols = dims
     tol = 1e-5
 
     # Check slopes information
     sdata, sdq, svp, svr, serr = slopes
 
-    check = np.array([[1.0000001, 1.0000002, 1.0000002]])
+    check = np.array([[1.0000001, 1.0000001, 1.0000001]])
     np.testing.assert_allclose(sdata, check, tol)
 
     check = np.array([[GOOD, GOOD, GOOD]])
     np.testing.assert_allclose(sdq, check, tol)
 
-    check = np.array([[0.005, 0.008, 0.005]])
+    check = np.array([[0.125, 0.2, 0.125]])
     np.testing.assert_allclose(svp, check, tol)
 
-    check = np.array([[0.19999999, 0.19047618, 0.09999999]])
+    check = np.array([[5.       , 4.7619047, 2.5000002]])
     np.testing.assert_allclose(svr, check, tol)
 
-    check = np.array([[0.45276925, 0.44550666, 0.32403702]])
+    check = np.array([[2.2638464, 2.2275333, 1.6201853]])
     np.testing.assert_allclose(serr, check, tol)
 
     # Check slopes information
     cdata, cdq, cvp, cvr, cerr = cube
 
-    check = np.array([[[np.nan,    1.,        1.0000001]],
+    check = np.array([[[np.nan,     1.,        1.0000001]],
                       [[1.0000001, 1.0000001, 1.0000001]]])
     np.testing.assert_allclose(cdata, check, tol)
 
     check = np.array([[[DNU | SAT, GOOD, GOOD]],
                       [[GOOD, GOOD, GOOD]]])
     np.testing.assert_allclose(cdq, check, tol)
 
-    check = np.array([[[0.,    0.04, 0.01]],
-                      [[0.005, 0.01, 0.01]]])
+    check = np.array([[[0.,    1., 0.25]],
+                      [[0.125, 0.25, 0.25]]])
     np.testing.assert_allclose(cvp, check, tol)
 
-    check = np.array([[[0.,         3.9999995,  0.19999999]],
-                      [[0.19999999, 0.19999999, 0.19999999]]])
+    check = np.array([[[0.,             100., 5.0000005]],
+                      [[5.0000005, 5.0000005, 5.0000005]]])
     np.testing.assert_allclose(cvr, check, tol)
 
-    check = np.array([[[0.,         2.0099752, 0.4582576]],
-                      [[0.45276922, 0.4582576, 0.4582576]]])
+    check = np.array([[[0.,         10.049875 ,  2.291288]],
+                      [[2.2638464,  2.291288 ,  2.291288]]])
     np.testing.assert_allclose(cerr, check, tol)
 
 
 def create_zero_frame_data():
     """
     A two integration three pixel image.
 
@@ -794,15 +794,15 @@
         "optimal", ncores, dqflags)
 
     tol = 1.e-5
 
     # Check slopes information
     sdata, sdq, svp, svr, serr = slopes
 
-    check = np.array([[32.78594, 18.62891, 23.787909]])
+    check = np.array([[48.965397, 18.628912, 47.863224]])
     np.testing.assert_allclose(sdata, check, tol, tol)
 
     check = np.array([[GOOD, GOOD, GOOD]])
     np.testing.assert_allclose(sdq, check, tol, tol)
 
     check = np.array([[0.13110262, 0.00867591, 0.29745975]])
     np.testing.assert_allclose(svp, check, tol, tol)
@@ -815,15 +815,15 @@
 
     # Check slopes information
     cdata, cdq, cvp, cvr, cerr = cube
 
     # The third pixel in integration zero has good data
     # because the zeroframe has good data, so the ramp
     # is not fully saturated.
-    check = np.array([[[149.0313, np.nan, 130.40239]],
+    check = np.array([[[298.0626, np.nan, 652.01196]],
                       [[18.62891, 18.62891, 18.62891]]])
     np.testing.assert_allclose(cdata, check, tol, tol)
 
     check = np.array([[[GOOD, DNU | SAT, GOOD]],
                       [[GOOD, GOOD, GOOD]]])
     np.testing.assert_allclose(cdq, check, tol, tol)
 
@@ -919,15 +919,15 @@
 
     # The slopes for the first two ramps should be the same, including
     # for the rateints directory.  The last ramp will be different
     # because a different time is used as the denominator for the slope.
     # Because the number of groups used in the first two ramps are different
     # the variances are expected to be different, even though the slopes
     # should be the same.
-    check = np.array([[37.257824,  37.257824, 149.0313]])
+    check = np.array([[37.257824,  37.257824, 496.77103]])
     np.testing.assert_allclose(sdata, check, tol, tol)
 
     check = np.array([[GOOD, GOOD, GOOD]])
     np.testing.assert_allclose(sdq, check, tol, tol)
 
     check = np.array([[0.03470363, 0.13881457, 6.169534]])
     np.testing.assert_allclose(svp, check, tol, tol)
@@ -1410,14 +1410,18 @@
     print(f"----> Line = {line_number} <----")
     base_print("real", real)
     print("=" * 80)
     base_print("check", check)
     print("=" * 80)
 
 
+def print_arr_str(arr):
+    return np.array2string(arr, max_line_width=np.nan, separator=", ")
+
+
 def base_print(label, arr):
     arr_str = np.array2string(arr, max_line_width=np.nan, separator=", ")
     print(label)
     print(arr_str)
 
 
 def print_slope_data(slopes):
@@ -1559,23 +1563,7 @@
         oyint, osigyint, opedestal, oweights, ocrmag = optional
     """
 
     print(" ")
     print_slopes(slopes)
     print_integ(cube)
     print_optional(optional)
-
-
-def print_ramp_data(ramp_data):
-    print(DELIM)
-    print_ramp_data_data(ramp_data)
-    print(DELIM)
-    print_ramp_data_dq(ramp_data)
-    print(DELIM)
-
-
-def print_ramp_data_data(ramp_data):
-    base_print("RampData Data:", ramp_data.data)
-
-
-def print_ramp_data_dq(ramp_data):
-    base_print("RampData Data Quality:", ramp_data.groupdq)
```

### Comparing `stcal-1.3.8/tests/test_ramp_fitting_gls_fit.py` & `stcal-1.4.0/tests/test_ramp_fitting_gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/test_saturation.py` & `stcal-1.4.0/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.8/tests/test_twopoint_difference.py` & `stcal-1.4.0/tests/test_twopoint_difference.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import numpy as np
+from astropy.io import fits
 
 from stcal.jump.twopoint_difference import find_crs, calc_med_first_diffs
 
 
 DQFLAGS = {'JUMP_DET': 4, 'SATURATED': 2, 'DO_NOT_USE': 1}
 
 
@@ -24,41 +25,41 @@
 
     return _cube
 
 
 def test_nocrs_noflux(setup_cube):
     ngroups = 5
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
 
     assert(0 == np.max(out_gdq))  # no CR found
 
 
 def test_5grps_cr3_noflux(setup_cube):
     ngroups = 5
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
 
     data[0, 0:2, 100, 100] = 10.0
     data[0, 2:5, 100, 100] = 1000
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(2 == np.argmax(out_gdq[0, :, 100, 100]))  # find the CR in the expected group
 
 
 def test_5grps_cr2_noflux(setup_cube):
     ngroups = 5
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
 
     data[0, 0, 100, 100] = 10.0
     data[0, 1:6, 100, 100] = 1000
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(1 == np.argmax(out_gdq[0, :, 100, 100]))  # find the CR in the expected group
 
 
 def test_6grps_negative_differences_zeromedian(setup_cube):
@@ -67,52 +68,52 @@
 
     data[0, 0, 100, 100] = 100
     data[0, 1, 100, 100] = 90
     data[0, 2, 100, 100] = 95
     data[0, 3, 100, 100] = 105
     data[0, 4, 100, 100] = 100
     data[0, 5, 100, 100] = 100
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(0 == np.max(out_gdq))  # no CR was found
 
 
 def test_5grps_cr2_negjumpflux(setup_cube):
     ngroups = 5
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
 
     data[0, 0, 100, 100] = 1000.0
     data[0, 1:6, 100, 100] = 10
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(1 == np.argmax(out_gdq[0, :, 100, 100]))  # find the CR in the expected group
 
 
 def test_3grps_cr2_noflux(setup_cube):
     ngroups = 3
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
     data[0, 0, 100, 100] = 10.0
     data[0, 1:4, 100, 100] = 1000
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     #    assert(1,np.argmax(out_gdq[0, :, 100, 100]))  # find the CR in the expected group
     assert(np.array_equal([0, 4, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_4grps_cr2_noflux(setup_cube):
     ngroups = 4
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
     data[0, 0, 100, 100] = 10.0
     data[0, 1:4, 100, 100] = 1000
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(1 == np.argmax(out_gdq[0, :, 100, 100]))  # find the CR in the expected group
 
 
 def test_5grps_cr2_nframe2(setup_cube):
@@ -120,15 +121,15 @@
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
     nframes = 2
     data[0, 0, 100, 100] = 10.0
     data[0, 1, 100, 100] = 500
     data[0, 2, 100, 100] = 1002
     data[0, 3, 100, 100] = 1001
     data[0, 4, 100, 100] = 1005
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 4, 0, 0], out_gdq[0, :, 100, 100]))
 
 
 @pytest.mark.xfail
@@ -136,30 +137,30 @@
     ngroups = 4
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
     nframes = 1
     data[0, 0, 100, 100] = 10.0
     data[0, 1, 100, 100] = 60
     data[0, 2, 100, 100] = 60
     data[0, 3, 100, 100] = 115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(np.max(out_gdq) == 4)  # a CR was found
 
 
 def test_5grps_twocrs_2nd_5th(setup_cube):
     ngroups = 5
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
     nframes = 1
     data[0, 0, 100, 100] = 10.0
     data[0, 1, 100, 100] = 60
     data[0, 2, 100, 100] = 60
     data[0, 3, 100, 100] = 60
     data[0, 4, 100, 100] = 115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 4], out_gdq[0, :, 100, 100]))
 
 
 def test_5grps_twocrs_2nd_5thbig(setup_cube):
@@ -167,15 +168,15 @@
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
     nframes = 1
     data[0, 0, 100, 100] = 10.0
     data[0, 1, 100, 100] = 60
     data[0, 2, 100, 100] = 60
     data[0, 3, 100, 100] = 60
     data[0, 4, 100, 100] = 2115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 4], out_gdq[0, :, 100, 100]))
 
 
 def test_10grps_twocrs_2nd_8th_big(setup_cube):
@@ -188,15 +189,15 @@
     data[0, 3, 100, 100] = 60
     data[0, 4, 100, 100] = 60
     data[0, 5, 100, 100] = 60
     data[0, 6, 100, 100] = 60
     data[0, 7, 100, 100] = 2115
     data[0, 8, 100, 100] = 2115
     data[0, 9, 100, 100] = 2115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 0, 0, 0, 4, 0, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_10grps_twocrs_10percenthit(setup_cube):
@@ -209,15 +210,15 @@
     data[0:200, 3, 100, 100] = 60
     data[0:200, 4, 100, 100] = 60
     data[0:200, 5, 100, 100] = 60
     data[0:200, 6, 100, 100] = 60
     data[0:200, 7, 100, 100] = 2115
     data[0:200, 8, 100, 100] = 2115
     data[0:200, 9, 100, 100] = 2115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 0, 0, 0, 4, 0, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_5grps_twocrs_2nd_5thbig_nframes2(setup_cube):
@@ -225,15 +226,15 @@
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=10 * np.sqrt(2))
     nframes = 2
     data[0, 0, 100, 100] = 10.0
     data[0, 1, 100, 100] = 60
     data[0, 2, 100, 100] = 60
     data[0, 3, 100, 100] = 60
     data[0, 4, 100, 100] = 2115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 4], out_gdq[0, :, 100, 100]))
 
 
 def test_6grps_twocrs_2nd_5th(setup_cube):
@@ -242,15 +243,15 @@
     nframes = 1
     data[0, 0, 100, 100] = 10.0
     data[0, 1, 100, 100] = 60
     data[0, 2, 100, 100] = 60
     data[0, 3, 100, 100] = 60
     data[0, 4, 100, 100] = 115
     data[0, 5, 100, 100] = 115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert np.array_equal([0, 4, 0, 0, 4, 0], out_gdq[0, :, 100, 100])
 
 
 def test_6grps_twocrs_2nd_5th_nframes2(setup_cube):
@@ -259,15 +260,15 @@
     nframes = 2
     data[0, 0, 100, 100] = 10.0
     data[0, 1, 100, 100] = 60
     data[0, 2, 100, 100] = 60
     data[0, 3, 100, 100] = 60
     data[0, 4, 100, 100] = 115
     data[0, 5, 100, 100] = 115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 4, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_6grps_twocrs_twopixels_nframes2(setup_cube):
@@ -282,15 +283,15 @@
     data[0, 5, 100, 100] = 115
     data[0, 0, 200, 100] = 10.0
     data[0, 1, 200, 100] = 10.0
     data[0, 2, 200, 100] = 60
     data[0, 3, 200, 100] = 60
     data[0, 4, 200, 100] = 115
     data[0, 5, 200, 100] = 115
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 4, 0], out_gdq[0, :, 100, 100]))
     assert(np.array_equal([0, 0, 4, 0, 4, 0], out_gdq[0, :, 200, 100]))
 
 
@@ -299,15 +300,15 @@
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups)
     nframes = 1
     data[0, 0, 100, 100] = 100.0
     data[0, 1, 100, 100] = 0
     data[0, 2, 100, 100] = -200
     data[0, 3, 100, 100] = -260
     data[0, 4, 100, 100] = -360
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 0, 4, 0, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_6grps_1cr(setup_cube):
@@ -316,15 +317,15 @@
     nframes = 1
     data[0, 0, 100, 100] = 0
     data[0, 1, 100, 100] = 10
     data[0, 2, 100, 100] = 21
     data[0, 3, 100, 100] = 33
     data[0, 4, 100, 100] = 46
     data[0, 5, 100, 100] = 1146
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert (4 == out_gdq[0, 5, 100, 100])
 
 
 def test_7grps_1cr(setup_cube):
     ngroups = 7
@@ -333,15 +334,15 @@
     data[0, 0, 100, 100] = 0
     data[0, 1, 100, 100] = 10
     data[0, 2, 100, 100] = 21
     data[0, 3, 100, 100] = 33
     data[0, 4, 100, 100] = 46
     data[0, 5, 100, 100] = 60
     data[0, 6, 100, 100] = 1160
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == out_gdq[0, 6, 100, 100])
 
 
 def test_8grps_1cr(setup_cube):
     ngroups = 8
@@ -351,15 +352,15 @@
     data[0, 1, 100, 100] = 10
     data[0, 2, 100, 100] = 21
     data[0, 3, 100, 100] = 33
     data[0, 4, 100, 100] = 46
     data[0, 5, 100, 100] = 60
     data[0, 6, 100, 100] = 1160
     data[0, 7, 100, 100] = 1175
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == out_gdq[0, 6, 100, 100])
 
 
 def test_9grps_1cr_1sat(setup_cube):
     ngroups = 9
@@ -371,15 +372,15 @@
     data[0, 3, 100, 100] = 33
     data[0, 4, 100, 100] = 46
     data[0, 5, 100, 100] = 60
     data[0, 6, 100, 100] = 1160
     data[0, 7, 100, 100] = 1175
     data[0, 8, 100, 100] = 6175
     gdq[0, 8, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == out_gdq[0, 6, 100, 100])
 
 
 def test_10grps_1cr_2sat(setup_cube):
     ngroups = 10
@@ -393,15 +394,15 @@
     data[0, 5, 100, 100] = 60
     data[0, 6, 100, 100] = 1160
     data[0, 7, 100, 100] = 1175
     data[0, 8, 100, 100] = 6175
     data[0, 9, 100, 100] = 6175
     gdq[0, 8, 100, 100] = DQFLAGS['SATURATED']
     gdq[0, 9, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == out_gdq[0, 6, 100, 100])
 
 
 def test_11grps_1cr_3sat(setup_cube):
     ngroups = 11
@@ -417,15 +418,15 @@
     data[0, 7, 100, 100] = 1175
     data[0, 8, 100, 100] = 6175
     data[0, 9, 100, 100] = 6175
     data[0, 10, 100, 100] = 6175
     gdq[0, 8, 100, 100] = DQFLAGS['SATURATED']
     gdq[0, 9, 100, 100] = DQFLAGS['SATURATED']
     gdq[0, 10, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == out_gdq[0, 6, 100, 100])
 
 
 def test_11grps_0cr_3donotuse(setup_cube):
     ngroups = 11
@@ -441,113 +442,113 @@
     data[0, 7, 100, 100] = 131
     data[0, 8, 100, 100] = 150
     data[0, 9, 100, 100] = 6175
     data[0, 10, 100, 100] = 6175
     gdq[0, 0, 100, 100] = DQFLAGS['DO_NOT_USE']
     gdq[0, 9, 100, 100] = DQFLAGS['DO_NOT_USE']
     gdq[0, 10, 100, 100] = DQFLAGS['DO_NOT_USE']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert (np.array_equal([0, 0, 0, 0, 0, 0, 0, 0], out_gdq[0, 1:-2, 100, 100]))
 
 
 def test_5grps_nocr(setup_cube):
     ngroups = 6
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=10)
     nframes = 1
     data[0, 0, 100, 100] = 0
     data[0, 1, 100, 100] = 10
     data[0, 2, 100, 100] = 21
     data[0, 3, 100, 100] = 33
     data[0, 4, 100, 100] = 46
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
 
 
 def test_6grps_nocr(setup_cube):
     ngroups = 6
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=10)
     nframes = 1
     data[0, 0, 100, 100] = 0
     data[0, 1, 100, 100] = 10
     data[0, 2, 100, 100] = 21
     data[0, 3, 100, 100] = 33
     data[0, 4, 100, 100] = 46
     data[0, 5, 100, 100] = 60
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
 
 
 def test_10grps_cr2_gt3sigma(setup_cube):
     ngroups = 10
     crmag = 16
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=5)
     nframes = 1
     data[0, 0, 100, 100] = 0
     data[0, 1:11, 100, 100] = crmag
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 0, 0, 0, 0, 0, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_10grps_cr2_3sigma_nocr(setup_cube):
     ngroups = 10
     crmag = 15
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=5)
     nframes = 1
     data[0, 0, 100, 100] = 0
     data[0, 1:11, 100, 100] = crmag
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(0 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 0, 0, 0, 0, 0, 0, 0, 0, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_10grps_cr2_gt3sigma_2frames(setup_cube):
     ngroups = 10
     crmag = 16
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=5 * np.sqrt(2))
     nframes = 2
     data[0, 0, 100, 100] = 0
     data[0, 1:11, 100, 100] = crmag
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 0, 0, 0, 0, 0, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_10grps_cr2_gt3sigma_2frames_offdiag(setup_cube):
     ngroups = 10
     crmag = 16
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=5 * np.sqrt(2))
     nframes = 2
     data[0, 0, 100, 110] = 0
     data[0, 1:11, 100, 110] = crmag
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(4 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 4, 0, 0, 0, 0, 0, 0, 0, 0], out_gdq[0, :, 100, 110]))
 
 
 def test_10grps_cr2_3sigma_2frames_nocr(setup_cube):
     ngroups = 10
     crmag = 15
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=5 * np.sqrt(2))
     nframes = 2
     data[0, 0, 100, 100] = 0
     data[0, 1:11, 100, 100] = crmag
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(0 == np.max(out_gdq))  # a CR was found
     assert(np.array_equal([0, 0, 0, 0, 0, 0, 0, 0, 0, 0], out_gdq[0, :, 100, 100]))
 
 
 def test_10grps_nocr_2pixels_sigma0(setup_cube):
@@ -555,15 +556,15 @@
     crmag = 15
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=5 * np.sqrt(2))
     nframes = 1
     data[0, 0, 100, 100] = crmag
     data[0, 1:11, 100, 100] = crmag
     read_noise[50, 50] = 0.0
     read_noise[60, 60] = 0.0
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert(0 == np.max(out_gdq))  # no CR was found
 
 
 def test_5grps_satat4_crat3(setup_cube):
     ngroups = 5
@@ -572,15 +573,15 @@
     data[0, 0, 100, 100] = 10000
     data[0, 1, 100, 100] = 30000
     data[0, 2, 100, 100] = 60000
     data[0, 3, 100, 100] = 61000
     data[0, 4, 100, 100] = 61000
     gdq[0, 3, 100, 100] = DQFLAGS['SATURATED']
     gdq[0, 4, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     # assert(4 == np.max(out_gdq))  # no CR was found
     assert np.array_equal(
         [0, 0, DQFLAGS['JUMP_DET'], DQFLAGS['SATURATED'], DQFLAGS['SATURATED']],
         out_gdq[0, :, 100, 100])
 
@@ -599,15 +600,15 @@
     data[0, 0, 100, 101] = 10000
     data[0, 1, 100, 101] = 15001
     data[0, 2, 100, 101] = 20003
     data[0, 3, 100, 101] = 25006
     data[0, 4, 100, 101] = 30010
     data[0, 5, 100, 101] = 35015
     gdq[0, 5, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     # assert(4 == np.max(out_gdq))  # no CR was found
     assert (np.array_equal([0, DQFLAGS['JUMP_DET'], 0, 0, 0, DQFLAGS['SATURATED']], out_gdq[0, :, 100, 100]))
 
 
 @pytest.mark.xfail
@@ -625,15 +626,15 @@
     data[0, 0, 100, 101] = 10000
     data[0, 1, 100, 101] = 15001
     data[0, 2, 100, 101] = 20003
     data[0, 3, 100, 101] = 25006
     data[0, 4, 100, 101] = 30010
     data[0, 5, 100, 101] = 35015
     gdq[0, 5, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     # assert(4 == np.max(out_gdq))  # no CR was found
     assert (np.array_equal([0, DQFLAGS['JUMP_DET'], 0, 0, 0, DQFLAGS['SATURATED']], out_gdq[0, :, 100, 100]))
     assert (np.array_equal([0, DQFLAGS['JUMP_DET'], 0, 0, 0, DQFLAGS['SATURATED']], out_gdq[0, :, 99, 100]))
 
 
@@ -647,15 +648,15 @@
     data[0, 2, 100, 100] = 15000  # CR
     data[0, 3, 100, 100] = 20000
     data[0, 4, 100, 100] = 25000
     data[0, 5, 100, 100] = 40000  # CR
     data[0, 6, 100, 100] = 45000
     data[0, 7:11, 100, 100] = 61000
     gdq[0, 7:11, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     # assert(4 == np.max(out_gdq))  # no CR was found
     assert np.array_equal(
         [0, 0, DQFLAGS['JUMP_DET'], 0, 0, DQFLAGS['JUMP_DET'], 0,
             DQFLAGS['SATURATED'], DQFLAGS['SATURATED'], DQFLAGS['SATURATED']],
         out_gdq[0, :, 100, 100])
@@ -672,15 +673,15 @@
     data[0, 3, 100, 100] = 13800
     data[0, 4, 100, 100] = 18600
     data[0, 5, 100, 100] = 40000  # CR
     data[0, 6, 100, 100] = 44850
     data[0, 7, 100, 100] = 49900
     data[0, 8:10, 100, 100] = 60000
     gdq[0, 7:10, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert (np.array_equal([0, 0, 0, 0, 0, 4, 0, 2, 2, 2], out_gdq[0, :, 100, 100]))
 
 
 def test_median_with_saturation_even_num_sat_frames(setup_cube):
     ngroups = 10
@@ -693,15 +694,15 @@
     data[0, 3, 100, 100] = 13800
     data[0, 4, 100, 100] = 18600
     data[0, 5, 100, 100] = 40000  # CR
     data[0, 6, 100, 100] = 44850
     data[0, 7, 100, 100] = 49900
     data[0, 8:10, 100, 100] = 60000
     gdq[0, 6:10, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert (np.array_equal([0, 0, 0, 0, 0, 4, 2, 2, 2, 2], out_gdq[0, :, 100, 100]))
 
 
 def test_median_with_saturation_odd_number_final_difference(setup_cube):
     ngroups = 9
@@ -714,15 +715,15 @@
     data[0, 3, 100, 100] = 13800
     data[0, 4, 100, 100] = 18600
     data[0, 5, 100, 100] = 40000  # CR
     data[0, 6, 100, 100] = 44850
     data[0, 7, 100, 100] = 49900
     data[0, 8:9, 100, 100] = 60000
     gdq[0, 6:9, 100, 100] = DQFLAGS['SATURATED']
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS)
     assert (np.array_equal([0, 0, 0, 0, 0, 4, 2, 2, 2], out_gdq[0, :, 100, 100]))
 
 
 def test_first_last_group(setup_cube):
     ngroups = 7
@@ -742,15 +743,15 @@
     data[0, 4, 100, 100] = 40020.0
     data[0, 5, 100, 100] = 40040.0
     #  set group 6 to be 50,000
     data[0, 6, 100, 100] = 50000.0
 
     gdq[0, 0, 100, 100] = DQFLAGS['DO_NOT_USE']
     gdq[0, 6, 100, 100] = DQFLAGS['DO_NOT_USE']
-    outgdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    outgdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                     rej_threshold, rej_threshold, nframes,
                                                     False, 200, 10, DQFLAGS)
 
     assert outgdq[0, 0, 100, 100] == DQFLAGS['DO_NOT_USE']
     assert outgdq[0, 6, 100, 100] == DQFLAGS['DO_NOT_USE']
     assert outgdq[0, 3, 100, 100] == DQFLAGS['JUMP_DET']
 
@@ -760,15 +761,15 @@
     ngroups = 2
     data, gdq, nframes, read_noise, rej_threshold = setup_cube(ngroups, readnoise=25.0)
 
     data[0, 0, 0, 0] = 10000.0
     #  set groups 1,2 - to be around 30,000
     data[0, 1, 0, 0] = 30000.0
 
-    outgdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    outgdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                     rej_threshold, rej_threshold, nframes,
                                                     False, 200, 10, DQFLAGS)
     assert outgdq[0, 1, 0, 0] == 0
     assert outgdq[0, 0, 0, 0] == 0
 
 
 def test_4group(setup_cube):
@@ -777,15 +778,15 @@
 
     data[0, 0, 0, 0] = 10000.0
     #  set groups 1,2 - to be around 30,000
     data[0, 1, 0, 0] = 30000.0
     data[0, 2, 0, 0] = 30020.0
     data[0, 3, 0, 0] = 30000.0
 
-    outgdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    outgdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                     rej_threshold, rej_threshold, nframes,
                                                     False, 200, 10, DQFLAGS)
     assert outgdq[0, 1, 0, 0] == 4
 
 
 def test_first_last_4group(setup_cube):
     ngroups = 4
@@ -797,15 +798,15 @@
     #  set groups 1,2 - to be around 30,000
     data[0, 1, 0, 0] = 30000.0
     data[0, 2, 0, 0] = 30020.0
     data[0, 3, 0, 0] = 30000.0
     # treat as MIRI data with first and last flagged
     gdq[0, 0, :, :] = DQFLAGS['DO_NOT_USE']
     gdq[0, 3, :, :] = DQFLAGS['DO_NOT_USE']
-    outgdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    outgdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                     rej_threshold, rej_threshold, nframes,
                                                     False, 200, 10, DQFLAGS)
 
     assert outgdq[0, 0, 0, 0] == DQFLAGS['DO_NOT_USE']
     assert outgdq[0, 3, 0, 0] == DQFLAGS['DO_NOT_USE']
     assert outgdq[0, 1, 0, 0] == 0
 
@@ -819,15 +820,15 @@
     #  and group 6-7. Add a jump between 3 and 4 just to make sure jump detection is working
     #  set group 1 to be 10,000
     data[0, 0, 0, 0] = 10000.0
     data[0, 1, 0, 0] = 10100.0
     data[0, 2, 0, 0] = 30020.0
 
     gdq[0, 2, 0, 0] = DQFLAGS['DO_NOT_USE']  # only flag the last group
-    outgdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    outgdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                     rej_threshold, rej_threshold, nframes,
                                                     False, 200, 10, DQFLAGS)
 
     assert outgdq[0, 0, 0, 0] == 0
     assert outgdq[0, 2, 0, 0] == DQFLAGS['DO_NOT_USE']
     assert outgdq[0, 1, 0, 0] == 0
 
@@ -844,15 +845,15 @@
     data[0, 5, 100, 100] = 60
     data[0, 6, 100, 100] = 1160
     data[0, 7, 100, 100] = 1175
     data[0, 8, 100, 100] = 1190
     data[0, 9, 100, 100] = 1209
 
     after_jump_flag_e1 = np.full(data.shape[2:4], 1.0) * 0.0
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS,
                                                      after_jump_flag_e1=after_jump_flag_e1,
                                                      after_jump_flag_n1=10)
     # all groups after CR should be flagged
     for k in range(6, 10):
         assert 4 == out_gdq[0, k, 100, 100], f"after jump flagging failed in group {k}"
@@ -870,15 +871,15 @@
     data[0, 5, 100, 100] = 60
     data[0, 6, 100, 100] = 1160
     data[0, 7, 100, 100] = 1175
     data[0, 8, 100, 100] = 1190
     data[0, 9, 100, 100] = 1209
 
     after_jump_flag_e1 = np.full(data.shape[2:4], 1.0) * 0.0
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS,
                                                      after_jump_flag_e1=after_jump_flag_e1,
                                                      after_jump_flag_n1=2)
 
     # 2 groups after CR should be flagged
     for k in range(6, 9):
@@ -901,15 +902,15 @@
     data[0, 5, 100, 100] = 60
     data[0, 6, 100, 100] = 1160
     data[0, 7, 100, 100] = 1175
     data[0, 8, 100, 100] = 1190
     data[0, 9, 100, 100] = 1209
 
     after_jump_flag_e1 = np.full(data.shape[2:4], 1.0) * 10000.0
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS,
                                                      after_jump_flag_e1=after_jump_flag_e1,
                                                      after_jump_flag_n1=10)
     # all groups after CR should be flagged
     for k in range(7, 10):
         assert 0 == out_gdq[0, k, 100, 100], f"after jump flagging incorrect in group {k}"
@@ -928,15 +929,15 @@
     data[0, 6, 100, 100] = 1160
     data[0, 7, 100, 100] = 1175
     data[0, 8, 100, 100] = 1190
     data[0, 9, 100, 100] = 1209
 
     after_jump_flag_e1 = np.full(data.shape[2:4], 1.0) * 500.
     after_jump_flag_e2 = np.full(data.shape[2:4], 1.0) * 10.
-    out_gdq, row_below_gdq, row_above_gdq = find_crs(data, gdq, read_noise, rej_threshold,
+    out_gdq, row_below_gdq, rows_above_gdq, total_crs, stddev = find_crs(data, gdq, read_noise, rej_threshold,
                                                      rej_threshold, rej_threshold, nframes,
                                                      False, 200, 10, DQFLAGS,
                                                      after_jump_flag_e1=after_jump_flag_e1,
                                                      after_jump_flag_n1=10,
                                                      after_jump_flag_e2=after_jump_flag_e2,
                                                      after_jump_flag_n2=2)
     # 2 groups after CR should be flagged
@@ -1014,7 +1015,129 @@
     # 1d, with nans
     arr = np.array([-1., -2., np.nan, np.nan])
     assert calc_med_first_diffs(arr) == -1
     # 3d, with nans
     arr = np.zeros(4 * 2 * 2).reshape(4, 2, 2)
     arr[:, 0, 0] = np.array([-1., -2., np.nan, np.nan])
     assert calc_med_first_diffs(arr)[0, 0] == -1
+@pytest.mark.skip("Used for local testing")
+def test_sigma_clip():
+#    hdul = fits.open('TSOjump_sc__refpix.fits')
+    hdul = fits.open('lrs_TSOjump_sigmaclip5_00_refpix.fits')
+    data = hdul['SCI'].data * 4.0
+    gdq = hdul['GROUPDQ'].data
+    indata = data[:53, :, :, :]
+    ingdq = gdq[:53, :, :, :]
+    read_noise = np.ones(shape=(indata.shape[2], indata.shape[3]), dtype=np.float32) * 5.9 * 4.0
+    hdul.close()
+    gdq, row_below_gdq, row_above_gdq, total_primary_crs, stddev = find_crs(indata, ingdq, read_noise, 3,
+             4, 5, 1,
+             False, 1000,
+             10, DQFLAGS,
+             after_jump_flag_e1=0.0,
+             after_jump_flag_n1=0,
+             after_jump_flag_e2=0.0,
+             after_jump_flag_n2=0,
+             copy_arrs=True, minimum_groups=3, minimum_sigclip_groups=50,)
+    fits.writeto("outgdq.fits", gdq, overwrite=True)
+@pytest.mark.skip("Used for local testing")
+def test_first_grp_flag_issue():
+    nints = 8
+    nrows = 2
+    ncols = 2
+    ngroups = 10
+    readnoise = 2
+    data = np.zeros(shape=(nints, ngroups, nrows, ncols), dtype=np.float32)
+    data = np.random.normal(0, readnoise, size=(nints, ngroups, nrows, ncols))
+    read_noise = np.full((nrows, ncols), readnoise, dtype=np.float32)
+    gdq = np.zeros(shape=(nints, ngroups, nrows, ncols), dtype=np.uint32)
+
+    gdq[:, 0, :, :] = DQFLAGS['DO_NOT_USE']
+    gdq[1:, 1, :, :] = DQFLAGS['DO_NOT_USE']
+    gdq[:, -1, :, :] = DQFLAGS['DO_NOT_USE']
+    gdq, row_below_gdq, row_above_gdq, total_total_crs, stddev = \
+        find_crs(data, gdq, read_noise, 3, 4, 5, 1, False, 1000, 10, DQFLAGS,
+                 after_jump_flag_e1=0.0, after_jump_flag_n1=0,
+                 after_jump_flag_e2=0.0, after_jump_flag_n2=0,
+                 copy_arrs=True, minimum_groups=3, minimum_sigclip_groups=50)
+    fits.writeto("outgdq.fits",gdq, overwrite=True)
+@pytest.mark.skip("Used for local testing")
+def test_5grp_TSO():
+    nints=20
+    nrows = 2
+    ncols = 2
+    ngroups = 5
+    readnoise = 25
+    data = np.random.normal(0, 0.1 * readnoise, size=(nints, ngroups, nrows, ncols))
+    read_noise = np.full((nrows, ncols), readnoise, dtype=np.float32)
+    gdq = np.zeros(shape=(nints, ngroups, nrows, ncols), dtype=np.uint32)
+    np.expand_dims(gdq, axis=0)
+    np.expand_dims(data, axis=0)
+    gdq[:, 0, :, :] = DQFLAGS['DO_NOT_USE']
+#    gdq[1:, 1, :, :] = DQFLAGS['DO_NOT_USE']
+    gdq[:, -1, :, :] = DQFLAGS['DO_NOT_USE']
+    data[0, :, 0, 0] = [21500, 37600, 52082, 65068, 58627]
+    data[0, :, 0, 1] = [21500, 37600, 52082, 65068, 58627]
+    gdq, row_below_gdq, row_above_gdq, total_primary_crs, stddev = \
+        find_crs(data, gdq, read_noise, 3, 4, 5, 1, False, 1000, 10, DQFLAGS,
+                 after_jump_flag_e1=0.0, after_jump_flag_n1=0,
+                 after_jump_flag_e2=0.0, after_jump_flag_n2=0,
+                 copy_arrs=True, minimum_groups=3, minimum_sigclip_groups=5000)
+    fits.writeto("new_gdq.fits", gdq, overwrite=True)
+@pytest.mark.skip("Used for local testing")
+def test_5grp_realTSO():
+    hdul = fits.open("obs2508_cutout_jump.fits")
+    gdq = hdul['groupdq'].data
+    data = hdul['sci'].data
+    readnoise = 25
+    read_noise = np.full((3, 3), readnoise, dtype=np.float32)
+
+    gdq, row_below_gdq, row_above_gdq, total_total_crs, stddev = \
+        find_crs(data, gdq, read_noise, 3, 4, 5, 1, False, 1000, 10, DQFLAGS,
+                 after_jump_flag_e1=0.0, after_jump_flag_n1=0,
+                 after_jump_flag_e2=0.0, after_jump_flag_n2=0,
+                 copy_arrs=True, minimum_groups=3, minimum_sigclip_groups=15000)
+    fits.writeto("new_gdq_cutout.fits", gdq, overwrite=True)
+@pytest.mark.skip("Used for local testing")
+def test_5grp_allTSO():
+    hdul = fits.open("obs2508_noshower_sigclip_base_00_dark_current.fits")
+    gdq = hdul['groupdq'].data
+    data = hdul['sci'].data * 5.5
+    readnoise = 5.5 * 6
+    read_noise = np.full((gdq.shape[2], gdq.shape[3]), readnoise, dtype=np.float32)
+
+    gdq, row_below_gdq, row_above_gdq, total_total_crs, stddev = \
+        find_crs(data, gdq, read_noise, 5, 4, 5, 1, False, 1000, 10, DQFLAGS,
+                 after_jump_flag_e1=0.0, after_jump_flag_n1=0,
+                 after_jump_flag_e2=0.0, after_jump_flag_n2=0,
+                 copy_arrs=True, minimum_groups=3, minimum_sigclip_groups=15000)
+    fits.writeto("new_no_sigma_clip_gdq.fits", gdq, overwrite=True)
+
+@pytest.mark.skip("Used for local testing")
+def test_1059():
+    hdul = fits.open("data/nircam_1059_00_dark_current.fits")
+    gdq = hdul['groupdq'].data
+    data = hdul['sci'].data * 5.5
+    readnoise = 5.5 * 6
+    read_noise = np.full((gdq.shape[2], gdq.shape[3]), readnoise, dtype=np.float32)
+
+    gdq, row_below_gdq, row_above_gdq, total_total_crs, stddev = \
+        find_crs(data, gdq, read_noise, 5, 4, 5, 1, False, 1000, 10, DQFLAGS,
+                 after_jump_flag_e1=0.0, after_jump_flag_n1=0,
+                 after_jump_flag_e2=0.0, after_jump_flag_n2=0,
+                 copy_arrs=True, minimum_groups=3, minimum_sigclip_groups=15000)
+    fits.writeto("new_no_sigma_clip_gdq.fits", gdq, overwrite=True)
+
+@pytest.mark.skip("Used for local testing")
+def test_1952():
+    hdul = fits.open("data/obs1952_sc_shower_00_dark_current.fits")
+    gdq = hdul['groupdq'].data
+    data = hdul['sci'].data * 5.5
+    readnoise = 5.5 * 6
+    read_noise = np.full((gdq.shape[2], gdq.shape[3]), readnoise, dtype=np.float32)
+    gain = np.full((gdq.shape[2], gdq.shape[3]), 5.5, dtype=np.float32)
+    gdq, row_below_gdq, row_above_gdq, total_total_crs, stddev = \
+        find_crs(data, gdq, read_noise, 5, 4, 5, 1, True, 1000, 10, DQFLAGS,
+                 after_jump_flag_e1=100.0 * gain, after_jump_flag_n1=20/2.77,
+                 after_jump_flag_e2=3000.0 * gain, after_jump_flag_n2=1000/2.77,
+                 copy_arrs=True, minimum_groups=3, minimum_sigclip_groups=150)
+    fits.writeto("new_obs1952_gdq.fits", gdq, overwrite=True)
```

### Comparing `stcal-1.3.8/tox.ini` & `stcal-1.4.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     xdist: pytest-xdist
     jwst: jwst[test] @ git+https://github.com/spacetelescope/jwst.git
     romancal: romancal[test] @ git+https://github.com/spacetelescope/romancal.git
     oldestdeps: minimum_dependencies
 pass_env =
     CI
 set_env =
-    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scipy-wheels-nightly/simple
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
     jwst: CRDS_SERVER_URL=https://jwst-crds.stsci.edu
     romancal: CRDS_SERVER_URL=https://roman-crds.stsci.edu
     jwst,romancal: CRDS_PATH={package_root}/crds_cache
     jwst,romancal: CRDS_CLIENT_RETRY_COUNT=3
     jwst,romancal: CRDS_CLIENT_RETRY_DELAY_SECONDS=20
 commands_pre =
     oldestdeps: minimum_dependencies stcal --filename requirements-min.txt
```

