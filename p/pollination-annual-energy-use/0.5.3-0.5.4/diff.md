# Comparing `tmp/pollination-annual-energy-use-0.5.3.tar.gz` & `tmp/pollination-annual-energy-use-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-annual-energy-use-0.5.3.tar", last modified: Tue Mar 14 18:04:33 2023, max compression
+gzip compressed data, was "dist/pollination-annual-energy-use-0.5.4.tar", last modified: Tue Jun 27 16:40:05 2023, max compression
```

## Comparing `pollination-annual-energy-use-0.5.3.tar` & `pollination-annual-energy-use-0.5.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/pollination/annual_energy_use/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/pollination/annual_energy_use/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/pollination/annual_energy_use/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:03:58.000000 pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:04:33.000000 pollination-annual-energy-use-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-14 18:03:39.000000 pollination-annual-energy-use-0.5.3/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/pollination/annual_energy_use/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/pollination/annual_energy_use/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/pollination/annual_energy_use/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:39:30.000000 pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:40:05.000000 pollination-annual-energy-use-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-27 16:39:11.000000 pollination-annual-energy-use-0.5.4/tests/validation_test.py
```

### Comparing `pollination-annual-energy-use-0.5.3/.github/workflows/ci.yaml` & `pollination-annual-energy-use-0.5.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.3/.github/workflows/tests.yaml` & `pollination-annual-energy-use-0.5.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.3/LICENSE` & `pollination-annual-energy-use-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.3/PKG-INFO` & `pollination-annual-energy-use-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-energy-use
-Version: 0.5.3
+Version: 0.5.4
 Summary: Run an annual energy simulation and compute energy use intensity.
 Home-page: https://github.com/pollination/annual-energy-use
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-energy-use-0.5.3/pollination/annual_energy_use/entry.py` & `pollination-annual-energy-use-0.5.4/pollination/annual_energy_use/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/PKG-INFO` & `pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-energy-use
-Version: 0.5.3
+Version: 0.5.4
 Summary: Run an annual energy simulation and compute energy use intensity.
 Home-page: https://github.com/pollination/annual-energy-use
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-energy-use-0.5.3/pollination_annual_energy_use.egg-info/SOURCES.txt` & `pollination-annual-energy-use-0.5.4/pollination_annual_energy_use.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.3/setup.py` & `pollination-annual-energy-use-0.5.4/setup.py`

 * *Files identical despite different names*

