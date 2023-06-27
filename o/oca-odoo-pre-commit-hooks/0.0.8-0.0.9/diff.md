# Comparing `tmp/oca-odoo-pre-commit-hooks-0.0.8.tar.gz` & `tmp/oca-odoo-pre-commit-hooks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oca-odoo-pre-commit-hooks-0.0.8.tar", last modified: Wed Oct 19 03:11:03 2022, max compression
+gzip compressed data, was "oca-odoo-pre-commit-hooks-0.0.9.tar", last modified: Wed Oct 19 05:30:18 2022, max compression
```

## Comparing `oca-odoo-pre-commit-hooks-0.0.8.tar` & `oca-odoo-pre-commit-hooks-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 03:11:03.433725 oca-odoo-pre-commit-hooks-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    21217 2022-10-19 03:11:03.433725 oca-odoo-pre-commit-hooks-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18666 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 03:11:03.433725 oca-odoo-pre-commit-hooks-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3102 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 03:11:03.425725 oca-odoo-pre-commit-hooks-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 03:11:03.429725 oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21217 2022-10-19 03:11:03.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-10-19 03:11:03.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 03:11:03.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-19 03:11:03.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 03:10:13.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-19 03:11:03.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-19 03:11:03.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 03:11:03.433725 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11374 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/checks_odoo_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/checks_odoo_module_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)    12111 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/checks_odoo_module_po.py
--rw-r--r--   0 runner    (1001) docker     (121)    14414 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/checks_odoo_module_xml.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-10-19 03:09:57.000000 oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 05:30:18.857122 oca-odoo-pre-commit-hooks-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    21255 2022-10-19 05:30:18.857122 oca-odoo-pre-commit-hooks-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18524 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 05:30:18.857122 oca-odoo-pre-commit-hooks-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3102 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 05:30:18.849122 oca-odoo-pre-commit-hooks-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 05:30:18.853122 oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    21255 2022-10-19 05:30:18.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-10-19 05:30:18.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 05:30:18.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-19 05:30:18.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 05:28:53.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-19 05:30:18.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-19 05:30:18.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 05:30:18.857122 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11430 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/checks_odoo_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/checks_odoo_module_csv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12111 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/checks_odoo_module_po.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14414 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/checks_odoo_module_xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-10-19 05:28:32.000000 oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/utils.py
```

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/LICENSE` & `oca-odoo-pre-commit-hooks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/PKG-INFO` & `oca-odoo-pre-commit-hooks-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oca-odoo-pre-commit-hooks
-Version: 0.0.8
+Version: 0.0.9
 Summary: odoo-pre-commit-hooks to use in pre-commit-config.yml files
 Home-page: https://github.com/OCA/odoo-pre-commit-hooks
 Author: Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: LGPL-3.0-or-later
 Project-URL: Issue Tracker, https://github.com/OCA/odoo-pre-commit-hooks/issues
 Keywords: pre-commit,OCA,Odoo Community Association,pre-commit-hook
@@ -28,15 +28,15 @@
 [//]: # (start-badges)
 
 [![Build Status](https://github.com/OCA/odoo-pre-commit-hooks/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/OCA/odoo-pre-commit-hooks/actions/workflows/test.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/OCA/odoo-pre-commit-hooks/branch/main/graph/badge.svg)](https://codecov.io/gh/OCA/odoo-pre-commit-hooks)
 [![version](https://img.shields.io/pypi/v/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
 [![wheel](https://img.shields.io/pypi/wheel/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
 [![supported-versions](https://img.shields.io/pypi/pyversions/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
-[![commits-since](https://img.shields.io/github/commits-since/OCA/odoo-pre-commit-hooks/v0.0.8.svg)](https://github.com/OCA/odoo-pre-commit-hooks/compare/v0.0.8...main)
+[![commits-since](https://img.shields.io/github/commits-since/OCA/odoo-pre-commit-hooks/v0.0.9.svg)](https://github.com/OCA/odoo-pre-commit-hooks/compare/v0.0.9...main)
 [![code-style-black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [//]: # (end-badges)
 
 # odoo-pre-commit-hooks
 
 OCA's custom pre-commit hooks for Odoo modules
@@ -56,27 +56,28 @@
 # Usage pre-commit-config.yaml
 
 Add to your ".pre-commit-config.yaml" configuration file the following input
 
 
 ```yaml
     - repo: https://github.com/OCA/odoo-pre-commit-hooks
-        rev: v0.0.8
+        rev: v0.0.9
         hooks:
         - id: oca-checks-odoo-module
 ```
 
 # Usage directly the entry points
 
 If you install directly the package use the entry point:
 
     oca-checks-odoo-module --help
 
 
 [//]: # (start-checks)
+
 # Checks
 
 * Check manifest-syntax-error
         Check if the manifest file has syntax error
 
 * Check missing-readme
         Check if a README file is missing
@@ -163,18 +164,20 @@
             <record id="xmlid_name1"...
                 <field name="field_name1"...
                 <field name="field_name1"...
 
 * Check xml-syntax-error
         Check syntax of XML files declared in the Odoo manifest
 
+
 [//]: # (end-checks)
 
 
 [//]: # (start-help)
+
 # Help
 ```bash
 usage: oca-checks-odoo-module [-h] [--no-verbose] [--no-exit]
                               [--disable DISABLE] [--enable ENABLE]
                               [filenames_or_modules [filenames_or_modules ...]]
 
 positional arguments:
@@ -189,161 +192,163 @@
                         separated by commas.
   --enable ENABLE, -e ENABLE
                         Enable the checker with the given 'check-name',
                         separated by commas. Default: All checks are enabled
                         by default
 
 ```
+
 [//]: # (end-help)
 
 
 [//]: # (start-example)
+
 # Examples
 
 
  * csv-duplicate-record-id
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/ir.model.access.csv#L5 Duplicate CSV record id "data/access_account_account_type" in test_repo/broken_module/ir.model.access.csv:6
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/ir.model.access.csv#L5 Duplicate CSV record id "data/access_account_account_type" in test_repo/broken_module/ir.model.access.csv:6
 
  * missing-readme
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
 
  * po-python-parse-printf
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L47 Translation string couldn't be parsed correctly using str%variables TypeError('not all arguments converted during string formatting')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L83 Translation string couldn't be parsed correctly using str%variables TypeError('%d format: a number is required, not str')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L47 Translation string couldn't be parsed correctly using str%variables TypeError('not all arguments converted during string formatting')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L83 Translation string couldn't be parsed correctly using str%variables TypeError('%d format: a number is required, not str')
 
  * po-python-parse-format
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L53 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L59 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L65 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L71 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L53 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L59 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L65 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L71 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
 
  * po-duplicate-message-definition
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L17 Duplicate PO message definition "Branch" in lines 23, 29
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L35 Duplicate PO message definition "Message id toooooooooooooooooooooooooooo..." in lines 41
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L65 Duplicate PO message definition "One variable {variable1}" in lines 71
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L17 Duplicate PO message definition "Branch" in lines 23, 29
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L35 Duplicate PO message definition "Message id toooooooooooooooooooooooooooo..." in lines 41
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L65 Duplicate PO message definition "One variable {variable1}" in lines 71
 
  * po-requires-module
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/broken_module.pot#L14 Translation entry requires comment '#. module: MODULE'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/broken_module.pot#L14 Translation entry requires comment '#. module: MODULE'
 
  * xml-dangerous-qweb-replace-low-priority
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L17 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L17 Dangerous use of "replace" from view with priority 0 < 99
 
  * xml-deprecated-data-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check.xml#L3 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check_3.xml#L4 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/demo/duplicated_id_demo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check.xml#L3 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check_3.xml#L4 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/demo/duplicated_id_demo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
 
  * xml-deprecated-openerp-xml-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check_2.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check_2.xml#L2 Deprecated <openerp> xml node
 
  * xml-redundant-module-name
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L15 Redundant module name <record id="broken_module.view_model_form2" better using only <record id="view_model_form2"
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L15 Redundant module name <record id="broken_module.view_model_form2" better using only <record id="view_model_form2"
 
  * xml-view-dangerous-replace-low-priority
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L25 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L37 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L47 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L70 Dangerous use of "replace" from view with priority 10 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L92 Dangerous use of "replace" from view with priority 10 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L108 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L25 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L37 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L47 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L70 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L92 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L108 Dangerous use of "replace" from view with priority 10 < 99
 
  * xml-deprecated-tree-attribute
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L31 Deprecated "<tree string=..."
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L42 Deprecated "<tree colors=..."
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L53 Deprecated "<tree fonts=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L31 Deprecated "<tree string=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L42 Deprecated "<tree colors=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L53 Deprecated "<tree fonts=..."
 
  * xml-dangerous-filter-wo-user
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L60 Dangerous filter without explicit `user_id`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L60 Dangerous filter without explicit `user_id`
 
  * xml-duplicate-record-id
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L5 Duplicate xml record id "data/view_model_form_noupdate_0" in test_repo/broken_module/model_view_odoo.xml:5, test_repo/broken_module/model_view_odoo2.xml:5
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L5 Duplicate xml record id "data/view_model_form2_noupdate_0" in test_repo/broken_module/model_view_odoo2.xml:17
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L103 Duplicate xml record id "data/view_model_form80_noupdate_0" in test_repo/broken_module/skip_xml_check.xml:5, test_repo/broken_module/skip_xml_check.xml:9, test_repo/broken_module/skip_xml_check_3.xml:6, test_repo/broken_module/skip_xml_check_3.xml:10
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L5 Duplicate xml record id "data/view_model_form_noupdate_0" in test_repo/broken_module/model_view_odoo.xml:5, test_repo/broken_module/model_view_odoo2.xml:5
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L5 Duplicate xml record id "data/view_model_form2_noupdate_0" in test_repo/broken_module/model_view_odoo2.xml:17
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L103 Duplicate xml record id "data/view_model_form80_noupdate_0" in test_repo/broken_module/skip_xml_check.xml:5, test_repo/broken_module/skip_xml_check.xml:9, test_repo/broken_module/skip_xml_check_3.xml:6, test_repo/broken_module/skip_xml_check_3.xml:10
 
  * xml-duplicate-fields
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L6 Duplicate xml field "name" in lines 13
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L41 Duplicate xml field "key_config" in lines 42
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L73 Duplicate xml field "arch" in lines 76
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L79 Duplicate xml field "user_id" in lines 81
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L80 Duplicate xml field "name" in lines 83
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L90 Duplicate xml field "date" in lines 93
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L91 Duplicate xml field "min_date" in lines 94
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L132 Duplicate xml field "name" in lines 133
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L138 Duplicate xml field "name" in lines 139
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L6 Duplicate xml field "name" in lines 13
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L41 Duplicate xml field "key_config" in lines 42
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L73 Duplicate xml field "arch" in lines 76
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L79 Duplicate xml field "user_id" in lines 81
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L80 Duplicate xml field "name" in lines 83
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L90 Duplicate xml field "date" in lines 93
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L91 Duplicate xml field "min_date" in lines 94
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L132 Duplicate xml field "name" in lines 133
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L138 Duplicate xml field "name" in lines 139
 
  * xml-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
 
  * manifest-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/manifest_werror/__manifest__.py#L1 could not be loaded Manifest /Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/manifest_werror/__manifest__.py with error malformed node or string: <_ast.Name object at 0x10ef69070>
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/manifest_werror/__manifest__.py#L1 could not be loaded manifest malformed
 
  * csv-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/ir.model.access.csv#L1 'utf-8' codec can't decode byte 0xf1 in position 47: invalid continuation byte
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/ir.model.access.csv#L1 'utf-8' codec can't decode byte 0xf1 in position 47: invalid continuation byte
 
  * missing-readme
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
 
  * po-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/i18n/es.po#L1 Syntax error in po file (line 19)
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/i18n/es.po#L1 Syntax error in po file (line 19)
 
  * xml-deprecated-data-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
 
  * xml-deprecated-openerp-xml-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/res_users.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/model_view.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/res_users.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/model_view.xml#L2 Deprecated <openerp> xml node
 
  * xml-deprecated-qweb-directive
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L7 Deprecated QWeb directive "t-esc-options". Use "t-options" instead
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L14 Deprecated QWeb directive "t-field-options". Use "t-options" instead
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L7 Deprecated QWeb directive "t-esc-options". Use "t-options" instead
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L14 Deprecated QWeb directive "t-field-options". Use "t-options" instead
 
  * xml-not-valid-char-link
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L21 The resource in in src/href contains a not valid character
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L23 The resource in in src/href contains a not valid character
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L21 The resource in in src/href contains a not valid character
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L23 The resource in in src/href contains a not valid character
 
  * xml-create-user-wo-reset-password
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/res_users.xml#L10 record res.users without context="{'no_reset_password': True}"
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/res_users.xml#L10 record res.users without context="{'no_reset_password': True}"
 
  * manifest-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/woinit_module/__manifest__.py#L1 could not be loaded
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/woinit_module/__manifest__.py#L1 could not be loaded
 
 [//]: # (end-example)
 
 ## Licenses
 
 This repository is licensed under [AGPL-3.0](LICENSE).
 
@@ -351,14 +356,21 @@
 OCA, or the [Odoo Community Association](http://odoo-community.org/), is a nonprofit
 organization whose mission is to support the collaborative development of Odoo features
 and promote its widespread use.
 
 CHANGES
 =======
 
+v0.0.9
+------
+
+* Bump version: 0.0.8 → 0.0.9
+* [FIX] README: Fix regex to replace autogenerated content (#18)
+* [REF] README: Detect from CI if README needs to be updated (#17)
+
 v0.0.8
 ------
 
 * Bump version: 0.0.7 → 0.0.8
 * [REF] README: Add examples of checks section and script to auto-generate it (#16)
 * [REF] README: Add help section and script to auto-generate it (#15)
```

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/README.md` & `oca-odoo-pre-commit-hooks-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [//]: # (start-badges)
 
 [![Build Status](https://github.com/OCA/odoo-pre-commit-hooks/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/OCA/odoo-pre-commit-hooks/actions/workflows/test.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/OCA/odoo-pre-commit-hooks/branch/main/graph/badge.svg)](https://codecov.io/gh/OCA/odoo-pre-commit-hooks)
 [![version](https://img.shields.io/pypi/v/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
 [![wheel](https://img.shields.io/pypi/wheel/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
 [![supported-versions](https://img.shields.io/pypi/pyversions/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
-[![commits-since](https://img.shields.io/github/commits-since/OCA/odoo-pre-commit-hooks/v0.0.8.svg)](https://github.com/OCA/odoo-pre-commit-hooks/compare/v0.0.8...main)
+[![commits-since](https://img.shields.io/github/commits-since/OCA/odoo-pre-commit-hooks/v0.0.9.svg)](https://github.com/OCA/odoo-pre-commit-hooks/compare/v0.0.9...main)
 [![code-style-black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [//]: # (end-badges)
 
 # odoo-pre-commit-hooks
 
 OCA's custom pre-commit hooks for Odoo modules
@@ -29,27 +29,28 @@
 # Usage pre-commit-config.yaml
 
 Add to your ".pre-commit-config.yaml" configuration file the following input
 
 
 ```yaml
     - repo: https://github.com/OCA/odoo-pre-commit-hooks
-        rev: v0.0.8
+        rev: v0.0.9
         hooks:
         - id: oca-checks-odoo-module
 ```
 
 # Usage directly the entry points
 
 If you install directly the package use the entry point:
 
     oca-checks-odoo-module --help
 
 
 [//]: # (start-checks)
+
 # Checks
 
 * Check manifest-syntax-error
         Check if the manifest file has syntax error
 
 * Check missing-readme
         Check if a README file is missing
@@ -136,18 +137,20 @@
             <record id="xmlid_name1"...
                 <field name="field_name1"...
                 <field name="field_name1"...
 
 * Check xml-syntax-error
         Check syntax of XML files declared in the Odoo manifest
 
+
 [//]: # (end-checks)
 
 
 [//]: # (start-help)
+
 # Help
 ```bash
 usage: oca-checks-odoo-module [-h] [--no-verbose] [--no-exit]
                               [--disable DISABLE] [--enable ENABLE]
                               [filenames_or_modules [filenames_or_modules ...]]
 
 positional arguments:
@@ -162,161 +165,163 @@
                         separated by commas.
   --enable ENABLE, -e ENABLE
                         Enable the checker with the given 'check-name',
                         separated by commas. Default: All checks are enabled
                         by default
 
 ```
+
 [//]: # (end-help)
 
 
 [//]: # (start-example)
+
 # Examples
 
 
  * csv-duplicate-record-id
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/ir.model.access.csv#L5 Duplicate CSV record id "data/access_account_account_type" in test_repo/broken_module/ir.model.access.csv:6
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/ir.model.access.csv#L5 Duplicate CSV record id "data/access_account_account_type" in test_repo/broken_module/ir.model.access.csv:6
 
  * missing-readme
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
 
  * po-python-parse-printf
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L47 Translation string couldn't be parsed correctly using str%variables TypeError('not all arguments converted during string formatting')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L83 Translation string couldn't be parsed correctly using str%variables TypeError('%d format: a number is required, not str')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L47 Translation string couldn't be parsed correctly using str%variables TypeError('not all arguments converted during string formatting')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L83 Translation string couldn't be parsed correctly using str%variables TypeError('%d format: a number is required, not str')
 
  * po-python-parse-format
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L53 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L59 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L65 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L71 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L53 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L59 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L65 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L71 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
 
  * po-duplicate-message-definition
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L17 Duplicate PO message definition "Branch" in lines 23, 29
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L35 Duplicate PO message definition "Message id toooooooooooooooooooooooooooo..." in lines 41
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L65 Duplicate PO message definition "One variable {variable1}" in lines 71
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L17 Duplicate PO message definition "Branch" in lines 23, 29
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L35 Duplicate PO message definition "Message id toooooooooooooooooooooooooooo..." in lines 41
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L65 Duplicate PO message definition "One variable {variable1}" in lines 71
 
  * po-requires-module
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/broken_module.pot#L14 Translation entry requires comment '#. module: MODULE'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/broken_module.pot#L14 Translation entry requires comment '#. module: MODULE'
 
  * xml-dangerous-qweb-replace-low-priority
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L17 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L17 Dangerous use of "replace" from view with priority 0 < 99
 
  * xml-deprecated-data-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check.xml#L3 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check_3.xml#L4 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/demo/duplicated_id_demo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check.xml#L3 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check_3.xml#L4 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/demo/duplicated_id_demo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
 
  * xml-deprecated-openerp-xml-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check_2.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check_2.xml#L2 Deprecated <openerp> xml node
 
  * xml-redundant-module-name
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L15 Redundant module name <record id="broken_module.view_model_form2" better using only <record id="view_model_form2"
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L15 Redundant module name <record id="broken_module.view_model_form2" better using only <record id="view_model_form2"
 
  * xml-view-dangerous-replace-low-priority
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L25 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L37 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L47 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L70 Dangerous use of "replace" from view with priority 10 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L92 Dangerous use of "replace" from view with priority 10 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L108 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L25 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L37 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L47 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L70 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L92 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L108 Dangerous use of "replace" from view with priority 10 < 99
 
  * xml-deprecated-tree-attribute
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L31 Deprecated "<tree string=..."
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L42 Deprecated "<tree colors=..."
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L53 Deprecated "<tree fonts=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L31 Deprecated "<tree string=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L42 Deprecated "<tree colors=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L53 Deprecated "<tree fonts=..."
 
  * xml-dangerous-filter-wo-user
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L60 Dangerous filter without explicit `user_id`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L60 Dangerous filter without explicit `user_id`
 
  * xml-duplicate-record-id
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L5 Duplicate xml record id "data/view_model_form_noupdate_0" in test_repo/broken_module/model_view_odoo.xml:5, test_repo/broken_module/model_view_odoo2.xml:5
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L5 Duplicate xml record id "data/view_model_form2_noupdate_0" in test_repo/broken_module/model_view_odoo2.xml:17
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L103 Duplicate xml record id "data/view_model_form80_noupdate_0" in test_repo/broken_module/skip_xml_check.xml:5, test_repo/broken_module/skip_xml_check.xml:9, test_repo/broken_module/skip_xml_check_3.xml:6, test_repo/broken_module/skip_xml_check_3.xml:10
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L5 Duplicate xml record id "data/view_model_form_noupdate_0" in test_repo/broken_module/model_view_odoo.xml:5, test_repo/broken_module/model_view_odoo2.xml:5
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L5 Duplicate xml record id "data/view_model_form2_noupdate_0" in test_repo/broken_module/model_view_odoo2.xml:17
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L103 Duplicate xml record id "data/view_model_form80_noupdate_0" in test_repo/broken_module/skip_xml_check.xml:5, test_repo/broken_module/skip_xml_check.xml:9, test_repo/broken_module/skip_xml_check_3.xml:6, test_repo/broken_module/skip_xml_check_3.xml:10
 
  * xml-duplicate-fields
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L6 Duplicate xml field "name" in lines 13
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L41 Duplicate xml field "key_config" in lines 42
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L73 Duplicate xml field "arch" in lines 76
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L79 Duplicate xml field "user_id" in lines 81
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L80 Duplicate xml field "name" in lines 83
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L90 Duplicate xml field "date" in lines 93
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L91 Duplicate xml field "min_date" in lines 94
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L132 Duplicate xml field "name" in lines 133
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L138 Duplicate xml field "name" in lines 139
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L6 Duplicate xml field "name" in lines 13
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L41 Duplicate xml field "key_config" in lines 42
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L73 Duplicate xml field "arch" in lines 76
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L79 Duplicate xml field "user_id" in lines 81
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L80 Duplicate xml field "name" in lines 83
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L90 Duplicate xml field "date" in lines 93
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L91 Duplicate xml field "min_date" in lines 94
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L132 Duplicate xml field "name" in lines 133
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L138 Duplicate xml field "name" in lines 139
 
  * xml-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
 
  * manifest-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/manifest_werror/__manifest__.py#L1 could not be loaded Manifest /Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/manifest_werror/__manifest__.py with error malformed node or string: <_ast.Name object at 0x10ef69070>
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/manifest_werror/__manifest__.py#L1 could not be loaded manifest malformed
 
  * csv-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/ir.model.access.csv#L1 'utf-8' codec can't decode byte 0xf1 in position 47: invalid continuation byte
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/ir.model.access.csv#L1 'utf-8' codec can't decode byte 0xf1 in position 47: invalid continuation byte
 
  * missing-readme
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
 
  * po-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/i18n/es.po#L1 Syntax error in po file (line 19)
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/i18n/es.po#L1 Syntax error in po file (line 19)
 
  * xml-deprecated-data-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
 
  * xml-deprecated-openerp-xml-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/res_users.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/model_view.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/res_users.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/model_view.xml#L2 Deprecated <openerp> xml node
 
  * xml-deprecated-qweb-directive
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L7 Deprecated QWeb directive "t-esc-options". Use "t-options" instead
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L14 Deprecated QWeb directive "t-field-options". Use "t-options" instead
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L7 Deprecated QWeb directive "t-esc-options". Use "t-options" instead
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L14 Deprecated QWeb directive "t-field-options". Use "t-options" instead
 
  * xml-not-valid-char-link
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L21 The resource in in src/href contains a not valid character
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L23 The resource in in src/href contains a not valid character
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L21 The resource in in src/href contains a not valid character
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L23 The resource in in src/href contains a not valid character
 
  * xml-create-user-wo-reset-password
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/res_users.xml#L10 record res.users without context="{'no_reset_password': True}"
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/res_users.xml#L10 record res.users without context="{'no_reset_password': True}"
 
  * manifest-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/woinit_module/__manifest__.py#L1 could not be loaded
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/woinit_module/__manifest__.py#L1 could not be loaded
 
 [//]: # (end-example)
 
 ## Licenses
 
 This repository is licensed under [AGPL-3.0](LICENSE).
```

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/setup.py` & `oca-odoo-pre-commit-hooks-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", generate_changelog()),
     )
     return long_description
 
 
 setup(
     name="oca-odoo-pre-commit-hooks",
-    version="0.0.8",
+    version="0.0.9",
     license="LGPL-3.0-or-later",
     description="odoo-pre-commit-hooks to use in pre-commit-config.yml files",
     long_description=generage_long_description(),
     long_description_content_type="text/markdown",
     author="Odoo Community Association (OCA)",
     author_email="support@odoo-community.org",
     url="https://github.com/OCA/odoo-pre-commit-hooks",
```

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/PKG-INFO` & `oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oca-odoo-pre-commit-hooks
-Version: 0.0.8
+Version: 0.0.9
 Summary: odoo-pre-commit-hooks to use in pre-commit-config.yml files
 Home-page: https://github.com/OCA/odoo-pre-commit-hooks
 Author: Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: LGPL-3.0-or-later
 Project-URL: Issue Tracker, https://github.com/OCA/odoo-pre-commit-hooks/issues
 Keywords: pre-commit,OCA,Odoo Community Association,pre-commit-hook
@@ -28,15 +28,15 @@
 [//]: # (start-badges)
 
 [![Build Status](https://github.com/OCA/odoo-pre-commit-hooks/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/OCA/odoo-pre-commit-hooks/actions/workflows/test.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/OCA/odoo-pre-commit-hooks/branch/main/graph/badge.svg)](https://codecov.io/gh/OCA/odoo-pre-commit-hooks)
 [![version](https://img.shields.io/pypi/v/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
 [![wheel](https://img.shields.io/pypi/wheel/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
 [![supported-versions](https://img.shields.io/pypi/pyversions/oca-odoo-pre-commit-hooks.svg)](https://pypi.org/project/oca-odoo-pre-commit-hooks)
-[![commits-since](https://img.shields.io/github/commits-since/OCA/odoo-pre-commit-hooks/v0.0.8.svg)](https://github.com/OCA/odoo-pre-commit-hooks/compare/v0.0.8...main)
+[![commits-since](https://img.shields.io/github/commits-since/OCA/odoo-pre-commit-hooks/v0.0.9.svg)](https://github.com/OCA/odoo-pre-commit-hooks/compare/v0.0.9...main)
 [![code-style-black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [//]: # (end-badges)
 
 # odoo-pre-commit-hooks
 
 OCA's custom pre-commit hooks for Odoo modules
@@ -56,27 +56,28 @@
 # Usage pre-commit-config.yaml
 
 Add to your ".pre-commit-config.yaml" configuration file the following input
 
 
 ```yaml
     - repo: https://github.com/OCA/odoo-pre-commit-hooks
-        rev: v0.0.8
+        rev: v0.0.9
         hooks:
         - id: oca-checks-odoo-module
 ```
 
 # Usage directly the entry points
 
 If you install directly the package use the entry point:
 
     oca-checks-odoo-module --help
 
 
 [//]: # (start-checks)
+
 # Checks
 
 * Check manifest-syntax-error
         Check if the manifest file has syntax error
 
 * Check missing-readme
         Check if a README file is missing
@@ -163,18 +164,20 @@
             <record id="xmlid_name1"...
                 <field name="field_name1"...
                 <field name="field_name1"...
 
 * Check xml-syntax-error
         Check syntax of XML files declared in the Odoo manifest
 
+
 [//]: # (end-checks)
 
 
 [//]: # (start-help)
+
 # Help
 ```bash
 usage: oca-checks-odoo-module [-h] [--no-verbose] [--no-exit]
                               [--disable DISABLE] [--enable ENABLE]
                               [filenames_or_modules [filenames_or_modules ...]]
 
 positional arguments:
@@ -189,161 +192,163 @@
                         separated by commas.
   --enable ENABLE, -e ENABLE
                         Enable the checker with the given 'check-name',
                         separated by commas. Default: All checks are enabled
                         by default
 
 ```
+
 [//]: # (end-help)
 
 
 [//]: # (start-example)
+
 # Examples
 
 
  * csv-duplicate-record-id
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/ir.model.access.csv#L5 Duplicate CSV record id "data/access_account_account_type" in test_repo/broken_module/ir.model.access.csv:6
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/ir.model.access.csv#L5 Duplicate CSV record id "data/access_account_account_type" in test_repo/broken_module/ir.model.access.csv:6
 
  * missing-readme
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
 
  * po-python-parse-printf
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L47 Translation string couldn't be parsed correctly using str%variables TypeError('not all arguments converted during string formatting')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L83 Translation string couldn't be parsed correctly using str%variables TypeError('%d format: a number is required, not str')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L47 Translation string couldn't be parsed correctly using str%variables TypeError('not all arguments converted during string formatting')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L83 Translation string couldn't be parsed correctly using str%variables TypeError('%d format: a number is required, not str')
 
  * po-python-parse-format
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L53 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L59 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L65 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L71 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L53 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L59 Translation string couldn't be parsed correctly using str.format IndexError('Replacement index 1 out of range for positional args tuple')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L65 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L71 Translation string couldn't be parsed correctly using str.format KeyError('variable2')
 
  * po-duplicate-message-definition
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L17 Duplicate PO message definition "Branch" in lines 23, 29
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L35 Duplicate PO message definition "Message id toooooooooooooooooooooooooooo..." in lines 41
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/es.po#L65 Duplicate PO message definition "One variable {variable1}" in lines 71
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L17 Duplicate PO message definition "Branch" in lines 23, 29
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L35 Duplicate PO message definition "Message id toooooooooooooooooooooooooooo..." in lines 41
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/es.po#L65 Duplicate PO message definition "One variable {variable1}" in lines 71
 
  * po-requires-module
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/i18n/broken_module.pot#L14 Translation entry requires comment '#. module: MODULE'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/i18n/broken_module.pot#L14 Translation entry requires comment '#. module: MODULE'
 
  * xml-dangerous-qweb-replace-low-priority
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/template1.xml#L17 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L3 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/template1.xml#L17 Dangerous use of "replace" from view with priority 0 < 99
 
  * xml-deprecated-data-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check.xml#L3 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check_3.xml#L4 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/demo/duplicated_id_demo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check.xml#L3 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check_3.xml#L4 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/demo/duplicated_id_demo.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
 
  * xml-deprecated-openerp-xml-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/skip_xml_check_2.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/skip_xml_check_2.xml#L2 Deprecated <openerp> xml node
 
  * xml-redundant-module-name
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L15 Redundant module name <record id="broken_module.view_model_form2" better using only <record id="view_model_form2"
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L15 Redundant module name <record id="broken_module.view_model_form2" better using only <record id="view_model_form2"
 
  * xml-view-dangerous-replace-low-priority
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L25 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L37 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L47 Dangerous use of "replace" from view with priority 0 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L70 Dangerous use of "replace" from view with priority 10 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L92 Dangerous use of "replace" from view with priority 10 < 99
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L108 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L25 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L37 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L47 Dangerous use of "replace" from view with priority 0 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L70 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L92 Dangerous use of "replace" from view with priority 10 < 99
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L108 Dangerous use of "replace" from view with priority 10 < 99
 
  * xml-deprecated-tree-attribute
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L31 Deprecated "<tree string=..."
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L42 Deprecated "<tree colors=..."
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L53 Deprecated "<tree fonts=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L31 Deprecated "<tree string=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L42 Deprecated "<tree colors=..."
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L53 Deprecated "<tree fonts=..."
 
  * xml-dangerous-filter-wo-user
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo.xml#L60 Dangerous filter without explicit `user_id`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo.xml#L60 Dangerous filter without explicit `user_id`
 
  * xml-duplicate-record-id
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view.xml#L5 Duplicate xml record id "data/view_model_form_noupdate_0" in test_repo/broken_module/model_view_odoo.xml:5, test_repo/broken_module/model_view_odoo2.xml:5
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L5 Duplicate xml record id "data/view_model_form2_noupdate_0" in test_repo/broken_module/model_view_odoo2.xml:17
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view2.xml#L103 Duplicate xml record id "data/view_model_form80_noupdate_0" in test_repo/broken_module/skip_xml_check.xml:5, test_repo/broken_module/skip_xml_check.xml:9, test_repo/broken_module/skip_xml_check_3.xml:6, test_repo/broken_module/skip_xml_check_3.xml:10
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view.xml#L5 Duplicate xml record id "data/view_model_form_noupdate_0" in test_repo/broken_module/model_view_odoo.xml:5, test_repo/broken_module/model_view_odoo2.xml:5
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L5 Duplicate xml record id "data/view_model_form2_noupdate_0" in test_repo/broken_module/model_view_odoo2.xml:17
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view2.xml#L103 Duplicate xml record id "data/view_model_form80_noupdate_0" in test_repo/broken_module/skip_xml_check.xml:5, test_repo/broken_module/skip_xml_check.xml:9, test_repo/broken_module/skip_xml_check_3.xml:6, test_repo/broken_module/skip_xml_check_3.xml:10
 
  * xml-duplicate-fields
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L6 Duplicate xml field "name" in lines 13
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L41 Duplicate xml field "key_config" in lines 42
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L73 Duplicate xml field "arch" in lines 76
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L79 Duplicate xml field "user_id" in lines 81
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L80 Duplicate xml field "name" in lines 83
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L90 Duplicate xml field "date" in lines 93
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L91 Duplicate xml field "min_date" in lines 94
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L132 Duplicate xml field "name" in lines 133
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/model_view_odoo2.xml#L138 Duplicate xml field "name" in lines 139
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L6 Duplicate xml field "name" in lines 13
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L41 Duplicate xml field "key_config" in lines 42
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L73 Duplicate xml field "arch" in lines 76
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L79 Duplicate xml field "user_id" in lines 81
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L80 Duplicate xml field "name" in lines 83
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L90 Duplicate xml field "date" in lines 93
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L91 Duplicate xml field "min_date" in lines 94
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L132 Duplicate xml field "name" in lines 133
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/model_view_odoo2.xml#L138 Duplicate xml field "name" in lines 139
 
  * xml-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/broken_module/file_no_exist.xml#L1 [Errno 2] No such file or directory: '/Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/broken_module/file_no_exist.xml'
 
  * manifest-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/manifest_werror/__manifest__.py#L1 could not be loaded Manifest /Users/moylop260/odoo/odoo-pre-commit-hooks/test_repo/manifest_werror/__manifest__.py with error malformed node or string: <_ast.Name object at 0x10ef69070>
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/manifest_werror/__manifest__.py#L1 could not be loaded manifest malformed
 
  * csv-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/ir.model.access.csv#L1 'utf-8' codec can't decode byte 0xf1 in position 47: invalid continuation byte
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/ir.model.access.csv#L1 'utf-8' codec can't decode byte 0xf1 in position 47: invalid continuation byte
 
  * missing-readme
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/README.rst#L1 missed file. Template here: https://github.com/OCA/maintainer-tools/blob/master/template/module/README.rst
 
  * po-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/syntax_err_module/i18n/es.po#L1 Syntax error in po file (line 19)
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/syntax_err_module/i18n/es.po#L1 Syntax error in po file (line 19)
 
  * xml-deprecated-data-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/model_view.xml#L2 Use `<odoo>` instead of `<odoo><data>` or use `<odoo noupdate="1">` instead of `<odoo><data noupdate="1">`
 
  * xml-deprecated-openerp-xml-node
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/res_users.xml#L2 Deprecated <openerp> xml node
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/model_view.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/res_users.xml#L2 Deprecated <openerp> xml node
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/model_view.xml#L2 Deprecated <openerp> xml node
 
  * xml-deprecated-qweb-directive
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L7 Deprecated QWeb directive "t-esc-options". Use "t-options" instead
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L14 Deprecated QWeb directive "t-field-options". Use "t-options" instead
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L7 Deprecated QWeb directive "t-esc-options". Use "t-options" instead
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L14 Deprecated QWeb directive "t-field-options". Use "t-options" instead
 
  * xml-not-valid-char-link
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L21 The resource in in src/href contains a not valid character
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/website_templates.xml#L23 The resource in in src/href contains a not valid character
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L21 The resource in in src/href contains a not valid character
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/website_templates.xml#L23 The resource in in src/href contains a not valid character
 
  * xml-create-user-wo-reset-password
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/test_module/res_users.xml#L10 record res.users without context="{'no_reset_password': True}"
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/test_module/res_users.xml#L10 record res.users without context="{'no_reset_password': True}"
 
  * manifest-syntax-error
 
-    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.8/test_repo/woinit_module/__manifest__.py#L1 could not be loaded
+    - https://github.com/OCA/odoo-pre-commit-hooks/blob/v0.0.9/test_repo/woinit_module/__manifest__.py#L1 could not be loaded
 
 [//]: # (end-example)
 
 ## Licenses
 
 This repository is licensed under [AGPL-3.0](LICENSE).
 
@@ -351,14 +356,21 @@
 OCA, or the [Odoo Community Association](http://odoo-community.org/), is a nonprofit
 organization whose mission is to support the collaborative development of Odoo features
 and promote its widespread use.
 
 CHANGES
 =======
 
+v0.0.9
+------
+
+* Bump version: 0.0.8 → 0.0.9
+* [FIX] README: Fix regex to replace autogenerated content (#18)
+* [REF] README: Detect from CI if README needs to be updated (#17)
+
 v0.0.8
 ------
 
 * Bump version: 0.0.7 → 0.0.8
 * [REF] README: Add examples of checks section and script to auto-generate it (#16)
 * [REF] README: Add help section and script to auto-generate it (#15)
```

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/src/oca_odoo_pre_commit_hooks.egg-info/SOURCES.txt` & `oca-odoo-pre-commit-hooks-0.0.9/src/oca_odoo_pre_commit_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/checks_odoo_module.py` & `oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/checks_odoo_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,17 @@
         if not os.path.isfile(os.path.join(self.odoo_addon_path, "__init__.py")):
             self.print(f"The path {self.manifest_path} does not have __init__.py file")
             return {}
         with open(self.manifest_path, "r", encoding="UTF-8") as f_manifest:
             try:
                 return ast.literal_eval(f_manifest.read())
             # Using same way than odoo
-            except BaseException as err:  # pylint: disable=broad-except
-                self.error = f"Manifest {self.manifest_path} with error {err}"
+            except BaseException:  # pylint: disable=broad-except
+                # Not use "exception error" string because it return mutable memory numbers
+                self.error = "manifest malformed"
         return {}
 
     def _is_installable(self):
         return self.manifest_dict and self.manifest_dict.get("installable", True)
 
     def _referenced_files_by_extension(self):
         ext_referenced_files = defaultdict(list)
```

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/checks_odoo_module_csv.py` & `oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/checks_odoo_module_csv.py`

 * *Files identical despite different names*

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/checks_odoo_module_po.py` & `oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/checks_odoo_module_po.py`

 * *Files identical despite different names*

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/checks_odoo_module_xml.py` & `oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/checks_odoo_module_xml.py`

 * *Files identical despite different names*

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/cli.py` & `oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/cli.py`

 * *Files identical despite different names*

### Comparing `oca-odoo-pre-commit-hooks-0.0.8/src/oca_pre_commit_hooks/utils.py` & `oca-odoo-pre-commit-hooks-0.0.9/src/oca_pre_commit_hooks/utils.py`

 * *Files identical despite different names*

