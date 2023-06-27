# Comparing `tmp/autopack_tools-0.1.4.tar.gz` & `tmp/autopack_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.1.4.tar", max compression
+gzip compressed data, was "autopack_tools-0.1.5.tar", max compression
```

## Comparing `autopack_tools-0.1.4.tar` & `autopack_tools-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.1.4/LICENSE
--rw-r--r--   0        0        0     2920 2023-06-25 23:21:07.938300 autopack_tools-0.1.4/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.1.4/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-25 23:21:01.956387 autopack_tools-0.1.4/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.1.4/autopack/__main__.py
--rw-r--r--   0        0        0     2245 2023-06-26 23:28:38.418992 autopack_tools-0.1.4/autopack/api.py
--rw-r--r--   0        0        0      864 2023-06-25 23:21:01.957129 autopack_tools-0.1.4/autopack/cli.py
--rw-r--r--   0        0        0      258 2023-06-25 23:21:01.957337 autopack_tools-0.1.4/autopack/errors.py
--rw-r--r--   0        0        0     4729 2023-06-26 23:45:40.137477 autopack_tools-0.1.4/autopack/get_pack.py
--rw-r--r--   0        0        0     2780 2023-06-26 23:38:47.664538 autopack_tools-0.1.4/autopack/installation.py
--rw-r--r--   0        0        0      951 2023-06-26 23:46:16.871143 autopack_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 autopack_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2920 2023-06-25 23:21:07.938300 autopack_tools-0.1.5/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.1.5/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-25 23:21:01.956387 autopack_tools-0.1.5/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.1.5/autopack/__main__.py
+-rw-r--r--   0        0        0     2245 2023-06-26 23:28:38.418992 autopack_tools-0.1.5/autopack/api.py
+-rw-r--r--   0        0        0      864 2023-06-25 23:21:01.957129 autopack_tools-0.1.5/autopack/cli.py
+-rw-r--r--   0        0        0      258 2023-06-25 23:21:01.957337 autopack_tools-0.1.5/autopack/errors.py
+-rw-r--r--   0        0        0     4729 2023-06-26 23:45:40.137477 autopack_tools-0.1.5/autopack/get_pack.py
+-rw-r--r--   0        0        0     2780 2023-06-26 23:38:47.664538 autopack_tools-0.1.5/autopack/installation.py
+-rw-r--r--   0        0        0      950 2023-06-26 23:51:55.166513 autopack_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 autopack_tools-0.1.5/PKG-INFO
```

### Comparing `autopack_tools-0.1.4/LICENSE` & `autopack_tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.4/README.md` & `autopack_tools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.4/autopack/api.py` & `autopack_tools-0.1.5/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.4/autopack/cli.py` & `autopack_tools-0.1.5/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.4/autopack/get_pack.py` & `autopack_tools-0.1.5/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.4/autopack/installation.py` & `autopack_tools-0.1.5/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.4/pyproject.toml` & `autopack_tools-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.1.4"
+version = "0.1.5"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
 
 [tool.poetry.scripts]
 autopack = 'autopack.cli:main'
 
 [tool.poetry.dependencies]
-python = ">=3.10.3"
+python = "^3.10.3"
 requests = "^2.31.0"
 dataclasses-json = "^0.5.8"
 urllib3 = "^1.26.16"
 gitpython = "^3.1.31"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `autopack_tools-0.1.4/PKG-INFO` & `autopack_tools-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
-Requires-Python: >=3.10.3
+Requires-Python: >=3.10.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.8,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
```

