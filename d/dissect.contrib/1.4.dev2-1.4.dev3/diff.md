# Comparing `tmp/dissect.contrib-1.4.dev2.tar.gz` & `tmp/dissect.contrib-1.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.contrib-1.4.dev2.tar", last modified: Thu Jun 22 14:33:33 2023, max compression
+gzip compressed data, was "dissect.contrib-1.4.dev3.tar", last modified: Tue Jun 27 07:48:42 2023, max compression
```

## Comparing `dissect.contrib-1.4.dev2.tar` & `dissect.contrib-1.4.dev3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.076774 dissect.contrib-1.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-22 14:33:33.076774 dissect.contrib-1.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.072774 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-22 14:33:33.000000 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 14:33:33.000000 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:33:33.000000 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:33:33.000000 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-22 14:33:21.000000 dissect.contrib-1.4.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:33:33.076774 dissect.contrib-1.4.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.072774 dissect.contrib-1.4.dev2/template/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.068773 dissect.contrib-1.4.dev2/template/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.068773 dissect.contrib-1.4.dev2/template/dissect/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.076774 dissect.contrib-1.4.dev2/template/dissect/contrib/template/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/template/dissect/contrib/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:42.535696 dissect.contrib-1.4.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-27 07:48:42.535696 dissect.contrib-1.4.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:42.531696 dissect.contrib-1.4.dev3/dissect.contrib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-27 07:48:42.000000 dissect.contrib-1.4.dev3/dissect.contrib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-27 07:48:42.000000 dissect.contrib-1.4.dev3/dissect.contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:48:42.000000 dissect.contrib-1.4.dev3/dissect.contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:48:42.000000 dissect.contrib-1.4.dev3/dissect.contrib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-27 07:48:31.000000 dissect.contrib-1.4.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:48:42.535696 dissect.contrib-1.4.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:42.531696 dissect.contrib-1.4.dev3/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:42.527696 dissect.contrib-1.4.dev3/template/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:42.527696 dissect.contrib-1.4.dev3/template/dissect/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:42.535696 dissect.contrib-1.4.dev3/template/dissect/contrib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/template/dissect/contrib/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-27 07:48:25.000000 dissect.contrib-1.4.dev3/tox.ini
```

### Comparing `dissect.contrib-1.4.dev2/LICENSE` & `dissect.contrib-1.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.4.dev2/PKG-INFO` & `dissect.contrib-1.4.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.contrib
-Version: 1.4.dev2
+Version: 1.4.dev3
 Summary: This project is a meta package: it reserves the namespace for Dissect packages made by external contributors
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect.contrib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `dissect.contrib-1.4.dev2/README.md` & `dissect.contrib-1.4.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.4.dev2/dissect.contrib.egg-info/PKG-INFO` & `dissect.contrib-1.4.dev3/dissect.contrib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.contrib
-Version: 1.4.dev2
+Version: 1.4.dev3
 Summary: This project is a meta package: it reserves the namespace for Dissect packages made by external contributors
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect.contrib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `dissect.contrib-1.4.dev2/pyproject.toml` & `dissect.contrib-1.4.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.4.dev2/template/pyproject.toml` & `dissect.contrib-1.4.dev3/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.4.dev2/tox.ini` & `dissect.contrib-1.4.dev3/tox.ini`

 * *Files identical despite different names*

