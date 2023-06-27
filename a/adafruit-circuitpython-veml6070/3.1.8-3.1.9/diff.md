# Comparing `tmp/adafruit-circuitpython-veml6070-3.1.8.tar.gz` & `tmp/adafruit-circuitpython-veml6070-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-veml6070-3.1.8.tar", last modified: Mon Nov 15 18:53:03 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-veml6070-3.1.9.tar", last modified: Fri Dec 24 13:49:04 2021, max compression
```

## Comparing `adafruit-circuitpython-veml6070-3.1.8.tar` & `adafruit-circuitpython-veml6070-3.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.339276 adafruit-circuitpython-veml6070-3.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.335276 adafruit-circuitpython-veml6070-3.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.335276 adafruit-circuitpython-veml6070-3.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.335276 adafruit-circuitpython-veml6070-3.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.335276 adafruit-circuitpython-veml6070-3.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2021-11-15 18:53:03.339276 adafruit-circuitpython-veml6070-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2990 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.335276 adafruit-circuitpython-veml6070-3.1.8/adafruit_circuitpython_veml6070.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2021-11-15 18:53:03.000000 adafruit-circuitpython-veml6070-3.1.8/adafruit_circuitpython_veml6070.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-11-15 18:53:03.000000 adafruit-circuitpython-veml6070-3.1.8/adafruit_circuitpython_veml6070.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:53:03.000000 adafruit-circuitpython-veml6070-3.1.8/adafruit_circuitpython_veml6070.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-15 18:53:03.000000 adafruit-circuitpython-veml6070-3.1.8/adafruit_circuitpython_veml6070.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-15 18:53:03.000000 adafruit-circuitpython-veml6070-3.1.8/adafruit_circuitpython_veml6070.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10527 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/adafruit_veml6070.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.339276 adafruit-circuitpython-veml6070-3.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.339276 adafruit-circuitpython-veml6070-3.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:53:03.339276 adafruit-circuitpython-veml6070-3.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      632 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/examples/veml6070_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:53:03.339276 adafruit-circuitpython-veml6070-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-11-15 18:52:52.000000 adafruit-circuitpython-veml6070-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.179166 adafruit-circuitpython-veml6070-3.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.175166 adafruit-circuitpython-veml6070-3.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.175166 adafruit-circuitpython-veml6070-3.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.175166 adafruit-circuitpython-veml6070-3.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.175166 adafruit-circuitpython-veml6070-3.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3838 2021-12-24 13:49:04.179166 adafruit-circuitpython-veml6070-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2990 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.175166 adafruit-circuitpython-veml6070-3.1.9/adafruit_circuitpython_veml6070.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3838 2021-12-24 13:49:04.000000 adafruit-circuitpython-veml6070-3.1.9/adafruit_circuitpython_veml6070.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2021-12-24 13:49:04.000000 adafruit-circuitpython-veml6070-3.1.9/adafruit_circuitpython_veml6070.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-24 13:49:04.000000 adafruit-circuitpython-veml6070-3.1.9/adafruit_circuitpython_veml6070.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-24 13:49:04.000000 adafruit-circuitpython-veml6070-3.1.9/adafruit_circuitpython_veml6070.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-24 13:49:04.000000 adafruit-circuitpython-veml6070-3.1.9/adafruit_circuitpython_veml6070.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10780 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/adafruit_veml6070.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.179166 adafruit-circuitpython-veml6070-3.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.179166 adafruit-circuitpython-veml6070-3.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5541 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-24 13:49:04.179166 adafruit-circuitpython-veml6070-3.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/examples/veml6070_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-24 13:49:04.179166 adafruit-circuitpython-veml6070-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-12-24 13:48:52.000000 adafruit-circuitpython-veml6070-3.1.9/setup.py
```

### Comparing `adafruit-circuitpython-veml6070-3.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-veml6070-3.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-veml6070-3.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-veml6070-3.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-veml6070-3.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/.pylintrc` & `adafruit-circuitpython-veml6070-3.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-veml6070-3.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/LICENSE` & `adafruit-circuitpython-veml6070-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-veml6070-3.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-veml6070-3.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-veml6070-3.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/PKG-INFO` & `adafruit-circuitpython-veml6070-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-veml6070
-Version: 3.1.8
+Version: 3.1.9
 Summary: CircuitPython library for VEML6070 UV Index Sensor Breakout.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_VEML6070
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit veml6070 uv index sensor breakout hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-veml6070-3.1.8/README.rst` & `adafruit-circuitpython-veml6070-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/adafruit_circuitpython_veml6070.egg-info/PKG-INFO` & `adafruit-circuitpython-veml6070-3.1.9/adafruit_circuitpython_veml6070.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-veml6070
-Version: 3.1.8
+Version: 3.1.9
 Summary: CircuitPython library for VEML6070 UV Index Sensor Breakout.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_VEML6070
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit veml6070 uv index sensor breakout hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-veml6070-3.1.8/adafruit_circuitpython_veml6070.egg-info/SOURCES.txt` & `adafruit-circuitpython-veml6070-3.1.9/adafruit_circuitpython_veml6070.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/adafruit_veml6070.py` & `adafruit-circuitpython-veml6070-3.1.9/adafruit_veml6070.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,20 @@
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_VEML6070.git"
 
 from adafruit_bus_device.i2c_device import I2CDevice
 from micropython import const
 
+try:
+    import typing  # pylint: disable=unused-import
+    from busio import I2C
+except ImportError:
+    pass
+
 
 # Set I2C addresses:
 _VEML6070_ADDR_ARA = const(0x18 >> 1)
 _VEML6070_ADDR_CMD = const(0x70 >> 1)
 _VEML6070_ADDR_LOW = const(0x71 >> 1)
 _VEML6070_ADDR_HIGH = const(0x73 >> 1)
 
@@ -121,15 +127,17 @@
         .. code-block:: python
 
             uv_raw = uv.uv_raw
             risk_level = uv.get_index(uv_raw)
 
     """
 
-    def __init__(self, i2c_bus, _veml6070_it="VEML6070_1_T", ack=False):
+    def __init__(
+        self, i2c_bus: I2C, _veml6070_it: str = "VEML6070_1_T", ack: bool = False
+    ) -> None:
         # Check if the IT is valid
         if _veml6070_it not in _VEML6070_INTEGRATION_TIME:
             raise ValueError(
                 "Integration Time invalid. Valid values are: ",
                 _VEML6070_INTEGRATION_TIME.keys(),
             )
 
@@ -158,85 +166,85 @@
         self.buf[0] = (
             self._ack << 5 | _VEML6070_INTEGRATION_TIME[self._it][0] << 2 | 0x02
         )
         with self.i2c_cmd as i2c_cmd:
             i2c_cmd.write(self.buf)
 
     @property
-    def uv_raw(self):
+    def uv_raw(self) -> int:
         """
         Reads and returns the value of the UV intensity.
         """
         buffer = bytearray(2)
         with self.i2c_low as i2c_low:
             i2c_low.readinto(buffer, end=1)
 
         with self.i2c_high as i2c_high:
             i2c_high.readinto(buffer, start=1)
 
         return buffer[1] << 8 | buffer[0]
 
     @property
-    def ack(self):
+    def ack(self) -> int:
         """
         Turns on or off the ACKnowledge function of the sensor. The ACK function will send
         a signal to the host when the value of the sensed UV light changes beyond the
         programmed threshold.
         """
         return self._ack
 
     @ack.setter
-    def ack(self, new_ack):
+    def ack(self, new_ack: int) -> None:
         if new_ack != bool(new_ack):
-            raise ValueError("ACK must be 'True' or 'False'.")
+            raise ValueError("ACK must be '1' (On) or '0' (Off).")
         self._ack = int(new_ack)
         self.buf[0] = (
             self._ack << 5
             | self._ack_thd << 4
             | _VEML6070_INTEGRATION_TIME[self._it][0] << 2
             | 0x02
         )
         with self.i2c_cmd as i2c_cmd:
             i2c_cmd.write(self.buf)
 
     @property
-    def ack_threshold(self):
+    def ack_threshold(self) -> int:
         """
         The ACKnowledge Threshold, which alerts the host controller to value changes
         greater than the threshold. Available settings are: :const:`0` = 102 steps;
         :const:`1` = 145 steps. :const:`0` is the default setting.
         """
         return self._ack_thd
 
     @ack_threshold.setter
-    def ack_threshold(self, new_ack_thd):
+    def ack_threshold(self, new_ack_thd: int) -> None:
         if new_ack_thd not in (0, 1):
             raise ValueError("ACK Threshold must be '0' or '1'.")
         self._ack_thd = int(new_ack_thd)
         self.buf[0] = (
             self._ack << 5
             | self._ack_thd << 4
             | _VEML6070_INTEGRATION_TIME[self._it][0] << 2
             | 0x02
         )
         with self.i2c_cmd as i2c_cmd:
             i2c_cmd.write(self.buf)
 
     @property
-    def integration_time(self):
+    def integration_time(self) -> str:
         """
         The Integration Time of the sensor, which is the refresh interval of the
         sensor. The higher the refresh interval, the more accurate the reading is (at
         the cost of less sampling). The available settings are: :const:`VEML6070_HALF_T`,
         :const:`VEML6070_1_T`, :const:`VEML6070_2_T`, :const:`VEML6070_4_T`.
         """
         return self._it
 
     @integration_time.setter
-    def integration_time(self, new_it):
+    def integration_time(self, new_it: str) -> None:
         if new_it not in _VEML6070_INTEGRATION_TIME:
             raise ValueError(
                 "Integration Time invalid. Valid values are: ",
                 _VEML6070_INTEGRATION_TIME.keys(),
             )
 
         self._it = new_it
@@ -245,37 +253,37 @@
             | self._ack_thd << 4
             | _VEML6070_INTEGRATION_TIME[new_it][0] << 2
             | 0x02
         )
         with self.i2c_cmd as i2c_cmd:
             i2c_cmd.write(self.buf)
 
-    def sleep(self):
+    def sleep(self) -> None:
         """
         Puts the VEML6070 into sleep ('shutdown') mode. Datasheet claims a current draw
         of 1uA while in shutdown.
         """
         self.buf[0] = 0x03
         with self.i2c_cmd as i2c_cmd:
             i2c_cmd.write(self.buf)
 
-    def wake(self):
+    def wake(self) -> None:
         """
         Wakes the VEML6070 from sleep. :class:`VEML6070.uv_raw` will also wake from sleep.
         """
         self.buf[0] = (
             self._ack << 5
             | self._ack_thd << 4
             | _VEML6070_INTEGRATION_TIME[self._it][0] << 2
             | 0x02
         )
         with self.i2c_cmd as i2c_cmd:
             i2c_cmd.write(self.buf)
 
-    def get_index(self, _raw):
+    def get_index(self, _raw: int) -> str:
         """
         Calculates the UV Risk Level based on the captured UV reading. Requires the ``_raw``
         argument (from :meth:`veml6070.uv_raw`). Risk level is available for Integration Times (IT)
         1, 2, & 4. The result is automatically scaled to the current IT setting.
 
             =========      ========
             LEVEL*         UV Index
```

### Comparing `adafruit-circuitpython-veml6070-3.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-veml6070-3.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/docs/conf.py` & `adafruit-circuitpython-veml6070-3.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/docs/index.rst` & `adafruit-circuitpython-veml6070-3.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/examples/veml6070_simpletest.py` & `adafruit-circuitpython-veml6070-3.1.9/examples/veml6070_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-veml6070-3.1.8/setup.py` & `adafruit-circuitpython-veml6070-3.1.9/setup.py`

 * *Files identical despite different names*

