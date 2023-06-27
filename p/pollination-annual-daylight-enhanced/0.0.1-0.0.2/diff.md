# Comparing `tmp/pollination-annual-daylight-enhanced-0.0.1.tar.gz` & `tmp/pollination-annual-daylight-enhanced-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-annual-daylight-enhanced-0.0.1.tar", last modified: Tue Jun 27 14:42:57 2023, max compression
+gzip compressed data, was "dist/pollination-annual-daylight-enhanced-0.0.2.tar", last modified: Tue Jun 27 14:58:57 2023, max compression
```

## Comparing `pollination-annual-daylight-enhanced-0.0.1.tar` & `pollination-annual-daylight-enhanced-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/pollination/annual_daylight/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/pollination/annual_daylight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/pollination/annual_daylight/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:42:20.000000 pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:42:57.000000 pollination-annual-daylight-enhanced-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-27 14:41:58.000000 pollination-annual-daylight-enhanced-0.0.1/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/pollination/annual_daylight_enhanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/pollination/annual_daylight_enhanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/pollination/annual_daylight_enhanced/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:58:11.000000 pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:58:57.000000 pollination-annual-daylight-enhanced-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-27 14:57:44.000000 pollination-annual-daylight-enhanced-0.0.2/tests/validation_test.py
```

### Comparing `pollination-annual-daylight-enhanced-0.0.1/.github/workflows/ci.yaml` & `pollination-annual-daylight-enhanced-0.0.2/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         with:
           python-version: 3.7
       - name: install python dependencies
         run: pip install .
       - name: deploy to staging
         run: |
           queenbee
-          pollination dsl push pollination-annual-enhanced --tag ${{needs.deploy.outputs.tag}} -e https://api.staging.pollination.cloud -src https://api.staging.pollination.cloud/registries --push-dependencies
+          pollination dsl push pollination-annual-daylight-enhanced --tag ${{needs.deploy.outputs.tag}} -e https://api.staging.pollination.cloud -src https://api.staging.pollination.cloud/registries --push-dependencies
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           QB_POLLINATION_TOKEN: ${{ secrets.POLLINATION_STAGING_LADYBUGBOT_TOKEN }}
 
   deploy-viz-and-full:
     name: Deploy `viz` and `full` branches
     runs-on: ubuntu-latest
```

### Comparing `pollination-annual-daylight-enhanced-0.0.1/.github/workflows/tests.yaml` & `pollination-annual-daylight-enhanced-0.0.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-enhanced-0.0.1/LICENSE` & `pollination-annual-daylight-enhanced-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-enhanced-0.0.1/PKG-INFO` & `pollination-annual-daylight-enhanced-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-enhanced
-Version: 0.0.1
+Version: 0.0.2
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-enhanced
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-enhanced-0.0.1/README.md` & `pollination-annual-daylight-enhanced-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-enhanced-0.0.1/pollination/annual_daylight/entry.py` & `pollination-annual-daylight-enhanced-0.0.2/pollination/annual_daylight_enhanced/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/PKG-INFO` & `pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-enhanced
-Version: 0.0.1
+Version: 0.0.2
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-enhanced
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-enhanced-0.0.1/pollination_annual_daylight_enhanced.egg-info/SOURCES.txt` & `pollination-annual-daylight-enhanced-0.0.2/pollination_annual_daylight_enhanced.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 extras-requirements.txt
 requirements.txt
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/tests.yaml
-pollination/annual_daylight/__init__.py
-pollination/annual_daylight/entry.py
+pollination/annual_daylight_enhanced/__init__.py
+pollination/annual_daylight_enhanced/entry.py
 pollination_annual_daylight_enhanced.egg-info/PKG-INFO
 pollination_annual_daylight_enhanced.egg-info/SOURCES.txt
 pollination_annual_daylight_enhanced.egg-info/dependency_links.txt
 pollination_annual_daylight_enhanced.egg-info/not-zip-safe
 pollination_annual_daylight_enhanced.egg-info/requires.txt
 pollination_annual_daylight_enhanced.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `pollination-annual-daylight-enhanced-0.0.1/setup.py` & `pollination-annual-daylight-enhanced-0.0.2/setup.py`

 * *Files identical despite different names*

