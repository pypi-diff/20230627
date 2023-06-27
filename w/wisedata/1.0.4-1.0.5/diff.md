# Comparing `tmp/wisedata-1.0.4.tar.gz` & `tmp/wisedata-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisedata-1.0.4.tar", max compression
+gzip compressed data, was "wisedata-1.0.5.tar", max compression
```

## Comparing `wisedata-1.0.4.tar` & `wisedata-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.4/LICENSE
--rw-r--r--   0        0        0     9918 2023-06-27 11:13:55.101088 wisedata-1.0.4/README.md
--rw-r--r--   0        0        0      622 2023-06-27 11:13:58.089282 wisedata-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     8358 2023-06-26 17:46:41.469930 wisedata-1.0.4/wisedata/__init__.py
--rw-r--r--   0        0        0      704 2023-06-26 12:18:32.144558 wisedata-1.0.4/wisedata/exceptions.py
--rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 wisedata-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.5/LICENSE
+-rw-r--r--   0        0        0     9918 2023-06-27 11:13:55.101088 wisedata-1.0.5/README.md
+-rw-r--r--   0        0        0      661 2023-06-27 11:23:40.424683 wisedata-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8358 2023-06-26 17:46:41.469930 wisedata-1.0.5/wisedata/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-26 12:18:32.144558 wisedata-1.0.5/wisedata/exceptions.py
+-rw-r--r--   0        0        0    10512 1970-01-01 00:00:00.000000 wisedata-1.0.5/PKG-INFO
```

### Comparing `wisedata-1.0.4/LICENSE` & `wisedata-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.4/README.md` & `wisedata-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.4/pyproject.toml` & `wisedata-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "wisedata"
-version = "1.0.4"
+version = "1.0.5"
 description = "AI Assistant for Python Data Analytics"
 authors = ["WiseData Team"]
 url = "https://www.wisedata.app/"
+homepage = "https://www.wisedata.app/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
 requests = "2.31.0"
 retry = "^0.9.2"
```

### Comparing `wisedata-1.0.4/wisedata/__init__.py` & `wisedata-1.0.5/wisedata/__init__.py`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.4/wisedata/exceptions.py` & `wisedata-1.0.5/wisedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.4/PKG-INFO` & `wisedata-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: wisedata
-Version: 1.0.4
+Version: 1.0.5
 Summary: AI Assistant for Python Data Analytics
+Home-page: https://www.wisedata.app/
 Author: WiseData Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

