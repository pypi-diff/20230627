# Comparing `tmp/dkist_data_simulator-3.1.6rc1.tar.gz` & `tmp/dkist_data_simulator-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_data_simulator-3.1.6rc1.tar", last modified: Fri May 19 16:01:28 2023, max compression
+gzip compressed data, was "dkist_data_simulator-3.2.0rc1.tar", last modified: Tue Jun 27 17:09:39 2023, max compression
```

## Comparing `dkist_data_simulator-3.1.6rc1.tar` & `dkist_data_simulator-3.2.0rc1.tar`

### file list

```diff
@@ -1,58 +1,55 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.029554 dkist_data_simulator-3.1.6rc1/
--rw-rw-rw-   0 root         (0) root         (0)     3308 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4989 2023-05-19 16:01:28.029554 dkist_data_simulator-3.1.6rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4650 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.025554 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.025554 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/data/
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/data/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    16806 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/dataset.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.025554 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/examples/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/examples/vtf_crisp_5d.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/expansions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10932 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     7180 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec122.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.025554 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26874 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/core.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/cryo.py
--rw-rw-rw-   0 root         (0) root         (0)     3446 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/dlnirsp.py
--rw-rw-rw-   0 root         (0) root         (0)     7627 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/vbi.py
--rw-rw-rw-   0 root         (0) root         (0)     6602 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/visp.py
--rw-rw-rw-   0 root         (0) root         (0)     3585 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/vtf.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.025554 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     8380 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/test_214_inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     5458 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/util.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-19 16:01:27.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.025554 dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4989 2023-05-19 16:01:27.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-05-19 16:01:27.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-19 16:01:27.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-19 16:01:27.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-05-19 16:01:27.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-19 16:01:27.000000 dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.029554 dkist_data_simulator-3.1.6rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.029554 dkist_data_simulator-3.1.6rc1/examples/
--rwxrwxrwx   0 root         (0) root         (0)      908 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/examples/vtf_crisp_5d.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 16:01:28.029554 dkist_data_simulator-3.1.6rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2656 2023-05-19 16:01:28.029554 dkist_data_simulator-3.1.6rc1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      607 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-05-19 16:01:00.000000 dkist_data_simulator-3.1.6rc1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     3308 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.812946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.812946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/data/
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/data/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16824 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10932 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     7180 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec122.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27073 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/cryo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3446 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/dlnirsp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7623 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/vbi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6602 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/visp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3585 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/vtf.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     8380 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     4339 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_214_inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.812946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     4098 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/examples/vtf_crisp_5d.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2634 2023-06-27 17:09:39.820946 dkist_data_simulator-3.2.0rc1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      607 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/tox.ini
```

### Comparing `dkist_data_simulator-3.1.6rc1/.gitignore` & `dkist_data_simulator-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/.pre-commit-config.yaml` & `dkist_data_simulator-3.2.0rc1/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 repos:
+  # This should be before any formatting hooks like isort
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.272"
+    hooks:
+      - id: ruff
+        args: ["--fix"]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.4.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: check-ast
       - id: debug-statements
       - id: check-added-large-files
       - id: check-case-conflict
       - id: trailing-whitespace
         exclude: ".*fits"
       - id: mixed-line-ending
         files: ".*.py"
       - id: end-of-file-fixer
         exclude: ".*fits"
-      - id: flake8
-        additional_dependencies: [flake8-docstrings]
-        args: ['--select', 'E101,W191,W291,W292,W293,W391,E111,E112,E113,E901,E902,F401']
-        exclude: ".*(__init__.py)$"
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies: [toml]
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
 
 ci:
   autofix_prs: false
```

### Comparing `dkist_data_simulator-3.1.6rc1/PKG-INFO` & `dkist_data_simulator-3.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_data_simulator
-Version: 3.1.6rc1
+Version: 3.2.0rc1
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Provides-Extra: all
```

### Comparing `dkist_data_simulator-3.1.6rc1/README.rst` & `dkist_data_simulator-3.2.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/dataset.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,14 @@
 
     def __init__(
         self,
         file_schema: Schema,
         dataset_shape: Tuple[int, ...],
         array_shape: Tuple[int, ...],
     ):
-
         self.random = file_schema.random
 
         self.file_schema = file_schema
         self.dataset_shape = dataset_shape
         self.array_shape = array_shape
 
         self.data_shape = tuple(d for d in array_shape if d != 1)
@@ -198,15 +197,15 @@
             )
 
         self.data_ndim = len(self.data_shape)
         self.array_ndim = len(array_shape)
         self.files_shape = self.dataset_shape[: -1 * self.data_ndim]
         self.files_ndim = len(self.files_shape)
         self.dataset_ndim = len(dataset_shape)
-        self.n_files = int(np.product(self.files_shape))
+        self.n_files = int(np.prod(self.files_shape))
 
         self._index = 0  # The current position in the dataset
         self._remove_keys: List[str] = list()
         self._fixed_keys: Dict[str, Any] = dict()
         self._generator_functions: Dict[str, Callable[[Dataset, str], Any]] = dict()
 
         # Register any generator functions passed in as kwarg
@@ -427,15 +426,17 @@
             image_hdu = fits.ImageHDU(
                 data=self.data, header=fits.Header(self.header(**kwargs))
             )
             return CompImageHDU(
                 data=image_hdu.data, header=image_hdu.header, **rice_compress
             )
 
-        return fits.PrimaryHDU(data=self.data, header=fits.Header(self.header(**kwargs)))
+        return fits.PrimaryHDU(
+            data=self.data, header=fits.Header(self.header(**kwargs))
+        )
 
     def file(
         self,
         target: Union[pathlib.Path, IOBase],
         rice_compress: Optional[Union[bool, dict]] = None,
         checksum: bool = True,
         **kwargs,
```

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/examples/vtf_crisp_5d.py` & `dkist_data_simulator-3.2.0rc1/examples/vtf_crisp_5d.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+#!/bin/env python
 """
-This file generates a 5D VTF-like dataset using observations from the CRISP instrument on the SST.
+Generate a VTF like 214 dataset based on some CRISP data.
+
+To run this example you need the input crisp file which should have one HDU
+with shape (980, 966, 19, 4, 128).
+
+Usage
+-----
+
+vtf_crisp_5d.py <input_filename> <output_directory>
 """
+import sys
+from pathlib import Path
+
 import astropy.units as u
 import numpy as np
 from astropy.io import fits
 from astropy.wcs import WCS
+from dkist_inventory.asdf_generator import dataset_from_fits
 
 from dkist_data_simulator.dataset import key_function
 from dkist_data_simulator.spec214.core import AOMixin, WCSAMixin
 from dkist_data_simulator.spec214.vtf import BaseVTFDataset
 
 
 class VTFCRISP5DDataset(WCSAMixin, AOMixin, BaseVTFDataset):
@@ -103,7 +116,23 @@
     def FRAMEWAV(self, key: str):
         wave_offset = self.framewave_delta * self.file_index[2]
         return (self.framewave_start + wave_offset).to_value(u.nm)
 
     @key_function("STOKES")
     def STOKES(self, key: str):
         return ["I", "Q", "U", "V"][self.file_index[0]]
+
+
+# Modify these with a path if you don't want to run this as a script.
+input_file = Path(sys.argv[1])
+output_dir = Path(sys.argv[2])
+
+# Set n_repeats to a lower number to make a smaller dataset. 5 is a good small value.
+ds = VTFCRISP5DDataset(input_file, n_repeats=5)
+
+ds.generate_files(
+    output_dir,
+    filename_template="{ds.index:05d}.fits",
+    expected_only=False,
+    progress_bar=True,
+)
+dataset_from_fits(output_dir, "vtf_crisp_5d.asdf", relative_to=output_dir)
```

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/expansions.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/schemas.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         type: str = "time",
         format: str = "isot",
     ):
         self.format = format
         super().__init__(key, required, expected, type)
 
     def generate_value(
-        self, start: str = "2019-11-08", stop: str = "2059-11-08"
+        self, start: str = "2019-11-08", stop: str = "2023-11-08"
     ) -> str:
         trange_start = datetime.datetime.fromisoformat(start).timestamp()
         trange_stop = datetime.datetime.fromisoformat(stop).timestamp()
 
         delta = trange_stop - trange_start
 
         rand_delta = self.random.uniform(0, delta)
```

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec122.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/core.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,25 +35,27 @@
         self,
         naxis: int,
         dnaxis: int,
         deaxes: int,
         daaxes: int,
         npropos: int = 1,
         nexpers: int = 1,
+        nspeclns: int = 0,
         instrument=None,
         random=None,
     ):
         random = random or np.random.default_rng()
         sections = spec214.load_expanded_spec214(
             NAXIS=naxis,
             DNAXIS=dnaxis,
             DEAXES=deaxes,
             DAAXES=daaxes,
             NPROPOS=npropos,
             NEXPERS=nexpers,
+            NSPECLNS=nspeclns,
         )
         sections.pop("compression", None)
         if instrument:
             if instrument not in KNOWN_INSTRUMENT_TABLES.keys():
                 raise ValueError(
                     f"{instrument} does not match one of the known "
                     "instrument table names: {tuple(KNOWN_INSTRUMENT_TABLES.keys())}"
@@ -87,26 +89,27 @@
         start_time: datetime.datetime = None,
         instrument: Literal[tuple(KNOWN_INSTRUMENT_TABLES.keys())] = None,
         swnbin: int = 0,
         hwnbin: int = 0,
         swnroi: int = 0,
         hwnroi: int = 0,
     ):
-
+        nspeclns = 3
         # We have to recalculate a bunch of stuff from the super init here to
         # expand the schema before we call the super constructor.
         data_shape = tuple(d for d in array_shape if d != 1)
         super().__init__(
             file_schema=Spec214Schema(
                 naxis=len(array_shape),
                 dnaxis=len(dataset_shape),
                 deaxes=len(dataset_shape) - len(data_shape),
                 daaxes=len(data_shape),
                 npropos=1,
                 nexpers=1,
+                nspeclns=nspeclns,
                 instrument=instrument,
             ),
             dataset_shape=dataset_shape,
             array_shape=array_shape,
         )
 
         self.time_delta = time_delta
@@ -187,15 +190,16 @@
         self.add_constant_key("WKFLVERS", "WORKFLOWVERSION")
         self.add_constant_key("HLSVERS", "HLSVERSION")
         self.add_constant_key("IDSPARID", 1)
         self.add_constant_key("IDSOBSID", 2)
         self.add_constant_key("IDSCALID", 3)
         self.add_constant_key("OBSPR_ID", "OPID")
         self.add_constant_key("IP_ID", "IPID")
-        self.add_constant_key("NSPECLNS", 3)
+        # This has to be passed through to the schema to expand the index
+        self.add_constant_key("NSPECLNS", nspeclns)
         self.add_constant_key("SPECLN01", "Ca II")
         self.add_constant_key("SPECLN02", "H alpha")
         self.add_constant_key("SPECLN03", "Fe I")
         self.add_constant_key("HEADVERS", "HEADERVERSION")
         self.add_constant_key("HEAD_URL", "HEADERURL")
         self.add_constant_key("INFO_URL", "INFOURL")
         self.add_constant_key("CAL_URL", "CALURL")
@@ -492,15 +496,16 @@
     FLTFWHM: This is the HOWFS filter fwhm, 20 nm.
     WFCLOCK: Same as AO___001 above, but here it is on a per-frame basis and there it is for the duration of the data acquisition. Use 0 to represent an anomolous condition, but 1 is the more likely real value.
     MATRIXID: Use any one of the following: 1600Modes, 1417Modes, 1049Modes, 663Modes, 423Modes, 256Modes, 143Modes, 74Modes, 33Modes, 18Modes, 7Modes, 3Modes. The higher number of modes are the more likely conditions. This varies depending on the seeing conditions. Larger r0 values (Fried's poaram) --> more modes that can be corrected.
     AOLOOPP: This can vary from 0 to some positive value, but 7 is a typical value. This can change from frame to frame, but not by much.
     AOLOOPI: Same as above but use 10 for a typical value.
     FRMRATE: This should always be 1970 Hz except in rare cases for engineering purposes
     FRMLOCK: This is similar to WFC__002 above but for the tip-tilt system. Use values as described above. They don't have to be the same as the WFC_002 values.
-    TTLOOPP, TTLOOPI: Similar to 004 and 005 above but use 0.2 and 1 for typical values, respectively."""
+    TTLOOPP, TTLOOPI: Similar to 004 and 005 above but use 0.2 and 1 for typical values, respectively.
+    """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Assume AO is on and Locked
         self.add_constant_key("AO_LOCK", True)
         self.add_constant_key("WFCLOCK", True)
```

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/cryo.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/cryo.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/dlnirsp.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/dlnirsp.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/vbi.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/vbi.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         time_delta,
         *,
         linewave,
         detector_shape=(4096, 4096),
         vbi_camera: Literal["red", "blue"] = "red",
         mosaic: bool = False
     ):
-
         if vbi_camera.lower() not in ["red", "blue"]:
             raise ValueError("vbi_camera must either be 'red' or 'blue'")
 
         if vbi_camera.lower() == "blue":
             n_pos = 9
             self.plate_scale = 0.011 * u.arcsec / u.pix
         else:
@@ -48,15 +47,15 @@
             dataset_shape_rev[::-1],
             array_shape,
             time_delta=time_delta,
             instrument="vbi",
         )
         self.files_shape = (*self.files_shape, n_pos)
         self.files_ndim = len(self.files_shape)
-        self.n_files = int(np.product(self.files_shape))
+        self.n_files = int(np.prod(self.files_shape))
 
         self.add_constant_key("DTYPE1", "SPATIAL")
         self.add_constant_key("DTYPE2", "SPATIAL")
         self.add_constant_key("DTYPE3", "TEMPORAL")
         self.add_constant_key("DPNAME1", "spatial x")
         self.add_constant_key("DPNAME2", "spatial y")
         self.add_constant_key("DPNAME3", "frame number")
```

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/visp.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/visp.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/spec214/vtf.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/vtf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/conftest.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/test_122.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/test_214.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/test_214_inventory.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_214_inventory.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,20 @@
 If you make large changes to dkist-inventory and the simulator which need to be
 co-versioned you should bump the major version number of dkist-inventory and
 update the skip directive here.
 
 This means that incremental changes to the simulator have unit tests which
 verify inventory generation doesn't fail spectacularly.
 """
-import pytest
-
-dkist_inventory = pytest.importorskip("dkist_inventory", minversion="0.8.0")
-
 import astropy.units as u
 import numpy as np
-from astropy.table import Table
+import pytest
 from astropy.wcs import WCS
-from dkist_inventory.inventory import extract_inventory
 from dkist_inventory.header_parsing import HeaderParser
+from dkist_inventory.inventory import extract_inventory
 
 from dkist_data_simulator.dataset import key_function
 from dkist_data_simulator.spec214 import Spec214Dataset
 from dkist_data_simulator.spec214.cryo import SimpleCryoCIDataset, SimpleCryoSPDataset
 from dkist_data_simulator.spec214.dlnirsp import SimpleDLNIRSPDataset
 from dkist_data_simulator.spec214.vbi import MosaicedVBIBlueDataset, SimpleVBIDataset
 from dkist_data_simulator.spec214.visp import SimpleVISPDataset
```

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/tests/test_dataset.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator/util.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/util.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/PKG-INFO` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-data-simulator
-Version: 3.1.6rc1
+Version: 3.2.0rc1
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Provides-Extra: all
```

### Comparing `dkist_data_simulator-3.1.6rc1/dkist_data_simulator.egg-info/SOURCES.txt` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 dkist_data_simulator.egg-info/PKG-INFO
 dkist_data_simulator.egg-info/SOURCES.txt
 dkist_data_simulator.egg-info/dependency_links.txt
 dkist_data_simulator.egg-info/not-zip-safe
 dkist_data_simulator.egg-info/requires.txt
 dkist_data_simulator.egg-info/top_level.txt
 dkist_data_simulator/data/README.rst
-dkist_data_simulator/examples/__init__.py
-dkist_data_simulator/examples/vtf_crisp_5d.py
 dkist_data_simulator/spec214/__init__.py
 dkist_data_simulator/spec214/core.py
 dkist_data_simulator/spec214/cryo.py
 dkist_data_simulator/spec214/dlnirsp.py
 dkist_data_simulator/spec214/vbi.py
 dkist_data_simulator/spec214/visp.py
 dkist_data_simulator/spec214/vtf.py
```

### Comparing `dkist_data_simulator-3.1.6rc1/docs/Makefile` & `dkist_data_simulator-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/docs/conf.py` & `dkist_data_simulator-3.2.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/docs/make.bat` & `dkist_data_simulator-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/licenses/LICENSE.rst` & `dkist_data_simulator-3.2.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/licenses/TEMPLATE_LICENSE.rst` & `dkist_data_simulator-3.2.0rc1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/setup.cfg` & `dkist_data_simulator-3.2.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 [options.extras_require]
 all = 
 test = 
 	pytest
 	pytest-doctestplus
 	pytest-cov
-	pytest-xdist < 3.0.2
 	dkist-inventory >= 0.14.0
 	dkist-header-validator
 docs = 
 	sphinx
 	sphinx-automodapi
 	sphinx-autodoc-typehints
```

### Comparing `dkist_data_simulator-3.1.6rc1/setup.py` & `dkist_data_simulator-3.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.6rc1/tox.ini` & `dkist_data_simulator-3.2.0rc1/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{38}-test
+    py{310,311}-test
     build_docs
     codestyle
 isolated_build = true
 # This is included for testing of the template. You can remove it safely.
 skip_missing_interpreters = True
 
 [testenv]
@@ -27,17 +27,20 @@
     run tests
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
     alldeps: all
 
+deps =
+    pytest-xdist
+
 commands =
     pip freeze
-    pytest --pyargs dkist_data_simulator {toxinidir}/docs --cov dkist_data_simulator --cov-config={toxinidir}/setup.cfg -n auto {posargs}
+    pytest --pyargs dkist_data_simulator {toxinidir}/docs --cov dkist_data_simulator -n auto {posargs}
 
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
     pip freeze
```

