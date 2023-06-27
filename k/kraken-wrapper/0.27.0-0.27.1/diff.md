# Comparing `tmp/kraken_wrapper-0.27.0.tar.gz` & `tmp/kraken_wrapper-0.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.27.0.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.27.1.tar", max compression
```

## Comparing `kraken_wrapper-0.27.0.tar` & `kraken_wrapper-0.27.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      998 2023-06-26 11:46:09.748133 kraken_wrapper-0.27.0/LICENSE
--rw-r--r--   0        0        0      378 2023-06-26 11:13:42.662140 kraken_wrapper-0.27.0/README.md
--rw-r--r--   0        0        0     2196 2023-06-27 00:25:10.711064 kraken_wrapper-0.27.0/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-27 00:25:10.711236 kraken_wrapper-0.27.0/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     7660 2023-06-26 11:13:42.663936 kraken_wrapper-0.27.0/src/kraken/wrapper/_buildend_venv.py
--rw-r--r--   0        0        0     3478 2023-06-26 11:13:42.664260 kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     5311 2023-06-20 12:31:06.105651 kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     3674 2023-06-20 12:31:06.105769 kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv_pex.py
--rw-r--r--   0        0        0     3250 2023-06-26 11:13:42.664763 kraken_wrapper-0.27.0/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4605 2023-06-20 12:31:06.106048 kraken_wrapper-0.27.0/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     3564 2023-06-20 12:31:06.106187 kraken_wrapper-0.27.0/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0     4222 2023-06-20 12:31:06.106313 kraken_wrapper-0.27.0/src/kraken/wrapper/_pex.py
--rw-r--r--   0        0        0    15982 2023-06-27 00:17:45.123581 kraken_wrapper-0.27.0/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2023-06-20 12:31:06.106556 kraken_wrapper-0.27.0/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 kraken_wrapper-0.27.0/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-06-26 11:46:09.748133 kraken_wrapper-0.27.1/LICENSE
+-rw-r--r--   0        0        0      378 2023-06-26 11:13:42.662140 kraken_wrapper-0.27.1/README.md
+-rw-r--r--   0        0        0     2196 2023-06-27 11:18:26.466074 kraken_wrapper-0.27.1/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-27 11:18:26.466180 kraken_wrapper-0.27.1/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     7660 2023-06-26 11:13:42.663936 kraken_wrapper-0.27.1/src/kraken/wrapper/_buildend_venv.py
+-rw-r--r--   0        0        0     3478 2023-06-26 11:13:42.664260 kraken_wrapper-0.27.1/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     5311 2023-06-20 12:31:06.105651 kraken_wrapper-0.27.1/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     3674 2023-06-20 12:31:06.105769 kraken_wrapper-0.27.1/src/kraken/wrapper/_buildenv_pex.py
+-rw-r--r--   0        0        0     3250 2023-06-26 11:13:42.664763 kraken_wrapper-0.27.1/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4605 2023-06-20 12:31:06.106048 kraken_wrapper-0.27.1/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     3564 2023-06-20 12:31:06.106187 kraken_wrapper-0.27.1/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0     4222 2023-06-20 12:31:06.106313 kraken_wrapper-0.27.1/src/kraken/wrapper/_pex.py
+-rw-r--r--   0        0        0    15982 2023-06-27 00:17:45.123581 kraken_wrapper-0.27.1/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2023-06-20 12:31:06.106556 kraken_wrapper-0.27.1/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 kraken_wrapper-0.27.1/PKG-INFO
```

### Comparing `kraken_wrapper-0.27.0/LICENSE` & `kraken_wrapper-0.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/pyproject.toml` & `kraken_wrapper-0.27.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.27.0"
+version = "0.27.1"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/wrapper", from = "src" }]
 classifiers = []
 keywords = []
@@ -18,15 +18,15 @@
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 keyring = "^23.8.2"
-kraken-common = "^0.27.0"
+kraken-common = "^0.27.1"
 pex = "^2.1.103"
 setuptools = ">=33.0.0"  # For pkg_resources
 termcolor = "^1.1.0"
 rich = "^13.4.2"
 
 # NOTE(@NiklasRosenstein): Need to pin transitive dependency markdown-it under 3.0 because it dropped Python 3.9
 #       support after that version. Technically this shouldn't be a big issue for runtime, but Mypy checks site
```

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/_buildend_venv.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/_buildend_venv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/_buildenv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv_pex.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/_buildenv_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/_config.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/_pex.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/src/kraken/wrapper/main.py` & `kraken_wrapper-0.27.1/src/kraken/wrapper/main.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.27.0/PKG-INFO` & `kraken_wrapper-0.27.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.27.0
+Version: 0.27.1
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keyring (>=23.8.2,<24.0.0)
-Requires-Dist: kraken-common (>=0.27.0,<0.28.0)
+Requires-Dist: kraken-common (>=0.27.1,<0.28.0)
 Requires-Dist: markdown-it-py (<3.0.0)
 Requires-Dist: pex (>=2.1.103,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: setuptools (>=33.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
```

