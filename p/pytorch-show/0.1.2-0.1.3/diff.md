# Comparing `tmp/pytorch_show-0.1.2.tar.gz` & `tmp/pytorch_show-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_show-0.1.2.tar", max compression
+gzip compressed data, was "pytorch_show-0.1.3.tar", max compression
```

## Comparing `pytorch_show-0.1.2.tar` & `pytorch_show-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      336 2023-06-27 11:44:19.613393 pytorch_show-0.1.2/README.md
--rw-r--r--   0        0        0      425 2023-06-27 11:50:04.582825 pytorch_show-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 11:06:48.250000 pytorch_show-0.1.2/pytorch_show/__init__.py
--rw-r--r--   0        0        0     1980 2023-06-27 11:49:43.982252 pytorch_show-0.1.2/pytorch_show/main.py
--rw-r--r--   0        0        0      881 2023-06-27 10:51:06.354697 pytorch_show-0.1.2/pytorch_show/test.py
--rw-r--r--   0        0        0     4616 2023-06-27 11:12:01.555489 pytorch_show-0.1.2/pytorch_show/utils.py
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 pytorch_show-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-06-27 11:44:19.613393 pytorch_show-0.1.3/README.md
+-rw-r--r--   0        0        0      444 2023-06-27 11:54:02.409505 pytorch_show-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-06-27 11:54:02.417505 pytorch_show-0.1.3/pytorch_show/__init__.py
+-rw-r--r--   0        0        0     1980 2023-06-27 11:49:43.982252 pytorch_show-0.1.3/pytorch_show/main.py
+-rw-r--r--   0        0        0      881 2023-06-27 10:51:06.354697 pytorch_show-0.1.3/pytorch_show/test.py
+-rw-r--r--   0        0        0     4616 2023-06-27 11:12:01.555489 pytorch_show-0.1.3/pytorch_show/utils.py
+-rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 pytorch_show-0.1.3/PKG-INFO
```

### Comparing `pytorch_show-0.1.2/pytorch_show/main.py` & `pytorch_show-0.1.3/pytorch_show/main.py`

 * *Files identical despite different names*

### Comparing `pytorch_show-0.1.2/pytorch_show/test.py` & `pytorch_show-0.1.3/pytorch_show/test.py`

 * *Files identical despite different names*

### Comparing `pytorch_show-0.1.2/pytorch_show/utils.py` & `pytorch_show-0.1.3/pytorch_show/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_show-0.1.2/PKG-INFO` & `pytorch_show-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pytorch-show
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is a tool to visualize models directly from py scripts
 Author: Yshelgi
 Author-email: 3041696596@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: torchvision (>=0.15.1,<0.16.0)
 Description-Content-Type: text/markdown
 
 # pytorch-show
```

