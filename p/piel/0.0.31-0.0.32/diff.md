# Comparing `tmp/piel-0.0.31.tar.gz` & `tmp/piel-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.31.tar", last modified: Sun Jun 25 21:54:53 2023, max compression
+gzip compressed data, was "piel-0.0.32.tar", last modified: Tue Jun 27 21:04:44 2023, max compression
```

## Comparing `piel-0.0.31.tar` & `piel-0.0.32.tar`

### file list

```diff
@@ -1,113 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.467561 piel-0.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-25 21:54:32.000000 piel-0.0.31/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-25 21:54:32.000000 piel-0.0.31/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-25 21:54:32.000000 piel-0.0.31/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-25 21:54:32.000000 piel-0.0.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-25 21:54:32.000000 piel-0.0.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-25 21:54:53.467561 piel-0.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-25 21:54:32.000000 piel-0.0.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-25 21:54:32.000000 piel-0.0.31/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-25 21:54:32.000000 piel-0.0.31/docs/authors.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/autoapi/piel/cocotb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/autoapi/piel/cocotb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/cocotb/core/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/file_system/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26266 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.455561 piel-0.0.31/docs/autoapi/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/integration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/integration/openlane_gdsfactory_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/integration/sax_cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/integration/sax_cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/migrate/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/parse/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/parse/run_output/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/parse/run_output/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/parse/sta_rpt/
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/parse/sta_rpt/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/parse/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/parse/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/openlane/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/openlane/v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/autoapi/piel/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-25 21:54:32.000000 piel-0.0.31/docs/autoapi/piel/piel/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-25 21:54:32.000000 piel-0.0.31/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 21:54:32.000000 piel-0.0.31/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.451561 piel-0.0.31/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.451561 piel-0.0.31/docs/examples/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/examples/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-25 21:54:32.000000 piel-0.0.31/docs/examples/simple_design/tb/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/examples/simple_design/tb/default/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-25 21:54:32.000000 piel-0.0.31/docs/examples/simple_design/tb/default/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-25 21:54:32.000000 piel-0.0.31/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-25 21:54:32.000000 piel-0.0.31/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-25 21:54:32.000000 piel-0.0.31/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-25 21:54:32.000000 piel-0.0.31/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 21:54:32.000000 piel-0.0.31/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.451561 piel-0.0.31/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/sections/about/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-25 21:54:32.000000 piel-0.0.31/docs/sections/about/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/sections/codesign/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-25 21:54:32.000000 piel-0.0.31/docs/sections/codesign/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-25 21:54:32.000000 piel-0.0.31/docs/sections/environment/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.459561 piel-0.0.31/docs/sections/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-25 21:54:32.000000 piel-0.0.31/docs/sections/integration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.463561 piel-0.0.31/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-25 21:54:32.000000 piel-0.0.31/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-25 21:54:32.000000 piel-0.0.31/piel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.463561 piel-0.0.31/piel/cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 21:54:32.000000 piel-0.0.31/piel/cocotb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-06-25 21:54:32.000000 piel-0.0.31/piel/cocotb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-25 21:54:32.000000 piel-0.0.31/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-25 21:54:32.000000 piel-0.0.31/piel/file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.463561 piel-0.0.31/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 21:54:32.000000 piel-0.0.31/piel/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-25 21:54:32.000000 piel-0.0.31/piel/integration/openlane_gdsfactory_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:32.000000 piel-0.0.31/piel/integration/sax_cocotb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.467561 piel-0.0.31/piel/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.467561 piel-0.0.31/piel/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/parse/run_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/parse/sta_rpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-25 21:54:32.000000 piel-0.0.31/piel/openlane/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-25 21:54:32.000000 piel-0.0.31/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 21:54:32.000000 piel-0.0.31/piel/piel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.463561 piel-0.0.31/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-25 21:54:53.000000 piel-0.0.31/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-25 21:54:53.000000 piel-0.0.31/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:54:53.000000 piel-0.0.31/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-25 21:54:53.000000 piel-0.0.31/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:54:53.000000 piel-0.0.31/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-25 21:54:53.000000 piel-0.0.31/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 21:54:53.000000 piel-0.0.31/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-25 21:54:53.467561 piel-0.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-25 21:54:32.000000 piel-0.0.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:53.467561 piel-0.0.31/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 21:54:32.000000 piel-0.0.31/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-25 21:54:32.000000 piel-0.0.31/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-27 21:04:28.000000 piel-0.0.32/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 21:04:28.000000 piel-0.0.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 21:04:28.000000 piel-0.0.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-27 21:04:44.256233 piel-0.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-27 21:04:28.000000 piel-0.0.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-27 21:04:28.000000 piel-0.0.32/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 21:04:28.000000 piel-0.0.32/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/cocotb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/cocotb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/cocotb/core/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/config/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/file_system/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/integration/openlane_gdsfactory_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/integration/sax_cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/integration/sax_cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/models/frequency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.240233 piel-0.0.32/docs/autoapi/piel/models/frequency/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/logic/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/logic/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/logic/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/logic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/logic/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/logic/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/electrical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/electrical/cable/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/electrical/cable/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/geometry/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/thermal/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/physical/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/physical/units/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/transient/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/transient/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/transient/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/transient/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/transient/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/transient/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/transient/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/models/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/openlane/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/migrate/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.244233 piel-0.0.32/docs/autoapi/piel/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/parse/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/openlane/parse/run_output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/parse/run_output/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/openlane/parse/sta_rpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/parse/sta_rpt/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/openlane/parse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/parse/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/openlane/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/openlane/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/openlane/v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/autoapi/piel/project_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-27 21:04:28.000000 piel-0.0.32/docs/autoapi/piel/project_structure/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-27 21:04:28.000000 piel-0.0.32/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 21:04:28.000000 piel-0.0.32/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.236233 piel-0.0.32/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.236233 piel-0.0.32/docs/examples/designs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.236233 piel-0.0.32/docs/examples/designs/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.236233 piel-0.0.32/docs/examples/designs/simple_design/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/examples/designs/simple_design/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-27 21:04:28.000000 piel-0.0.32/docs/examples/designs/simple_design/simple_design/tb/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/examples/designs/simple_design/simple_design/tb/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-27 21:04:28.000000 piel-0.0.32/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 21:04:28.000000 piel-0.0.32/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 21:04:28.000000 piel-0.0.32/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-27 21:04:28.000000 piel-0.0.32/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-27 21:04:28.000000 piel-0.0.32/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 21:04:28.000000 piel-0.0.32/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.236233 piel-0.0.32/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/sections/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-27 21:04:28.000000 piel-0.0.32/docs/sections/about/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-27 21:04:28.000000 piel-0.0.32/docs/sections/about/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/sections/codesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-27 21:04:28.000000 piel-0.0.32/docs/sections/codesign/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/sections/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 21:04:28.000000 piel-0.0.32/docs/sections/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 21:04:28.000000 piel-0.0.32/docs/sections/environment/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/sections/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-27 21:04:28.000000 piel-0.0.32/docs/sections/integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/docs/sections/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 21:04:28.000000 piel-0.0.32/docs/sections/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-27 21:04:28.000000 piel-0.0.32/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-27 21:04:28.000000 piel-0.0.32/piel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/piel/cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 21:04:28.000000 piel-0.0.32/piel/cocotb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-06-27 21:04:28.000000 piel-0.0.32/piel/cocotb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-27 21:04:28.000000 piel-0.0.32/piel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-27 21:04:28.000000 piel-0.0.32/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-27 21:04:28.000000 piel-0.0.32/piel/file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 21:04:28.000000 piel-0.0.32/piel/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-27 21:04:28.000000 piel-0.0.32/piel/integration/openlane_gdsfactory_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/integration/sax_cocotb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/frequency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/frequency/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/frequency/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/directional_coupler_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/directional_coupler_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/directional_coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/grating_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/mmi1x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/mmi2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/frequency/photonic/straight_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/logic/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/logic/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/logic/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/logic/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/logic/photonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/physical/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/physical/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/electrical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/electrical/cable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/physical/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/electronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/physical/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.252233 piel-0.0.32/piel/models/transient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/transient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/transient/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/transient/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/transient/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/transient/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/transient/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:28.000000 piel-0.0.32/piel/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/piel/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/piel/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/parse/run_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/parse/sta_rpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-27 21:04:28.000000 piel-0.0.32/piel/openlane/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-27 21:04:28.000000 piel-0.0.32/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-27 21:04:28.000000 piel-0.0.32/piel/project_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.248233 piel-0.0.32/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-27 21:04:44.000000 piel-0.0.32/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-27 21:04:44.000000 piel-0.0.32/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:04:44.000000 piel-0.0.32/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 21:04:44.000000 piel-0.0.32/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:04:44.000000 piel-0.0.32/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-27 21:04:44.000000 piel-0.0.32/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 21:04:44.000000 piel-0.0.32/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-27 21:04:44.256233 piel-0.0.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-27 21:04:28.000000 piel-0.0.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:04:44.256233 piel-0.0.32/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 21:04:28.000000 piel-0.0.32/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-27 21:04:28.000000 piel-0.0.32/tests/test_piel.py
```

### Comparing `piel-0.0.31/CONTRIBUTING.rst` & `piel-0.0.32/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/LICENSE` & `piel-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/PKG-INFO` & `piel-0.0.32/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.31
+Version: 0.0.32
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
-License-File: AUTHORS.rst
 
 # `piel` - Photonic and Integrated ELectronic tools
 [![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
 [![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
 [![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
 [![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
 
@@ -32,29 +31,22 @@
 - Free software: MIT license
 - Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
 
 ## Target functionality
 * Co-simulation and optimisation between integrated photonic and electronic chip design.
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
+* Multi-domain electronics and photonics component models
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
 ## Dependency Toolset
 This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some individual tools already integrated are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 
-Coming next GDSFactory netlisting and layout integration.
-
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
-
-## Credits
-This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
-
-- Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
-- `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `piel-0.0.31/README.md` & `piel-0.0.32/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,22 @@
 - Free software: MIT license
 - Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
 
 ## Target functionality
 * Co-simulation and optimisation between integrated photonic and electronic chip design.
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
+* Multi-domain electronics and photonics component models
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
 ## Dependency Toolset
 This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some individual tools already integrated are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 
-Coming next GDSFactory netlisting and layout integration.
-
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
-
-## Credits
-This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
-
-- Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
-- `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `piel-0.0.31/docs/Makefile` & `piel-0.0.32/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/autoapi/piel/cocotb/core/index.rst` & `piel-0.0.32/docs/autoapi/piel/cocotb/core/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 
 
 Attributes
 ~~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.cocotb.core.write_cocotb_makefile
-   piel.cocotb.core.make_cocotb
+   piel.cocotb.core.delete_simulation_output_files
 
 
 .. py:function:: check_cocotb_testbench_exists(design_directory: str | pathlib.Path) -> bool
 
    Checks if a cocotb testbench exists in the design directory.
 
    :param design_directory: Design directory.
@@ -51,28 +50,34 @@
 
 .. py:function:: configure_cocotb_simulation(design_directory: str | pathlib.Path, simulator: Literal[icarus, verilator], top_level_language: Literal[verilog, vhdl], top_level_verilog_module: str, test_python_module: str, design_sources_list: list | None = None)
 
    Writes a cocotb makefile.
 
    If no design_sources_list is provided then it adds all the design sources under the `src` folder.
 
-   In the form::
-       Makefile
+   In the form
+   .. code-block::
+
+       #!/bin/sh
+       # Makefile
        # defaults
        SIM ?= icarus
        TOPLEVEL_LANG ?= verilog
 
+       # Note we need to include the test script to the PYTHONPATH
+       export PYTHONPATH =
+
        VERILOG_SOURCES += $(PWD)/my_design.sv
        # use VHDL_SOURCES for VHDL files
 
        # TOPLEVEL is the name of the toplevel module in your Verilog or VHDL file
-       TOPLEVEL = my_design
+       TOPLEVEL := my_design
 
        # MODULE is the basename of the Python test file
-       MODULE = test_my_design
+       MODULE := test_my_design
 
        # include cocotb's make rules to take care of the simulator setup
        include $(shell cocotb-config --makefiles)/Makefile.sim
 
 
    :param design_directory: The directory where the design is located.
    :type design_directory: str | pathlib.Path
@@ -86,24 +91,23 @@
    :type test_python_module: str
    :param design_sources_list: A list of design sources. Defaults to None.
    :type design_sources_list: list | None, optional
 
    :returns: None
 
 
+.. py:data:: delete_simulation_output_files
+
+
+
 .. py:function:: run_cocotb_simulation(design_directory: str) -> subprocess.CompletedProcess
 
-   Equivalent to running the cocotb makefile::
+   Equivalent to running the cocotb makefile
+   .. code-block::
+
        make
 
    :param design_directory: The directory where the design is located.
    :type design_directory: str
 
    :returns: The subprocess.CompletedProcess object.
    :rtype: subprocess.CompletedProcess
-
-
-.. py:data:: write_cocotb_makefile
-
-
-
-.. py:data:: make_cocotb
```

### Comparing `piel-0.0.31/docs/autoapi/piel/cocotb/index.rst` & `piel-0.0.32/docs/autoapi/piel/cocotb/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 
 
 Attributes
 ~~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.cocotb.make_cocotb
-   piel.cocotb.write_cocotb_makefile
+   piel.cocotb.delete_simulation_output_files
 
 
 .. py:function:: check_cocotb_testbench_exists(design_directory: str | pathlib.Path) -> bool
 
    Checks if a cocotb testbench exists in the design directory.
 
    :param design_directory: Design directory.
@@ -50,28 +49,34 @@
 
 .. py:function:: configure_cocotb_simulation(design_directory: str | pathlib.Path, simulator: Literal[icarus, verilator], top_level_language: Literal[verilog, vhdl], top_level_verilog_module: str, test_python_module: str, design_sources_list: list | None = None)
 
    Writes a cocotb makefile.
 
    If no design_sources_list is provided then it adds all the design sources under the `src` folder.
 
-   In the form::
-       Makefile
+   In the form
+   .. code-block::
+
+       #!/bin/sh
+       # Makefile
        # defaults
        SIM ?= icarus
        TOPLEVEL_LANG ?= verilog
 
+       # Note we need to include the test script to the PYTHONPATH
+       export PYTHONPATH =
+
        VERILOG_SOURCES += $(PWD)/my_design.sv
        # use VHDL_SOURCES for VHDL files
 
        # TOPLEVEL is the name of the toplevel module in your Verilog or VHDL file
-       TOPLEVEL = my_design
+       TOPLEVEL := my_design
 
        # MODULE is the basename of the Python test file
-       MODULE = test_my_design
+       MODULE := test_my_design
 
        # include cocotb's make rules to take care of the simulator setup
        include $(shell cocotb-config --makefiles)/Makefile.sim
 
 
    :param design_directory: The directory where the design is located.
    :type design_directory: str | pathlib.Path
@@ -85,24 +90,23 @@
    :type test_python_module: str
    :param design_sources_list: A list of design sources. Defaults to None.
    :type design_sources_list: list | None, optional
 
    :returns: None
 
 
-.. py:data:: make_cocotb
+.. py:data:: delete_simulation_output_files
 
 
 
 .. py:function:: run_cocotb_simulation(design_directory: str) -> subprocess.CompletedProcess
 
-   Equivalent to running the cocotb makefile::
+   Equivalent to running the cocotb makefile
+   .. code-block::
+
        make
 
    :param design_directory: The directory where the design is located.
    :type design_directory: str
 
    :returns: The subprocess.CompletedProcess object.
    :rtype: subprocess.CompletedProcess
-
-
-.. py:data:: write_cocotb_makefile
```

### Comparing `piel-0.0.31/docs/autoapi/piel/index.rst` & `piel-0.0.32/docs/autoapi/piel/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,32 @@
 Subpackages
 -----------
 .. toctree::
    :titlesonly:
    :maxdepth: 3
 
    cocotb/index.rst
+   components/index.rst
    integration/index.rst
+   models/index.rst
    openlane/index.rst
 
 
 Submodules
 ----------
 .. toctree::
    :titlesonly:
    :maxdepth: 1
 
    cli/index.rst
+   config/index.rst
    defaults/index.rst
    file_system/index.rst
    parametric/index.rst
-   piel/index.rst
+   project_structure/index.rst
 
 
 Package Contents
 ----------------
 
 
 Functions
@@ -44,16 +47,22 @@
 
    piel.check_cocotb_testbench_exists
    piel.configure_cocotb_simulation
    piel.run_cocotb_simulation
    piel.check_path_exists
    piel.check_example_design
    piel.copy_source_folder
+   piel.create_new_directory
+   piel.delete_path
+   piel.delete_path_list_in_directory
+   piel.get_files_recursively_in_directory
+   piel.permit_directory_all
    piel.permit_script_execution
    piel.setup_example_design
+   piel.read_json
    piel.return_path
    piel.run_script
    piel.write_script
    piel.create_gdsfactory_component_from_openlane
    piel.get_design_directory_from_root_openlane_v1
    piel.return_path
    piel.get_design_from_openlane_migration
@@ -71,40 +80,42 @@
    piel.filter_timing_sta_files
    piel.filter_power_sta_files
    piel.get_all_timing_sta_files
    piel.get_all_power_sta_files
    piel.contains_in_lines
    piel.read_file_lines
    piel.get_file_line_by_keyword
+   piel.create_file_lines_dataframe
    piel.calculate_max_frame_amount
    piel.calculate_propagation_delay_from_timing_data
    piel.calculate_propagation_delay_from_file
    piel.configure_timing_data_rows
    piel.configure_frame_id
    piel.filter_timing_data_by_net_name_and_type
    piel.get_frame_meta_data
+   piel.get_frame_lines_data
    piel.get_frame_timing_data
    piel.get_all_timing_data_from_file
    piel.read_sta_rpt_fwf_file
    piel.check_path_exists
-   piel.create_dataframe
    piel.read_file
    piel.run_openlane_flow
    piel.single_parameter_sweep
    piel.multi_parameter_sweep
 
 
 
 Attributes
 ~~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.make_cocotb
-   piel.write_cocotb_makefile
+   piel.delete_simulation_output_files
+   piel.numerical_solver
+   piel.nso
    piel.test_spm_open_lane_configuration
    piel.example_open_lane_configuration
    piel.__author__
    piel.__email__
    piel.__version__
 
 
@@ -121,28 +132,34 @@
 
 .. py:function:: configure_cocotb_simulation(design_directory: str | pathlib.Path, simulator: Literal[icarus, verilator], top_level_language: Literal[verilog, vhdl], top_level_verilog_module: str, test_python_module: str, design_sources_list: list | None = None)
 
    Writes a cocotb makefile.
 
    If no design_sources_list is provided then it adds all the design sources under the `src` folder.
 
-   In the form::
-       Makefile
+   In the form
+   .. code-block::
+
+       #!/bin/sh
+       # Makefile
        # defaults
        SIM ?= icarus
        TOPLEVEL_LANG ?= verilog
 
+       # Note we need to include the test script to the PYTHONPATH
+       export PYTHONPATH =
+
        VERILOG_SOURCES += $(PWD)/my_design.sv
        # use VHDL_SOURCES for VHDL files
 
        # TOPLEVEL is the name of the toplevel module in your Verilog or VHDL file
-       TOPLEVEL = my_design
+       TOPLEVEL := my_design
 
        # MODULE is the basename of the Python test file
-       MODULE = test_my_design
+       MODULE := test_my_design
 
        # include cocotb's make rules to take care of the simulator setup
        include $(shell cocotb-config --makefiles)/Makefile.sim
 
 
    :param design_directory: The directory where the design is located.
    :type design_directory: str | pathlib.Path
@@ -156,31 +173,37 @@
    :type test_python_module: str
    :param design_sources_list: A list of design sources. Defaults to None.
    :type design_sources_list: list | None, optional
 
    :returns: None
 
 
-.. py:data:: make_cocotb
+.. py:data:: delete_simulation_output_files
 
 
 
 .. py:function:: run_cocotb_simulation(design_directory: str) -> subprocess.CompletedProcess
 
-   Equivalent to running the cocotb makefile::
+   Equivalent to running the cocotb makefile
+   .. code-block::
+
        make
 
    :param design_directory: The directory where the design is located.
    :type design_directory: str
 
    :returns: The subprocess.CompletedProcess object.
    :rtype: subprocess.CompletedProcess
 
 
-.. py:data:: write_cocotb_makefile
+.. py:data:: numerical_solver
+
+
+
+.. py:data:: nso
 
 
 
 .. py:data:: test_spm_open_lane_configuration
 
 
 
@@ -217,14 +240,75 @@
    :type source_directory: str
    :param target_directory: Target directory.
    :type target_directory: str
 
    :returns: None
 
 
+.. py:function:: create_new_directory(directory_path: str | pathlib.Path) -> None
+
+   Creates a new directory.
+
+   If the parents of the target_directory do not exist, they will be created too.
+
+   :param directory_path: Input path.
+   :type directory_path: str | pathlib.Path
+
+   :returns: None
+
+
+.. py:function:: delete_path(path: str | pathlib.Path) -> None
+
+   Deletes a path.
+
+   :param path: Input path.
+   :type path: str | pathlib.Path
+
+   :returns: None
+
+
+.. py:function:: delete_path_list_in_directory(directory_path: str | pathlib.Path, path_list: list, ignore_confirmation: bool = False, validate_individual: bool = False) -> None
+
+   Deletes a list of files in a directory.
+
+   :param directory_path: Input path.
+   :type directory_path: str | pathlib.Path
+   :param path_list: List of files.
+   :type path_list: list
+   :param ignore_confirmation: Ignore confirmation. Default: False.
+   :type ignore_confirmation: bool
+   :param validate_individual: Validate individual files. Default: False.
+   :type validate_individual: bool
+
+   :returns: None
+
+
+.. py:function:: get_files_recursively_in_directory(path: str | pathlib.Path, extension: str = '*')
+
+   Returns a list of files in a directory.
+
+   :param path: Input path.
+   :type path: str | pathlib.Path
+   :param extension: File extension.
+   :type extension: str
+
+   :returns: List of files.
+   :rtype: file_list(list)
+
+
+.. py:function:: permit_directory_all(directory_path: str | pathlib.Path) -> None
+
+   Permits a directory to be read, written and executed. Use with care as it can be a source for security issues.
+
+   :param directory_path: Input path.
+   :type directory_path: str | pathlib.Path
+
+   :returns: None
+
+
 .. py:function:: permit_script_execution(script_path: str | pathlib.Path) -> None
 
    Permits the execution of a script.
 
    :param script_path: Script path.
    :type script_path: str
 
@@ -239,14 +323,25 @@
    :type project_source: str
    :param example_name: Name of the example design.
    :type example_name: str
 
    :returns: None
 
 
+.. py:function:: read_json(path: str | pathlib.Path) -> dict
+
+   Reads a JSON file.
+
+   :param path: Input path.
+   :type path: str | pathlib.Path
+
+   :returns: JSON data.
+   :rtype: json_data(dict)
+
+
 .. py:function:: return_path(input_path: str | pathlib.Path) -> pathlib.Path
 
    Returns a pathlib.Path to be able to perform operations accordingly internally.
 
    This allows us to maintain compatibility between POSIX and Windows systems.
 
    :param input_path: Input path.
@@ -529,19 +624,20 @@
    :param keyword: Keyword to search for
    :type keyword: str
 
    :returns: Dataframe containing the file lines
    :rtype: file_lines_data (pd.DataFrame)
 
 
-.. py:function:: read_file_lines(file)
+.. py:function:: read_file_lines(file_path: str | pathlib.Path)
 
    Extract lines from the file
 
-   :param file: the opened file
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: list containing the file lines
    :rtype: file_lines_raw (list)
 
 
 .. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
 
@@ -554,14 +650,25 @@
    :param regex: Regex to extract the data
    :type regex: str
 
    :returns: Dataframe containing the extracted values
    :rtype: extracted_values (pd.DataFrame)
 
 
+.. py:function:: create_file_lines_dataframe(file_lines_raw)
+
+   Create a DataFrame from the raw lines of a file
+
+   :param file_lines_raw: list containing the file lines
+   :type file_lines_raw: list
+
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
 .. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
    Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
 
@@ -580,20 +687,20 @@
    :param timing_data: Dataframe containing the timing data
    :type timing_data: pd.DataFrame
 
    :returns: Dataframe containing the propagation delay
    :rtype: propagation_delay_dataframe (pd.DataFrame)
 
 
-.. py:function:: calculate_propagation_delay_from_file(file: str | pathlib.Path)
+.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
 
    Calculate the propagation delay for each frame in the file
 
-   :param file: Path to the file
-   :type file: str | pathlib.Path
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: Dictionary containing the propagation delay
    :rtype: propagation_delay (dict)
 
 
 .. py:function:: configure_timing_data_rows(file_lines_data: pandas.DataFrame)
 
@@ -642,14 +749,25 @@
    :returns: DataFrame containing the start point name
              end_point_name (pd.DataFrame): DataFrame containing the end point name
              path_group_name (pd.DataFrame): DataFrame containing the path group name
              path_type_name (pd.DataFrame): DataFrame containing the path type name
    :rtype: start_point_name (pd.DataFrame)
 
 
+.. py:function:: get_frame_lines_data(file_path: str | pathlib.Path)
+
+   Calculate the timing data for each frame in the file
+
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
+
+   :returns: DataFrame containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
 .. py:function:: get_frame_timing_data(file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0)
 
    Extract the timing data from the file
 
    :param file: Address of the file
    :type file: str | pathlib.Path
    :param frame_meta_data: Dictionary containing the frame metadata
@@ -657,20 +775,20 @@
    :param frame_id: Frame ID to be read
    :type frame_id: int
 
    :returns: DataFrame containing the timing data
    :rtype: timing_data (pd.DataFrame)
 
 
-.. py:function:: get_all_timing_data_from_file(file: str | pathlib.Path)
+.. py:function:: get_all_timing_data_from_file(file_path: str | pathlib.Path)
 
    Calculate the timing data for each frame in the file
 
-   :param file: Path to the file
-   :type file: str | pathlib.Path
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: Dictionary containing the timing data for each frame
    :rtype: frame_timing_data (dict)
 
 
 .. py:function:: read_sta_rpt_fwf_file(file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0)
 
@@ -694,25 +812,14 @@
    :param path: Input path.
    :type path: str | pathlib.Path
 
    :returns: True if directory exists.
    :rtype: directory_exists(bool)
 
 
-.. py:function:: create_dataframe(file_lines_raw)
-
-   Create a DataFrame from the raw lines of a file
-
-   :param file_lines_raw: list containing the file lines
-   :type file_lines_raw: list
-
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
-
-
 .. py:function:: read_file(file_path: str | pathlib.Path)
 
    Read the file from the given path
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
 
@@ -787,8 +894,8 @@
 
 .. py:data:: __email__
    :value: 'darioaquintero@gmail.com'
 
 
 
 .. py:data:: __version__
-   :value: '0.0.30'
+   :value: '0.0.31'
```

### Comparing `piel-0.0.31/docs/autoapi/piel/integration/index.rst` & `piel-0.0.32/docs/autoapi/piel/integration/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst` & `piel-0.0.32/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/autoapi/piel/openlane/index.rst` & `piel-0.0.32/docs/autoapi/piel/openlane/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -53,26 +53,27 @@
    piel.openlane.filter_timing_sta_files
    piel.openlane.filter_power_sta_files
    piel.openlane.get_all_timing_sta_files
    piel.openlane.get_all_power_sta_files
    piel.openlane.contains_in_lines
    piel.openlane.read_file_lines
    piel.openlane.get_file_line_by_keyword
+   piel.openlane.create_file_lines_dataframe
    piel.openlane.calculate_max_frame_amount
    piel.openlane.calculate_propagation_delay_from_timing_data
    piel.openlane.calculate_propagation_delay_from_file
    piel.openlane.configure_timing_data_rows
    piel.openlane.configure_frame_id
    piel.openlane.filter_timing_data_by_net_name_and_type
    piel.openlane.get_frame_meta_data
+   piel.openlane.get_frame_lines_data
    piel.openlane.get_frame_timing_data
    piel.openlane.get_all_timing_data_from_file
    piel.openlane.read_sta_rpt_fwf_file
    piel.openlane.check_path_exists
-   piel.openlane.create_dataframe
    piel.openlane.read_file
    piel.openlane.run_openlane_flow
 
 
 
 .. py:function:: get_design_directory_from_root_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> pathlib.Path
 
@@ -330,19 +331,20 @@
    :param keyword: Keyword to search for
    :type keyword: str
 
    :returns: Dataframe containing the file lines
    :rtype: file_lines_data (pd.DataFrame)
 
 
-.. py:function:: read_file_lines(file)
+.. py:function:: read_file_lines(file_path: str | pathlib.Path)
 
    Extract lines from the file
 
-   :param file: the opened file
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: list containing the file lines
    :rtype: file_lines_raw (list)
 
 
 .. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
 
@@ -355,14 +357,25 @@
    :param regex: Regex to extract the data
    :type regex: str
 
    :returns: Dataframe containing the extracted values
    :rtype: extracted_values (pd.DataFrame)
 
 
+.. py:function:: create_file_lines_dataframe(file_lines_raw)
+
+   Create a DataFrame from the raw lines of a file
+
+   :param file_lines_raw: list containing the file lines
+   :type file_lines_raw: list
+
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
 .. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
    Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
 
@@ -381,20 +394,20 @@
    :param timing_data: Dataframe containing the timing data
    :type timing_data: pd.DataFrame
 
    :returns: Dataframe containing the propagation delay
    :rtype: propagation_delay_dataframe (pd.DataFrame)
 
 
-.. py:function:: calculate_propagation_delay_from_file(file: str | pathlib.Path)
+.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
 
    Calculate the propagation delay for each frame in the file
 
-   :param file: Path to the file
-   :type file: str | pathlib.Path
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: Dictionary containing the propagation delay
    :rtype: propagation_delay (dict)
 
 
 .. py:function:: configure_timing_data_rows(file_lines_data: pandas.DataFrame)
 
@@ -443,14 +456,25 @@
    :returns: DataFrame containing the start point name
              end_point_name (pd.DataFrame): DataFrame containing the end point name
              path_group_name (pd.DataFrame): DataFrame containing the path group name
              path_type_name (pd.DataFrame): DataFrame containing the path type name
    :rtype: start_point_name (pd.DataFrame)
 
 
+.. py:function:: get_frame_lines_data(file_path: str | pathlib.Path)
+
+   Calculate the timing data for each frame in the file
+
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
+
+   :returns: DataFrame containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
 .. py:function:: get_frame_timing_data(file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0)
 
    Extract the timing data from the file
 
    :param file: Address of the file
    :type file: str | pathlib.Path
    :param frame_meta_data: Dictionary containing the frame metadata
@@ -458,20 +482,20 @@
    :param frame_id: Frame ID to be read
    :type frame_id: int
 
    :returns: DataFrame containing the timing data
    :rtype: timing_data (pd.DataFrame)
 
 
-.. py:function:: get_all_timing_data_from_file(file: str | pathlib.Path)
+.. py:function:: get_all_timing_data_from_file(file_path: str | pathlib.Path)
 
    Calculate the timing data for each frame in the file
 
-   :param file: Path to the file
-   :type file: str | pathlib.Path
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: Dictionary containing the timing data for each frame
    :rtype: frame_timing_data (dict)
 
 
 .. py:function:: read_sta_rpt_fwf_file(file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0)
 
@@ -495,25 +519,14 @@
    :param path: Input path.
    :type path: str | pathlib.Path
 
    :returns: True if directory exists.
    :rtype: directory_exists(bool)
 
 
-.. py:function:: create_dataframe(file_lines_raw)
-
-   Create a DataFrame from the raw lines of a file
-
-   :param file_lines_raw: list containing the file lines
-   :type file_lines_raw: list
-
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
-
-
 .. py:function:: read_file(file_path: str | pathlib.Path)
 
    Read the file from the given path
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
```

### Comparing `piel-0.0.31/docs/autoapi/piel/openlane/migrate/index.rst` & `piel-0.0.32/docs/autoapi/piel/openlane/migrate/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/autoapi/piel/openlane/parse/index.rst` & `piel-0.0.32/docs/autoapi/piel/openlane/parse/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -37,28 +37,30 @@
    piel.openlane.parse.filter_power_sta_files
    piel.openlane.parse.get_all_timing_sta_files
    piel.openlane.parse.get_all_power_sta_files
    piel.openlane.parse.return_path
    piel.openlane.parse.contains_in_lines
    piel.openlane.parse.read_file_lines
    piel.openlane.parse.get_file_line_by_keyword
+   piel.openlane.parse.create_file_lines_dataframe
    piel.openlane.parse.calculate_max_frame_amount
    piel.openlane.parse.calculate_propagation_delay_from_timing_data
    piel.openlane.parse.calculate_propagation_delay_from_file
    piel.openlane.parse.configure_timing_data_rows
    piel.openlane.parse.configure_frame_id
    piel.openlane.parse.filter_timing_data_by_net_name_and_type
    piel.openlane.parse.get_frame_meta_data
+   piel.openlane.parse.get_frame_lines_data
    piel.openlane.parse.get_frame_timing_data
    piel.openlane.parse.get_all_timing_data_from_file
    piel.openlane.parse.read_sta_rpt_fwf_file
    piel.openlane.parse.check_path_exists
    piel.openlane.parse.return_path
    piel.openlane.parse.contains_in_lines
-   piel.openlane.parse.create_dataframe
+   piel.openlane.parse.create_file_lines_dataframe
    piel.openlane.parse.get_file_line_by_keyword
    piel.openlane.parse.read_file_lines
    piel.openlane.parse.read_file
 
 
 
 .. py:function:: return_path(input_path: str | pathlib.Path) -> pathlib.Path
@@ -153,19 +155,20 @@
    :param keyword: Keyword to search for
    :type keyword: str
 
    :returns: Dataframe containing the file lines
    :rtype: file_lines_data (pd.DataFrame)
 
 
-.. py:function:: read_file_lines(file)
+.. py:function:: read_file_lines(file_path: str | pathlib.Path)
 
    Extract lines from the file
 
-   :param file: the opened file
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: list containing the file lines
    :rtype: file_lines_raw (list)
 
 
 .. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
 
@@ -178,14 +181,25 @@
    :param regex: Regex to extract the data
    :type regex: str
 
    :returns: Dataframe containing the extracted values
    :rtype: extracted_values (pd.DataFrame)
 
 
+.. py:function:: create_file_lines_dataframe(file_lines_raw)
+
+   Create a DataFrame from the raw lines of a file
+
+   :param file_lines_raw: list containing the file lines
+   :type file_lines_raw: list
+
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
 .. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
    Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
 
@@ -204,20 +218,20 @@
    :param timing_data: Dataframe containing the timing data
    :type timing_data: pd.DataFrame
 
    :returns: Dataframe containing the propagation delay
    :rtype: propagation_delay_dataframe (pd.DataFrame)
 
 
-.. py:function:: calculate_propagation_delay_from_file(file: str | pathlib.Path)
+.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
 
    Calculate the propagation delay for each frame in the file
 
-   :param file: Path to the file
-   :type file: str | pathlib.Path
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: Dictionary containing the propagation delay
    :rtype: propagation_delay (dict)
 
 
 .. py:function:: configure_timing_data_rows(file_lines_data: pandas.DataFrame)
 
@@ -266,14 +280,25 @@
    :returns: DataFrame containing the start point name
              end_point_name (pd.DataFrame): DataFrame containing the end point name
              path_group_name (pd.DataFrame): DataFrame containing the path group name
              path_type_name (pd.DataFrame): DataFrame containing the path type name
    :rtype: start_point_name (pd.DataFrame)
 
 
+.. py:function:: get_frame_lines_data(file_path: str | pathlib.Path)
+
+   Calculate the timing data for each frame in the file
+
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
+
+   :returns: DataFrame containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
 .. py:function:: get_frame_timing_data(file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0)
 
    Extract the timing data from the file
 
    :param file: Address of the file
    :type file: str | pathlib.Path
    :param frame_meta_data: Dictionary containing the frame metadata
@@ -281,20 +306,20 @@
    :param frame_id: Frame ID to be read
    :type frame_id: int
 
    :returns: DataFrame containing the timing data
    :rtype: timing_data (pd.DataFrame)
 
 
-.. py:function:: get_all_timing_data_from_file(file: str | pathlib.Path)
+.. py:function:: get_all_timing_data_from_file(file_path: str | pathlib.Path)
 
    Calculate the timing data for each frame in the file
 
-   :param file: Path to the file
-   :type file: str | pathlib.Path
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: Dictionary containing the timing data for each frame
    :rtype: frame_timing_data (dict)
 
 
 .. py:function:: read_sta_rpt_fwf_file(file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0)
 
@@ -344,15 +369,15 @@
    :param keyword: Keyword to search for
    :type keyword: str
 
    :returns: Dataframe containing the file lines
    :rtype: file_lines_data (pd.DataFrame)
 
 
-.. py:function:: create_dataframe(file_lines_raw)
+.. py:function:: create_file_lines_dataframe(file_lines_raw)
 
    Create a DataFrame from the raw lines of a file
 
    :param file_lines_raw: list containing the file lines
    :type file_lines_raw: list
 
    :returns: Dataframe containing the file lines
@@ -370,19 +395,20 @@
    :param regex: Regex to extract the data
    :type regex: str
 
    :returns: Dataframe containing the extracted values
    :rtype: extracted_values (pd.DataFrame)
 
 
-.. py:function:: read_file_lines(file)
+.. py:function:: read_file_lines(file_path: str | pathlib.Path)
 
    Extract lines from the file
 
-   :param file: the opened file
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: list containing the file lines
    :rtype: file_lines_raw (list)
 
 
 .. py:function:: read_file(file_path: str | pathlib.Path)
```

### Comparing `piel-0.0.31/docs/autoapi/piel/openlane/parse/run_output/index.rst` & `piel-0.0.32/docs/autoapi/piel/openlane/parse/run_output/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/autoapi/piel/openlane/parse/sta_rpt/index.rst` & `piel-0.0.32/docs/autoapi/piel/openlane/parse/sta_rpt/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
    piel.openlane.parse.sta_rpt.calculate_max_frame_amount
    piel.openlane.parse.sta_rpt.calculate_propagation_delay_from_timing_data
    piel.openlane.parse.sta_rpt.calculate_propagation_delay_from_file
    piel.openlane.parse.sta_rpt.configure_timing_data_rows
    piel.openlane.parse.sta_rpt.configure_frame_id
    piel.openlane.parse.sta_rpt.filter_timing_data_by_net_name_and_type
    piel.openlane.parse.sta_rpt.get_frame_meta_data
+   piel.openlane.parse.sta_rpt.get_frame_lines_data
    piel.openlane.parse.sta_rpt.get_frame_timing_data
    piel.openlane.parse.sta_rpt.get_all_timing_data_from_file
    piel.openlane.parse.sta_rpt.read_sta_rpt_fwf_file
 
 
 
 .. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
@@ -48,20 +49,20 @@
    :param timing_data: Dataframe containing the timing data
    :type timing_data: pd.DataFrame
 
    :returns: Dataframe containing the propagation delay
    :rtype: propagation_delay_dataframe (pd.DataFrame)
 
 
-.. py:function:: calculate_propagation_delay_from_file(file: str | pathlib.Path)
+.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
 
    Calculate the propagation delay for each frame in the file
 
-   :param file: Path to the file
-   :type file: str | pathlib.Path
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: Dictionary containing the propagation delay
    :rtype: propagation_delay (dict)
 
 
 .. py:function:: configure_timing_data_rows(file_lines_data: pandas.DataFrame)
 
@@ -110,14 +111,25 @@
    :returns: DataFrame containing the start point name
              end_point_name (pd.DataFrame): DataFrame containing the end point name
              path_group_name (pd.DataFrame): DataFrame containing the path group name
              path_type_name (pd.DataFrame): DataFrame containing the path type name
    :rtype: start_point_name (pd.DataFrame)
 
 
+.. py:function:: get_frame_lines_data(file_path: str | pathlib.Path)
+
+   Calculate the timing data for each frame in the file
+
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
+
+   :returns: DataFrame containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
 .. py:function:: get_frame_timing_data(file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0)
 
    Extract the timing data from the file
 
    :param file: Address of the file
    :type file: str | pathlib.Path
    :param frame_meta_data: Dictionary containing the frame metadata
@@ -125,20 +137,20 @@
    :param frame_id: Frame ID to be read
    :type frame_id: int
 
    :returns: DataFrame containing the timing data
    :rtype: timing_data (pd.DataFrame)
 
 
-.. py:function:: get_all_timing_data_from_file(file: str | pathlib.Path)
+.. py:function:: get_all_timing_data_from_file(file_path: str | pathlib.Path)
 
    Calculate the timing data for each frame in the file
 
-   :param file: Path to the file
-   :type file: str | pathlib.Path
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: Dictionary containing the timing data for each frame
    :rtype: frame_timing_data (dict)
 
 
 .. py:function:: read_sta_rpt_fwf_file(file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0)
```

### Comparing `piel-0.0.31/docs/autoapi/piel/openlane/parse/utils/index.rst` & `piel-0.0.32/docs/autoapi/piel/openlane/parse/utils/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
    piel.openlane.parse.utils.contains_in_lines
-   piel.openlane.parse.utils.create_dataframe
+   piel.openlane.parse.utils.create_file_lines_dataframe
    piel.openlane.parse.utils.get_file_line_by_keyword
    piel.openlane.parse.utils.read_file_lines
    piel.openlane.parse.utils.read_file
 
 
 
 .. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
@@ -30,15 +30,15 @@
    :param keyword: Keyword to search for
    :type keyword: str
 
    :returns: Dataframe containing the file lines
    :rtype: file_lines_data (pd.DataFrame)
 
 
-.. py:function:: create_dataframe(file_lines_raw)
+.. py:function:: create_file_lines_dataframe(file_lines_raw)
 
    Create a DataFrame from the raw lines of a file
 
    :param file_lines_raw: list containing the file lines
    :type file_lines_raw: list
 
    :returns: Dataframe containing the file lines
@@ -56,19 +56,20 @@
    :param regex: Regex to extract the data
    :type regex: str
 
    :returns: Dataframe containing the extracted values
    :rtype: extracted_values (pd.DataFrame)
 
 
-.. py:function:: read_file_lines(file)
+.. py:function:: read_file_lines(file_path: str | pathlib.Path)
 
    Extract lines from the file
 
-   :param file: the opened file
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
    :returns: list containing the file lines
    :rtype: file_lines_raw (list)
 
 
 .. py:function:: read_file(file_path: str | pathlib.Path)
```

### Comparing `piel-0.0.31/docs/autoapi/piel/openlane/v1/index.rst` & `piel-0.0.32/docs/autoapi/piel/openlane/v1/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/autoapi/piel/openlane/v2/index.rst` & `piel-0.0.32/docs/autoapi/piel/openlane/v2/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.32/docs/autoapi/piel/parametric/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/conf.py` & `piel-0.0.32/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 mathjax3_config = {
     "tex": {"tags": "ams", "useLabelIds": True},
 }
 nbsphinx_allow_errors = True  # Continue through Jupyter errors
 nbsphinx_custom_formats = {
     ".py": lambda s: jupytext.reads(s, ".py"),
 }
+nbsphinx_execute = "never"
 version = piel.__version__
 
 latex_elements: dict = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
```

### Comparing `piel-0.0.31/docs/examples/simple_design/tb/default/Makefile` & `piel-0.0.32/docs/examples/designs/simple_design/simple_design/tb/default/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/docs/make.bat` & `piel-0.0.32/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/piel/cocotb/core.py` & `piel-0.0.32/piel/cocotb/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 The objective of this file is to provide the simulation ports and interconnection to consider modelling digital and mixed signal logic.
 
 The main simulation driver is cocotb, and this generates a set of files that correspond to time-domain digital simulations.
 The cocotb verification software can also be used to perform mixed signal simulation, and digital data can be inputted as a bitstream into a photonic solver, although the ideal situation would be to have integrated photonic time-domain models alongside the electronic simulation solver, and maybe this is where it will go. It can be assumed that, as is currently, cocotb can interface python with multiple solvers until someone (and I'd love to do this) writes an equivalent python-based or C++ based python time-domain simulation solver.
 
 The nice thing about cocotb is that as long as the photonic simulations can be written asyncrhonously, time-domain simulations can be closely integrated or simulated through this verification software.
 """
+import functools
 import pathlib
 import subprocess
 from typing import Literal
-from piel.file_system import return_path, write_script
+from piel.file_system import return_path, write_script, delete_path_list_in_directory
 
 
 def check_cocotb_testbench_exists(
     design_directory: str | pathlib.Path,
 ) -> bool:
     """
     Checks if a cocotb testbench exists in the design directory.
@@ -51,28 +52,34 @@
     design_sources_list: list | None = None,
 ):
     """
     Writes a cocotb makefile.
 
     If no design_sources_list is provided then it adds all the design sources under the `src` folder.
 
-    In the form::
-        Makefile
+    In the form
+    .. code-block::
+
+        #!/bin/sh
+        # Makefile
         # defaults
         SIM ?= icarus
         TOPLEVEL_LANG ?= verilog
 
+        # Note we need to include the test script to the PYTHONPATH
+        export PYTHONPATH =
+
         VERILOG_SOURCES += $(PWD)/my_design.sv
         # use VHDL_SOURCES for VHDL files
 
         # TOPLEVEL is the name of the toplevel module in your Verilog or VHDL file
-        TOPLEVEL = my_design
+        TOPLEVEL := my_design
 
         # MODULE is the basename of the Python test file
-        MODULE = test_my_design
+        MODULE := test_my_design
 
         # include cocotb's make rules to take care of the simulator setup
         include $(shell cocotb-config --makefiles)/Makefile.sim
 
 
     Args:
         design_directory (str | pathlib.Path): The directory where the design is located.
@@ -89,15 +96,16 @@
     design_sources_directory = design_directory / "src"
 
     if design_sources_list is not None:
         # Include all the design sources files in a list
         design_sources_list = list(design_sources_directory.iterdir())
 
     top_commands_list = [
-        "Makefile",
+        "#!/bin/bash",
+        "# Makefile",
         "SIM ?= " + simulator,
         "TOPLEVEL_LANG ?= " + top_level_language,
     ]
 
     middle_commands_list = []
     # TODO: Implement mixed source designs.
     if top_level_language == "verilog":
@@ -106,61 +114,64 @@
                 "VERILOG_SOURCES += " + str(source_file.resolve())
             )
     elif top_level_language == "vhdl":
         for source_file in design_sources_list:
             middle_commands_list.append("VHDL_SOURCES += " + str(source_file.resolve()))
 
     bottom_commands_list = [
-        "TOPLEVEL = " + top_level_verilog_module,
-        "MODULE = " + test_python_module,
+        "TOPLEVEL := " + top_level_verilog_module,
+        "MODULE := " + test_python_module,
         "include $(shell cocotb-config --makefiles)/Makefile.sim",
     ]
 
     commands_list = []
     commands_list.extend(top_commands_list)
     commands_list.extend(middle_commands_list)
     commands_list.extend(bottom_commands_list)
 
-    script = ";\n".join(commands_list)
+    script = " \n".join(commands_list)
     write_script(
         directory_path=design_directory / "tb", script=script, script_name="Makefile"
     )
 
 
+delete_simulation_output_files = functools.partial(
+    delete_path_list_in_directory,
+    path_list=["sim_build", "__pycache__", "ivl_vhdl_work"],
+)
+
+
 def run_cocotb_simulation(
     design_directory: str,
 ) -> subprocess.CompletedProcess:
     """
-    Equivalent to running the cocotb makefile::
+    Equivalent to running the cocotb makefile
+    .. code-block::
+
         make
 
     Args:
         design_directory (str): The directory where the design is located.
 
     Returns:
         subprocess.CompletedProcess: The subprocess.CompletedProcess object.
 
     """
     test_directory = return_path(design_directory) / "tb"
-    commands_list = ["cd" + str(test_directory.resolve()), "make"]
-    script = ";\n".join(commands_list)
+    commands_list = ["cd " + str(test_directory.resolve()), "make"]
+    script = "; \n".join(commands_list)
     # Save script if desired to run directly
     write_script(
         directory_path=test_directory,
         script=script,
         script_name="run_cocotb_simulation.sh",
     )
-    run = subprocess.run(script, capture_output=True, shell=True)
+    run = subprocess.run(script, capture_output=True, shell=True, check=True)
     return run
 
 
-write_cocotb_makefile = configure_cocotb_simulation
-make_cocotb = run_cocotb_simulation
-
-
 __all__ = [
     "check_cocotb_testbench_exists",
     "configure_cocotb_simulation",
-    "make_cocotb",
+    "delete_simulation_output_files",
     "run_cocotb_simulation",
-    "write_cocotb_makefile",
 ]
```

### Comparing `piel-0.0.31/piel/defaults.py` & `piel-0.0.32/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/piel/file_system.py` & `piel-0.0.32/piel/file_system.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import glob
+import json
 import openlane
 import os
 import pathlib
 import shutil
 import stat
 import subprocess
 from typing import Literal
@@ -81,14 +82,33 @@
         ignore=None,
         copy_function=shutil.copy2,
         ignore_dangling_symlinks=False,
         dirs_exist_ok=False,
     )
 
 
+def convert_list_to_path_list(
+    input_list: list[str | pathlib.Path],
+) -> list[pathlib.Path]:
+    """
+    Converts a list of strings or pathlib.Path to a list of pathlib.Path.
+
+    Args:
+        input_list(list[str | pathlib.Path]): Input list.
+
+    Returns:
+        output_list(list[pathlib.Path]): Output list.
+    """
+    output_list = []
+    for item in input_list:
+        item = return_path(item)
+        output_list.append(item)
+    return output_list
+
+
 def create_new_directory(
     directory_path: str | pathlib.Path,
 ) -> None:
     """
     Creates a new directory.
 
     If the parents of the target_directory do not exist, they will be created too.
@@ -109,14 +129,80 @@
     if parent_directory_permissions != "0o777":
         permit_directory_all(parent_directory)
 
     # Create the directory
     directory_path.mkdir(parents=True)
 
 
+def delete_path(path: str | pathlib.Path) -> None:
+    """
+    Deletes a path.
+
+    Args:
+        path(str | pathlib.Path): Input path.
+
+    Returns:
+        None
+    """
+    path = return_path(path)
+    if path.exists():
+        if path.is_dir():
+            shutil.rmtree(path)
+        elif path.is_file():
+            path.unlink()
+
+
+def delete_path_list_in_directory(
+    directory_path: str | pathlib.Path,
+    path_list: list,
+    ignore_confirmation: bool = False,
+    validate_individual: bool = False,
+) -> None:
+    """
+    Deletes a list of files in a directory.
+
+    Args:
+        directory_path(str | pathlib.Path): Input path.
+        path_list(list): List of files.
+        ignore_confirmation(bool): Ignore confirmation. Default: False.
+        validate_individual(bool): Validate individual files. Default: False.
+
+    Returns:
+        None
+    """
+    directory_path = return_path(directory_path)
+    path_list = convert_list_to_path_list(path_list)
+    if validate_individual:
+        if ignore_confirmation:
+            for path in path_list:
+                if path.exists():
+                    delete_path(path)
+        else:
+            for path in path_list:
+                if path.exists():
+                    answer = input("Confirm deletion of: " + str(path))
+                    if answer.upper() in ["Y", "YES"]:
+                        delete_path(path)
+                    elif answer.upper() in ["N", "NO"]:
+                        print("Skipping deletion of: " + str(path))
+    else:
+        if ignore_confirmation:
+            for path in path_list:
+                if path.exists():
+                    delete_path(path)
+        else:
+            answer = input("Confirm deletion of: " + str(path_list))
+            if answer.upper() in ["Y", "YES"]:
+                for path in path_list:
+                    if path.exists():
+                        delete_path(path)
+            elif answer.upper() in ["N", "NO"]:
+                print("Skipping deletion of: " + str(path_list))
+
+
 def get_files_recursively_in_directory(
     path: str | pathlib.Path,
     extension: str = "*",
 ):
     """
     Returns a list of files in a directory.
 
@@ -168,14 +254,30 @@
                 "Could not change permissions of directory: "
                 + str(directory_path.resolve())
                 + " to 777. Your Python executable might not have the required permissions. Restructure your project directory so Python does not have to change permissions."
             )
         )
 
 
+def read_json(path: str | pathlib.Path) -> dict:
+    """
+    Reads a JSON file.
+
+    Args:
+        path(str | pathlib.Path): Input path.
+
+    Returns:
+        json_data(dict): JSON data.
+    """
+    path = return_path(path)
+    with open(path, "r") as json_file:
+        json_data = json.load(json_file)
+    return json_data
+
+
 def return_path(input_path: str | pathlib.Path) -> pathlib.Path:
     """
     Returns a pathlib.Path to be able to perform operations accordingly internally.
 
     This allows us to maintain compatibility between POSIX and Windows systems.
 
     Args:
@@ -221,15 +323,17 @@
         example_name(str): Name of the example design.
 
     Returns:
         None
     """
     if project_source == "piel":
         example_design_folder = (
-            os.environ["PIEL_PACKAGE_DIRECTORY"] + "/docs/examples/" + example_name
+            os.environ["PIEL_PACKAGE_DIRECTORY"]
+            + "/docs/examples/designs/"
+            + example_name
         )
     elif project_source == "openlane":
         example_design_folder = (
             pathlib.Path(openlane.__file__).parent.resolve() / example_name
         )
     design_folder = os.environ["DESIGNS"] + "/" + example_name
     copy_source_folder(
@@ -276,13 +380,19 @@
     file.close()
 
 
 __all__ = [
     "check_path_exists",
     "check_example_design",
     "copy_source_folder",
+    "create_new_directory",
+    "delete_path",
+    "delete_path_list_in_directory",
+    "get_files_recursively_in_directory",
+    "permit_directory_all",
     "permit_script_execution",
     "setup_example_design",
+    "read_json",
     "return_path",
     "run_script",
     "write_script",
 ]
```

### Comparing `piel-0.0.31/piel/integration/openlane_gdsfactory_core.py` & `piel-0.0.32/piel/integration/openlane_gdsfactory_core.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/piel/openlane/migrate.py` & `piel-0.0.32/piel/openlane/migrate.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/piel/openlane/parse/run_output.py` & `piel-0.0.32/piel/openlane/parse/run_output.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/piel/openlane/parse/sta_rpt.py` & `piel-0.0.32/piel/openlane/parse/sta_rpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import pandas as pd
 import pathlib
 from ...file_system import return_path
-from .utils import contains_in_lines, read_file_lines, get_file_line_by_keyword
+from .utils import (
+    contains_in_lines,
+    read_file_lines,
+    get_file_line_by_keyword,
+    create_file_lines_dataframe,
+)
 
 
 def calculate_max_frame_amount(
     file_lines_data: pd.DataFrame,
 ):
     """
     Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
     Args:
         file_lines_data (pd.DataFrame): Dataframe containing the file lines
 
     Returns:
         maximum_frame_amount (int): Maximum number of frames in the file
     """
-    return max(file_lines_data["frame_id"].tolist())
+    return max(file_lines_data["frame_id"].tolist()) + 1
 
 
 def calculate_propagation_delay_from_timing_data(
     net_name_in: str,
     net_name_out: str,
     timing_data: pd.DataFrame,
 ):
@@ -60,38 +65,36 @@
         propagation_delay_dataframe["propagation_delay"] = pd.to_numeric(
             output_net_dataframe.iloc[:].Time_out.values
         ) - pd.to_numeric(input_net_dataframe.iloc[:].Time_in.values)
         return propagation_delay_dataframe
 
 
 def calculate_propagation_delay_from_file(
-    file: str | pathlib.Path,
+    file_path: str | pathlib.Path,
 ):
     """
     Calculate the propagation delay for each frame in the file
 
     Args:
-        file (str | pathlib.Path): Path to the file
+        file_path (str | pathlib.Path): Path to the file
 
     Returns:
         propagation_delay (dict): Dictionary containing the propagation delay
     """
-    file = return_path(file)
     # TODO Check file is RPT
-    file_lines_data = read_file_lines(file)
+    file_lines_data = get_frame_lines_data(file_path)
     maximum_frame_amount = calculate_max_frame_amount(file_lines_data)
-
     (
         start_point_name,
         end_point_name,
         path_group_name,
         path_type_name,
     ) = get_frame_meta_data(file_lines_data)
 
-    frame_timing_data = {}
+    frame_timing_data = get_all_timing_data_from_file(file_path)
     propagation_delay = {}
     for frame_id in range(maximum_frame_amount):
         if len(start_point_name.values) > frame_id:
             frame_net_in = start_point_name.values[frame_id][0]
             frame_net_out = end_point_name.values[frame_id][0]
             propagation_delay[frame_id] = calculate_propagation_delay_from_timing_data(
                 frame_net_in, frame_net_out, frame_timing_data[frame_id]
@@ -113,15 +116,15 @@
     """
     frame_meta_data = {}
     maximum_frame_amount = calculate_max_frame_amount(file_lines_data)
     for frame in range(maximum_frame_amount):
         timing_rows_index = file_lines_data.index[
             file_lines_data["timing_data_line"] & (file_lines_data["frame_id"] == frame)
         ].tolist()
-        if len(timing_rows_index) >= 1:
+        if len(timing_rows_index) > 0:
             frame_meta_data[frame] = {
                 "start_index": timing_rows_index[0],
                 "end_index": timing_rows_index[-1],
                 "start_rows_skip": timing_rows_index[0] + 1,
                 "end_rows_skip": len(file_lines_data) - timing_rows_index[-1],
             }
         else:
@@ -220,14 +223,34 @@
     path_type_name = get_file_line_by_keyword(
         file_lines_data, "path_type", r"((?<=Path Type:\s).*)"
     )
 
     return start_point_name, end_point_name, path_group_name, path_type_name
 
 
+def get_frame_lines_data(
+    file_path: str | pathlib.Path,
+):
+    """
+    Calculate the timing data for each frame in the file
+
+    Args:
+        file_path (str | pathlib.Path): Path to the file
+
+    Returns:
+        file_lines_data (pd.DataFrame): DataFrame containing the file lines
+    """
+    file_path = return_path(file_path)
+    # TODO Check file is RPT
+    file_lines = read_file_lines(file_path)
+    file_lines_data = create_file_lines_dataframe(file_lines)
+    file_lines_data = configure_frame_id(file_lines_data)
+    return file_lines_data
+
+
 def get_frame_timing_data(
     file: str | pathlib.Path, frame_meta_data: dict, frame_id: int = 0
 ):
     """
     Extract the timing data from the file
 
     Args:
@@ -242,34 +265,32 @@
     timing_data = read_sta_rpt_fwf_file(file, frame_meta_data, frame_id)
     timing_data["net_type"] = timing_data["Description"].str.extract(r"\(([^()]+)\)")
     timing_data["net_name"] = timing_data["Description"].str.extract(r"(.*?)\s?\(.*?\)")
     return timing_data
 
 
 def get_all_timing_data_from_file(
-    file: str | pathlib.Path,
+    file_path: str | pathlib.Path,
 ):
     """
     Calculate the timing data for each frame in the file
 
     Args:
-        file (str | pathlib.Path): Path to the file
+        file_path (str | pathlib.Path): Path to the file
 
     Returns:
         frame_timing_data (dict): Dictionary containing the timing data for each frame
     """
-    file = return_path(file)
-    # TODO Check file is RPT
-    file_lines_data = read_file_lines(file)
+    file_lines_data = get_frame_lines_data(file_path)
     maximum_frame_amount = calculate_max_frame_amount(file_lines_data)
     frame_meta_data = configure_timing_data_rows(file_lines_data)
     frame_timing_data = {}
     for frame_id in range(maximum_frame_amount):
         frame_timing_data[frame_id] = get_frame_timing_data(
-            file, frame_meta_data, frame_id
+            file_path, frame_meta_data, frame_id
         )
     return frame_timing_data
 
 
 def read_sta_rpt_fwf_file(
     file: str | pathlib.Path,
     frame_meta_data: dict,
```

### Comparing `piel-0.0.31/piel/openlane/parse/utils.py` & `piel-0.0.32/piel/openlane/parse/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Returns:
         file_lines_data (pd.DataFrame): Dataframe containing the file lines
     """
     return file_lines_data.lines.str.contains(keyword)
 
 
-def create_dataframe(file_lines_raw):
+def create_file_lines_dataframe(file_lines_raw):
     """
     Create a DataFrame from the raw lines of a file
 
     Args:
         file_lines_raw (list): list containing the file lines
 
     Returns:
@@ -50,24 +50,26 @@
         extracted_values (pd.DataFrame): Dataframe containing the extracted values
     """
     lines_with_keyword = file_lines_data.lines[file_lines_data[f"{keyword}_line"]]
     extracted_values = lines_with_keyword.str.extract(regex)
     return extracted_values
 
 
-def read_file_lines(file):
+def read_file_lines(file_path: str | pathlib.Path):
     """
     Extract lines from the file
 
     Args:
-        file: the opened file
+        file_path (str | pathlib.Path): Path to the file
 
     Returns:
         file_lines_raw (list): list containing the file lines
     """
+    file_path = return_path(file_path)
+    file = read_file(file_path)
     return file.readlines()
 
 
 def read_file(file_path: str | pathlib.Path):
     """
     Read the file from the given path
```

### Comparing `piel-0.0.31/piel/openlane/utils.py` & `piel-0.0.32/piel/openlane/utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/piel/openlane/v1.py` & `piel-0.0.32/piel/openlane/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import pathlib
 import json
 from ..parametric import multi_parameter_sweep
 from ..file_system import (
     copy_source_folder,
     permit_script_execution,
+    read_json,
     return_path,
     run_script,
     write_script,
 )
 
 
 def check_config_json_exists_openlane_v1(
@@ -282,16 +283,15 @@
         configuration(dict): Configuration dictionary.
     """
     config_json_exists = check_config_json_exists_openlane_v1(design_name)
     if config_json_exists:
         design_directory = get_design_directory_from_root_openlane_v1(
             design_name=design_name, root_directory=root_directory
         )
-        with open(str((design_directory / "config.json").resolve()), "r") as read_file:
-            configuration = json.load(read_file)
+        configuration = read_json(design_directory / "config.json")
         return configuration
     else:
         raise ValueError(
             "Configuration file for design: "
             + design_name
             + " is not found in "
             + str(root_directory / "designs" / design_name)
```

### Comparing `piel-0.0.31/piel/openlane/v2.py` & `piel-0.0.32/piel/openlane/v2.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/piel/parametric.py` & `piel-0.0.32/piel/parametric.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.31/piel.egg-info/PKG-INFO` & `piel-0.0.32/piel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.31
+Version: 0.0.32
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
-License-File: AUTHORS.rst
 
 # `piel` - Photonic and Integrated ELectronic tools
 [![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
 [![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
 [![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
 [![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
 
@@ -32,29 +31,22 @@
 - Free software: MIT license
 - Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
 
 ## Target functionality
 * Co-simulation and optimisation between integrated photonic and electronic chip design.
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
+* Multi-domain electronics and photonics component models
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
 ## Dependency Toolset
 This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some individual tools already integrated are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 
-Coming next GDSFactory netlisting and layout integration.
-
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
-
-## Credits
-This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
-
-- Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
-- `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `piel-0.0.31/setup.py` & `piel-0.0.32/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-with open("HISTORY.rst") as history_file:
-    history = history_file.read()
-
 requirements = [
     "Click>=7.0",
-    "openlane",
     "cocotb",
     "gdsfactory",
+    "openlane",
     "pandas",
+    "sax",
 ]
 
 test_requirements = [
     "pytest>=3",
 ]
 
 setup(
@@ -64,10 +62,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/daquintero/piel",
-    version="0.0.31",
+    version="0.0.32",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.31/tests/test_piel.py` & `piel-0.0.32/tests/test_piel.py`

 * *Files identical despite different names*

