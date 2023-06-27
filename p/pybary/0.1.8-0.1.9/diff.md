# Comparing `tmp/pybary-0.1.8.tar.gz` & `tmp/pybary-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybary-0.1.8.tar", max compression
+gzip compressed data, was "pybary-0.1.9.tar", max compression
```

## Comparing `pybary-0.1.8.tar` & `pybary-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-01-04 01:02:39.166381 pybary-0.1.8/LICENSE
--rw-r--r--   0        0        0     1075 2023-01-12 12:35:58.202434 pybary-0.1.8/README.md
--rw-r--r--   0        0        0      243 2023-01-05 18:35:02.344069 pybary-0.1.8/pybary/__init__.py
--rw-r--r--   0        0        0     2924 2023-01-09 22:26:55.758266 pybary-0.1.8/pybary/pybary.py
--rw-r--r--   0        0        0     1823 2023-01-12 12:36:03.074411 pybary-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1886 1970-01-01 00:00:00.000000 pybary-0.1.8/setup.py
--rw-r--r--   0        0        0     2214 1970-01-01 00:00:00.000000 pybary-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-01-22 18:18:23.343715 pybary-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1075 2023-01-22 18:18:23.347715 pybary-0.1.9/README.md
+-rw-r--r--   0        0        0      285 2023-06-27 18:24:02.974989 pybary-0.1.9/pybary/__init__.py
+-rw-r--r--   0        0        0     2924 2023-01-22 18:18:23.543714 pybary-0.1.9/pybary/pybary.py
+-rw-r--r--   0        0        0     1823 2023-06-27 18:26:21.459529 pybary-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2214 1970-01-01 00:00:00.000000 pybary-0.1.9/PKG-INFO
```

### Comparing `pybary-0.1.8/LICENSE` & `pybary-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybary-0.1.8/README.md` & `pybary-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pybary-0.1.8/pybary/pybary.py` & `pybary-0.1.9/pybary/pybary.py`

 * *Files identical despite different names*

### Comparing `pybary-0.1.8/pyproject.toml` & `pybary-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybary"
-version = "0.1.8"
+version = "0.1.9"
 description = "Barycenter method in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "pybary"}]
 homepage = "https://pypi.org/project/pybary/"
 repository = "https://github.com/asmove/pybary"
```

### Comparing `pybary-0.1.8/PKG-INFO` & `pybary-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybary
-Version: 0.1.8
+Version: 0.1.9
 Summary: Barycenter method in python
 Home-page: https://pypi.org/project/pybary/
 License: MIT
 Keywords: optimization,discrete
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<3.12
```

