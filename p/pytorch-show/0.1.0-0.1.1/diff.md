# Comparing `tmp/pytorch_show-0.1.0.tar.gz` & `tmp/pytorch_show-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_show-0.1.0.tar", max compression
+gzip compressed data, was "pytorch_show-0.1.1.tar", max compression
```

## Comparing `pytorch_show-0.1.0.tar` & `pytorch_show-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      257 2023-06-27 11:23:27.784469 pytorch_show-0.1.0/README.md
--rw-r--r--   0        0        0      425 2023-06-27 11:25:35.724290 pytorch_show-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 11:06:48.250000 pytorch_show-0.1.0/pytorch_show/__init__.py
--rw-r--r--   0        0        0     1979 2023-06-27 11:12:01.539488 pytorch_show-0.1.0/pytorch_show/main.py
--rw-r--r--   0        0        0      881 2023-06-27 10:51:06.354697 pytorch_show-0.1.0/pytorch_show/test.py
--rw-r--r--   0        0        0     4616 2023-06-27 11:12:01.555489 pytorch_show-0.1.0/pytorch_show/utils.py
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 pytorch_show-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-06-27 11:44:19.613393 pytorch_show-0.1.1/README.md
+-rw-r--r--   0        0        0      425 2023-06-27 11:44:49.114183 pytorch_show-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 11:06:48.250000 pytorch_show-0.1.1/pytorch_show/__init__.py
+-rw-r--r--   0        0        0     1979 2023-06-27 11:12:01.539488 pytorch_show-0.1.1/pytorch_show/main.py
+-rw-r--r--   0        0        0      881 2023-06-27 10:51:06.354697 pytorch_show-0.1.1/pytorch_show/test.py
+-rw-r--r--   0        0        0     4616 2023-06-27 11:12:01.555489 pytorch_show-0.1.1/pytorch_show/utils.py
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 pytorch_show-0.1.1/PKG-INFO
```

### Comparing `pytorch_show-0.1.0/pytorch_show/main.py` & `pytorch_show-0.1.1/pytorch_show/main.py`

 * *Files identical despite different names*

### Comparing `pytorch_show-0.1.0/pytorch_show/test.py` & `pytorch_show-0.1.1/pytorch_show/test.py`

 * *Files identical despite different names*

### Comparing `pytorch_show-0.1.0/pytorch_show/utils.py` & `pytorch_show-0.1.1/pytorch_show/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_show-0.1.0/PKG-INFO` & `pytorch_show-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-show
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a tool to visualize models directly from py scripts
 Author: Yshelgi
 Author-email: 3041696596@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,9 +19,10 @@
 
 This is a tool to visualize models directly from py scripts  and it can automatically find all nn.Module in the file
 
 
 **RUN**
 
 `python main.py -f python_file -i 240 240 -d -n`
-![img.png](img.png)
-![TestModel.svg](..%2FSave%2FTestModel.svg)
+![img.png](https://s2.loli.net/2023/06/27/k4psbUREQHlXV2O.png)
+
+![image-20230627194415687](https://s2.loli.net/2023/06/27/ahbLlf6yOZ57KYw.png)
```

