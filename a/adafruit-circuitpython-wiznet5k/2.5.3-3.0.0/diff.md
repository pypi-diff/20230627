# Comparing `tmp/adafruit-circuitpython-wiznet5k-2.5.3.tar.gz` & `tmp/adafruit-circuitpython-wiznet5k-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wiznet5k-2.5.3.tar", last modified: Tue May 30 13:27:10 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-wiznet5k-3.0.0.tar", last modified: Tue Jun 27 17:30:01 2023, max compression
```

## Comparing `adafruit-circuitpython-wiznet5k-2.5.3.tar` & `adafruit-circuitpython-wiznet5k-3.0.0.tar`

### file list

```diff
@@ -1,67 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.681176 adafruit-circuitpython-wiznet5k-2.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.673175 adafruit-circuitpython-wiznet5k-2.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.673175 adafruit-circuitpython-wiznet5k-2.5.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.673175 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.673175 adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-30 13:27:10.681176 adafruit-circuitpython-wiznet5k-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50486 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    27777 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27027 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:27:10.681176 adafruit-circuitpython-wiznet5k-2.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.681176 adafruit-circuitpython-wiznet5k-2.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/dhcp_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/extract_unique_dns_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    31513 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/test_dhcp_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/test_dns_server_nonbreaking_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/test_parse_dns_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.967476 adafruit-circuitpython-wiznet5k-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.967476 adafruit-circuitpython-wiznet5k-3.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.967476 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51329 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27103 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wiznet5k-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/.gitignore` & `adafruit-circuitpython-wiznet5k-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/.pre-commit-config.yaml` & `adafruit-circuitpython-wiznet5k-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/.pylintrc` & `adafruit-circuitpython-wiznet5k-3.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wiznet5k-3.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/LICENSE` & `adafruit-circuitpython-wiznet5k-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/MIT.txt` & `adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/PKG-INFO` & `adafruit-circuitpython-wiznet5k-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 2.5.3
+Version: 3.0.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/README.rst` & `adafruit-circuitpython-wiznet5k-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 2.5.3
+Version: 3.0.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -42,13 +42,8 @@
 docs/_static/favicon.ico.license
 examples/wiznet5k_aio_post.py
 examples/wiznet5k_cheerlights.py
 examples/wiznet5k_cpython_client_for_simpleserver.py
 examples/wiznet5k_simpleserver.py
 examples/wiznet5k_simpletest.py
 examples/wiznet5k_simpletest_manual_network.py
-examples/wiznet5k_wsgiserver.py
-tests/dhcp_dummy_data.py
-tests/extract_unique_dns_responses.py
-tests/test_dhcp_helper_functions.py
-tests/test_dns_server_nonbreaking_changes.py
-tests/test_parse_dns_function.py
+examples/wiznet5k_wsgiserver.py
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # SPDX-FileCopyrightText: 2010 WIZnet
 # SPDX-FileCopyrightText: 2010 Arduino LLC
 # SPDX-FileCopyrightText: 2008 Bjoern Hartmann
 # SPDX-FileCopyrightText: 2018 Paul Stoffregen
 # SPDX-FileCopyrightText: 2020 Brent Rubell for Adafruit Industries
 # SPDX-FileCopyrightText: 2021 Patrick Van Oosterwijck
 # SPDX-FileCopyrightText: 2021 Adam Cummick
+# SPDX-FileCopyrightText: 2023 Martin Stephens
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_wiznet5k`
 ================================================================================
 
 Pure-Python interface for WIZNET 5k ethernet modules.
 
 * Author(s): WIZnet, Arduino LLC, Bjoern Hartmann, Paul Stoffregen, Brent Rubell,
-  Patrick Van Oosterwijck
+  Patrick Van Oosterwijck, Martin Stephens
 
 Implementation Notes
 --------------------
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
@@ -27,63 +28,95 @@
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 try:
-    from typing import TYPE_CHECKING, Optional, Union, List, Tuple, Sequence
+    from typing import TYPE_CHECKING, Optional, Union, Tuple
 
     if TYPE_CHECKING:
         from circuitpython_typing import WriteableBuffer
         import busio
         import digitalio
+
+        IpAddress4Raw = Union[bytes, Tuple[int, int, int, int]]
+        MacAddressRaw = Union[bytes, Tuple[int, int, int, int, int, int]]
 except ImportError:
     pass
 
-__version__ = "2.5.3"
+__version__ = "3.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
 
 from adafruit_bus_device.spi_device import SPIDevice
 import adafruit_wiznet5k.adafruit_wiznet5k_dhcp as dhcp
 import adafruit_wiznet5k.adafruit_wiznet5k_dns as dns
 from adafruit_wiznet5k.adafruit_wiznet5k_debug import debug_msg
 
-# Wiznet5k Registers
-_REG_MR = const(0x0000)  # Mode
-_REG_GAR = const(0x0001)  # Gateway IP Address
-_REG_SUBR = const(0x0005)  # Subnet Mask Address
-_REG_VERSIONR_W5500 = const(0x0039)  # W5500 Silicon Version
-_REG_VERSIONR_W5100S = const(0x0080)  # W5100S Silicon Version
-_REG_SHAR = const(0x0009)  # Source Hardware Address
-_REG_SIPR = const(0x000F)  # Source IP Address
-_REG_PHYCFGR = const(0x002E)  # W5500 PHY Configuration
-_REG_PHYCFGR_W5100S = const(0x003C)  # W5100S PHY Configuration
-_REG_RCR_5100s = const(0x0019)  # Retry Count
-_REG_RTR_5100s = const(0x0017)  # Retry Time
-_REG_RCR_5500 = const(0x001B)  # Retry Count
-_REG_RTR_5500 = const(0x0019)  # Retry Time
-
-# Wiznet5k Socket Registers
-_REG_SNMR = const(0x0000)  # Socket n Mode
-_REG_SNCR = const(0x0001)  # Socket n Command
-_REG_SNIR = const(0x0002)  # Socket n Interrupt
-_REG_SNSR = const(0x0003)  # Socket n Status
-_REG_SNPORT = const(0x0004)  # Socket n Source Port
-_REG_SNDIPR = const(0x000C)  # Destination IP Address
-_REG_SNDPORT = const(0x0010)  # Destination Port
-_REG_SNRX_RSR = const(0x0026)  # RX Free Size
-_REG_SNRX_RD = const(0x0028)  # Read Size Pointer
-_REG_SNTX_FSR = const(0x0020)  # Socket n TX Free Size
-_REG_SNTX_WR = const(0x0024)  # TX Write Pointer
+# *** Wiznet Common Registers ***
+_REG_MR = {"w5100s": const(0x0000), "w5500": const(0x0000)}
+# Gateway IPv4 Address.
+_REG_GAR = {"w5100s": const(0x0001), "w5500": const(0x0001), "w6100": const(0x4130)}
+# Subnet Mask Address
+_REG_SUBR = {"w5100s": const(0x0005), "w5500": const(0x0005), "w6100": const(0x4134)}
+# Chip version.
+_REG_VERSIONR = {
+    "w5100s": const(0x0080),
+    "w5500": const(0x0039),
+    "w6100": const(0x0000),
+}
+# Source Hardware Address
+_REG_SHAR = {"w5100s": const(0x0009), "w5500": const(0x0009), "w6100": const(0x4120)}
+# Source IP Address
+_REG_SIPR = {"w5100s": const(0x000F), "w5500": const(0x000F), "w6100": const(0x4138)}
+# Register with link status flag (PHYCFGR for 5xxxx, PHYSR for 6100).
+_REG_LINK_FLAG = {
+    "w5100s": const(0x003C),
+    "w5500": const(0x002E),
+    "w6100": const(0x3000),
+}
+_REG_RCR = {"w5100s": const(0x0019), "w5500": const(0x001B), "w6100": const(0x4204)}
+_REG_RTR = {"w5100s": const(0x0017), "w5500": const(0x0019), "w6100": const(0x4200)}
+
+# *** Wiznet Socket Registers ***
+# Socket n Mode.
+_REG_SNMR = const(0x0000)
+# Socket n Command.
+_REG_SNCR = {"w5100s": const(0x0001), "w5500": const(0x0001), "w6100": const(0x0010)}
+# Socket n Interrupt.
+_REG_SNIR = {"w5100s": const(0x0002), "w5500": const(0x0002), "w6100": const(0x0020)}
+# Socket n Status.
+_REG_SNSR = {"w5100s": const(0x0003), "w5500": const(0x0003), "w6100": const(0x0030)}
+# Socket n Source Port.
+_REG_SNPORT = {"w5100s": const(0x0004), "w5500": const(0x0004), "w6100": const(0x0114)}
+# Destination IPv4 Address.
+_REG_SNDIPR = {"w5100s": const(0x000C), "w5500": const(0x000C), "w6100": const(0x0120)}
+# Destination Port.
+_REG_SNDPORT = {"w5100s": const(0x0010), "w5500": const(0x0010), "w6100": const(0x0140)}
+# RX Free Size.
+_REG_SNRX_RSR = {
+    "w5100s": const(0x0026),
+    "w5500": const(0x0026),
+    "w6100": const(0x0224),
+}
+# Read Size Pointer.
+_REG_SNRX_RD = {"w5100s": const(0x0028), "w5500": const(0x0028), "w6100": const(0x0228)}
+# Socket n TX Free Size.
+_REG_SNTX_FSR = {
+    "w5100s": const(0x0020),
+    "w5500": const(0x0020),
+    "w6100": const(0x0204),
+}
+# TX Write Pointer.
+_REG_SNTX_WR = {"w5100s": const(0x0024), "w5500": const(0x0024), "w6100": const(0x020C)}
 
 # SNSR Commands
 SNSR_SOCK_CLOSED = const(0x00)
 _SNSR_SOCK_INIT = const(0x13)
 SNSR_SOCK_LISTEN = const(0x14)
 _SNSR_SOCK_SYNSENT = const(0x15)
 SNSR_SOCK_SYNRECV = const(0x16)
@@ -119,32 +152,36 @@
 _CH_SIZE = const(0x100)
 _SOCK_SIZE = const(0x800)  # MAX W5k socket size
 _SOCK_MASK = const(0x7FF)
 # Register commands
 _MR_RST = const(0x80)  # Mode Register RST
 # Socket mode register
 _SNMR_CLOSE = const(0x00)
-_SNMR_TCP = const(0x21)
+SNMR_TCP = const(0x21)
 SNMR_UDP = const(0x02)
 _SNMR_IPRAW = const(0x03)
 _SNMR_MACRAW = const(0x04)
 _SNMR_PPPOE = const(0x05)
 
 _MAX_PACKET = const(4000)
 _LOCAL_PORT = const(0x400)
 # Default hardware MAC address
 _DEFAULT_MAC = (0xDE, 0xAD, 0xBE, 0xEF, 0xFE, 0xED)
 
 # Maximum number of sockets to support, differs between chip versions.
-_W5200_W5500_MAX_SOCK_NUM = const(0x08)
-_W5100_MAX_SOCK_NUM = const(0x04)
-_SOCKET_INVALID = const(255)
+_MAX_SOCK_NUM = {"w5100s": const(0x04), "w5500": const(0x08), "w6100": const(0x08)}
+_SOCKET_INVALID = const(0xFF)
+
 
-# Source ports in use
-_SRC_PORTS = [0] * _W5200_W5500_MAX_SOCK_NUM
+def _unprettyfy(data: str, seperator: str, correct_length: int) -> bytes:
+    """Helper for converting . or : delimited strings to bytes objects."""
+    data = bytes(int(x) for x in data.split(seperator))
+    if len(data) == correct_length:
+        return data
+    raise ValueError("Invalid IP or MAC address.")
 
 
 class WIZNET5K:  # pylint: disable=too-many-public-methods, too-many-instance-attributes
     """Interface for WIZNET5K module."""
 
     _TCP_MODE = const(0x21)
     _UDP_MODE = const(0x02)
@@ -155,1186 +192,1153 @@
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         spi_bus: busio.SPI,
         cs: digitalio.DigitalInOut,  # pylint: disable=invalid-name
         reset: Optional[digitalio.DigitalInOut] = None,
         is_dhcp: bool = True,
-        mac: Union[List[int], Tuple[int]] = _DEFAULT_MAC,
+        mac: Union[MacAddressRaw, str] = _DEFAULT_MAC,
         hostname: Optional[str] = None,
         debug: bool = False,
     ) -> None:
         """
         :param busio.SPI spi_bus: The SPI bus the Wiznet module is connected to.
         :param digitalio.DigitalInOut cs: Chip select pin.
         :param digitalio.DigitalInOut reset: Optional reset pin, defaults to None.
         :param bool is_dhcp: Whether to start DHCP automatically or not, defaults to True.
-        :param Union[List[int], Tuple[int]] mac: The Wiznet's MAC Address, defaults to
+        :param Union[MacAddressRaw, str] mac: The Wiznet's MAC Address, defaults to
             (0xDE, 0xAD, 0xBE, 0xEF, 0xFE, 0xED).
         :param str hostname: The desired hostname, with optional {} to fill in the MAC
             address, defaults to None.
         :param bool debug: Enable debugging output, defaults to False.
         """
         self._debug = debug
         self._chip_type = None
         self._device = SPIDevice(spi_bus, cs, baudrate=8000000, polarity=0, phase=0)
         # init c.s.
         self._cs = cs
 
-        # reset wiznet module prior to initialization
+        # Reset wiznet module prior to initialization.
         if reset:
             reset.value = False
             time.sleep(0.1)
             reset.value = True
             time.sleep(0.1)
 
+        # Setup chip_select pin.
+        time.sleep(1)
+        self._cs.switch_to_output()
+        self._cs.value = 1
+
         # Buffer for reading params from module
         self._pbuff = bytearray(8)
         self._rxbuf = bytearray(_MAX_PACKET)
 
         # attempt to initialize the module
         self._ch_base_msb = 0
-        if self._w5xxx_init() != 1:
-            raise RuntimeError("Failed to initialize WIZnet module.")
-        if self._chip_type == "w5100s":
-            WIZNET5K._sockets_reserved = [False] * (_W5100_MAX_SOCK_NUM - 1)
-        elif self._chip_type == "w5500":
-            WIZNET5K._sockets_reserved = [False] * (_W5200_W5500_MAX_SOCK_NUM - 1)
-        else:
-            raise RuntimeError("Unrecognized chip type.")
+        self._src_ports_in_use = []
+        self._wiznet_chip_init()
 
         # Set MAC address
         self.mac_address = mac
         self.src_port = 0
-        self._dns = (0, 0, 0, 0)
+        self._dns = b"\x00\x00\x00\x00"
         # udp related
-        self.udp_datasize = [0] * self.max_sockets
         self.udp_from_ip = [b"\x00\x00\x00\x00"] * self.max_sockets
         self.udp_from_port = [0] * self.max_sockets
 
-        # First, wait link status is on
-        # to avoid the code during DHCP, socket listen, connect ...
-        # assert self.link_status, "Ethernet cable disconnected!"
-        start_time = time.monotonic()
-        while True:
-            if self.link_status or ((time.monotonic() - start_time) > 5):
+        # Wait to give the Ethernet link to initialise.
+        stop_time = time.monotonic() + 5
+        while time.monotonic() < stop_time:
+            if self.link_status:
                 break
-            time.sleep(1)
-            debug_msg("My Link is: {}".format(self.link_status), self._debug)
+            debug_msg("Ethernet link is down…", self._debug)
+            time.sleep(0.5)
         self._dhcp_client = None
 
         # Set DHCP
         if is_dhcp:
-            ret = self.set_dhcp(hostname)
-            if ret != 0:
-                self._dhcp_client = None
-            if ret != 0:
-                raise RuntimeError("Failed to configure DHCP Server!")
+            self.set_dhcp(hostname)
 
-    def set_dhcp(self, hostname: Optional[str] = None) -> int:
+    def set_dhcp(self, hostname: Optional[str] = None) -> None:
         """
         Initialize the DHCP client and attempt to retrieve and set network
         configuration from the DHCP server.
 
         :param Optional[str] hostname: The desired hostname for the DHCP server with
             optional {} to fill in the MAC address, defaults to None.
 
-        :return int: 0 if DHCP configured, -1 otherwise.
+        :raises RuntimeError: If DHCP lease cannot be established.
         """
         debug_msg("* Initializing DHCP", self._debug)
-        # Return IP assigned by DHCP
         self._dhcp_client = dhcp.DHCP(self, self.mac_address, hostname, self._debug)
-        ret = self._dhcp_client.request_dhcp_lease()
-        if ret == 1:
+        if self._dhcp_client.request_dhcp_lease():
             debug_msg(
                 "Found DHCP Server:\nIP: {}\n  Subnet Mask: {}\n  GW Addr: {}"
                 "\n  DNS Server: {}".format(*self.ifconfig),
                 self._debug,
             )
-            return 0
-        return -1
+        else:
+            self._dhcp_client = None
+            raise RuntimeError("Failed to configure DHCP Server!")
 
     def maintain_dhcp_lease(self) -> None:
         """Maintain the DHCP lease."""
-        if self._dhcp_client is not None:
+        if self._dhcp_client:
             self._dhcp_client.maintain_dhcp_lease()
 
     def get_host_by_name(self, hostname: str) -> bytes:
         """
         Convert a hostname to a packed 4-byte IP Address.
 
         :param str hostname: The host name to be converted.
 
-        :return Union[int, bytes]: a 4 bytearray.
+        :return bytes: The IPv4 address as a 4 byte array.
+
+        :raises RuntimeError: If the DNS lookup fails.
         """
         debug_msg("Get host by name", self._debug)
         if isinstance(hostname, str):
             hostname = bytes(hostname, "utf-8")
         # Return IP assigned by DHCP
         _dns_client = dns.DNS(
             self, self.pretty_ip(bytearray(self._dns)), debug=self._debug
         )
-        ret = _dns_client.gethostbyname(hostname)
-        debug_msg("* Resolved IP: {}".format(ret), self._debug)
-        if ret == -1:
+        ipv4 = _dns_client.gethostbyname(hostname)
+        debug_msg("* Resolved IP: {}".format(ipv4), self._debug)
+        if ipv4 == -1:
             raise RuntimeError("Failed to resolve hostname!")
-        return ret
+        return ipv4
 
     @property
     def max_sockets(self) -> int:
         """
         Maximum number of sockets supported by chip.
 
         :return int: Maximum supported sockets.
         """
-        if self._chip_type == "w5500":
-            return _W5200_W5500_MAX_SOCK_NUM
-        if self._chip_type == "w5100s":
-            return _W5100_MAX_SOCK_NUM
-        return -1
+        return _MAX_SOCK_NUM[self._chip_type]
 
     @property
     def chip(self) -> str:
         """
         Ethernet controller chip type.
 
         :return str: The chip type.
         """
         return self._chip_type
 
     @property
-    def ip_address(self) -> bytearray:
+    def ip_address(self) -> bytes:
         """
-        Configured IP address.
+        Configured IP address for the WIZnet Ethernet hardware.
 
-        :return bytearray: IP address as four bytes.
+        :return bytes: IP address as four bytes.
         """
-        return self.read(_REG_SIPR, 0x00, 4)
+        return self._read(_REG_SIPR[self._chip_type], 0x00, 4)
 
-    def pretty_ip(
-        self,
-        # pylint: disable=no-self-use, invalid-name
-        ip: bytearray,
-    ) -> str:
+    @staticmethod
+    def pretty_ip(ipv4: bytes) -> str:
         """
         Convert a 4 byte IP address to a dotted-quad string for printing.
 
-        :param bytearray ip: A four byte IP address.
+        :param bytearray ipv4: A four byte IP address.
 
         :return str: The IP address (a string of the form '255.255.255.255').
+
+        :raises ValueError: If IP address is not 4 bytes.
         """
-        return "%d.%d.%d.%d" % (ip[0], ip[1], ip[2], ip[3])
+        if len(ipv4) != 4:
+            raise ValueError("Wrong length for IPv4 address.")
+        return ".".join(f"{byte}" for byte in ipv4)
 
-    def unpretty_ip(
-        self,
-        # pylint: disable=no-self-use, invalid-name
-        ip: str,
-    ) -> bytes:
+    @staticmethod
+    def unpretty_ip(ipv4: str) -> bytes:
         """
         Convert a dotted-quad string to a four byte IP address.
 
-        :param str ip: IP address (a string of the form '255.255.255.255') to be converted.
+        :param str ipv4: IPv4 address (a string of the form '255.255.255.255') to be converted.
+
+        :return bytes: IPv4 address in four bytes.
 
-        :return bytes: IP address in four bytes.
+        :raises ValueError: If IPv4 address is not 4 bytes.
         """
-        octets = [int(x) for x in ip.split(".")]
-        return bytes(octets)
+        return _unprettyfy(ipv4, ".", 4)
 
     @property
     def mac_address(self) -> bytes:
         """
-        Ethernet hardware's MAC address.
+        The WIZnet Ethernet hardware MAC address.
 
-        :return bytearray: Six byte MAC address."""
-        return bytes(self.read(_REG_SHAR, 0x00, 6))
+        :return bytes: Six byte MAC address.
+        """
+        return self._read(_REG_SHAR[self._chip_type], 0x00, 6)
 
     @mac_address.setter
-    def mac_address(self, address: Tuple[int]) -> None:
+    def mac_address(self, address: Union[MacAddressRaw, str]) -> None:
         """
-        Set the hardware MAC address.
+        Set the WIZnet hardware MAC address.
 
-        :param Tuple address: A 6 byte hardware MAC address.
+        :param Union[MacAddressRaw, str] address: A hardware MAC address.
 
-        :raises ValueError: If the MAC address in invalid
+        :raises ValueError: If the MAC address is invalid
         """
-        # Check that the MAC is a valid 6 byte address.
-        if len(address) == 6 and False not in [
-            (isinstance(x, int) and 0 <= x <= 255) for x in address
-        ]:
-            self.write(_REG_SHAR, 0x04, address)
-        else:
+        try:
+            address = [int(x, 16) for x in address.split(":")]
+        except AttributeError:
+            pass
+        try:
+            if len(address) != 6:
+                raise ValueError()
+            # Bytes conversion will raise ValueError if values are not 0-255
+            self._write(_REG_SHAR[self._chip_type], 0x04, bytes(address))
+        except ValueError:
+            # pylint: disable=raise-missing-from
             raise ValueError("Invalid MAC address.")
 
-    def pretty_mac(
-        self,
-        # pylint: disable=no-self-use, invalid-name
-        mac: bytearray,
-    ) -> str:
+    @staticmethod
+    def pretty_mac(mac: bytes) -> str:
         """
-        Convert a bytearray MAC address to a ':' seperated string for display.
+        Convert a bytes MAC address to a ':' seperated string for display.
 
-        :param bytearray mac: The MAC address.
+        :param bytes mac: The MAC address.
 
         :return str: Mac Address in the form 00:00:00:00:00:00
+
+        :raises ValueError: If MAC address is not 6 bytes.
         """
-        return "%s:%s:%s:%s:%s:%s" % (
-            hex(mac[0]),
-            hex(mac[1]),
-            hex(mac[2]),
-            hex(mac[3]),
-            hex(mac[4]),
-            hex(mac[5]),
-        )
+        if len(mac) != 6:
+            raise ValueError("Incorrect length for MAC address.")
+        return ":".join(f"{byte:02x}" for byte in mac)
 
-    def remote_ip(self, socket_num: int) -> Union[str, bytearray]:
+    def remote_ip(self, socket_num: int) -> str:
         """
         IP address of the host which sent the current incoming packet.
 
         :param int socket_num: ID number of the socket to check.
 
-        :return Union[str, bytearray]: A four byte IP address.
+        :return str: The IPv4 address.
+
+        :raises ValueError: If the socket number is out of range.
         """
-        if socket_num >= self.max_sockets:
-            return self._pbuff
-        for octet in range(0, 4):
-            self._pbuff[octet] = self._read_socket(socket_num, _REG_SNDIPR + octet)[0]
-        return self.pretty_ip(self._pbuff)
+        self._sock_num_in_range(socket_num)
+        for octet in range(4):
+            self._pbuff[octet] = self._read_socket_register(
+                socket_num, _REG_SNDIPR[self._chip_type] + octet
+            )
+        return self.pretty_ip(self._pbuff[:4])
 
-    @property
-    def link_status(self) -> int:
-        """Physical hardware (PHY) connection status.
+    def remote_port(self, socket_num: int) -> int:
+        """
+        Port number of the host which sent the current incoming packet.
 
-        :return int: 1 if the link is up, 0 if the link is down.
+        :param int socket_num: ID number of the socket to check.
+
+        :return int: The incoming port number of the socket connection.
+
+        :raises ValueError: If the socket number is out of range.
         """
-        if self._chip_type == "w5500":
-            data = self.read(_REG_PHYCFGR, 0x00)
-            return data[0] & 0x01
-        if self._chip_type == "w5100s":
-            data = self.read(_REG_PHYCFGR_W5100S, 0x00)
-            return data[0] & 0x01
-        return 0
+        self._sock_num_in_range(socket_num)
+        return self._read_two_byte_sock_reg(socket_num, _REG_SNDPORT[self._chip_type])
 
-    def remote_port(self, socket_num: int) -> Union[int, bytearray]:
+    @property
+    def link_status(self) -> bool:
         """
-        Port of the host which sent the current incoming packet.
+        Physical hardware (PHY) connection status.
 
-        :param int socket_num: ID number of the socket to check.
+        Whether the WIZnet hardware is physically connected to an Ethernet network.
 
-        :return Union[int, bytearray]: The port number of the socket connection.
+        :return bool: True if the link is up, False if the link is down.
         """
-        if socket_num >= self.max_sockets:
-            return self._pbuff
-        for octet in range(2):
-            self._pbuff[octet] = self._read_socket(socket_num, _REG_SNDPORT + octet)[0]
-        return int((self._pbuff[0] << 8) | self._pbuff[0])
+        return bool(
+            int.from_bytes(self._read(_REG_LINK_FLAG[self._chip_type], 0x00), "big")
+            & 0x01
+        )
 
     @property
-    def ifconfig(
-        self,
-    ) -> Tuple[bytearray, bytearray, bytearray, Tuple[int, int, int, int]]:
+    def ifconfig(self) -> Tuple[bytes, bytes, bytes, bytes]:
         """
         Network configuration information.
 
-        :return Tuple[bytearray, bytearray, bytearray, Tuple[int, int, int, int]]: \
-            The IP address, subnet mask, gateway address and DNS server address."""
+        :return Tuple[bytes, bytes, bytes, bytes]: The IP address, subnet mask, gateway
+            address and DNS server address.
+        """
         return (
             self.ip_address,
-            self.read(_REG_SUBR, 0x00, 4),
-            self.read(_REG_GAR, 0x00, 4),
+            self._read(_REG_SUBR[self._chip_type], 0x00, 4),
+            self._read(_REG_GAR[self._chip_type], 0x00, 4),
             self._dns,
         )
 
     @ifconfig.setter
     def ifconfig(
-        self, params: Tuple[bytearray, bytearray, bytearray, Tuple[int, int, int, int]]
+        self, params: Tuple[IpAddress4Raw, IpAddress4Raw, IpAddress4Raw, IpAddress4Raw]
     ) -> None:
         """
         Set network configuration.
 
-        :param Tuple[bytearray, bytearray, bytearray, Tuple[int, int, int, int]]:
-            Configuration settings - (ip_address, subnet_mask, gateway_address, dns_server).
+        :param Tuple[Address4Bytes, Address4Bytes, Address4Bytes, Address4Bytes]: Configuration
+            settings - (ip_address, subnet_mask, gateway_address, dns_server).
         """
+        for param in params:
+            if len(param) != 4:
+                raise ValueError("IPv4 address must be 4 bytes.")
         ip_address, subnet_mask, gateway_address, dns_server = params
 
-        self.write(_REG_SIPR, 0x04, ip_address)
-        self.write(_REG_SUBR, 0x04, subnet_mask)
-        self.write(_REG_GAR, 0x04, gateway_address)
+        self._write(_REG_SIPR[self._chip_type], 0x04, bytes(ip_address))
+        self._write(_REG_SUBR[self._chip_type], 0x04, bytes(subnet_mask))
+        self._write(_REG_GAR[self._chip_type], 0x04, bytes(gateway_address))
 
-        self._dns = dns_server
+        self._dns = bytes(dns_server)
 
-    # pylint: disable=too-many-return-statements
-    def _w5xxx_init(self) -> int:
-        """
-        Detect and initialize a Wiznet5k ethernet module.
+    # *** Public Socket Methods ***
 
-        :return int: 1 if the initialization succeeds, 0 if it fails.
-        """
-
-        def _detect_and_reset_w5500() -> bool:
-            """
-            Detect and reset a W5500 chip. Called at startup to initialize the
-            interface hardware.
-
-            :return bool: True if a W5500 chip is detected, False if not.
-            """
-            self._chip_type = "w5500"
-            self._write_mr(0x80)
-            time.sleep(0.05)
-            if self._read_mr()[0] & 0x80:
-                return False
-
-            # assert self.sw_reset() == 0, "Chip not reset properly!"
-            self._write_mr(0x80)
-            time.sleep(0.05)
-            if self._read_mr()[0] & 0x80:
-                return False
-
-            self._write_mr(0x08)
-            # assert self._read_mr()[0] == 0x08, "Expected 0x08."
-            if self._read_mr()[0] != 0x08:
-                return False
-
-            self._write_mr(0x10)
-            # assert self._read_mr()[0] == 0x10, "Expected 0x10."
-            if self._read_mr()[0] != 0x10:
-                return False
-
-            self._write_mr(0x00)
-            # assert self._read_mr()[0] == 0x00, "Expected 0x00."
-            if self._read_mr()[0] != 0x00:
-                return False
-
-            if self.read(_REG_VERSIONR_W5500, 0x00)[0] != 0x04:
-                return False
-            # self._chip_type = "w5500"
-            # self._ch_base_msb = 0x10
-            return True
-
-        def _detect_and_reset_w5100s() -> bool:
-            """
-            Detect and reset a W5100S chip. Called at startup to initialize the
-            interface hardware.
-
-            :return bool: True if a W5100 chip is detected, False if not.
-            """
-            self._chip_type = "w5100s"
-            # sw reset
-            assert self.sw_reset() == 0, "Chip not reset properly!"
-            if self.read(_REG_VERSIONR_W5100S, 0x00)[0] != 0x51:
-                return False
-
-            self._ch_base_msb = 0x0400
-            return True
-
-        time.sleep(1)
-        self._cs.switch_to_output()
-        self._cs.value = 1
-
-        # Detect if chip is Wiznet W5500
-        if _detect_and_reset_w5500():
-            # perform w5500 initialization
-            for i in range(0, _W5200_W5500_MAX_SOCK_NUM):
-                ctrl_byte = 0x0C + (i << 5)
-                self.write(0x1E, ctrl_byte, 2)
-                self.write(0x1F, ctrl_byte, 2)
-        else:
-            # Detect if chip is Wiznet W5100S
-            if _detect_and_reset_w5100s():
-                pass
-            else:
-                return 0
-        return 1
-
-    def sw_reset(self) -> int:
-        """Perform a soft-reset on the Wiznet chip.
-
-        Perform a soft reset by writing to the chip's MR register reset bit.
-
-        :return int: 0 if the reset succeeds, -1 if not.
-        """
-        mode_reg = self._read_mr()
-        self._write_mr(0x80)
-        mode_reg = self._read_mr()
-
-        # W5100S case => 0x03
-        if (mode_reg[0] != 0x00) and (mode_reg[0] != 0x03):
-            return -1
-        return 0
-
-    def _read_mr(self) -> bytearray:
-        """Read from the Mode Register (MR)."""
-        res = self.read(_REG_MR, 0x00)
-        return res
-
-    def _write_mr(self, data: int) -> None:
-        """Write to the mode register (MR)."""
-        self.write(_REG_MR, 0x04, data)
-
-    def read(
-        self,
-        addr: int,
-        callback: int,
-        length: int = 1,
-        buffer: Optional[WriteableBuffer] = None,
-    ) -> Union[WriteableBuffer, bytearray]:
-        """
-        Read data from a register address.
-
-        :param int addr: Register address to read.
-        :param int callback: Callback reference.
-        :param int length: Number of bytes to read from the register, defaults to 1.
-        :param Optional[WriteableBuffer] buffer: Buffer to read data into, defaults to None.
-
-        :return Union[WriteableBuffer, bytearray]: Data read from the chip.
-        """
-        with self._device as bus_device:
-            if self._chip_type == "w5500":
-                bus_device.write(bytes([addr >> 8]))  # pylint: disable=no-member
-                bus_device.write(bytes([addr & 0xFF]))  # pylint: disable=no-member
-                bus_device.write(bytes([callback]))  # pylint: disable=no-member
-            else:
-                # if self._chip_type == "w5100s":
-                bus_device.write(bytes([0x0F]))  # pylint: disable=no-member
-                bus_device.write(bytes([addr >> 8]))  # pylint: disable=no-member
-                bus_device.write(bytes([addr & 0xFF]))  # pylint: disable=no-member
-
-            if buffer is None:
-                self._rxbuf = bytearray(length)
-                bus_device.readinto(self._rxbuf)  # pylint: disable=no-member
-                return self._rxbuf
-            bus_device.readinto(buffer, end=length)  # pylint: disable=no-member
-            return buffer
-
-    def write(
-        self, addr: int, callback: int, data: Union[int, Sequence[Union[int, bytes]]]
-    ) -> None:
-        """
-        Write data to a register address.
-
-        :param int addr: Destination address.
-        :param int callback: Callback reference.
-        :param Union[int, Sequence[Union[int, bytes]]] data: Data to write to the register address.
-        """
-        with self._device as bus_device:
-            if self._chip_type == "w5500":
-                bus_device.write(bytes([addr >> 8]))  # pylint: disable=no-member
-                bus_device.write(bytes([addr & 0xFF]))  # pylint: disable=no-member
-                bus_device.write(bytes([callback]))  # pylint: disable=no-member
-            else:
-                # if self._chip_type == "w5100s":
-                bus_device.write(bytes([0xF0]))  # pylint: disable=no-member
-                bus_device.write(bytes([addr >> 8]))  # pylint: disable=no-member
-                bus_device.write(bytes([addr & 0xFF]))  # pylint: disable=no-member
-
-            if hasattr(data, "from_bytes"):
-                bus_device.write(bytes([data]))  # pylint: disable=no-member
-            else:
-                for data_comp in data:
-                    bus_device.write(bytes([data_comp]))  # pylint: disable=no-member
-
-    # Socket-Register API
-
-    def socket_available(self, socket_num: int, sock_type: int = _SNMR_TCP) -> int:
+    def socket_available(self, socket_num: int, sock_type: int = SNMR_TCP) -> int:
         """
         Number of bytes available to be read from the socket.
 
         :param int socket_num: Socket to check for available bytes.
-        :param int sock_type: Socket type. Use SNMR_TCP for TCP or SNMR_UDP for UDP, \
+        :param int sock_type: Socket type. Use SNMR_TCP for TCP or SNMR_UDP for UDP,
             defaults to SNMR_TCP.
 
         :return int: Number of bytes available to read.
+
+        :raises ValueError: If the socket number is out of range.
+        :raises ValueError: If the number of bytes on a UDP socket is negative.
         """
         debug_msg(
             "socket_available called on socket {}, protocol {}".format(
                 socket_num, sock_type
             ),
             self._debug,
         )
-        if socket_num > self.max_sockets:
-            raise ValueError("Provided socket exceeds max_sockets.")
+        self._sock_num_in_range(socket_num)
 
-        res = self._get_rx_rcv_size(socket_num)
+        number_of_bytes = self._get_rx_rcv_size(socket_num)
+        if self.read_snsr(socket_num) == SNMR_UDP:
+            number_of_bytes -= 8  # Subtract UDP header from packet size.
+        if number_of_bytes < 0:
+            raise ValueError("Negative number of bytes found on socket.")
+        return number_of_bytes
 
-        if sock_type == _SNMR_TCP:
-            return res
-        if res > 0:
-            if self.udp_datasize[socket_num]:
-                return self.udp_datasize[socket_num]
-            # parse the udp rx packet
-            # read the first 8 header bytes
-            ret, self._pbuff = self.socket_read(socket_num, 8)
-            if ret > 0:
-                self.udp_from_ip[socket_num] = self._pbuff[:4]
-                self.udp_from_port[socket_num] = (self._pbuff[4] << 8) + self._pbuff[5]
-                self.udp_datasize[socket_num] = (self._pbuff[6] << 8) + self._pbuff[7]
-                ret = self.udp_datasize[socket_num]
-                return ret
-        return 0
-
-    def socket_status(self, socket_num: int) -> Optional[bytearray]:
+    def socket_status(self, socket_num: int) -> int:
         """
         Socket connection status.
 
         Can be: SNSR_SOCK_CLOSED, SNSR_SOCK_INIT, SNSR_SOCK_LISTEN, SNSR_SOCK_SYNSENT,
         SNSR_SOCK_SYNRECV, SNSR_SYN_SOCK_ESTABLISHED, SNSR_SOCK_FIN_WAIT,
         SNSR_SOCK_CLOSING, SNSR_SOCK_TIME_WAIT, SNSR_SOCK_CLOSE_WAIT, SNSR_LAST_ACK,
         SNSR_SOCK_UDP, SNSR_SOCK_IPRAW, SNSR_SOCK_MACRAW, SNSR_SOCK_PPOE.
 
         :param int socket_num: ID of socket to check.
 
-        :return: Optional[bytearray]
+        :return int: The connection status.
         """
         return self.read_snsr(socket_num)
 
     def socket_connect(
         self,
         socket_num: int,
-        dest: Union[bytes, bytearray],
+        dest: IpAddress4Raw,
         port: int,
-        conn_mode: int = _SNMR_TCP,
+        conn_mode: int = SNMR_TCP,
     ) -> int:
         """
-        Open and verify a connection from a socket to a destination IP address
+        Open and verify a connection from a socket to a destination IPv4 address
         or hostname. A TCP connection is made by default. A UDP connection can also
         be made.
 
         :param int socket_num: ID of the socket to be connected.
-        :param Union[bytes, bytearray] dest: The destination as a host name or IP address.
-        :param int port: Port to connect to (0 - 65,536).
+        :param IpAddress4Raw dest: The destination as a host name or IP address.
+        :param int port: Port to connect to (0 - 65,535).
         :param int conn_mode: The connection mode. Use SNMR_TCP for TCP or SNMR_UDP for UDP,
             defaults to SNMR_TCP.
+
+        :raises ValueError: if the socket number is out of range.
+        :raises ConnectionError: If the connection to the socket cannot be established.
         """
-        if not self.link_status:
-            raise ConnectionError("Ethernet cable disconnected!")
+        self._sock_num_in_range(socket_num)
+        self._check_link_status()
         debug_msg(
             "W5K socket connect, protocol={}, port={}, ip={}".format(
                 conn_mode, port, self.pretty_ip(dest)
             ),
             self._debug,
         )
         # initialize a socket and set the mode
-        res = self.socket_open(socket_num, conn_mode=conn_mode)
-        if res == 1:
-            raise ConnectionError("Failed to initialize a connection with the socket.")
-
+        self.socket_open(socket_num, conn_mode=conn_mode)
         # set socket destination IP and port
         self.write_sndipr(socket_num, dest)
         self.write_sndport(socket_num, port)
-        self._send_socket_cmd(socket_num, _CMD_SOCK_CONNECT)
+        self.write_sncr(socket_num, _CMD_SOCK_CONNECT)
 
-        if conn_mode == _SNMR_TCP:
+        if conn_mode == SNMR_TCP:
             # wait for tcp connection establishment
-            while self.socket_status(socket_num)[0] != SNSR_SOCK_ESTABLISHED:
+            while self.socket_status(socket_num) != SNSR_SOCK_ESTABLISHED:
                 time.sleep(0.001)
                 debug_msg(
-                    "SNSR: {}".format(self.socket_status(socket_num)[0]), self._debug
+                    "SNSR: {}".format(self.socket_status(socket_num)), self._debug
                 )
-                if self.socket_status(socket_num)[0] == SNSR_SOCK_CLOSED:
+                if self.socket_status(socket_num) == SNSR_SOCK_CLOSED:
                     raise ConnectionError("Failed to establish connection.")
-        elif conn_mode == SNMR_UDP:
-            self.udp_datasize[socket_num] = 0
         return 1
 
-    def _send_socket_cmd(self, socket: int, cmd: int) -> None:
-        """Send a socket command to a socket."""
-        self.write_sncr(socket, cmd)
-        while self.read_sncr(socket) != b"\x00":
-            debug_msg("waiting for SNCR to clear...", self._debug)
-
     def get_socket(self, *, reserve_socket=False) -> int:
         """
-        Request, allocate and return a socket from the W5k chip.
+        Request, allocate and return a socket from the WIZnet 5k chip.
 
         Cycle through the sockets to find the first available one. If the called with
         reserve_socket=True, update the list of reserved sockets (intended to be used with
         socket.socket()). Note that reserved sockets must be released by calling
-        cancel_reservation() once they are no longer needed.
+        release_socket() once they are no longer needed.
 
         If all sockets are reserved, no sockets are available for DNS calls, etc. Therefore,
         one socket cannot be reserved. Since socket 0 is the only socket that is capable of
         operating in MacRAW mode, it is the non-reservable socket.
 
         :param bool reserve_socket: Whether to reserve the socket.
 
         :returns int: The first available socket.
 
         :raises RuntimeError: If no socket is available.
         """
         debug_msg("*** Get socket.", self._debug)
         # Prefer socket zero for none reserved calls as it cannot be reserved.
-        if not reserve_socket and self.socket_status(0)[0] == SNSR_SOCK_CLOSED:
+        if not reserve_socket and self.socket_status(0) == SNSR_SOCK_CLOSED:
             debug_msg("Allocated socket # 0", self._debug)
             return 0
         # Then check the other sockets.
 
         #  Call garbage collection to encourage socket.__del__() be called to on any
         #  destroyed instances. Not at all guaranteed to work!
         gc.collect()
         debug_msg(
             "Reserved sockets: {}".format(WIZNET5K._sockets_reserved), self._debug
         )
 
         for socket_number, reserved in enumerate(WIZNET5K._sockets_reserved, start=1):
-            if (
-                not reserved
-                and self.socket_status(socket_number)[0] == SNSR_SOCK_CLOSED
-            ):
+            if not reserved and self.socket_status(socket_number) == SNSR_SOCK_CLOSED:
                 if reserve_socket:
                     WIZNET5K._sockets_reserved[socket_number - 1] = True
                     debug_msg(
                         "Allocated socket # {}.".format(socket_number),
                         self._debug,
                     )
                 return socket_number
-        raise RuntimeError("Out of sockets.")
+        raise RuntimeError("All sockets in use.")
 
-    @staticmethod
-    def release_socket(socket_number):
+    def release_socket(self, socket_number):
         """
         Update the socket reservation list when a socket is no longer reserved.
 
         :param int socket_number: The socket to release.
+
+        :raises ValueError: If the socket number is out of range.
         """
+        self._sock_num_in_range(socket_number)
         WIZNET5K._sockets_reserved[socket_number - 1] = False
 
     def socket_listen(
-        self, socket_num: int, port: int, conn_mode: int = _SNMR_TCP
+        self, socket_num: int, port: int, conn_mode: int = SNMR_TCP
     ) -> None:
         """
         Listen on a socket's port.
 
         :param int socket_num: ID of socket to listen on.
         :param int port: Port to listen on (0 - 65,535).
         :param int conn_mode: Connection mode SNMR_TCP for TCP or SNMR_UDP for
             UDP, defaults to SNMR_TCP.
+
+        :raises ValueError: If the socket number is out of range.
+        :raises ConnectionError: If the Ethernet link is down.
+        :raises RuntimeError: If unable to connect to a hardware socket.
         """
-        if not self.link_status:
-            raise ConnectionError("Ethernet cable disconnected!")
+        self._sock_num_in_range(socket_num)
+        self._check_link_status()
         debug_msg(
             "* Listening on port={}, ip={}".format(
                 port, self.pretty_ip(self.ip_address)
             ),
             self._debug,
         )
         # Initialize a socket and set the mode
         self.src_port = port
-        res = self.socket_open(socket_num, conn_mode=conn_mode)
+        self.socket_open(socket_num, conn_mode=conn_mode)
         self.src_port = 0
-        if res == 1:
-            raise RuntimeError("Failed to initialize the socket.")
         # Send listen command
-        self._send_socket_cmd(socket_num, _CMD_SOCK_LISTEN)
+        self.write_sncr(socket_num, _CMD_SOCK_LISTEN)
         # Wait until ready
-        status = [SNSR_SOCK_CLOSED]
-        while status[0] not in (
+        status = SNSR_SOCK_CLOSED
+        while status not in (
             SNSR_SOCK_LISTEN,
             SNSR_SOCK_ESTABLISHED,
             _SNSR_SOCK_UDP,
         ):
             status = self.read_snsr(socket_num)
-            if status[0] == SNSR_SOCK_CLOSED:
+            if status == SNSR_SOCK_CLOSED:
                 raise RuntimeError("Listening socket closed.")
 
-    def socket_accept(
-        self, socket_num: int
-    ) -> Tuple[int, Tuple[Union[str, bytearray], Union[int, bytearray]]]:
+    def socket_accept(self, socket_num: int) -> Tuple[int, Tuple[str, int]]:
         """
-        Destination IP address and port from an incoming connection.
+        Destination IPv4 address and port from an incoming connection.
 
         Return the next socket number so listening can continue, along with
         the IP address and port of the incoming connection.
 
         :param int socket_num: Socket number with connection to check.
+
         :return Tuple[int, Tuple[Union[str, bytearray], Union[int, bytearray]]]:
             If successful, the next (socket number, (destination IP address, destination port)).
 
-        If errors occur, the destination IP address and / or the destination port may be
-        returned as bytearrays.
+        :raises ValueError: If the socket number is out of range.
         """
+        self._sock_num_in_range(socket_num)
         dest_ip = self.remote_ip(socket_num)
         dest_port = self.remote_port(socket_num)
         next_socknum = self.get_socket()
         debug_msg(
             "Dest is ({}, {}), Next listen socknum is #{}".format(
                 dest_ip, dest_port, next_socknum
             ),
             self._debug,
         )
         return next_socknum, (dest_ip, dest_port)
 
-    def socket_open(self, socket_num: int, conn_mode: int = _SNMR_TCP) -> int:
+    def socket_open(self, socket_num: int, conn_mode: int = SNMR_TCP) -> None:
         """
         Open an IP socket.
 
         The socket may connect via TCP or UDP protocols.
 
         :param int socket_num: The socket number to open.
         :param int conn_mode: The protocol to use. Use SNMR_TCP for TCP or SNMR_UDP for \
             UDP, defaults to SNMR_TCP.
-        :return int: 1 if the socket was opened, 0 if not.
+
+        :raises ValueError: If the socket number is out of range.
+        :raises ConnectionError: If the Ethernet link is down or no connection to socket.
+        :raises RuntimeError: If unable to open a socket in UDP or TCP mode.
         """
-        if not self.link_status:
-            raise ConnectionError("Ethernet cable disconnected!")
+        self._sock_num_in_range(socket_num)
+        self._check_link_status()
         debug_msg("*** Opening socket {}".format(socket_num), self._debug)
-        status = self.read_snsr(socket_num)[0]
-        if status in (
+        if self.read_snsr(socket_num) not in (
             SNSR_SOCK_CLOSED,
             SNSR_SOCK_TIME_WAIT,
             SNSR_SOCK_FIN_WAIT,
             SNSR_SOCK_CLOSE_WAIT,
             _SNSR_SOCK_CLOSING,
             _SNSR_SOCK_UDP,
         ):
-            debug_msg(
-                "* Opening W5k Socket, protocol={}".format(conn_mode), self._debug
-            )
-            time.sleep(0.00025)
+            raise ConnectionError("Failed to initialize a connection with the socket.")
+        debug_msg("* Opening W5k Socket, protocol={}".format(conn_mode), self._debug)
+        time.sleep(0.00025)
 
-            self.write_snmr(socket_num, conn_mode)
-            self.write_snir(socket_num, 0xFF)
+        self.write_snmr(socket_num, conn_mode)
+        self.write_snir(socket_num, 0xFF)
 
-            if self.src_port > 0:
-                # write to socket source port
-                self.write_sock_port(socket_num, self.src_port)
-            else:
+        if self.src_port > 0:
+            # write to socket source port
+            self.write_sock_port(socket_num, self.src_port)
+        else:
+            s_port = randint(49152, 65535)
+            while s_port in self._src_ports_in_use:
                 s_port = randint(49152, 65535)
-                while s_port in _SRC_PORTS:
-                    s_port = randint(49152, 65535)
-                self.write_sock_port(socket_num, s_port)
-                _SRC_PORTS[socket_num] = s_port
-
-            # open socket
-            self.write_sncr(socket_num, _CMD_SOCK_OPEN)
-            self.read_sncr(socket_num)
-            if self.read_snsr((socket_num))[0] not in [0x13, 0x22]:
-                raise RuntimeError("Could not open socket in TCP or UDP mode.")
-            return 0
-        return 1
+            self.write_sock_port(socket_num, s_port)
+            self._src_ports_in_use[socket_num] = s_port
+
+        # open socket
+        self.write_sncr(socket_num, _CMD_SOCK_OPEN)
+        if self.read_snsr(socket_num) not in [_SNSR_SOCK_INIT, _SNSR_SOCK_UDP]:
+            raise RuntimeError("Could not open socket in TCP or UDP mode.")
 
     def socket_close(self, socket_num: int) -> None:
         """
         Close a socket.
 
         :param int socket_num: The socket to close.
+
+        :raises ValueError: If the socket number is out of range.
         """
         debug_msg("*** Closing socket {}".format(socket_num), self._debug)
-        timeout = time.monotonic() + 5.0
+        self._sock_num_in_range(socket_num)
         self.write_sncr(socket_num, _CMD_SOCK_CLOSE)
-        debug_msg("  Waiting for close command to process…", self._debug)
-        while self.read_sncr(socket_num)[0]:
-            if time.monotonic() < timeout:
-                raise RuntimeError(
-                    "Wiznet5k failed to complete command, status = {}.".format(
-                        self.read_sncr(socket_num)[0]
-                    )
-                )
-            time.sleep(0.0001)
         debug_msg("  Waiting for socket to close…", self._debug)
         timeout = time.monotonic() + 5.0
-        while self.read_snsr(socket_num)[0] != SNSR_SOCK_CLOSED:
+        while self.read_snsr(socket_num) != SNSR_SOCK_CLOSED:
             if time.monotonic() > timeout:
                 raise RuntimeError(
                     "Wiznet5k failed to close socket, status = {}.".format(
-                        self.read_snsr(socket_num)[0]
+                        self.read_snsr(socket_num)
                     )
                 )
             time.sleep(0.0001)
         debug_msg("  Socket has closed.", self._debug)
 
     def socket_disconnect(self, socket_num: int) -> None:
         """
         Disconnect a TCP or UDP connection.
 
         :param int socket_num: The socket to close.
+
+        :raises ValueError: If the socket number is out of range.
         """
         debug_msg("*** Disconnecting socket {}".format(socket_num), self._debug)
+        self._sock_num_in_range(socket_num)
         self.write_sncr(socket_num, _CMD_SOCK_DISCON)
-        self.read_sncr(socket_num)
 
     def socket_read(self, socket_num: int, length: int) -> Tuple[int, bytes]:
         """
-        Read data from a TCP socket.
+        Read data from a hardware socket. Called directly by TCP socket objects and via
+        read_udp() for UDP socket objects.
 
         :param int socket_num: The socket to read data from.
         :param int length: The number of bytes to read from the socket.
 
-        :return Tuple[int, Union[int, bytearray]]: If the read was successful then the first
-            item of the tuple is the length of the data and the second is the data. If the read
-            was unsuccessful then both items equal an error code, 0 for no data waiting and -1
-            for no connection to the socket.
+        :returns Tuple[int, bytes]: If the read was successful then the first
+            item of the tuple is the length of the data and the second is the data.
+            If the read was unsuccessful then 0, b"" is returned.
+
+        :raises ValueError: If the socket number is out of range.
+        :raises ConnectionError: If the Ethernet link is down.
+        :raises RuntimeError: If the socket connection has been lost.
         """
-        # pylint: disable=too-many-branches
-        if not self.link_status:
-            raise ConnectionError("Ethernet cable disconnected!")
-        if socket_num > self.max_sockets:
-            raise ValueError("Provided socket exceeds max_sockets.")
+        self._sock_num_in_range(socket_num)
+        self._check_link_status()
 
         # Check if there is data available on the socket
-        ret = self._get_rx_rcv_size(socket_num)
-        debug_msg("Bytes avail. on sock: {}".format(ret), self._debug)
-        if ret == 0:
-            # no data on socket?
-            status = self._read_snmr(socket_num)
-            if status in (SNSR_SOCK_LISTEN, SNSR_SOCK_CLOSED, SNSR_SOCK_CLOSE_WAIT):
-                # remote end closed its side of the connection, EOF state
-                raise RuntimeError("Lost connection to peer.")
-                # connection is alive, no data waiting to be read
-            ret = -1
-        elif ret > length:
-            # set ret to the length of buffer
-            ret = length
-        if ret > 0:
-            debug_msg("* Processing {} bytes of data".format(ret), self._debug)
-            # Read the starting save address of the received data
-            ptr = self._read_snrx_rd(socket_num)
-
-            if self._chip_type == "w5500":
-                # Read data from the starting address of snrx_rd
-                ctrl_byte = 0x18 + (socket_num << 5)
-
-                resp = self.read(ptr, ctrl_byte, ret)
-            else:
-                # if self._chip_type == "w5100s":
-                offset = ptr & _SOCK_MASK
-                src_addr = offset + (socket_num * _SOCK_SIZE + 0x6000)
-                if offset + ret > _SOCK_SIZE:
-                    size = _SOCK_SIZE - offset
-                    resp1 = self.read(src_addr, 0x00, size)
-                    size = ret - size
-                    src_addr = socket_num * _SOCK_SIZE + 0x6000
-                    resp2 = self.read(src_addr, 0x00, size)
-                    resp = resp1 + resp2
-                else:
-                    resp = self.read(src_addr, 0x00, ret)
-
-            #  After reading the received data, update Sn_RX_RD to the increased
-            # value as many as the reading size.
-            ptr = (ptr + ret) & 0xFFFF
-            self._write_snrx_rd(socket_num, ptr)
-
-            # Notify the W5k of the updated Sn_Rx_RD
+        bytes_on_socket = self._get_rx_rcv_size(socket_num)
+        debug_msg("Bytes avail. on sock: {}".format(bytes_on_socket), self._debug)
+        if bytes_on_socket:
+            bytes_on_socket = length if bytes_on_socket > length else bytes_on_socket
+            debug_msg(
+                "* Processing {} bytes of data".format(bytes_on_socket), self._debug
+            )
+            # Read the starting save address of the received data.
+            pointer = self._read_snrx_rd(socket_num)
+            # Read data from the hardware socket.
+            bytes_read = self._chip_socket_read(socket_num, pointer, bytes_on_socket)
+            # After reading the received data, update Sn_RX_RD register.
+            pointer = (pointer + bytes_on_socket) & 0xFFFF
+            self._write_snrx_rd(socket_num, pointer)
             self.write_sncr(socket_num, _CMD_SOCK_RECV)
-            while self.read_sncr(socket_num)[0] & _CMD_SOCK_RECV:
-                time.sleep(0.0001)
-        return ret, resp
+        else:
+            # no data on socket
+            if self._read_snmr(socket_num) in (
+                SNSR_SOCK_LISTEN,
+                SNSR_SOCK_CLOSED,
+                SNSR_SOCK_CLOSE_WAIT,
+            ):
+                raise RuntimeError("Lost connection to peer.")
+            bytes_read = b""
+        return bytes_on_socket, bytes_read
 
     def read_udp(self, socket_num: int, length: int) -> Tuple[int, bytes]:
         """
         Read UDP socket's current message bytes.
 
         :param int socket_num: The socket to read data from.
         :param int length: The number of bytes to read from the socket.
 
         :return Tuple[int, bytes]: If the read was successful then the first
             item of the tuple is the length of the data and the second is the data.
             If the read was unsuccessful then (0, b"") is returned.
+
+        :raises ValueError: If the socket number is out of range.
         """
-        if self.udp_datasize[socket_num] > 0:
-            if self.udp_datasize[socket_num] <= length:
-                ret, resp = self.socket_read(socket_num, self.udp_datasize[socket_num])
-            else:
-                ret, resp = self.socket_read(socket_num, length)
-                # just consume the rest, it is lost to the higher layers
-                self.socket_read(socket_num, self.udp_datasize[socket_num] - length)
-            self.udp_datasize[socket_num] = 0
-            return ret, resp
-        return 0, b""
+        self._sock_num_in_range(socket_num)
+        bytes_on_socket, bytes_read = 0, b""
+        # Parse the UDP packet header.
+        header_length, self._pbuff[:8] = self.socket_read(socket_num, 8)
+        if header_length:
+            if header_length != 8:
+                raise ValueError("Invalid UDP header.")
+            data_length = self._chip_parse_udp_header(socket_num)
+            # Read the UDP packet data.
+            if data_length:
+                if data_length <= length:
+                    bytes_on_socket, bytes_read = self.socket_read(
+                        socket_num, data_length
+                    )
+                else:
+                    bytes_on_socket, bytes_read = self.socket_read(socket_num, length)
+                    # just consume the rest, it is lost to the higher layers
+                    self.socket_read(socket_num, data_length - length)
+        return bytes_on_socket, bytes_read
 
     def socket_write(
-        self, socket_num: int, buffer: bytearray, timeout: float = 0
+        self, socket_num: int, buffer: bytearray, timeout: float = 0.0
     ) -> int:
         """
         Write data to a socket.
 
         :param int socket_num: The socket to write to.
         :param bytearray buffer: The data to write to the socket.
         :param float timeout: Write data timeout in seconds, defaults to 0.0 which waits
             indefinitely.
 
-        :return int: The number of bytes written to the buffer.
+        :return int: The number of bytes written to the socket.
+
+        :raises ConnectionError: If the Ethernet link is down.
+        :raises ValueError: If the socket number is out of range.
+        :raises RuntimeError: If the data cannot be sent.
         """
-        # pylint: disable=too-many-branches
-        if not self.link_status:
-            raise ConnectionError("Ethernet cable disconnected!")
-        if socket_num > self.max_sockets:
-            raise ValueError("Provided socket exceeds max_sockets.")
+        self._sock_num_in_range(socket_num)
+        self._check_link_status()
         if len(buffer) > _SOCK_SIZE:
-            ret = _SOCK_SIZE
+            bytes_to_write = _SOCK_SIZE
         else:
-            ret = len(buffer)
-        stamp = time.monotonic()
+            bytes_to_write = len(buffer)
+        stop_time = time.monotonic() + timeout
 
         # If buffer is available, start the transfer
         free_size = self._get_tx_free_size(socket_num)
-        while free_size < ret:
+        while free_size < bytes_to_write:
             free_size = self._get_tx_free_size(socket_num)
-            status = self.socket_status(socket_num)[0]
+            status = self.socket_status(socket_num)
             if status not in (SNSR_SOCK_ESTABLISHED, SNSR_SOCK_CLOSE_WAIT) or (
-                timeout and time.monotonic() - stamp > timeout
+                timeout and time.monotonic() > stop_time
             ):
-                ret = 0
-                break
+                raise RuntimeError("Unable to write data to the socket.")
 
         # Read the starting address for saving the transmitting data.
-        ptr = self._read_sntx_wr(socket_num)
-        offset = ptr & _SOCK_MASK
-        if self._chip_type == "w5500":
-            dst_addr = offset + (socket_num * _SOCK_SIZE + 0x8000)
-            txbuf = buffer[:ret]
-            cntl_byte = 0x14 + (socket_num << 5)
-            self.write(dst_addr, cntl_byte, txbuf)
-
-        else:
-            # if self._chip_type == "w5100s":
-            dst_addr = offset + (socket_num * _SOCK_SIZE + 0x4000)
-
-            if offset + ret > _SOCK_SIZE:
-                size = _SOCK_SIZE - offset
-                txbuf = buffer[0:size]
-                self.write(dst_addr, 0x00, txbuf)
-                txbuf = buffer[size:ret]
-                size = ret - size
-                dst_addr = socket_num * _SOCK_SIZE + 0x4000
-                self.write(dst_addr, 0x00, txbuf)
-            else:
-                txbuf = buffer[:ret]
-                self.write(dst_addr, 0x00, buffer[:ret])
-
+        pointer = self._read_sntx_wr(socket_num)
+        offset = pointer & _SOCK_MASK
+        self._chip_socket_write(socket_num, offset, bytes_to_write, buffer)
         # update sn_tx_wr to the value + data size
-        ptr = (ptr + ret) & 0xFFFF
-        self._write_sntx_wr(socket_num, ptr)
+        pointer = (pointer + bytes_to_write) & 0xFFFF
+        self._write_sntx_wr(socket_num, pointer)
         self.write_sncr(socket_num, _CMD_SOCK_SEND)
-        while self.read_sncr(socket_num) != b"\x00":
-            time.sleep(0.001)
 
         # check data was  transferred correctly
-        while not self.read_snir(socket_num)[0] & _SNIR_SEND_OK:
-            if self.socket_status(socket_num)[0] in (
+        while not self.read_snir(socket_num) & _SNIR_SEND_OK:
+            if self.socket_status(socket_num) in (
                 SNSR_SOCK_CLOSED,
                 SNSR_SOCK_TIME_WAIT,
                 SNSR_SOCK_FIN_WAIT,
                 SNSR_SOCK_CLOSE_WAIT,
                 _SNSR_SOCK_CLOSING,
             ):
-                raise RuntimeError("Socket closed before data was sent.")
-            if timeout and time.monotonic() - stamp > timeout:
+                raise RuntimeError("No data was sent, socket was closed.")
+            if timeout and time.monotonic() > stop_time:
                 raise RuntimeError("Operation timed out. No data sent.")
-            if self.read_snir(socket_num)[0] & SNIR_TIMEOUT:
-                raise TimeoutError(
-                    "Hardware timeout while sending on socket {}.".format(socket_num)
-                )
+            if self.read_snir(socket_num) & SNIR_TIMEOUT:
+                self.write_snir(socket_num, SNIR_TIMEOUT)
+                # TCP sockets are closed by the hardware timeout
+                # so that will be caught at the while statement.
+                # UDP sockets are 1:many so not closed thus return 0.
+                if self._read_snmr(socket_num) == SNMR_UDP:
+                    return 0
             time.sleep(0.001)
         self.write_snir(socket_num, _SNIR_SEND_OK)
-        return ret
+        return bytes_to_write
+
+    def sw_reset(self) -> None:
+        """
+        Soft reset and reinitialize the WIZnet chip.
+
+        :raises RuntimeError: If reset fails.
+        """
+        self._wiznet_chip_init()
+
+    def _sw_reset_5x00(self) -> bool:
+        """
+        Perform a soft reset on the WIZnet 5100s and 5500 chips.
+
+        :returns bool: True if reset was success
+        """
+        self._write_mr(_MR_RST)
+        time.sleep(0.05)
+        return self._read_mr() == {"w5500": 0x00, "w5100s": 0x03}[self._chip_type]
+
+    def _wiznet_chip_init(self) -> None:
+        """
+        Detect and initialize a WIZnet 5k Ethernet module.
+
+        :raises RuntimeError: If no WIZnet chip is detected.
+        """
+
+        def _setup_sockets() -> None:
+            """Initialise sockets for w5500 and w6100 chips."""
+            for sock_num in range(_MAX_SOCK_NUM[self._chip_type]):
+                ctrl_byte = 0x0C + (sock_num << 5)
+                self._write(0x1E, ctrl_byte, 2)
+                self._write(0x1F, ctrl_byte, 2)
+            self._ch_base_msb = 0x00
+            WIZNET5K._sockets_reserved = [False] * (_MAX_SOCK_NUM[self._chip_type] - 1)
+            self._src_ports_in_use = [0] * _MAX_SOCK_NUM[self._chip_type]
+
+        def _detect_and_reset_w6100() -> bool:
+            """
+            Detect and reset a W6100 chip. Called at startup to initialize the
+            interface hardware.
+
+            :return bool: True if a W6100 chip is detected, False if not.
+            """
+            self._chip_type = "w6100"
+
+            # Reset w6100
+            self._write(0x41F4, 0x04, 0xCE)  # Unlock chip settings.
+            time.sleep(0.05)  # Wait for unlock.
+            self._write(0x2004, 0x04, 0x00)  # Reset chip.
+            time.sleep(0.05)  # Wait for reset.
+
+            if self._read(_REG_VERSIONR[self._chip_type], 0x00)[0] != 0x61:
+                return False
+            # Initialize w6100.
+            self._write(0x41F5, 0x04, 0x3A)  # Unlock network settings.
+            _setup_sockets()
+            return True
+
+        def _detect_and_reset_w5500() -> bool:
+            """
+            Detect and reset a W5500 chip. Called at startup to initialize the
+            interface hardware.
+
+            :return bool: True if a W5500 chip is detected, False if not.
+            """
+            self._chip_type = "w5500"
+            if not self._sw_reset_5x00():
+                return False
+
+            self._write_mr(0x08)
+            if self._read_mr() != 0x08:
+                return False
+
+            self._write_mr(0x10)
+            if self._read_mr() != 0x10:
+                return False
+
+            self._write_mr(0x00)
+            if self._read_mr() != 0x00:
+                return False
+
+            if self._read(_REG_VERSIONR[self._chip_type], 0x00)[0] != 0x04:
+                return False
+            # Initialize w5500
+            _setup_sockets()
+            return True
+
+        def _detect_and_reset_w5100s() -> bool:
+            """
+            Detect and reset a W5100S chip. Called at startup to initialize the
+            interface hardware.
+
+            :return bool: True if a W5100 chip is detected, False if not.
+            """
+            self._chip_type = "w5100s"
+            if not self._sw_reset_5x00():
+                return False
+
+            if self._read(_REG_VERSIONR[self._chip_type], 0x00)[0] != 0x51:
+                return False
+
+            # Initialise w5100s
+            self._ch_base_msb = 0x0400
+            WIZNET5K._sockets_reserved = [False] * (_MAX_SOCK_NUM[self._chip_type] - 1)
+            self._src_ports_in_use = [0] * _MAX_SOCK_NUM[self._chip_type]
+            return True
+
+        for func in [
+            _detect_and_reset_w5100s,
+            _detect_and_reset_w5500,
+            _detect_and_reset_w6100,
+        ]:
+            if func():
+                return
+        self._chip_type = None
+        raise RuntimeError("Failed to initialize WIZnet module.")
+
+    def _sock_num_in_range(self, sock: int) -> None:
+        """Check that the socket number is in the range 0 - maximum sockets."""
+        if not 0 <= sock < self.max_sockets:
+            raise ValueError("Socket number out of range.")
+
+    def _check_link_status(self):
+        """Raise an exception if the link is down."""
+        if not self.link_status:
+            raise ConnectionError("The Ethernet connection is down.")
+
+    def _read_mr(self) -> int:
+        """Read from the Mode Register (MR)."""
+        return int.from_bytes(self._read(_REG_MR[self._chip_type], 0x00), "big")
+
+    def _write_mr(self, data: int) -> None:
+        """Write to the mode register (MR)."""
+        self._write(_REG_MR[self._chip_type], 0x04, data)
+
+    # *** Low Level Methods ***
+
+    def _read(
+        self,
+        addr: int,
+        callback: int,
+        length: int = 1,
+    ) -> bytes:
+        """
+        Read data from a register address.
+
+        :param int addr: Register address to read.
+        :param int callback: Callback reference.
+        :param int length: Number of bytes to read from the register, defaults to 1.
+
+        :return bytes: Data read from the chip.
+        """
+        with self._device as bus_device:
+            self._chip_read(bus_device, addr, callback)
+            self._rxbuf = bytearray(length)
+            bus_device.readinto(self._rxbuf)
+            return bytes(self._rxbuf)
+
+    def _write(self, addr: int, callback: int, data: Union[int, bytes]) -> None:
+        """
+        Write data to a register address.
+
+        :param int addr: Destination address.
+        :param int callback: Callback reference.
+        :param Union[int, bytes] data: Data to write to the register address, if data
+            is an integer, it must be 1 or 2 bytes.
+
+        :raises OverflowError: if integer data is more than 2 bytes.
+        """
+        with self._device as bus_device:
+            self._chip_write(bus_device, addr, callback)
+            try:
+                data = data.to_bytes(1, "big")
+            except OverflowError:
+                data = data.to_bytes(2, "big")
+            except AttributeError:
+                pass
+            bus_device.write(data)
+
+    def _read_two_byte_sock_reg(self, sock: int, reg_address: int) -> int:
+        """Read a two byte socket register."""
+        register = self._read_socket_register(sock, reg_address) << 8
+        register += self._read_socket_register(sock, reg_address + 1)
+        return register
+
+    def _write_two_byte_sock_reg(self, sock: int, reg_address: int, data: int) -> None:
+        """Write to a two byte socket register."""
+        self._write_socket_register(sock, reg_address, data >> 8 & 0xFF)
+        self._write_socket_register(sock, reg_address + 1, data & 0xFF)
+
+    # *** Socket Register Methods ***
 
-    # Socket-Register Methods
     def _get_rx_rcv_size(self, sock: int) -> int:
         """Size of received and saved in socket buffer."""
         val = 0
         val_1 = self._read_snrx_rsr(sock)
         while val != val_1:
             val_1 = self._read_snrx_rsr(sock)
             if val_1 != 0:
                 val = self._read_snrx_rsr(sock)
-        return int.from_bytes(val, "big")
+        return val
 
     def _get_tx_free_size(self, sock: int) -> int:
         """Free size of socket's tx buffer block."""
         val = 0
         val_1 = self._read_sntx_fsr(sock)
         while val != val_1:
             val_1 = self._read_sntx_fsr(sock)
             if val_1 != 0:
                 val = self._read_sntx_fsr(sock)
-        return int.from_bytes(val, "big")
+        return val
 
     def _read_snrx_rd(self, sock: int) -> int:
         """Read socket n RX Read Data Pointer Register."""
-        self._pbuff[0] = self._read_socket(sock, _REG_SNRX_RD)[0]
-        self._pbuff[1] = self._read_socket(sock, _REG_SNRX_RD + 1)[0]
-        return self._pbuff[0] << 8 | self._pbuff[1]
+        return self._read_two_byte_sock_reg(sock, _REG_SNRX_RD[self._chip_type])
 
     def _write_snrx_rd(self, sock: int, data: int) -> None:
         """Write socket n RX Read Data Pointer Register."""
-        self._write_socket(sock, _REG_SNRX_RD, data >> 8 & 0xFF)
-        self._write_socket(sock, _REG_SNRX_RD + 1, data & 0xFF)
-
-    def _write_sntx_wr(self, sock: int, data: int) -> None:
-        """Write the socket write buffer pointer for socket `sock`."""
-        self._write_socket(sock, _REG_SNTX_WR, data >> 8 & 0xFF)
-        self._write_socket(sock, _REG_SNTX_WR + 1, data & 0xFF)
+        self._write_two_byte_sock_reg(sock, _REG_SNRX_RD[self._chip_type], data)
 
     def _read_sntx_wr(self, sock: int) -> int:
         """Read the socket write buffer pointer for socket `sock`."""
-        self._pbuff[0] = self._read_socket(sock, 0x0024)[0]
-        self._pbuff[1] = self._read_socket(sock, 0x0024 + 1)[0]
-        return self._pbuff[0] << 8 | self._pbuff[1]
+        return self._read_two_byte_sock_reg(sock, _REG_SNTX_WR[self._chip_type])
 
-    def _read_sntx_fsr(self, sock: int) -> Optional[bytearray]:
+    def _write_sntx_wr(self, sock: int, data: int) -> None:
+        """Write the socket write buffer pointer for socket `sock`."""
+        self._write_two_byte_sock_reg(sock, _REG_SNTX_WR[self._chip_type], data)
+
+    def _read_sntx_fsr(self, sock: int) -> int:
         """Read socket n TX Free Size Register"""
-        data = self._read_socket(sock, _REG_SNTX_FSR)
-        data += self._read_socket(sock, _REG_SNTX_FSR + 1)
-        return data
+        return self._read_two_byte_sock_reg(sock, _REG_SNTX_FSR[self._chip_type])
 
-    def _read_snrx_rsr(self, sock: int) -> Optional[bytearray]:
+    def _read_snrx_rsr(self, sock: int) -> int:
         """Read socket n Received Size Register"""
-        data = self._read_socket(sock, _REG_SNRX_RSR)
-        data += self._read_socket(sock, _REG_SNRX_RSR + 1)
-        return data
-
-    def write_sndipr(self, sock: int, ip_addr: bytearray) -> None:
-        """Write to socket destination IP Address."""
-        for offset in range(4):
-            self._write_socket(sock, _REG_SNDIPR + offset, ip_addr[offset])
+        return self._read_two_byte_sock_reg(sock, _REG_SNRX_RSR[self._chip_type])
 
-    def _read_sndipr(self, sock) -> bytearray:
+    def _read_sndipr(self, sock) -> bytes:
         """Read socket destination IP address."""
-        data = b""
+        data = []
         for offset in range(4):
-            data += self._read_socket(sock, _REG_SIPR + offset)
-        return bytearray(data)
+            data.append(
+                self._read_socket_register(sock, _REG_SNDIPR[self._chip_type] + offset)
+            )
+        return bytes(data)
+
+    def write_sndipr(self, sock: int, ip_addr: bytes) -> None:
+        """Write to socket destination IP Address."""
+        for offset, value in enumerate(ip_addr):
+            self._write_socket_register(
+                sock, _REG_SNDIPR[self._chip_type] + offset, value
+            )
 
     def write_sndport(self, sock: int, port: int) -> None:
         """Write to socket destination port."""
-        self._write_socket(sock, _REG_SNDPORT, port >> 8)
-        self._write_socket(sock, _REG_SNDPORT + 1, port & 0xFF)
+        self._write_two_byte_sock_reg(sock, _REG_SNDPORT[self._chip_type], port)
 
-    def read_snsr(self, sock: int) -> Optional[bytearray]:
+    def read_snsr(self, sock: int) -> int:
         """Read Socket n Status Register."""
-        return self._read_socket(sock, _REG_SNSR)
+        return self._read_socket_register(sock, _REG_SNSR[self._chip_type])
 
-    def read_snir(self, sock: int) -> Optional[bytearray]:
+    def read_snir(self, sock: int) -> int:
         """Read Socket n Interrupt Register."""
-        return self._read_socket(sock, _REG_SNIR)
-
-    def write_snmr(self, sock: int, protocol: int) -> None:
-        """Write to Socket n Mode Register."""
-        self._write_socket(sock, _REG_SNMR, protocol)
+        return self._read_socket_register(sock, _REG_SNIR[self._chip_type])
 
     def write_snir(self, sock: int, data: int) -> None:
         """Write to Socket n Interrupt Register."""
-        self._write_socket(sock, _REG_SNIR, data)
+        self._write_socket_register(sock, _REG_SNIR[self._chip_type], data)
+
+    def _read_snmr(self, sock: int) -> int:
+        """Read the socket MR register."""
+        return self._read_socket_register(sock, _REG_SNMR)
+
+    def write_snmr(self, sock: int, protocol: int) -> None:
+        """Write to Socket n Mode Register."""
+        self._write_socket_register(sock, _REG_SNMR, protocol)
 
     def write_sock_port(self, sock: int, port: int) -> None:
         """Write to the socket port number."""
-        self._write_socket(sock, _REG_SNPORT, port >> 8)
-        self._write_socket(sock, _REG_SNPORT + 1, port & 0xFF)
+        self._write_two_byte_sock_reg(sock, _REG_SNPORT[self._chip_type], port)
 
     def write_sncr(self, sock: int, data: int) -> None:
         """Write to socket command register."""
-        self._write_socket(sock, _REG_SNCR, data)
-
-    def read_sncr(self, sock: int) -> Optional[bytearray]:
-        """Read socket command register."""
-        return self._read_socket(sock, _REG_SNCR)
-
-    def _read_snmr(self, sock: int) -> Optional[bytearray]:
-        return self._read_socket(sock, _REG_SNMR)
-
-    def _write_socket(self, sock: int, address: int, data: int) -> None:
-        """Write to a W5k socket register."""
-        if self._chip_type == "w5500":
-            cntl_byte = (sock << 5) + 0x0C
-            return self.write(address, cntl_byte, data)
-        if self._chip_type == "w5100s":
-            cntl_byte = 0
-            return self.write(
-                self._ch_base_msb + sock * _CH_SIZE + address, cntl_byte, data
-            )
-        return None
-
-    def _read_socket(self, sock: int, address: int) -> bytearray:
-        """Read a W5k socket register."""
-        if self._chip_type == "w5500":
-            cntl_byte = (sock << 5) + 0x08
-            return self.read(address, cntl_byte)
-        if self._chip_type == "w5100s":
-            cntl_byte = 0
-            return self.read(self._ch_base_msb + sock * _CH_SIZE + address, cntl_byte)
-        raise RuntimeError("Invalid Wiznet chip type.")
+        self._write_socket_register(sock, _REG_SNCR[self._chip_type], data)
+        # Wait for command to complete before continuing.
+        while self._read_socket_register(sock, _REG_SNCR[self._chip_type]):
+            pass
 
     @property
     def rcr(self) -> int:
         """Retry count register."""
-        if self._chip_type == "w5500":
-            rcr_reg = _REG_RCR_5500
-        else:
-            # Assume a W5100s
-            rcr_reg = _REG_RCR_5100s
-        return self.read(rcr_reg, 0x00)
+        return int.from_bytes(self._read(_REG_RCR[self._chip_type], 0x00), "big")
 
     @rcr.setter
     def rcr(self, retry_count: int) -> None:
+        """Retry count register."""
         if 0 > retry_count > 255:
             raise ValueError("Retries must be from 0 to 255.")
-        if self._chip_type == "w5500":
-            rcr_reg = _REG_RCR_5500
-        else:
-            # Assume a W5100s
-            rcr_reg = _REG_RCR_5100s
-        self.write(rcr_reg, 0x04, retry_count)
+        self._write(_REG_RCR[self._chip_type], 0x04, retry_count)
 
     @property
     def rtr(self) -> int:
         """Retry time register."""
-        if self._chip_type == "w5500":
-            reg = _REG_RTR_5500
-        else:
-            # Assume a W5100s
-            reg = _REG_RTR_5100s
-        return self.read(reg, 0x00, 2)
+        return int.from_bytes(self._read(_REG_RTR[self._chip_type], 0x00, 2), "big")
 
     @rtr.setter
-    def rtr(self, retry_count: int) -> None:
-        if 0 > retry_count > 2**16:
-            raise ValueError("Retry time must be from 0 to {}".format(2**16))
-        if self._chip_type == "w5500":
-            reg = _REG_RTR_5500
-        else:
-            # Assume a W5100s
-            reg = _REG_RTR_5100s
-        self.write(reg, 0x04, retry_count)
+    def rtr(self, retry_time: int) -> None:
+        """Retry time register."""
+        if 0 > retry_time >= 2**16:
+            raise ValueError("Retry time must be from 0 to 65535")
+        self._write(_REG_RTR[self._chip_type], 0x04, retry_time)
+
+    # *** Chip Specific Methods ***
+
+    def _chip_read(self, device: "busio.SPI", address: int, call_back: int) -> None:
+        """Chip specific calls for _read method."""
+        if self._chip_type in ("w5500", "w6100"):
+            device.write((address >> 8).to_bytes(1, "big"))
+            device.write((address & 0xFF).to_bytes(1, "big"))
+            device.write(call_back.to_bytes(1, "big"))
+        elif self._chip_type == "w5100s":
+            device.write((0x0F).to_bytes(1, "big"))
+            device.write((address >> 8).to_bytes(1, "big"))
+            device.write((address & 0xFF).to_bytes(1, "big"))
+
+    def _chip_write(self, device: "busio.SPI", address: int, call_back: int) -> None:
+        """Chip specific calls for _write."""
+        if self._chip_type in ("w5500", "w6100"):
+            device.write((address >> 8).to_bytes(1, "big"))
+            device.write((address & 0xFF).to_bytes(1, "big"))
+            device.write(call_back.to_bytes(1, "big"))
+        elif self._chip_type == "w5100s":
+            device.write((0xF0).to_bytes(1, "big"))
+            device.write((address >> 8).to_bytes(1, "big"))
+            device.write((address & 0xFF).to_bytes(1, "big"))
+
+    def _chip_socket_read(self, socket_number, pointer, bytes_to_read):
+        """Chip specific calls for socket_read."""
+        if self._chip_type in ("w5500", "w6100"):
+            # Read data from the starting address of snrx_rd
+            ctrl_byte = 0x18 + (socket_number << 5)
+            bytes_read = self._read(pointer, ctrl_byte, bytes_to_read)
+        elif self._chip_type == "w5100s":
+            offset = pointer & _SOCK_MASK
+            src_addr = offset + (socket_number * _SOCK_SIZE + 0x6000)
+            if offset + bytes_to_read > _SOCK_SIZE:
+                split_point = _SOCK_SIZE - offset
+                bytes_read = self._read(src_addr, 0x00, split_point)
+                split_point = bytes_to_read - split_point
+                src_addr = socket_number * _SOCK_SIZE + 0x6000
+                bytes_read += self._read(src_addr, 0x00, split_point)
+            else:
+                bytes_read = self._read(src_addr, 0x00, bytes_to_read)
+        return bytes_read
 
-    def _ip_address_in_use(self, socknum, local_ip) -> bool:
-        """
-        Send an ARP to the IPv4 address supplied and wait for a response.
+    def _chip_socket_write(
+        self, socket_number: int, offset: int, bytes_to_write: int, buffer: bytes
+    ):
+        """Chip specific calls for socket_write."""
+        if self._chip_type in ("w5500", "w6100"):
+            dst_addr = offset + (socket_number * _SOCK_SIZE + 0x8000)
+            cntl_byte = 0x14 + (socket_number << 5)
+            self._write(dst_addr, cntl_byte, buffer[:bytes_to_write])
+
+        elif self._chip_type == "w5100s":
+            dst_addr = offset + (socket_number * _SOCK_SIZE + 0x4000)
+
+            if offset + bytes_to_write > _SOCK_SIZE:
+                split_point = _SOCK_SIZE - offset
+                self._write(dst_addr, 0x00, buffer[:split_point])
+                dst_addr = socket_number * _SOCK_SIZE + 0x4000
+                self._write(dst_addr, 0x00, buffer[split_point:bytes_to_write])
+            else:
+                self._write(dst_addr, 0x00, buffer[:bytes_to_write])
 
-        A helper function for the DHCP client to confirm that the offered IP address is
-        not in use before setting up the DHCP parameters. May also be called by the user
-        before setting a manual IP address, to make sure that it is not already in use.
+    def _chip_parse_udp_header(self, socket_num) -> int:
+        """
+        Parse chip specific UDP header data for IPv4 packets.
 
-        According to RFC5227 section 2.1.1 of , we check for ARP Probe or ARPResponse
-        reception from other devices for 1 second after sending ARPProbe. If there is no
-        reception for 1 second, the probe is repeated three times in total, and if there
-        is no reception, it is determined that there is no conflict.
+        Sets the source IPv4 address and port number and returns the UDP data length.
 
-        :param bytes local_ip: The 4 byte IPv4 address to test for a conflict.
-        :param int socknum: The socket to test.
+        :return int: The UDP data length.
+        """
+        if self._chip_type in ("w5100s", "w5500"):
+            self.udp_from_ip[socket_num] = self._pbuff[:4]
+            self.udp_from_port[socket_num] = int.from_bytes(self._pbuff[4:6], "big")
+            return int.from_bytes(self._pbuff[6:], "big")
+        if self._chip_type == "w6100":
+            self.udp_from_ip[socket_num] = self._pbuff[3:7]
+            self.udp_from_port[socket_num] = int.from_bytes(self._pbuff[6:], "big")
+            return int.from_bytes(self._pbuff[:2], "big") & 0x07FF
+        raise ValueError("Unsupported chip type.")
 
-        :returns bool: True if the he address is already in use), False if not.
+    def _write_socket_register(self, sock: int, address: int, data: int) -> None:
+        """Write to a WIZnet 5k socket register."""
+        if self._chip_type in ("w5500", "w6100"):
+            cntl_byte = (sock << 5) + 0x0C
+            self._write(address, cntl_byte, data)
+        elif self._chip_type == "w5100s":
+            cntl_byte = 0
+            self._write(self._ch_base_msb + sock * _CH_SIZE + address, cntl_byte, data)
 
-        :raises RuntimeError: If the Ethernet link is down or could not connect to the socket.
-        """
-        # Check link status
-        if not self.link_status:
-            raise RuntimeError("Ethernet link is down")
-        # Store current RTR, RCR and destination IPv4 address.
-        temp_rcr = self.rcr
-        temp_rtr = self.rtr
-        temp_ip = self._read_sndipr(socknum)
-        # Set current retry timer and retry count to 1 sec and 3 tries to match DHCP standard.
-        self.rcr = 3
-        self.rtr = 100000  # 100us * 10000 = 1 second
-        # Send a dummy packet to the assigned address on the DHCP socket to mimic ARP.
-        ip_in_use = True
-        try:
-            if self.socket_connect(socknum, bytes(local_ip), 5000, conn_mode=0x02) != 1:
-                raise RuntimeError("Unable to connect to socket {}.".format(socknum))
-            self.socket_write(socknum, b"CHECK_IP_CONFLICT")
-        except TimeoutError:
-            ip_in_use = False
-        finally:
-            # Reset the RTR, RCR and destination IPv4 registers.
-            self.write_sndipr(socknum, temp_ip)
-            self.rcr = temp_rcr
-            self.rtr = temp_rtr
-        return ip_in_use
+    def _read_socket_register(self, sock: int, address: int) -> int:
+        """Read a WIZnet 5k socket register."""
+        if self._chip_type in ("w5500", "w6100"):
+            cntl_byte = (sock << 5) + 0x08
+            register = self._read(address, cntl_byte)
+        elif self._chip_type == "w5100s":
+            cntl_byte = 0
+            register = self._read(
+                self._ch_base_msb + sock * _CH_SIZE + address, cntl_byte
+            )
+        return int.from_bytes(register, "big")
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,19 +241,15 @@
             self._wiz_sock = self._eth.get_socket()
             if self._wiz_sock == 0xFF:
                 self._wiz_sock = None
         while time.monotonic() < stop_time:
             self._eth.write_snmr(self._wiz_sock, 0x02)  # Set UDP connection
             self._eth.write_sock_port(self._wiz_sock, 68)  # Set DHCP client port.
             self._eth.write_sncr(self._wiz_sock, 0x01)  # Open the socket.
-            while (
-                self._eth.read_sncr(self._wiz_sock) != b"\x00"
-            ):  # Wait for command to complete.
-                time.sleep(0.001)
-            if self._eth.read_snsr(self._wiz_sock) == b"\x22":
+            if self._eth.read_snsr(self._wiz_sock) == 0x22:
                 self._eth.write_sndport(2, _DHCP_SERVER_PORT)
                 debug_msg("+ Connection OK, port set.", self._debug)
                 return
         self._wiz_sock = None
         raise RuntimeError("Unable to initialize UDP socket.")
 
     def _increment_transaction_id(self) -> None:
@@ -295,38 +291,26 @@
         maximum packet size is limited by the size of the global buffer.
 
         :param float timeout: time.monotonic at which attempt should timeout.
 
         :returns int: The number of bytes stored in the global buffer.
         """
         debug_msg("Receiving a DHCP response.", self._debug)
-        # DHCP returns the query plus additional data. The query length is 236 bytes.
-        minimum_packet_length = 236
-        buffer = bytearray(b"")
-        bytes_read = 0
-        debug_msg("+ Beginning to receive…", self._debug)
-        while bytes_read < minimum_packet_length and time.monotonic() < timeout:
-            if self._eth.socket_available(self._wiz_sock, _SNMR_UDP):
-                x = self._eth.read_udp(self._wiz_sock, _BUFF_LENGTH - bytes_read)[1]
-                buffer.extend(x)
-                bytes_read = len(buffer)
-                debug_msg("+ Bytes read so far {}".format(bytes_read), self._debug)
-                debug_msg(x, self._debug)
-            if bytes_read == _BUFF_LENGTH:
-                break
-        debug_msg("Received {} bytes".format(bytes_read), self._debug)
-        if bytes_read < minimum_packet_length:
-            bytes_read = 0
-        else:
-            _BUFF[:bytes_read] = buffer
-            _BUFF[bytes_read:] = bytearray(_BUFF_LENGTH - bytes_read)
-        del buffer
-        gc.collect()
-        debug_msg(_BUFF[:bytes_read], self._debug)
-        return bytes_read
+        while time.monotonic() < timeout:
+            # DHCP returns the query plus additional data. The query length is 236 bytes.
+            if self._eth.socket_available(self._wiz_sock, _SNMR_UDP) > 236:
+                bytes_count, bytes_read = self._eth.read_udp(
+                    self._wiz_sock, _BUFF_LENGTH
+                )
+                _BUFF[:bytes_count] = bytes_read
+                debug_msg("Received {} bytes".format(bytes_count), self._debug)
+                del bytes_read
+                gc.collect()
+                return bytes_count
+        raise TimeoutError("No DHCP response received.")
 
     def _process_messaging_states(self, *, message_type: int):
         """
         Process a message while the FSM is in SELECTING or REQUESTING state.
 
         Check the message and update the FSM state if it is a valid type.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         _debug_print(debug=self._debug, message="* DNS: Sending request packet...")
         self._iface.socket_write(dns_socket, buffer)
 
         # Read and parse the DNS response
         ipaddress = -1
         for _ in range(5):
             #  wait for a response
-            socket_timeout = time.monotonic() + 1.0
+            socket_timeout = time.monotonic() + 5.0
             while not self._iface.socket_available(dns_socket, 0x02):
                 if time.monotonic() > socket_timeout:
                     _debug_print(
                         debug=self._debug,
                         message="* DNS ERROR: Did not receive DNS response (socket timeout).",
                     )
                     self._iface.socket_close(dns_socket)
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if TYPE_CHECKING:
         from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
 except ImportError:
     pass
 import time
 import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
 
-# __version__ = "2.5.3"
+# __version__ = "3.0.0"
 # __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NTP.git"
 
 
 class NTP:
     """Wiznet5k NTP Client."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,22 +250,22 @@
                 self._socknum, 0xFF
             )  # Reset socket interrupt register.
             _the_interface.socket_disconnect(self._socknum)
             mask = (
                 wiznet5k.adafruit_wiznet5k.SNIR_TIMEOUT
                 | wiznet5k.adafruit_wiznet5k.SNIR_DISCON
             )
-            while not _the_interface.read_snir(self._socknum)[0] & mask:
+            while not _the_interface.read_snir(self._socknum) & mask:
                 pass
         _the_interface.write_snir(
             self._socknum, 0xFF
         )  # Reset socket interrupt register.
         _the_interface.socket_close(self._socknum)
         while (
-            _the_interface.socket_status(self._socknum)[0]
+            _the_interface.socket_status(self._socknum)
             != wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSED
         ):
             pass
 
     # This works around problems with using a class method as a decorator.
     def _check_socket_closed(func):  # pylint: disable=no-self-argument
         """Decorator to check whether the socket object has been closed."""
@@ -280,28 +280,28 @@
     @property
     def _status(self) -> int:
         """
         Return the status of the socket.
 
         :return int: Status of the socket.
         """
-        return _the_interface.socket_status(self._socknum)[0]
+        return _the_interface.socket_status(self._socknum)
 
     @property
     def _connected(self) -> bool:
         """
         Return whether connected to the socket.
 
         :return bool: Whether connected.
         """
         # pylint: disable=protected-access
 
         if self._socknum >= _the_interface.max_sockets:
             return False
-        status = _the_interface.socket_status(self._socknum)[0]
+        status = _the_interface.socket_status(self._socknum)
         if (
             status == wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSE_WAIT
             and self._available() == 0
         ):
             result = False
         else:
             result = status not in (
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/docs/_static/favicon.ico` & `adafruit-circuitpython-wiznet5k-3.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/docs/api.rst` & `adafruit-circuitpython-wiznet5k-3.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/docs/conf.py` & `adafruit-circuitpython-wiznet5k-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/docs/index.rst` & `adafruit-circuitpython-wiznet5k-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_aio_post.py` & `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_cheerlights.py` & `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpleserver.py` & `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpletest.py` & `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpletest_manual_network.py` & `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.3/pyproject.toml` & `adafruit-circuitpython-wiznet5k-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "2.5.3"
+version = "3.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

