# Comparing `tmp/gripa-0.1.0.tar.gz` & `tmp/gripa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gripa-0.1.0.tar", max compression
+gzip compressed data, was "gripa-0.1.1.tar", max compression
```

## Comparing `gripa-0.1.0.tar` & `gripa-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-06-17 22:17:32.758169 gripa-0.1.0/LICENSE
--rw-r--r--   0        0        0      186 2023-06-19 22:31:03.452108 gripa-0.1.0/gripa/__init__.py
--rw-r--r--   0        0        0     4268 2023-06-19 22:31:03.452603 gripa-0.1.0/gripa/_hpf.py
--rw-r--r--   0        0        0     6022 2023-06-19 23:09:26.836446 gripa-0.1.0/gripa/_ssa.py
--rw-r--r--   0        0        0      819 2023-06-19 22:31:03.453426 gripa-0.1.0/gripa/base.py
--rw-r--r--   0        0        0     3832 2023-06-19 23:09:26.836775 gripa-0.1.0/gripa/detector.py
--rw-r--r--   0        0        0        0 2023-06-19 22:30:28.858072 gripa-0.1.0/gripa/tests/__init__.py
--rw-r--r--   0        0        0    10670 2023-06-19 22:31:03.454235 gripa-0.1.0/gripa/tests/test_detector.py
--rw-r--r--   0        0        0      518 2023-06-19 22:31:03.454564 gripa-0.1.0/gripa/utils.py
--rw-r--r--   0        0        0     1274 2023-06-27 08:16:52.179261 gripa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 gripa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-17 22:17:32.758169 gripa-0.1.1/LICENSE
+-rw-r--r--   0        0        0      186 2023-06-19 22:31:03.452108 gripa-0.1.1/gripa/__init__.py
+-rw-r--r--   0        0        0     4268 2023-06-19 22:31:03.452603 gripa-0.1.1/gripa/_hpf.py
+-rw-r--r--   0        0        0     6022 2023-06-19 23:09:26.836446 gripa-0.1.1/gripa/_ssa.py
+-rw-r--r--   0        0        0      819 2023-06-19 22:31:03.453426 gripa-0.1.1/gripa/base.py
+-rw-r--r--   0        0        0     3832 2023-06-19 23:09:26.836775 gripa-0.1.1/gripa/detector.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:30:28.858072 gripa-0.1.1/gripa/tests/__init__.py
+-rw-r--r--   0        0        0    10670 2023-06-19 22:31:03.454235 gripa-0.1.1/gripa/tests/test_detector.py
+-rw-r--r--   0        0        0      518 2023-06-19 22:31:03.454564 gripa-0.1.1/gripa/utils.py
+-rw-r--r--   0        0        0     1327 2023-06-27 09:37:39.660903 gripa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 gripa-0.1.1/PKG-INFO
```

### Comparing `gripa-0.1.0/LICENSE` & `gripa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gripa-0.1.0/gripa/_hpf.py` & `gripa-0.1.1/gripa/_hpf.py`

 * *Files identical despite different names*

### Comparing `gripa-0.1.0/gripa/_ssa.py` & `gripa-0.1.1/gripa/_ssa.py`

 * *Files identical despite different names*

### Comparing `gripa-0.1.0/gripa/base.py` & `gripa-0.1.1/gripa/base.py`

 * *Files identical despite different names*

### Comparing `gripa-0.1.0/gripa/detector.py` & `gripa-0.1.1/gripa/detector.py`

 * *Files identical despite different names*

### Comparing `gripa-0.1.0/gripa/tests/test_detector.py` & `gripa-0.1.1/gripa/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `gripa-0.1.0/gripa/utils.py` & `gripa-0.1.1/gripa/utils.py`

 * *Files identical despite different names*

### Comparing `gripa-0.1.0/pyproject.toml` & `gripa-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "gripa"
-version = "0.1.0"
+version = "0.1.1"
 description = "Time series anomaly detection"
 authors = ["hamiddimyati <hamid.dimyati@outlook.com>"]
 license = "MIT license"
+repository = "https://github.com/hamiddimyati/gripa"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 numpy = "^1.25.0"
 pandas = "^2.0.2"
 scikit-learn = "^1.2.2"
 scipy = "^1.10.1"
```

### Comparing `gripa-0.1.0/PKG-INFO` & `gripa-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: gripa
-Version: 0.1.0
+Version: 0.1.1
 Summary: Time series anomaly detection
+Home-page: https://github.com/hamiddimyati/gripa
 License: MIT
 Author: hamiddimyati
 Author-email: hamid.dimyati@outlook.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Project-URL: Repository, https://github.com/hamiddimyati/gripa
```

