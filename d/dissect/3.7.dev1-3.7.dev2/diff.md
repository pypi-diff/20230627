# Comparing `tmp/dissect-3.7.dev1.tar.gz` & `tmp/dissect-3.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect-3.7.dev1.tar", last modified: Fri Jun 16 12:48:28 2023, max compression
+gzip compressed data, was "dissect-3.7.dev2.tar", last modified: Tue Jun 27 07:49:47 2023, max compression
```

## Comparing `dissect-3.7.dev1.tar` & `dissect-3.7.dev2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:28.847288 dissect-3.7.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-16 12:48:15.000000 dissect-3.7.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:48:15.000000 dissect-3.7.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:15.000000 dissect-3.7.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-16 12:48:28.847288 dissect-3.7.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-16 12:48:15.000000 dissect-3.7.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:28.847288 dissect-3.7.dev1/dissect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:28.000000 dissect-3.7.dev1/dissect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-16 12:48:19.000000 dissect-3.7.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:48:28.847288 dissect-3.7.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-16 12:48:15.000000 dissect-3.7.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:47.769994 dissect-3.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 07:49:30.000000 dissect-3.7.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:49:30.000000 dissect-3.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:49:30.000000 dissect-3.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-27 07:49:47.765994 dissect-3.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-27 07:49:30.000000 dissect-3.7.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:47.765994 dissect-3.7.dev2/dissect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-27 07:49:35.000000 dissect-3.7.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:47.769994 dissect-3.7.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-27 07:49:30.000000 dissect-3.7.dev2/tox.ini
```

### Comparing `dissect-3.7.dev1/LICENSE` & `dissect-3.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect-3.7.dev1/PKG-INFO` & `dissect-3.7.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.7.dev1
+Version: 3.7.dev2
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect-3.7.dev1/README.md` & `dissect-3.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect-3.7.dev1/dissect.egg-info/PKG-INFO` & `dissect-3.7.dev2/dissect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.7.dev1
+Version: 3.7.dev2
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect-3.7.dev1/pyproject.toml` & `dissect-3.7.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect-3.7.dev1/tox.ini` & `dissect-3.7.dev2/tox.ini`

 * *Files identical despite different names*

