# Comparing `tmp/paco.models-7.8.8.tar.gz` & `tmp/paco.models-7.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paco.models-7.8.8.tar", last modified: Mon Apr 19 20:17:26 2021, max compression
+gzip compressed data, was "dist/paco.models-7.8.9.tar", last modified: Fri Apr 23 23:51:33 2021, max compression
```

## Comparing `paco.models-7.8.8.tar` & `paco.models-7.8.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:26.000000 paco.models-7.8.8/
--rw-r--r--   0 klindsay   (501) staff       (20)      280 2021-04-19 20:17:25.000000 paco.models-7.8.8/.gitignore
--rw-r--r--   0 klindsay   (501) staff       (20)    24613 2021-04-19 20:17:25.000000 paco.models-7.8.8/CHANGELOG.md
--rw-r--r--   0 klindsay   (501) staff       (20)    16725 2021-04-19 20:17:25.000000 paco.models-7.8.8/LICENSE
--rw-r--r--   0 klindsay   (501) staff       (20)       55 2021-04-19 20:17:25.000000 paco.models-7.8.8/MANIFEST.in
--rw-r--r--   0 klindsay   (501) staff       (20)    34765 2021-04-19 20:17:26.000000 paco.models-7.8.8/PKG-INFO
--rw-r--r--   0 klindsay   (501) staff       (20)     2009 2021-04-19 20:17:25.000000 paco.models-7.8.8/README.md
--rw-r--r--   0 klindsay   (501) staff       (20)      306 2021-04-19 20:17:25.000000 paco.models-7.8.8/buildout.cfg
--rw-r--r--   0 klindsay   (501) staff       (20)       38 2021-04-19 20:17:26.000000 paco.models-7.8.8/setup.cfg
--rw-r--r--   0 klindsay   (501) staff       (20)     1337 2021-04-19 20:17:25.000000 paco.models-7.8.8/setup.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco/
--rw-r--r--   0 klindsay   (501) staff       (20)       65 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/__init__.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco/aws/
--rw-r--r--   0 klindsay   (501) staff       (20)      383 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/aws/__init__.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco/codegen/
--rw-r--r--   0 klindsay   (501) staff       (20)       69 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/codegen/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5245 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/codegen/update_gen_vocabulary.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco/models/
--rw-r--r--   0 klindsay   (501) staff       (20)      823 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2235 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/accounts.py
--rw-r--r--   0 klindsay   (501) staff       (20)   120867 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/applications.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2484 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/backup.py
--rw-r--r--   0 klindsay   (501) staff       (20)    25233 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/base.py
--rw-r--r--   0 klindsay   (501) staff       (20)    11438 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/cfn_init.py
--rw-r--r--   0 klindsay   (501) staff       (20)      839 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/events.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1394 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/exceptions.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2346 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/formatter.py
--rw-r--r--   0 klindsay   (501) staff       (20)   165410 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/gen_vocabulary.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4476 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/iam.py
--rw-r--r--   0 klindsay   (501) staff       (20)     8133 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/iot.py
--rw-r--r--   0 klindsay   (501) staff       (20)   116876 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/loader.py
--rw-r--r--   0 klindsay   (501) staff       (20)      548 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/locations.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4384 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/logging.py
--rw-r--r--   0 klindsay   (501) staff       (20)    16610 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/metrics.py
--rw-r--r--   0 klindsay   (501) staff       (20)     9547 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/networks.py
--rw-r--r--   0 klindsay   (501) staff       (20)     6943 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/project.py
--rw-r--r--   0 klindsay   (501) staff       (20)    15308 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/references.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3168 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/reftypes.py
--rw-r--r--   0 klindsay   (501) staff       (20)      195 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/registry.py
--rw-r--r--   0 klindsay   (501) staff       (20)    31876 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/resources.py
--rw-r--r--   0 klindsay   (501) staff       (20)   352763 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/schemas.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1710 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/services.py
--rw-r--r--   0 klindsay   (501) staff       (20)      186 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/storages.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco/models/tests/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/tests/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)    27259 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/tests/test_loader.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1115 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/tests/test_references.py
--rw-r--r--   0 klindsay   (501) staff       (20)    17832 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/vocabulary.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3353 2021-04-19 20:17:25.000000 paco.models-7.8.8/src/paco/models/yaml.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco.models.egg-info/
--rw-r--r--   0 klindsay   (501) staff       (20)    34765 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco.models.egg-info/PKG-INFO
--rw-r--r--   0 klindsay   (501) staff       (20)     1325 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco.models.egg-info/SOURCES.txt
--rw-r--r--   0 klindsay   (501) staff       (20)        1 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco.models.egg-info/dependency_links.txt
--rw-r--r--   0 klindsay   (501) staff       (20)       83 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco.models.egg-info/entry_points.txt
--rw-r--r--   0 klindsay   (501) staff       (20)        1 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco.models.egg-info/not-zip-safe
--rw-r--r--   0 klindsay   (501) staff       (20)       47 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco.models.egg-info/requires.txt
--rw-r--r--   0 klindsay   (501) staff       (20)        5 2021-04-19 20:17:26.000000 paco.models-7.8.8/src/paco.models.egg-info/top_level.txt
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:33.000000 paco.models-7.8.9/
+-rw-r--r--   0 klindsay   (501) staff       (20)      280 2021-04-23 23:51:32.000000 paco.models-7.8.9/.gitignore
+-rw-r--r--   0 klindsay   (501) staff       (20)    24765 2021-04-23 23:51:32.000000 paco.models-7.8.9/CHANGELOG.md
+-rw-r--r--   0 klindsay   (501) staff       (20)    16725 2021-04-23 23:51:32.000000 paco.models-7.8.9/LICENSE
+-rw-r--r--   0 klindsay   (501) staff       (20)       55 2021-04-23 23:51:32.000000 paco.models-7.8.9/MANIFEST.in
+-rw-r--r--   0 klindsay   (501) staff       (20)    34989 2021-04-23 23:51:33.000000 paco.models-7.8.9/PKG-INFO
+-rw-r--r--   0 klindsay   (501) staff       (20)     2009 2021-04-23 23:51:32.000000 paco.models-7.8.9/README.md
+-rw-r--r--   0 klindsay   (501) staff       (20)      306 2021-04-23 23:51:32.000000 paco.models-7.8.9/buildout.cfg
+-rw-r--r--   0 klindsay   (501) staff       (20)       38 2021-04-23 23:51:33.000000 paco.models-7.8.9/setup.cfg
+-rw-r--r--   0 klindsay   (501) staff       (20)     1337 2021-04-23 23:51:32.000000 paco.models-7.8.9/setup.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco/
+-rw-r--r--   0 klindsay   (501) staff       (20)       65 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/__init__.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco/aws/
+-rw-r--r--   0 klindsay   (501) staff       (20)      383 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/aws/__init__.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco/codegen/
+-rw-r--r--   0 klindsay   (501) staff       (20)       69 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/codegen/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5245 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/codegen/update_gen_vocabulary.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco/models/
+-rw-r--r--   0 klindsay   (501) staff       (20)      823 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2235 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/accounts.py
+-rw-r--r--   0 klindsay   (501) staff       (20)   121189 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/applications.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2484 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/backup.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    25233 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/base.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    11438 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/cfn_init.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      839 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/events.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1394 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/exceptions.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2346 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/formatter.py
+-rw-r--r--   0 klindsay   (501) staff       (20)   165410 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/gen_vocabulary.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4476 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/iam.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     8133 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/iot.py
+-rw-r--r--   0 klindsay   (501) staff       (20)   116876 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/loader.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      548 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/locations.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4384 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/logging.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    16610 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/metrics.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     9547 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/networks.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     6943 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/project.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    15308 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/references.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3168 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/reftypes.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      195 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/registry.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    31876 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/resources.py
+-rw-r--r--   0 klindsay   (501) staff       (20)   353234 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/schemas.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1710 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/services.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      186 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/storages.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco/models/tests/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/tests/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    27259 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/tests/test_loader.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1115 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/tests/test_references.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    17832 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/vocabulary.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3353 2021-04-23 23:51:32.000000 paco.models-7.8.9/src/paco/models/yaml.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco.models.egg-info/
+-rw-r--r--   0 klindsay   (501) staff       (20)    34989 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco.models.egg-info/PKG-INFO
+-rw-r--r--   0 klindsay   (501) staff       (20)     1325 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco.models.egg-info/SOURCES.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)        1 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco.models.egg-info/dependency_links.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)       83 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco.models.egg-info/entry_points.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)        1 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco.models.egg-info/not-zip-safe
+-rw-r--r--   0 klindsay   (501) staff       (20)       47 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco.models.egg-info/requires.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)        5 2021-04-23 23:51:33.000000 paco.models-7.8.9/src/paco.models.egg-info/top_level.txt
```

### Comparing `paco.models-7.8.8/CHANGELOG.md` & `paco.models-7.8.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog for paco.models
 =========================
 
+7.8.9 (2021-04-23)
+------------------
+
+### Added
+
+- Added support to disable Target Groups on ASGs
+
+- Added support to disable services in ECSServices
+
 7.8.8 (2021-04-19)
 ------------------
 
 ### Fixed
 
 -  Added resolve_ref to ApplicationEngine model object to fix some paco ref lookups.
```

### Comparing `paco.models-7.8.8/LICENSE` & `paco.models-7.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/PKG-INFO` & `paco.models-7.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paco.models
-Version: 7.8.8
+Version: 7.8.9
 Summary: paco.models: Semantic cloud infrastructure configuration file format and object model
 Home-page: https://github.com/waterbear-cloud/paco.models
 Author: Waterbear Cloud
 Author-email: hello@waterbear.cloud
 License: UNKNOWN
 Description: # paco.models
         
@@ -56,14 +56,23 @@
             buildout
             source profile.sh
         
         
         Changelog for paco.models
         =========================
         
+        7.8.9 (2021-04-23)
+        ------------------
+        
+        ### Added
+        
+        - Added support to disable Target Groups on ASGs
+        
+        - Added support to disable services in ECSServices
+        
         7.8.8 (2021-04-19)
         ------------------
         
         ### Fixed
         
         -  Added resolve_ref to ApplicationEngine model object to fix some paco ref lookups.
```

### Comparing `paco.models-7.8.8/README.md` & `paco.models-7.8.9/README.md`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/setup.py` & `paco.models-7.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
     long_description += '\n\n'
 with open('CHANGELOG.md') as f:
     long_description += f.read()
 
 setup(
     name='paco.models',
-    version='7.8.8',
+    version='7.8.9',
     description='paco.models: Semantic cloud infrastructure configuration file format and object model',
     author='Waterbear Cloud',
     author_email='hello@waterbear.cloud',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/waterbear-cloud/paco.models',
     install_requires=['Setuptools', 'ruamel.yaml', 'zope.schema', 'troposphere'],
```

### Comparing `paco.models-7.8.8/src/paco/codegen/update_gen_vocabulary.py` & `paco.models-7.8.9/src/paco/codegen/update_gen_vocabulary.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/__init__.py` & `paco.models-7.8.9/src/paco/models/__init__.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/accounts.py` & `paco.models-7.8.9/src/paco/models/accounts.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/applications.py` & `paco.models-7.8.9/src/paco/models/applications.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,14 +494,17 @@
     managed_instance_protection = FieldProperty(schemas.IECSCapacityProvider['managed_instance_protection'])
     maximum_scaling_step_size = FieldProperty(schemas.IECSCapacityProvider['maximum_scaling_step_size'])
 
     def get_aws_name(self):
         asg = self.__parent__.__parent__
         return f"{asg.netenv_name}-{asg.env_name}-{asg.app_name}-{asg.group_name}-{asg.name}"
 
+    def resolve_ref(self, ref):
+        return self.resolve_ref_obj.resolve_ref(ref)
+
 @implementer(schemas.IECSASGConfiguration)
 class ECSASGConfiguration(Named):
     cluster = FieldProperty(schemas.IECSASGConfiguration['cluster'])
     log_level = FieldProperty(schemas.IECSASGConfiguration['log_level'])
     capacity_provider = FieldProperty(schemas.IECSASGConfiguration['capacity_provider'])
 
     def __init__(self, name, parent):
@@ -574,14 +577,15 @@
     instance_ami_ignore_changes = FieldProperty(schemas.IASG['instance_ami_ignore_changes'])
     instance_ami_type = FieldProperty(schemas.IASG['instance_ami_type'])
     instance_key_pair = FieldProperty(schemas.IASG['instance_key_pair'])
     instance_type = FieldProperty(schemas.IASG['instance_type'])
     segment = FieldProperty(schemas.IASG['segment'])
     termination_policies = FieldProperty(schemas.IASG['termination_policies'])
     security_groups = FieldProperty(schemas.IASG['security_groups'])
+    disable_target_groups = FieldProperty(schemas.IASG['disable_target_groups'])
     target_groups = FieldProperty(schemas.IASG['target_groups'])
     load_balancers = FieldProperty(schemas.IASG['load_balancers'])
     termination_policies = FieldProperty(schemas.IASG['termination_policies'])
     user_data_script = FieldProperty(schemas.IASG['user_data_script'])
     user_data_pre_script = FieldProperty(schemas.IASG['user_data_pre_script'])
     instance_monitoring = FieldProperty(schemas.IASG['instance_monitoring'])
     scaling_policy_cpu_average = FieldProperty(schemas.IASG['scaling_policy_cpu_average'])
@@ -1034,14 +1038,15 @@
 @implementer(schemas.IECSService)
 class ECSService(Named, Monitorable):
     type = 'ECSService'
     deployment_controller = FieldProperty(schemas.IECSService['deployment_controller'])
     deployment_minimum_healthy_percent = FieldProperty(schemas.IECSService['deployment_minimum_healthy_percent'])
     deployment_maximum_percent = FieldProperty(schemas.IECSService['deployment_maximum_percent'])
     desired_count = FieldProperty(schemas.IECSService['desired_count'])
+    disable_service = FieldProperty(schemas.IECSService['disable_service'])
     minimum_tasks = FieldProperty(schemas.IECSService['minimum_tasks'])
     maximum_tasks = FieldProperty(schemas.IECSService['maximum_tasks'])
     suspend_scaling = FieldProperty(schemas.IECSService['suspend_scaling'])
     target_tracking_scaling_policies = FieldProperty(schemas.IECSService['target_tracking_scaling_policies'])
     health_check_grace_period_seconds = FieldProperty(schemas.IECSService['health_check_grace_period_seconds'])
     task_definition = FieldProperty(schemas.IECSService['task_definition'])
     launch_type = FieldProperty(schemas.IECSService['launch_type'])
@@ -1137,14 +1142,15 @@
 @implementer(schemas.IECSSettingsGroups)
 class ECSSettingsGroups(Named, dict):
     pass
 
 @implementer(schemas.IECSServices)
 class ECSServices(Resource, Monitorable):
     cluster = FieldProperty(schemas.IECSServices['cluster'])
+    disable_services = FieldProperty(schemas.IECSServices['disable_services'])
     setting_groups = FieldProperty(schemas.IECSServices['setting_groups'])
     services = FieldProperty(schemas.IECSServices['services'])
     service_discovery_namespace_name = FieldProperty(schemas.IECSServices['service_discovery_namespace_name'])
     secrets_manager_access = FieldProperty(schemas.IECSServices['secrets_manager_access'])
     task_definitions = FieldProperty(schemas.IECSServices['task_definitions'])
 
     def __init__(self, name, parent):
```

### Comparing `paco.models-7.8.8/src/paco/models/backup.py` & `paco.models-7.8.9/src/paco/models/backup.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/base.py` & `paco.models-7.8.9/src/paco/models/base.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/cfn_init.py` & `paco.models-7.8.9/src/paco/models/cfn_init.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/events.py` & `paco.models-7.8.9/src/paco/models/events.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/exceptions.py` & `paco.models-7.8.9/src/paco/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/formatter.py` & `paco.models-7.8.9/src/paco/models/formatter.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/gen_vocabulary.py` & `paco.models-7.8.9/src/paco/models/gen_vocabulary.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/iam.py` & `paco.models-7.8.9/src/paco/models/iam.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/iot.py` & `paco.models-7.8.9/src/paco/models/iot.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/loader.py` & `paco.models-7.8.9/src/paco/models/loader.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/locations.py` & `paco.models-7.8.9/src/paco/models/locations.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/logging.py` & `paco.models-7.8.9/src/paco/models/logging.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/metrics.py` & `paco.models-7.8.9/src/paco/models/metrics.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/networks.py` & `paco.models-7.8.9/src/paco/models/networks.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/project.py` & `paco.models-7.8.9/src/paco/models/project.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/references.py` & `paco.models-7.8.9/src/paco/models/references.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/reftypes.py` & `paco.models-7.8.9/src/paco/models/reftypes.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/resources.py` & `paco.models-7.8.9/src/paco/models/resources.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/schemas.py` & `paco.models-7.8.9/src/paco/models/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -5604,14 +5604,15 @@
     max_instances: 3
     min_instances: 1
     rolling_update_policy:
       max_batch_size: 1
       min_instances_in_service: 1
       pause_time: PT3M
       wait_on_resource_signals: false
+    disable_target_groups: false
     target_groups:
       - paco.ref netenv.mynet.applications.app.groups.web.resources.alb.target_groups.cloud
     security_groups:
       - paco.ref netenv.mynet.network.vpc.security_groups.web.asg
     segment: private
     termination_policies:
       - Default
@@ -5968,14 +5969,19 @@
     )
     ssh_access = zope.schema.Object(
         title="SSH Access",
         description="",
         schema=ISSHAccess,
         required=False,
     )
+    disable_target_groups = zope.schema.Bool(
+        title="Disable Target Groups",
+        required=False,
+        default=False,
+    )
     target_groups = zope.schema.List(
         title="Target groups",
         description="",
         value_type=PacoReference(
             title="Paco reference",
             schema_constraint='ITargetGroup'
         ),
@@ -6605,14 +6611,19 @@
     )
     desired_count = zope.schema.Int(
         title="Desired Count",
         min=0,
         required=False,
         # ToDo: constraint require if schedulingStrategy=REPLICA
     )
+    disable_service = zope.schema.Bool(
+        title="Disable the service and stop all tasks",
+        default=False,
+        required=False,
+    )
     capacity_providers = zope.schema.List(
         title="Capacity Providers",
         required=False,
         default=[],
         value_type=zope.schema.Object(IECSCapacityProviderStrategyItem)
     )
     launch_type = zope.schema.Choice(
@@ -6793,14 +6804,19 @@
     """
     cluster = PacoReference(
         title='Cluster',
         required=True,
         str_ok=False,
         schema_constraint='IECSCluster'
     )
+    disable_services = zope.schema.Bool(
+        title="Disable all services and stop all tasks",
+        default=False,
+        required=False,
+    )
     setting_groups = zope.schema.Object(
         title="Setting Groups",
         description="",
         schema=IECSSettingsGroups,
         required=False
     )
     task_definitions = zope.schema.Object(
```

### Comparing `paco.models-7.8.8/src/paco/models/services.py` & `paco.models-7.8.9/src/paco/models/services.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/tests/test_loader.py` & `paco.models-7.8.9/src/paco/models/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/tests/test_references.py` & `paco.models-7.8.9/src/paco/models/tests/test_references.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/vocabulary.py` & `paco.models-7.8.9/src/paco/models/vocabulary.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco/models/yaml.py` & `paco.models-7.8.9/src/paco/models/yaml.py`

 * *Files identical despite different names*

### Comparing `paco.models-7.8.8/src/paco.models.egg-info/PKG-INFO` & `paco.models-7.8.9/src/paco.models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paco.models
-Version: 7.8.8
+Version: 7.8.9
 Summary: paco.models: Semantic cloud infrastructure configuration file format and object model
 Home-page: https://github.com/waterbear-cloud/paco.models
 Author: Waterbear Cloud
 Author-email: hello@waterbear.cloud
 License: UNKNOWN
 Description: # paco.models
         
@@ -56,14 +56,23 @@
             buildout
             source profile.sh
         
         
         Changelog for paco.models
         =========================
         
+        7.8.9 (2021-04-23)
+        ------------------
+        
+        ### Added
+        
+        - Added support to disable Target Groups on ASGs
+        
+        - Added support to disable services in ECSServices
+        
         7.8.8 (2021-04-19)
         ------------------
         
         ### Fixed
         
         -  Added resolve_ref to ApplicationEngine model object to fix some paco ref lookups.
```

### Comparing `paco.models-7.8.8/src/paco.models.egg-info/SOURCES.txt` & `paco.models-7.8.9/src/paco.models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

