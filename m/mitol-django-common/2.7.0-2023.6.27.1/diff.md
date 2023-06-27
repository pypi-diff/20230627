# Comparing `tmp/mitol-django-common-2.7.0.tar.gz` & `tmp/mitol-django-common-2023.6.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-common-2.7.0.tar", last modified: Tue Jan 17 16:11:54 2023, max compression
+gzip compressed data, was "mitol-django-common-2023.6.27.1.tar", last modified: Tue Jun 27 20:11:20 2023, max compression
```

## Comparing `mitol-django-common-2.7.0.tar` & `mitol-django-common-2023.6.27.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.900974 mitol-django-common-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-01-17 16:11:54.900974 mitol-django-common-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.892974 mitol-django-common-2.7.0/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.896974 mitol-django-common-2.7.0/mitol/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2591 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2868 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)    12201 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.896974 mitol-django-common-2.7.0/mitol/common/factories/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/factories/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.896974 mitol-django-common-2.7.0/mitol/common/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.896974 mitol-django-common-2.7.0/mitol/common/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/management/commands/generate_app_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/pytest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.896974 mitol-django-common-2.7.0/mitol/common/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/settings/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.896974 mitol-django-common-2.7.0/mitol/common/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)     3190 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/templatetags/render_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.896974 mitol-django-common-2.7.0/mitol/common/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/currency.py
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/http_requests.py
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol/common/utils/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:11:54.900974 mitol-django-common-2.7.0/mitol_django_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol_django_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol_django_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol_django_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol_django_common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol_django_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol_django_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/mitol_django_common.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:11:54.900974 mitol-django-common-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-01-17 16:11:54.000000 mitol-django-common-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.428603 mitol-django-common-2023.6.27.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-27 20:11:20.428603 mitol-django-common-2023.6.27.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.424603 mitol-django-common-2023.6.27.1/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.424603 mitol-django-common-2023.6.27.1/mitol/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     3159 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2868 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13674 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.424603 mitol-django-common-2023.6.27.1/mitol/common/factories/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/factories/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.424603 mitol-django-common-2023.6.27.1/mitol/common/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.424603 mitol-django-common-2023.6.27.1/mitol/common/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/management/commands/generate_app_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/pytest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.424603 mitol-django-common-2023.6.27.1/mitol/common/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/settings/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.424603 mitol-django-common-2023.6.27.1/mitol/common/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)     3190 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/templatetags/render_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.428603 mitol-django-common-2023.6.27.1/mitol/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/currency.py
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/http_requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/mitol/common/utils/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 20:11:20.428603 mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-27 20:11:20.000000 mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-06-27 20:11:20.000000 mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 20:11:20.000000 mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-27 20:11:20.000000 mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-06-27 20:11:20.000000 mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-27 20:11:20.000000 mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 20:11:20.000000 mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 20:11:20.428603 mitol-django-common-2023.6.27.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-06-27 20:11:19.000000 mitol-django-common-2023.6.27.1/setup.py
```

### Comparing `mitol-django-common-2.7.0/PKG-INFO` & `mitol-django-common-2023.6.27.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-common
-Version: 2.7.0
+Version: 2023.6.27.1
 Summary: MIT Open Learning django app extensions for common utilities
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-common
 ---
 
 This is the Open Learning Django Common app. It provides common functionality used across all our applications.
```

### Comparing `mitol-django-common-2.7.0/backend_shim.py` & `mitol-django-common-2023.6.27.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/CHANGELOG.md` & `mitol-django-common-2023.6.27.1/mitol/common/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,40 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+and this project uses date-based versioning.
 
-## [Unreleased]
+<!-- scriv-insert-here -->
+
+<a id='changelog-2023.6.27.1'></a>
+## [2023.6.27.1] - 2023-06-27
+
+### Added
+
+- Added `mitol.common.envs.get_crontab_kwargs` for crontab parsing from environment variables.
+
+### Changed
+
+- Updated changelog management and versioning scheme.
+
+- Updated `pytest` dependency to allow versions `>=7.0.0`.
+
+<a id='changelog-2023.01.17'></a>
+## [2023.01.17] - 2023-06-27
+
+### Added
+
+- Added `mitol.common.envs.get_crontab_kwargs` for crontab parsing from environment variables.
+
+### Changed
+
+- Updated changelog management and versioning scheme.
+
+- Updated `pytest` dependency to allow versions `>=7.0.0`.
 
 ## [2.7.0] - 2023-01-17
 
 ## [2.6.1] - 2023-01-13
 
 ## [2.6.0] - 2022-10-28
```

### Comparing `mitol-django-common-2.7.0/mitol/common/admin.py` & `mitol-django-common-2023.6.27.1/mitol/common/admin.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/apps.py` & `mitol-django-common-2023.6.27.1/mitol/common/apps.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/decorators.py` & `mitol-django-common-2023.6.27.1/mitol/common/decorators.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/envs.py` & `mitol-django-common-2023.6.27.1/mitol/common/envs.py`

 * *Files 19% similar despite different names*

```diff
@@ -217,14 +217,62 @@
     parsed_value = value
     if isinstance(value, str):
         parsed_value = value.split(",")
 
     return [item.strip(" ") for item in parsed_value]
 
 
+CRONTAB_KEYS = ["minute", "hour", "day_of_week", "day_of_month", "month_of_year"]
+
+
+def parse_crontab_kwargs(name, value, default):
+    """
+    Parses a crontab string into structured kwargs
+
+    Argumments:
+        value (str):
+            the crontab string value
+        default (str or dict):
+            the default crontab as either a string or dict
+
+    Returns:
+        dict:
+            the parsed crontab kwargs
+    """
+
+    if isinstance(value, str):
+        units = value.split(" ")
+
+        if len(units) != len(CRONTAB_KEYS):
+            raise ImproperlyConfigured(
+                f"Crontab value '{value}' is required to have {len(CRONTAB_KEYS)} units"
+            )
+
+        if not all(units):
+            raise ImproperlyConfigured(
+                f"Crontab value '{value}' does not have values for all units"
+            )
+
+        return dict(zip(CRONTAB_KEYS, units))
+
+    # an empty string would be falsy and we want to catch that above so default the value here
+    value = value or {}
+
+    if isinstance(value, dict):
+        invalid_keys = set(value.keys()) - set(CRONTAB_KEYS)
+        if invalid_keys:
+            raise ImproperlyConfigured(
+                f"Crontab value has invalid keys: {invalid_keys}"
+            )
+
+        return value
+    else:
+        raise ImproperlyConfigured(f"Crontab value is an invalid type: {type(value)}")
+
+
 class EnvParser:
     """Stateful tracker for environment variable parsing"""
 
     _env: Dict[str, str]
     _configured_vars: Dict[str, EnvVariable]
     _imported_modules: List[str]
 
@@ -377,24 +425,27 @@
                     scope[setting_name] = setting_value
 
     get_string = var_parser(parse_str)
     get_bool = var_parser(parse_bool)
     get_int = var_parser(parse_int)
     get_list_literal = var_parser(parse_list_literal)
     get_delimited_list = var_parser(parse_delimited_list)
+    get_crontab_kwargs = var_parser(parse_crontab_kwargs)
 
 
 env = EnvParser()
 
 # methods below are our exported module interface
 get_string = env.get_string
 get_int = env.get_int
 get_bool = env.get_bool
 get_list_literal = env.get_list_literal
 get_delimited_list = env.get_delimited_list
+get_crontab_kwargs = env.get_crontab_kwargs
+
 reload = env.reload
 validate = env.validate
 list_environment_vars = env.list_environment_vars
 get_features = env.get_features
 init_app_settings = env.init_app_settings
 app_namespaced = env.app_namespaced
 get_site_name = env.get_site_name
```

### Comparing `mitol-django-common-2.7.0/mitol/common/factories/defaults.py` & `mitol-django-common-2023.6.27.1/mitol/common/factories/defaults.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/management/commands/generate_app_json.py` & `mitol-django-common-2023.6.27.1/mitol/common/management/commands/generate_app_json.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/models.py` & `mitol-django-common-2023.6.27.1/mitol/common/models.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/pytest_utils.py` & `mitol-django-common-2023.6.27.1/mitol/common/pytest_utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/settings/webpack.py` & `mitol-django-common-2023.6.27.1/mitol/common/settings/webpack.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/templatetags/render_bundle.py` & `mitol-django-common-2023.6.27.1/mitol/common/templatetags/render_bundle.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/utils/base.py` & `mitol-django-common-2023.6.27.1/mitol/common/utils/base.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/utils/collections.py` & `mitol-django-common-2023.6.27.1/mitol/common/utils/collections.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/utils/datetime.py` & `mitol-django-common-2023.6.27.1/mitol/common/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/utils/http_requests.py` & `mitol-django-common-2023.6.27.1/mitol/common/utils/http_requests.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/utils/serializers.py` & `mitol-django-common-2023.6.27.1/mitol/common/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/utils/urls.py` & `mitol-django-common-2023.6.27.1/mitol/common/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol/common/utils/webpack.py` & `mitol-django-common-2023.6.27.1/mitol/common/utils/webpack.py`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/mitol_django_common.egg-info/PKG-INFO` & `mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-common
-Version: 2.7.0
+Version: 2023.6.27.1
 Summary: MIT Open Learning django app extensions for common utilities
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-common
 ---
 
 This is the Open Learning Django Common app. It provides common functionality used across all our applications.
```

### Comparing `mitol-django-common-2.7.0/mitol_django_common.egg-info/SOURCES.txt` & `mitol-django-common-2023.6.27.1/mitol_django_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-common-2.7.0/setup.py` & `mitol-django-common-2023.6.27.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ],
     'description': 'MIT Open Learning django app extensions for common utilities',
     'install_requires': (
         'django-redis~=5.0.0',
         'django-webpack-loader>=0.7.0',
         'django<4.0,>=2.2.12',
         'factory-boy~=3.2',
-        'pytest==6.1.2',
+        'pytest>=7.0.0',
         'pytz>=2020.4',
         'requests>=2.20.0',
         'setuptools',
         'typing-extensions',
     ),
     'license': 'BSD 3-Clause License',
     'long_description': """mitol-django-common
@@ -61,11 +61,11 @@
         'mitol.common.factories',
         'mitol.common.management',
         'mitol.common.management.commands',
         'mitol.common.settings',
         'mitol.common.templatetags',
         'mitol.common.utils',
     ),
-    'python_requires': '>=3.7',
-    'version': '2.7.0',
+    'python_requires': '>=3.8',
+    'version': '2023.6.27.1',
     'zip_safe': True,
 })
```

