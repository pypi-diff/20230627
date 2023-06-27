# Comparing `tmp/adafruit-circuitpython-matrixportal-3.0.9.tar.gz` & `tmp/adafruit-circuitpython-matrixportal-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-matrixportal-3.0.9.tar", last modified: Mon Aug 22 19:00:13 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-matrixportal-3.1.0.tar", last modified: Tue Jun 27 19:11:27 2023, max compression
```

## Comparing `adafruit-circuitpython-matrixportal-3.0.9.tar` & `adafruit-circuitpython-matrixportal-3.1.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.624096 adafruit-circuitpython-matrixportal-3.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.604096 adafruit-circuitpython-matrixportal-3.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.612096 adafruit-circuitpython-matrixportal-3.0.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.612096 adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.612096 adafruit-circuitpython-matrixportal-3.0.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-08-22 19:00:13.624096 adafruit-circuitpython-matrixportal-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.616096 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.616096 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2575 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7726 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10453 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/matrixportal.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2750 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/network.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.620096 adafruit-circuitpython-matrixportal-3.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.620096 adafruit-circuitpython-matrixportal-3.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5554 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.624096 adafruit-circuitpython-matrixportal-3.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/examples/matrixportal_scrolling_bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/examples/matrixportal_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 19:00:13.624096 adafruit-circuitpython-matrixportal-3.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.085154 adafruit-circuitpython-matrixportal-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.077154 adafruit-circuitpython-matrixportal-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.081154 adafruit-circuitpython-matrixportal-3.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.081154 adafruit-circuitpython-matrixportal-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.081154 adafruit-circuitpython-matrixportal-3.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-27 19:11:27.085154 adafruit-circuitpython-matrixportal-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.081154 adafruit-circuitpython-matrixportal-3.1.0/adafruit_circuitpython_matrixportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-27 19:11:27.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-27 19:11:27.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:11:27.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_circuitpython_matrixportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-27 19:11:27.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_circuitpython_matrixportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 19:11:27.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_circuitpython_matrixportal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.085154 adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:18.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2575 2023-06-27 19:11:18.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7813 2023-06-27 19:11:18.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10651 2023-06-27 19:11:18.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/matrixportal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3054 2023-06-27 19:11:18.000000 adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.085154 adafruit-circuitpython-matrixportal-3.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.085154 adafruit-circuitpython-matrixportal-3.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:11:27.085154 adafruit-circuitpython-matrixportal-3.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-27 19:11:18.000000 adafruit-circuitpython-matrixportal-3.1.0/examples/matrixportal_scrolling_bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-27 19:11:18.000000 adafruit-circuitpython-matrixportal-3.1.0/examples/matrixportal_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-27 19:11:18.000000 adafruit-circuitpython-matrixportal-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-27 19:11:08.000000 adafruit-circuitpython-matrixportal-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:11:27.085154 adafruit-circuitpython-matrixportal-3.1.0/setup.cfg
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-matrixportal-3.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/.gitignore` & `adafruit-circuitpython-matrixportal-3.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/.pre-commit-config.yaml` & `adafruit-circuitpython-matrixportal-3.1.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/.pylintrc` & `adafruit-circuitpython-matrixportal-3.1.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-matrixportal-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/LICENSE` & `adafruit-circuitpython-matrixportal-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-matrixportal-3.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/LICENSES/MIT.txt` & `adafruit-circuitpython-matrixportal-3.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-matrixportal-3.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/PKG-INFO` & `adafruit-circuitpython-matrixportal-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-matrixportal
-Version: 3.0.9
+Version: 3.1.0
 Summary: CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal
 Keywords: adafruit,matrixportal,matrix,rgb,led,feather,featherwing,shieldbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/README.rst` & `adafruit-circuitpython-matrixportal-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO` & `adafruit-circuitpython-matrixportal-3.1.0/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-matrixportal
-Version: 3.0.9
+Version: 3.1.0
 Summary: CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal
 Keywords: adafruit,matrixportal,matrix,rgb,led,feather,featherwing,shieldbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt` & `adafruit-circuitpython-matrixportal-3.1.0/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 README.rst.license
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_matrixportal.egg-info/PKG-INFO
 adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt
 adafruit_circuitpython_matrixportal.egg-info/dependency_links.txt
 adafruit_circuitpython_matrixportal.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/graphics.py` & `adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 from adafruit_portalbase.graphics import GraphicsBase
 from adafruit_matrixportal.matrix import Matrix
 
-__version__ = "3.0.9"
+__version__ = "3.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the MatrixPortal Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/matrix.py` & `adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os
 import board
 import displayio
 import rgbmatrix
 import framebufferio
 
 
-__version__ = "3.0.9"
+__version__ = "3.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Matrix:
     """Class representing the Adafruit RGB Matrix. This is used to automatically
     initialize the display.
 
@@ -64,28 +64,30 @@
         bit_depth=2,
         alt_addr_pins=None,
         color_order="RGB",
         serpentine=True,
         tile_rows=1,
         rotation=0,
     ):
-
         panel_height = height // tile_rows
 
         if not isinstance(color_order, str):
             raise ValueError("color_index should be a string")
         color_order = color_order.lower()
         red_index = color_order.find("r")
         green_index = color_order.find("g")
         blue_index = color_order.find("b")
         if -1 in (red_index, green_index, blue_index):
             raise ValueError("color_order should contain R, G, and B")
 
-        if "Matrix Portal M4" in os.uname().machine:
-            # MatrixPortal M4 Board
+        if (
+            "Adafruit Matrix Portal" in os.uname().machine
+            or "Adafruit MatrixPortal" in os.uname().machine
+        ):
+            # MatrixPortal Board
             addr_pins = [board.MTX_ADDRA, board.MTX_ADDRB, board.MTX_ADDRC]
             if panel_height > 16:
                 addr_pins.append(board.MTX_ADDRD)
             if panel_height > 32:
                 addr_pins.append(board.MTX_ADDRE)
             rgb_pins = [
                 board.MTX_R1,
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/matrixportal.py` & `adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/matrixportal.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import gc
 from time import sleep
 import terminalio
 from adafruit_portalbase import PortalBase
 from adafruit_matrixportal.network import Network
 from adafruit_matrixportal.graphics import Graphics
 
-__version__ = "3.0.9"
+__version__ = "3.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class MatrixPortal(PortalBase):
     """Class representing the Adafruit RGB Matrix Portal.
 
     :param url: The URL of your data source. Defaults to ``None``.
@@ -89,15 +89,14 @@
         debug=False,
         width=64,
         height=32,
         serpentine=True,
         tile_rows=1,
         rotation=0,
     ):
-
         graphics = Graphics(
             default_bg=default_bg,
             bit_depth=bit_depth,
             width=width,
             height=height,
             alt_addr_pins=alt_addr_pins,
             color_order=color_order,
@@ -140,14 +139,15 @@
         text_maxlen=0,
         text_transform=None,
         text_scale=1,
         scrolling=False,
         line_spacing=1.25,
         text_anchor_point=(0, 0.5),
         is_data=True,
+        text=None,
     ):
         """
         Add text labels with settings
 
         :param str text_font: The path to your font file for your data text display.
         :param text_position: The position of your extracted text on the display in an (x, y) tuple.
                               Can be a list of tuples for when there's a list of json_paths, for
@@ -162,14 +162,19 @@
         :param int text_scale: The factor to scale the default size of the text by
         :param bool scrolling: If true, text is placed offscreen and the scroll() function is used
                                to scroll text on a pixel-by-pixel basis. Multiple text labels with
                                the scrolling set to True will be cycled through.
         :param (float, float) text_anchor_point: Values between 0 and 1 to indicate where the text
                                                  position is relative to the label
         :param bool is_data: If True, fetch will attempt to update the label
+        :param str text: If this is provided, it will set the initial text of the label.
+
+        :return: Index of the new text label.
+        :rtype: int
+
         """
         if scrolling:
             if text_position is None:
                 # Center text if position not specified
                 text_position = (self.display.width, self.display.height // 2 - 1)
             else:
                 text_position = (self.display.width, text_position[1])
@@ -181,14 +186,15 @@
             text_wrap=text_wrap,
             text_maxlen=text_maxlen,
             text_transform=text_transform,
             text_scale=text_scale,
             line_spacing=line_spacing,
             text_anchor_point=text_anchor_point,
             is_data=is_data,
+            text=text,
         )
 
         self._text[index]["scrolling"] = scrolling
 
         if scrolling and self._scrolling_index is None:  # Not initialized yet
             self._scrolling_index = self._get_next_scrollable_text_index()
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/network.py` & `adafruit-circuitpython-matrixportal-3.1.0/adafruit_matrixportal/network.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,25 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
+import os
 import gc
 import neopixel
 from adafruit_portalbase.network import NetworkBase
-from adafruit_portalbase.wifi_coprocessor import WiFi
 
-__version__ = "3.0.9"
+if os.uname().sysname == "samd51":
+    from adafruit_portalbase.wifi_coprocessor import WiFi
+else:
+    from adafruit_portalbase.wifi_esp32s2 import WiFi
+
+__version__ = "3.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Network(NetworkBase):
     """Class representing the Adafruit RGB Matrix Portal.
 
     :param status_neopixel: The pin for the status NeoPixel. Use ``board.NEOPIXEL`` for the on-board
@@ -53,14 +58,20 @@
         extract_values = True
         debug = False
         if "extract_values" in kwargs:
             extract_values = kwargs.pop("extract_values")
         if "debug" in kwargs:
             debug = kwargs.pop("debug")
 
+        if os.uname().sysname != "samd51":
+            if "external_spi" in kwargs:
+                kwargs.pop("external_spi")
+            if "esp" in kwargs:
+                kwargs.pop("esp")
+
         status_neopixel = kwargs.pop("status_neopixel", None)
         if status_neopixel:
             status_led = neopixel.NeoPixel(status_neopixel, 1, brightness=0.2)
         else:
             status_led = None
         kwargs["status_led"] = status_led
         wifi = WiFi(**kwargs)
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/docs/_static/favicon.ico` & `adafruit-circuitpython-matrixportal-3.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/docs/conf.py` & `adafruit-circuitpython-matrixportal-3.1.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,45 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
-autodoc_mock_imports = ["supervisor", "rtc", "rgbmatrix", "framebufferio", "secrets"]
+autodoc_mock_imports = [
+    "supervisor",
+    "rtc",
+    "rgbmatrix",
+    "framebufferio",
+    "secrets",
+    "wifi",
+    "ssl",
+    "socketpool",
+]
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
@@ -39,15 +50,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit MatrixPortal Library"
-copyright = "2020 Melissa LeBlanc-Williams"
+creation_year = "2020"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Melissa LeBlanc-Williams"
 author = "Melissa LeBlanc-Williams"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/docs/index.rst` & `adafruit-circuitpython-matrixportal-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/examples/matrixportal_scrolling_bitcoin.py` & `adafruit-circuitpython-matrixportal-3.1.0/examples/matrixportal_scrolling_bitcoin.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/examples/matrixportal_simpletest.py` & `adafruit-circuitpython-matrixportal-3.1.0/examples/matrixportal_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.9/pyproject.toml` & `adafruit-circuitpython-matrixportal-3.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-matrixportal"
 description = "CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings"
-version = "3.0.9"
+version = "3.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal"}
 keywords = [
     "adafruit",
```

