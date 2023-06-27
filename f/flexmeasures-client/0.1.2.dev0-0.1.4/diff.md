# Comparing `tmp/flexmeasures-client-0.1.2.dev0.tar.gz` & `tmp/flexmeasures-client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexmeasures-client-0.1.2.dev0.tar", last modified: Fri Jun  2 13:33:06 2023, max compression
+gzip compressed data, was "flexmeasures-client-0.1.4.tar", last modified: Tue Jun 27 14:25:20 2023, max compression
```

## Comparing `flexmeasures-client-0.1.2.dev0.tar` & `flexmeasures-client-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.743238 flexmeasures-client-0.1.2.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.743238 flexmeasures-client-0.1.2.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.747238 flexmeasures-client-0.1.2.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.747238 flexmeasures-client-0.1.2.dev0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.743238 flexmeasures-client-0.1.2.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.747238 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/response_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.989271 flexmeasures-client-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.969271 flexmeasures-client-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.977271 flexmeasures-client-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-27 14:25:20.993271 flexmeasures-client-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.981271 flexmeasures-client-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.981271 flexmeasures-client-0.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-27 14:25:20.993271 flexmeasures-client-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.969271 flexmeasures-client-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.981271 flexmeasures-client-0.1.4/src/flexmeasures_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/response_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.985271 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/cem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.985271 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/control_types/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.985271 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/control_types/FRBC/
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/control_types/FRBC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/control_types/FRBC/frbc_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/control_types/FRBC/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/control_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.969271 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/python_s2_protocol/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.989271 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/python_s2_protocol/FRBC/
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/python_s2_protocol/FRBC/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/python_s2_protocol/FRBC/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.989271 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/python_s2_protocol/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/python_s2_protocol/common/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/python_s2_protocol/common/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.989271 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/script/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/script/demo_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/script/websockets_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/script/websockets_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/src/flexmeasures_client/s2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.985271 flexmeasures-client-0.1.4/src/flexmeasures_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-27 14:25:20.000000 flexmeasures-client-0.1.4/src/flexmeasures_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-27 14:25:20.000000 flexmeasures-client-0.1.4/src/flexmeasures_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:25:20.000000 flexmeasures-client-0.1.4/src/flexmeasures_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:25:20.000000 flexmeasures-client-0.1.4/src/flexmeasures_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-27 14:25:20.000000 flexmeasures-client-0.1.4/src/flexmeasures_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 14:25:20.000000 flexmeasures-client-0.1.4/src/flexmeasures_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:25:20.989271 flexmeasures-client-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/tests/test_frbc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/tests/test_s2_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-27 14:24:46.000000 flexmeasures-client-0.1.4/tox.ini
```

### Comparing `flexmeasures-client-0.1.2.dev0/.coveragerc` & `flexmeasures-client-0.1.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/.github/workflows/ci.yml` & `flexmeasures-client-0.1.4/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 name: tests
 
 on:
   push:
     # Avoid using all the resources/limits available by checking only
     # relevant branches and tags. Other branches can be checked via PRs.
-    branches: [main, hackathon]
+    branches: [main, hotfix/hackathon]
     tags:
+      - 'v[0-9]+\.[0-9]+\.[0-9]+\.dev[0-9]+'  # Match tags that resemble a version
       - 'v[0-9]+\.[0-9]+\.[0-9]+'  # Match tags that resemble a version
-      - 'v[0-9]+\.[0-9]+\.[0-9]+.dev[0-9]+'  # Match tags that resemble a version
   pull_request:  # Run in every PR
   workflow_dispatch:  # Allow manually triggering the workflow
   schedule:
     # Run roughly every 15 days at 00:00 UTC
     # (useful to check if updates on dependencies break the package)
     - cron: '0 0 1,16 * *'
```

### Comparing `flexmeasures-client-0.1.2.dev0/.gitignore` & `flexmeasures-client-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/.pre-commit-config.yaml` & `flexmeasures-client-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/.readthedocs.yml` & `flexmeasures-client-0.1.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/CONTRIBUTING.rst` & `flexmeasures-client-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/LICENSE.txt` & `flexmeasures-client-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/PKG-INFO` & `flexmeasures-client-0.1.4/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: flexmeasures-client
-Version: 0.1.2.dev0
-Summary: Async client to connect to the FlexMeasures API
-Home-page: https://github.com/FlexMeasures/flexmeasures-client
-Author: Flexmeasures
-Author-email: info@seita.nl
-License: APACHE
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/flexmeasures-client.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/flexmeasures-client
     .. image:: https://readthedocs.org/projects/flexmeasures-client/badge/?version=latest
@@ -51,14 +36,16 @@
 ===================
 
 
 The FlexMeasures Client provides a python package to connect to a `FlexMeasures <https://github.com/FlexMeasures/flexmeasures>`_ server to manage flexible assets.
 
 The Flexmeasures Client package provides functionality for authentication, posting sensor data, triggering schedules and retrieving schedules from a FlexMeasures instance through the API.
 
+As the Flexmeasures Client is still in active development and on version 0.1 it should be considered in beta.
+
 
 Getting Started
 ===============
 
 To get started using the FlexMeasures Client package first an account needs to be registered with a FlexMeasures instance or a local FlexMeasures instance needs to be created. Registring a to a FlexMeasures instance can be done through `Seita BV <https://seita.nl/>`_. To create a local instance of FlexMeasures follow the `FlexMeasures documentation <https://flexmeasures.readthedocs.io/en/latest/index.html>`_.
 
 In this example we are connecting to ``localhost:5000``, To connect to a different host add the host in the initialization of the client.
@@ -84,26 +71,48 @@
             start="2023-03-26T10:00+02:00", #iso datetime
             duration="PT6H", # iso timedelta
             values=[1,2,3,4], # list
             unit="kWh",
             entity_address=<sensor_entity_address>, # string
         )
 
-With FlexMeasures a schedule can be requested to optimize at what time the flexible assets can be activated to optimize for price of energy or emissions. The calculation of the schedule can take some time depending on the complexity of the calculations and therefore the requests have been split in a trigger for the schedule and a retrieve schedule call.
+With FlexMeasures a schedule can be requested to optimize at what time the flexible assets can be activated to optimize for price of energy or emissions.
+
+The calculation of the schedule can take some time depending on the complexity of the calculations. A polling function is used to check if a schedule is available after triggering the schedule.
+
+Trigger and retrieve a schedule::
+
+    schedule = await flexmeasures_client.trigger_and_get_schedule(
+            sensor_id=<sensor_id>, # int
+            start="2015-06-02T10:00:00+00:00", # iso datetime
+            duration="PT45M", # iso timedelta
+            soc_unit="MWh",
+            soc_at_start=50, # soc_units (MWh)
+            soc_targets=[
+                {
+                    "value": 100, # soc_units (MWh)
+                    "datetime": "2023-03-03T11:00+02:00", # iso datetime
+                }
+            ],
+            consumption_price_sensor=<consumption_price_sensor_id>, # int
+        )
+
+The trigger and get schedule function can also be separated to trigger the schedule first and later retrieve the schedule using the ``schedule_uuid``.
+
 Trigger a schedule::
 
     schedule_uuid = await flexmeasures_client.trigger_storage_schedule(
             sensor_id=<sensor_id>, # int
             start="2023-03-26T10:00+02:00", # iso datetime
-            duration="PT12H", #iso timedelta
+            duration="PT12H", # iso timedelta
             soc_unit="kWh",
-            soc_at_start=50, #soc_units (kWh)
+            soc_at_start=50, # soc_units (kWh)
             soc_targets=[
                 {
-                    "value": 100, #soc_units (kWh)
+                    "value": 100, # soc_units (kWh)
                     "datetime": "2023-03-03T11:00+02:00", # iso datetime
                 }
             ],
             consumption_price_sensor=<consumption_price_sensor_id>, # int
         )
 
 The ``trigger_storage_schedule`` return a ``schedule_uuid``. This can be used to retrieve the schedule. The client will re-try if until the schedule is available or the ``MAX_POLLING_STEPS`` of ``10`` is reached. Retrieve schedule::
@@ -135,12 +144,46 @@
 
     pre-commit autoupdate
 
 Don't forget to tell your contributors to also install and use pre-commit.
 
 .. _pre-commit: https://pre-commit.com/
 
+===================
+S2 Protocol
+===================
+
+Disclaimer
+==========
+
+The `S2 Protocol <https://github.com/flexiblepower/s2-ws-json>`_ integration is still under active development. Please, beware that the logic and interfaces can change.
+
+
+Run Demo
+=========
+
+Run the following commands in the flexmeasures folder to create a toy-account and an admin user::
+
+    flexmeasures add toy-account
+    flexmeasures add user --username admin --account-id 1 --email admin@mycompany.io --roles admin
+
+Launch server::
+
+    flexmeasures run
+
+To load the data, run the following command in the flexmeasures-client repository::
+
+    python src/flexmeasures_client/s2/script/demo_setup.py
+
+Start the S2 server::
+
+    python src/flexmeasures_client/s2/script/websockets_server.py
+
+In a separate window, start the S2 Client::
+
+    python src/flexmeasures_client/s2/script/websockets_client.py
+
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `flexmeasures-client-0.1.2.dev0/README.rst` & `flexmeasures-client-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: flexmeasures-client
+Version: 0.1.4
+Summary: Async client to connect to the FlexMeasures API
+Home-page: https://github.com/FlexMeasures/flexmeasures-client
+Author: Flexmeasures
+Author-email: info@seita.nl
+License: APACHE
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: testing
+License-File: LICENSE.txt
+
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/flexmeasures-client.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/flexmeasures-client
     .. image:: https://readthedocs.org/projects/flexmeasures-client/badge/?version=latest
@@ -36,14 +51,16 @@
 ===================
 
 
 The FlexMeasures Client provides a python package to connect to a `FlexMeasures <https://github.com/FlexMeasures/flexmeasures>`_ server to manage flexible assets.
 
 The Flexmeasures Client package provides functionality for authentication, posting sensor data, triggering schedules and retrieving schedules from a FlexMeasures instance through the API.
 
+As the Flexmeasures Client is still in active development and on version 0.1 it should be considered in beta.
+
 
 Getting Started
 ===============
 
 To get started using the FlexMeasures Client package first an account needs to be registered with a FlexMeasures instance or a local FlexMeasures instance needs to be created. Registring a to a FlexMeasures instance can be done through `Seita BV <https://seita.nl/>`_. To create a local instance of FlexMeasures follow the `FlexMeasures documentation <https://flexmeasures.readthedocs.io/en/latest/index.html>`_.
 
 In this example we are connecting to ``localhost:5000``, To connect to a different host add the host in the initialization of the client.
@@ -69,26 +86,48 @@
             start="2023-03-26T10:00+02:00", #iso datetime
             duration="PT6H", # iso timedelta
             values=[1,2,3,4], # list
             unit="kWh",
             entity_address=<sensor_entity_address>, # string
         )
 
-With FlexMeasures a schedule can be requested to optimize at what time the flexible assets can be activated to optimize for price of energy or emissions. The calculation of the schedule can take some time depending on the complexity of the calculations and therefore the requests have been split in a trigger for the schedule and a retrieve schedule call.
+With FlexMeasures a schedule can be requested to optimize at what time the flexible assets can be activated to optimize for price of energy or emissions.
+
+The calculation of the schedule can take some time depending on the complexity of the calculations. A polling function is used to check if a schedule is available after triggering the schedule.
+
+Trigger and retrieve a schedule::
+
+    schedule = await flexmeasures_client.trigger_and_get_schedule(
+            sensor_id=<sensor_id>, # int
+            start="2015-06-02T10:00:00+00:00", # iso datetime
+            duration="PT45M", # iso timedelta
+            soc_unit="MWh",
+            soc_at_start=50, # soc_units (MWh)
+            soc_targets=[
+                {
+                    "value": 100, # soc_units (MWh)
+                    "datetime": "2023-03-03T11:00+02:00", # iso datetime
+                }
+            ],
+            consumption_price_sensor=<consumption_price_sensor_id>, # int
+        )
+
+The trigger and get schedule function can also be separated to trigger the schedule first and later retrieve the schedule using the ``schedule_uuid``.
+
 Trigger a schedule::
 
     schedule_uuid = await flexmeasures_client.trigger_storage_schedule(
             sensor_id=<sensor_id>, # int
             start="2023-03-26T10:00+02:00", # iso datetime
-            duration="PT12H", #iso timedelta
+            duration="PT12H", # iso timedelta
             soc_unit="kWh",
-            soc_at_start=50, #soc_units (kWh)
+            soc_at_start=50, # soc_units (kWh)
             soc_targets=[
                 {
-                    "value": 100, #soc_units (kWh)
+                    "value": 100, # soc_units (kWh)
                     "datetime": "2023-03-03T11:00+02:00", # iso datetime
                 }
             ],
             consumption_price_sensor=<consumption_price_sensor_id>, # int
         )
 
 The ``trigger_storage_schedule`` return a ``schedule_uuid``. This can be used to retrieve the schedule. The client will re-try if until the schedule is available or the ``MAX_POLLING_STEPS`` of ``10`` is reached. Retrieve schedule::
@@ -120,12 +159,46 @@
 
     pre-commit autoupdate
 
 Don't forget to tell your contributors to also install and use pre-commit.
 
 .. _pre-commit: https://pre-commit.com/
 
+===================
+S2 Protocol
+===================
+
+Disclaimer
+==========
+
+The `S2 Protocol <https://github.com/flexiblepower/s2-ws-json>`_ integration is still under active development. Please, beware that the logic and interfaces can change.
+
+
+Run Demo
+=========
+
+Run the following commands in the flexmeasures folder to create a toy-account and an admin user::
+
+    flexmeasures add toy-account
+    flexmeasures add user --username admin --account-id 1 --email admin@mycompany.io --roles admin
+
+Launch server::
+
+    flexmeasures run
+
+To load the data, run the following command in the flexmeasures-client repository::
+
+    python src/flexmeasures_client/s2/script/demo_setup.py
+
+Start the S2 server::
+
+    python src/flexmeasures_client/s2/script/websockets_server.py
+
+In a separate window, start the S2 Client::
+
+    python src/flexmeasures_client/s2/script/websockets_client.py
+
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `flexmeasures-client-0.1.2.dev0/docs/Makefile` & `flexmeasures-client-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/docs/conf.py` & `flexmeasures-client-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/docs/index.rst` & `flexmeasures-client-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/setup.cfg` & `flexmeasures-client-0.1.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 package_dir = 
 	=src
 python_requires > = 3.9
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	aiohttp
 	pandas
+	pydantic
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `flexmeasures-client-0.1.2.dev0/setup.py` & `flexmeasures-client-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/response_handling.py` & `flexmeasures-client-0.1.4/src/flexmeasures_client/response_handling.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,44 +8,63 @@
 
 from flexmeasures_client.constants import CONTENT_TYPE
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
     from flexmeasures_client.client import FlexMeasuresClient
 
 
-async def check_response(self: FlexMeasuresClient, response, polling_step: int):
+async def check_response(
+    self: FlexMeasuresClient, response, polling_step: int, reauth_once: bool
+) -> tuple[int, bool]:
     """
     <300: passes
     401: reauthenticate
     todo: 503 + Retry-After header: poll again
     otherwise: call error_handler
     """
     status = response.status
     payload = await response.json()
     headers = response.headers
     if status < 300:
         pass
-    elif status == 401:
+    elif status == 401 and reauth_once:
+        message = f"""Authentication failed with"
+        status: {status}
+        headers: {headers}
+        payload: {payload}.
+        Re-authenticating!
+        """
+        logging.debug(message)
         await self.get_access_token()
-        self.reauth_once = False
+        reauth_once = False
     elif status == 503 and "Retry-After" in headers:
         polling_step += 1
         await asyncio.sleep(self.polling_interval)
     elif status == 400 and (
         "Scheduling job waiting" in payload.get("message", "")
         or "Scheduling job in progress" in payload.get("message", "")
     ):
         # can be removed in a later version GH issue #645 of the FlexMeasures repo
         message = f"Server indicated to try again later. Retrying in {self.polling_interval} seconds..."  # noqa: E501
-        logging.info(message)
+        logging.debug(message)
         polling_step += 1
         await asyncio.sleep(self.polling_interval)
+    elif payload.get("errors"):
+        # try to raise any error messages from the response
+        raise ValueError(" ,".join(payload.get("errors")))
     else:
+        message = f"""
+        status: {status}
+        headers: {headers}
+        payload: {payload}.
+        """
+        logging.error(message)
+        # otherwise, raise if the status does not indicate okay
         response.raise_for_status()
-    return polling_step
+    return polling_step, reauth_once
 
 
 def check_content_type(response):
     """Check if response is in format application/json"""
     content_type = response.headers.get("Content-Type", "")
     if CONTENT_TYPE not in content_type:
         text = response.text()
```

### Comparing `flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/PKG-INFO` & `flexmeasures-client-0.1.4/src/flexmeasures_client.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmeasures-client
-Version: 0.1.2.dev0
+Version: 0.1.4
 Summary: Async client to connect to the FlexMeasures API
 Home-page: https://github.com/FlexMeasures/flexmeasures-client
 Author: Flexmeasures
 Author-email: info@seita.nl
 License: APACHE
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -51,14 +51,16 @@
 ===================
 
 
 The FlexMeasures Client provides a python package to connect to a `FlexMeasures <https://github.com/FlexMeasures/flexmeasures>`_ server to manage flexible assets.
 
 The Flexmeasures Client package provides functionality for authentication, posting sensor data, triggering schedules and retrieving schedules from a FlexMeasures instance through the API.
 
+As the Flexmeasures Client is still in active development and on version 0.1 it should be considered in beta.
+
 
 Getting Started
 ===============
 
 To get started using the FlexMeasures Client package first an account needs to be registered with a FlexMeasures instance or a local FlexMeasures instance needs to be created. Registring a to a FlexMeasures instance can be done through `Seita BV <https://seita.nl/>`_. To create a local instance of FlexMeasures follow the `FlexMeasures documentation <https://flexmeasures.readthedocs.io/en/latest/index.html>`_.
 
 In this example we are connecting to ``localhost:5000``, To connect to a different host add the host in the initialization of the client.
@@ -84,26 +86,48 @@
             start="2023-03-26T10:00+02:00", #iso datetime
             duration="PT6H", # iso timedelta
             values=[1,2,3,4], # list
             unit="kWh",
             entity_address=<sensor_entity_address>, # string
         )
 
-With FlexMeasures a schedule can be requested to optimize at what time the flexible assets can be activated to optimize for price of energy or emissions. The calculation of the schedule can take some time depending on the complexity of the calculations and therefore the requests have been split in a trigger for the schedule and a retrieve schedule call.
+With FlexMeasures a schedule can be requested to optimize at what time the flexible assets can be activated to optimize for price of energy or emissions.
+
+The calculation of the schedule can take some time depending on the complexity of the calculations. A polling function is used to check if a schedule is available after triggering the schedule.
+
+Trigger and retrieve a schedule::
+
+    schedule = await flexmeasures_client.trigger_and_get_schedule(
+            sensor_id=<sensor_id>, # int
+            start="2015-06-02T10:00:00+00:00", # iso datetime
+            duration="PT45M", # iso timedelta
+            soc_unit="MWh",
+            soc_at_start=50, # soc_units (MWh)
+            soc_targets=[
+                {
+                    "value": 100, # soc_units (MWh)
+                    "datetime": "2023-03-03T11:00+02:00", # iso datetime
+                }
+            ],
+            consumption_price_sensor=<consumption_price_sensor_id>, # int
+        )
+
+The trigger and get schedule function can also be separated to trigger the schedule first and later retrieve the schedule using the ``schedule_uuid``.
+
 Trigger a schedule::
 
     schedule_uuid = await flexmeasures_client.trigger_storage_schedule(
             sensor_id=<sensor_id>, # int
             start="2023-03-26T10:00+02:00", # iso datetime
-            duration="PT12H", #iso timedelta
+            duration="PT12H", # iso timedelta
             soc_unit="kWh",
-            soc_at_start=50, #soc_units (kWh)
+            soc_at_start=50, # soc_units (kWh)
             soc_targets=[
                 {
-                    "value": 100, #soc_units (kWh)
+                    "value": 100, # soc_units (kWh)
                     "datetime": "2023-03-03T11:00+02:00", # iso datetime
                 }
             ],
             consumption_price_sensor=<consumption_price_sensor_id>, # int
         )
 
 The ``trigger_storage_schedule`` return a ``schedule_uuid``. This can be used to retrieve the schedule. The client will re-try if until the schedule is available or the ``MAX_POLLING_STEPS`` of ``10`` is reached. Retrieve schedule::
@@ -135,12 +159,46 @@
 
     pre-commit autoupdate
 
 Don't forget to tell your contributors to also install and use pre-commit.
 
 .. _pre-commit: https://pre-commit.com/
 
+===================
+S2 Protocol
+===================
+
+Disclaimer
+==========
+
+The `S2 Protocol <https://github.com/flexiblepower/s2-ws-json>`_ integration is still under active development. Please, beware that the logic and interfaces can change.
+
+
+Run Demo
+=========
+
+Run the following commands in the flexmeasures folder to create a toy-account and an admin user::
+
+    flexmeasures add toy-account
+    flexmeasures add user --username admin --account-id 1 --email admin@mycompany.io --roles admin
+
+Launch server::
+
+    flexmeasures run
+
+To load the data, run the following command in the flexmeasures-client repository::
+
+    python src/flexmeasures_client/s2/script/demo_setup.py
+
+Start the S2 server::
+
+    python src/flexmeasures_client/s2/script/websockets_server.py
+
+In a separate window, start the S2 Client::
+
+    python src/flexmeasures_client/s2/script/websockets_client.py
+
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `flexmeasures-client-0.1.2.dev0/tests/test_client.py` & `flexmeasures-client-0.1.4/tests/test_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         "email": email,
         "access_token": None,
         "host": asserted_host,
         "scheme": asserted_scheme,
         "ssl": asserted_ssl,
         "api_version": asserted_version,
         "path": "/api/v3_0/",
-        "reauth_once": True,
         "max_polling_steps": 10,
         "polling_timeout": 200.0,
         "request_timeout": 20.0,
         "polling_interval": 10.0,
         "session": None,
     }
     assert flexmeasures_client.__dict__ == assert_dict
@@ -220,14 +219,16 @@
 
         schedule_id = await flexmeasures_client.trigger_storage_schedule(
             sensor_id=3,
             start="2023-03-26T10:00+02:00",
             duration="PT12H",
             soc_unit="kWh",
             soc_at_start=50,
+            soc_max=400,
+            soc_min=20,
             soc_targets=[
                 {
                     "value": 100,
                     "datetime": "2023-03-03T11:00+02:00",
                 }
             ],
             consumption_price_sensor=3,
@@ -240,14 +241,16 @@
             headers={"Content-Type": "application/json", "Authorization": "test-token"},
             json={
                 "start": "2023-03-26T10:00:00+02:00",
                 "duration": "P0DT12H0M0S",
                 "flex-model": {
                     "soc-unit": "kWh",
                     "soc-at-start": 50,
+                    "soc-max": 400,
+                    "soc-min": 20,
                     "soc-targets": [
                         {"value": 100, "datetime": "2023-03-03T11:00+02:00"}
                     ],
                 },
                 "flex-context": {"consumption-price-sensor": 3},
             },
             url="http://localhost:5000/api/v3_0/sensors/3/schedules/trigger",
@@ -255,40 +258,42 @@
             ssl=False,
         )
 
     await flexmeasures_client.close()
 
 
 @pytest.mark.asyncio
-async def test_get_schedule() -> None:
+async def test_get_schedule_polling() -> None:
     # todo: relies on https://github.com/pnuckowski/aioresponses/pull/237 to use repeat instead of 3 times the same aioresponse. # noqa: E501
+
+    url = "http://localhost:5000/api/v3_0/sensors/1/schedules/some-uuid?duration=P0DT0H45M0S"  # noqa 501
     with aioresponses() as m:
         # m.get(
         #     "http://localhost:5000/api/v3_0/sensors/1/schedules/some-uuid",
         #     status=400,
         #     payload={"message": "Scheduling job waiting"},
         #     repeat=3
         # )
         m.get(
-            "http://localhost:5000/api/v3_0/sensors/1/schedules/some-uuid",
+            url=url,
             status=400,
             payload={"message": "Scheduling job waiting"},
         )
         m.get(
-            "http://localhost:5000/api/v3_0/sensors/1/schedules/some-uuid",
+            url=url,
             status=400,
             payload={"message": "Scheduling job waiting"},
         )
         m.get(
-            "http://localhost:5000/api/v3_0/sensors/1/schedules/some-uuid",
+            url=url,
             status=400,
             payload={"message": "Scheduling job waiting"},
         )
         m.get(
-            "http://localhost:5000/api/v3_0/sensors/1/schedules/some-uuid",
+            url=url,
             status=200,
             payload={
                 "values": [2.15, 3, 2],
                 "start": "2015-06-02T10:00:00+00:00",
                 "duration": "PT45M",
                 "unit": "MW",
             },
@@ -356,17 +361,17 @@
                     "latitude": 52.374,
                     "longitude": 4.88969,
                     "name": "toy-battery",
                 }
             ],
         )
 
-        response = await flexmeasures_client.get_assets()
-        assert len(response) == 1
-        assert response[0]["account_id"] == 2
+        assets = await flexmeasures_client.get_assets()
+        assert len(assets) == 1
+        assert assets[0]["account_id"] == 2
 
     await flexmeasures_client.close()
 
 
 @pytest.mark.asyncio
 async def test_get_sensors() -> None:
     with aioresponses() as m:
@@ -385,17 +390,17 @@
                     "name": "discharging",
                     "timezone": "Europe/Amsterdam",
                     "unit": "MW",
                 }
             ],
         )
 
-        response = await flexmeasures_client.get_sensors()
-        assert len(response) == 1
-        assert response[0]["entity_address"] == "ea1.2023-06.localhost:fm1.2"
+        sensors = await flexmeasures_client.get_sensors()
+        assert len(sensors) == 1
+        assert sensors[0]["entity_address"] == "ea1.2023-06.localhost:fm1.2"
 
     await flexmeasures_client.close()
 
 
 @pytest.mark.asyncio
 async def test_get_sensors2() -> None:
     with aioresponses() as m:
@@ -416,44 +421,46 @@
 
     await flexmeasures_client.close()
 
 
 @pytest.mark.asyncio
 async def test_trigger_and_get_schedule() -> None:
     # todo: relies on https://github.com/pnuckowski/aioresponses/pull/237 to use repeat instead of 3 times the same aioresponse. # noqa: E501
+
+    url = "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid?duration=P0DT0H45M0S"  # noqa 501
     with aioresponses() as m:
         # m.get(
         #     "http://localhost:5000/api/v3_0/sensors/1/schedules/some-uuid",
         #     status=400,
         #     payload={"message": "Scheduling job waiting"},
         #     repeat=3
         # )
         m.post(
             "http://localhost:5000/api/v3_0/sensors/1/schedules/trigger",
             status=200,
             payload={"schedule": "schedule-uuid"},
         )
 
         m.get(
-            "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid",
+            url=url,
             status=400,
             payload={"message": "Scheduling job waiting"},
         )
         m.get(
-            "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid",
+            url=url,
             status=400,
             payload={"message": "Scheduling job waiting"},
         )
         m.get(
-            "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid",
+            url=url,
             status=400,
             payload={"message": "Scheduling job waiting"},
         )
         m.get(
-            "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid",
+            url=url,
             status=200,
             payload={
                 "values": [2.15, 3, 2],
                 "start": "2015-06-02T10:00:00+00:00",
                 "duration": "PT45M",
                 "unit": "MW",
             },
@@ -478,7 +485,121 @@
                     "datetime": "2023-03-03T11:00+02:00",
                 }
             ],
             consumption_price_sensor=3,
         )
     assert schedule["values"] == [2.15, 3, 2]
     await flexmeasures_client.close()
+
+
+@pytest.mark.asyncio
+async def test_get_sensor_data() -> None:
+    with aioresponses() as m:
+        flexmeasures_client = FlexMeasuresClient(
+            email="test@test.test", password="test"
+        )
+        flexmeasures_client.access_token = "test-token"
+        m.get(
+            "http://localhost:5000/api/v3_0/sensors/data?duration=P0DT0H45M0S&resolution=PT15M&sensor=ea1.2023-06.localhost%253Afm1.2&start=2023-06-01T10%253A00%253A00%252B02%253A00&unit=MW",  # noqa: E501
+            status=200,
+            payload={
+                "duration": "PT45M",
+                "message": "Request has been processed.",
+                "resolution": "PT15M",
+                "start": "2023-06-01T10:00:00+02:00",
+                "status": "PROCESSED",
+                "unit": "MW",
+                "values": [8.5, 8.5, 8.5],
+            },
+        )
+
+        sensor_id = 2
+        start = "2023-06-01T10:00:00+02:00"
+        duration = "PT45M"
+        unit = "MW"
+        entity_address = "ea1.2023-06.localhost:fm1"
+        resolution = "PT15M"
+
+        sensor_data = await flexmeasures_client.get_sensor_data(
+            sensor_id=sensor_id,
+            start=start,
+            duration=duration,
+            unit=unit,
+            entity_address=entity_address,
+            resolution=resolution,
+        )
+        assert sensor_data["values"] == [8.5, 8.5, 8.5]
+
+    await flexmeasures_client.close()
+
+
+@pytest.mark.asyncio
+async def test_reauth_with_access_token() -> None:
+    with aioresponses() as m:
+        m.get(
+            "http://localhost:5000/api/v3_0/sensors",
+            status=401,
+            payload={"status": "UNAUTHORIZED"},
+        )
+        m.post(
+            "http://localhost:5000/api/requestAuthToken",
+            status=200,
+            payload={"auth_token": "test-token"},
+        )
+        m.get(
+            "http://localhost:5000/api/v3_0/sensors",
+            status=200,
+            payload=[],
+        )
+        flexmeasures_client = FlexMeasuresClient(
+            email="test@test.test", password="password", access_token="wrong-token"
+        )
+
+        await flexmeasures_client.get_sensors()
+        m.assert_called_with(
+            "http://localhost:5000/api/v3_0/sensors",
+            method="GET",
+            headers={"Content-Type": "application/json", "Authorization": "test-token"},
+            params=None,
+            ssl=False,
+            json=None,
+            allow_redirects=True,
+        )
+
+    await flexmeasures_client.close()
+
+
+@pytest.mark.parametrize(
+    "email, password, payload, error",  # noqa: E501
+    [
+        (
+            "test@test.test",
+            "wrong_password",
+            {"errors": ["User password does not match."], "status": 401},
+            "User password does not match.",
+        ),
+        (
+            "wrong_email@test.test",
+            "password",
+            {
+                "errors": ["User with email 'wrong_email@test.test' does not exist"],
+                "status": 404,
+            },
+            "User with email 'wrong_email@test.test' does not exist",
+        ),
+    ],
+)
+@pytest.mark.asyncio
+async def test_reauth_wrong_cred(email, password, payload, error) -> None:
+    with aioresponses() as m:
+        m.post(
+            "http://localhost:5000/api/requestAuthToken",
+            status=401,
+            payload=payload,
+        )
+
+        flexmeasures_client = FlexMeasuresClient(email=email, password=password)
+
+        with pytest.raises(ValueError, match=error):
+            await flexmeasures_client.get_sensors()
+
+    await flexmeasures_client.close()
```

### Comparing `flexmeasures-client-0.1.2.dev0/tox.ini` & `flexmeasures-client-0.1.4/tox.ini`

 * *Files identical despite different names*

