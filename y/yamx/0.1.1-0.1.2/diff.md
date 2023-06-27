# Comparing `tmp/yamx-0.1.1.tar.gz` & `tmp/yamx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamx-0.1.1.tar", max compression
+gzip compressed data, was "yamx-0.1.2.tar", max compression
```

## Comparing `yamx-0.1.1.tar` & `yamx-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     9893 2023-04-11 11:37:11.485830 yamx-0.1.1/LICENSE
--rw-r--r--   0        0        0     1724 2023-06-27 08:17:29.427389 yamx-0.1.1/README.md
--rw-r--r--   0        0        0     1063 2023-06-27 08:57:51.601654 yamx-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-27 08:17:29.430991 yamx-0.1.1/yamx/__init__.py
--rw-r--r--   0        0        0     1065 2023-06-27 08:34:55.316759 yamx-0.1.1/yamx/constants.py
--rw-r--r--   0        0        0      398 2023-06-27 08:17:29.431599 yamx-0.1.1/yamx/containers/__init__.py
--rw-r--r--   0        0        0     6993 2023-06-27 08:39:18.867870 yamx-0.1.1/yamx/containers/data.py
--rw-r--r--   0        0        0      105 2023-06-27 08:17:29.432156 yamx-0.1.1/yamx/containers/settings.py
--rw-r--r--   0        0        0     1532 2023-06-27 08:17:29.432409 yamx-0.1.1/yamx/extra.py
--rw-r--r--   0        0        0        0 2023-06-27 08:17:29.432483 yamx-0.1.1/yamx/jinja/__init__.py
--rw-r--r--   0        0        0     4474 2023-06-27 08:17:29.432958 yamx-0.1.1/yamx/jinja/condition.py
--rw-r--r--   0        0        0      169 2023-06-27 08:17:29.433219 yamx-0.1.1/yamx/loader/__init__.py
--rw-r--r--   0        0        0     3725 2023-06-27 08:17:29.433444 yamx-0.1.1/yamx/loader/grouper.py
--rw-r--r--   0        0        0     6253 2023-06-27 08:39:18.879819 yamx-0.1.1/yamx/loader/preprocessor.py
--rw-r--r--   0        0        0      637 2023-06-27 08:17:29.433836 yamx-0.1.1/yamx/loader/utils.py
--rw-r--r--   0        0        0      518 2023-06-27 08:17:29.434122 yamx-0.1.1/yamx/loader/validator.py
--rw-r--r--   0        0        0      244 2023-06-27 08:17:29.434292 yamx-0.1.1/yamx/representer/__init__.py
--rw-r--r--   0        0        0     9448 2023-06-27 08:17:29.434469 yamx-0.1.1/yamx/representer/common.py
--rw-r--r--   0        0        0      611 2023-06-27 08:17:29.434619 yamx-0.1.1/yamx/representer/conditional_map.py
--rw-r--r--   0        0        0      580 2023-06-27 08:17:29.434741 yamx-0.1.1/yamx/representer/conditional_seq.py
--rw-r--r--   0        0        0    18945 2023-06-27 08:17:29.435048 yamx-0.1.1/yamx/representer/rendering.py
--rw-r--r--   0        0        0     6271 2023-06-27 08:52:12.176499 yamx-0.1.1/yamx/yamx.py
--rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 yamx-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     9893 2023-04-11 11:37:11.485830 yamx-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1724 2023-06-27 08:17:29.427389 yamx-0.1.2/README.md
+-rw-r--r--   0        0        0     1063 2023-06-27 09:29:42.854931 yamx-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-27 08:17:29.430991 yamx-0.1.2/yamx/__init__.py
+-rw-r--r--   0        0        0     1065 2023-06-27 08:34:55.316759 yamx-0.1.2/yamx/constants.py
+-rw-r--r--   0        0        0      398 2023-06-27 08:17:29.431599 yamx-0.1.2/yamx/containers/__init__.py
+-rw-r--r--   0        0        0     6993 2023-06-27 08:39:18.867870 yamx-0.1.2/yamx/containers/data.py
+-rw-r--r--   0        0        0      105 2023-06-27 08:17:29.432156 yamx-0.1.2/yamx/containers/settings.py
+-rw-r--r--   0        0        0     1532 2023-06-27 08:17:29.432409 yamx-0.1.2/yamx/extra.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:17:29.432483 yamx-0.1.2/yamx/jinja/__init__.py
+-rw-r--r--   0        0        0     4474 2023-06-27 08:17:29.432958 yamx-0.1.2/yamx/jinja/condition.py
+-rw-r--r--   0        0        0      169 2023-06-27 08:17:29.433219 yamx-0.1.2/yamx/loader/__init__.py
+-rw-r--r--   0        0        0     3725 2023-06-27 08:17:29.433444 yamx-0.1.2/yamx/loader/grouper.py
+-rw-r--r--   0        0        0     6253 2023-06-27 08:39:18.879819 yamx-0.1.2/yamx/loader/preprocessor.py
+-rw-r--r--   0        0        0      637 2023-06-27 08:17:29.433836 yamx-0.1.2/yamx/loader/utils.py
+-rw-r--r--   0        0        0      518 2023-06-27 08:17:29.434122 yamx-0.1.2/yamx/loader/validator.py
+-rw-r--r--   0        0        0      244 2023-06-27 08:17:29.434292 yamx-0.1.2/yamx/representer/__init__.py
+-rw-r--r--   0        0        0     9448 2023-06-27 08:17:29.434469 yamx-0.1.2/yamx/representer/common.py
+-rw-r--r--   0        0        0      611 2023-06-27 08:17:29.434619 yamx-0.1.2/yamx/representer/conditional_map.py
+-rw-r--r--   0        0        0      580 2023-06-27 08:17:29.434741 yamx-0.1.2/yamx/representer/conditional_seq.py
+-rw-r--r--   0        0        0    18945 2023-06-27 08:17:29.435048 yamx-0.1.2/yamx/representer/rendering.py
+-rw-r--r--   0        0        0     6271 2023-06-27 08:52:12.176499 yamx-0.1.2/yamx/yamx.py
+-rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 yamx-0.1.2/PKG-INFO
```

### Comparing `yamx-0.1.1/LICENSE` & `yamx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/README.md` & `yamx-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/pyproject.toml` & `yamx-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yamx"
-version = "0.1.1"
+version = "0.1.2"
 description = "YAML parser that supports jinja conditional expressions"
 
 license = "Apache-2.0"
 
 authors = [
     "Eduard Trott <eduard.trott@workday.com>"
 ]
@@ -18,15 +18,15 @@
 keywords = ["yaml", "jinja", "language"]
 
 [tool.poetry.dependencies]
 # Compatible Python versions
 python = ">=3.8"
 
 # Standard dependencies with semver constraints
-attrs = "^22.2.0"
+attrs = "^23.1.0"
 jinja2 = "^3.1.2"
 immutables= "^0.19"
 "ruamel.yaml" = "0.17.32"
 "ruamel.yaml.string" = "0.1.0"
 
 
 [tool.poetry.group.test]
```

### Comparing `yamx-0.1.1/yamx/constants.py` & `yamx-0.1.2/yamx/constants.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/containers/data.py` & `yamx-0.1.2/yamx/containers/data.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/extra.py` & `yamx-0.1.2/yamx/extra.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/jinja/condition.py` & `yamx-0.1.2/yamx/jinja/condition.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/loader/grouper.py` & `yamx-0.1.2/yamx/loader/grouper.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/loader/preprocessor.py` & `yamx-0.1.2/yamx/loader/preprocessor.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/loader/utils.py` & `yamx-0.1.2/yamx/loader/utils.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/loader/validator.py` & `yamx-0.1.2/yamx/loader/validator.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/representer/common.py` & `yamx-0.1.2/yamx/representer/common.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/representer/conditional_map.py` & `yamx-0.1.2/yamx/representer/conditional_map.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/representer/conditional_seq.py` & `yamx-0.1.2/yamx/representer/conditional_seq.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/representer/rendering.py` & `yamx-0.1.2/yamx/representer/rendering.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/yamx/yamx.py` & `yamx-0.1.2/yamx/yamx.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.1/PKG-INFO` & `yamx-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: yamx
-Version: 0.1.1
+Version: 0.1.2
 Summary: YAML parser that supports jinja conditional expressions
 Home-page: https://github.com/maybelinot/yamx
 License: Apache-2.0
 Keywords: yaml,jinja,language
 Author: Eduard Trott
 Author-email: eduard.trott@workday.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: immutables (>=0.19,<0.20)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: ruamel.yaml (==0.17.32)
 Requires-Dist: ruamel.yaml.string (==0.1.0)
 Project-URL: Repository, https://github.com/maybelinot/yamx
 Description-Content-Type: text/markdown
```

