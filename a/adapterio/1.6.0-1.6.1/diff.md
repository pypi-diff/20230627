# Comparing `tmp/adapterio-1.6.0.tar.gz` & `tmp/adapterio-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapterio-1.6.0.tar", last modified: Thu May 11 11:25:29 2023, max compression
+gzip compressed data, was "adapterio-1.6.1.tar", last modified: Tue Jun 27 02:03:53 2023, max compression
```

## Comparing `adapterio-1.6.0.tar` & `adapterio-1.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-05-11 11:25:29.788978 adapterio-1.6.0/
--rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2023-05-11 11:25:29.788695 adapterio-1.6.0/PKG-INFO
--rw-r--r--   0 mgrahovac   (502) staff       (20)     7012 2023-05-05 11:27:35.000000 adapterio-1.6.0/README.md
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-05-11 11:25:29.784495 adapterio-1.6.0/adapter/
--rw-r--r--   0 mgrahovac   (502) staff       (20)      120 2023-05-05 11:27:35.000000 adapterio-1.6.0/adapter/Secret_example.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)      168 2023-05-11 11:21:57.000000 adapterio-1.6.0/adapter/__init__.py
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-05-11 11:25:29.786775 adapterio-1.6.0/adapter/comm/
--rw-r--r--   0 mgrahovac   (502) staff       (20)        0 2023-05-05 11:27:35.000000 adapterio-1.6.0/adapter/comm/__init__.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    25380 2023-05-05 11:27:35.000000 adapterio-1.6.0/adapter/comm/excel.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)     5015 2023-05-05 11:27:35.000000 adapterio-1.6.0/adapter/comm/sql.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)     6547 2023-05-05 11:27:35.000000 adapterio-1.6.0/adapter/comm/tools.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    29217 2023-05-11 11:21:57.000000 adapterio-1.6.0/adapter/i_o.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)      632 2023-05-05 11:27:35.000000 adapterio-1.6.0/adapter/label_map.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    14700 2023-05-05 11:27:35.000000 adapterio-1.6.0/adapter/to_python.py
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-05-11 11:25:29.788344 adapterio-1.6.0/adapterio.egg-info/
--rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2023-05-11 11:25:29.000000 adapterio-1.6.0/adapterio.egg-info/PKG-INFO
--rw-r--r--   0 mgrahovac   (502) staff       (20)      389 2023-05-11 11:25:29.000000 adapterio-1.6.0/adapterio.egg-info/SOURCES.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)        1 2023-05-11 11:25:29.000000 adapterio-1.6.0/adapterio.egg-info/dependency_links.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)       88 2023-05-11 11:25:29.000000 adapterio-1.6.0/adapterio.egg-info/requires.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)        8 2023-05-11 11:25:29.000000 adapterio-1.6.0/adapterio.egg-info/top_level.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)      103 2023-05-05 11:27:35.000000 adapterio-1.6.0/pyproject.toml
--rw-r--r--   0 mgrahovac   (502) staff       (20)       38 2023-05-11 11:25:29.789097 adapterio-1.6.0/setup.cfg
--rw-r--r--   0 mgrahovac   (502) staff       (20)     2779 2023-05-05 11:27:35.000000 adapterio-1.6.0/setup.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-06-27 02:03:53.711484 adapterio-1.6.1/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2023-06-27 02:03:53.711042 adapterio-1.6.1/PKG-INFO
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     7012 2023-05-05 11:27:35.000000 adapterio-1.6.1/README.md
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-06-27 02:03:53.705217 adapterio-1.6.1/adapter/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      120 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/Secret_example.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      168 2023-06-27 02:03:37.000000 adapterio-1.6.1/adapter/__init__.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-06-27 02:03:53.707908 adapterio-1.6.1/adapter/comm/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        0 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/comm/__init__.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    25380 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/comm/excel.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     5015 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/comm/sql.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     6547 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/comm/tools.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    29220 2023-06-27 02:03:37.000000 adapterio-1.6.1/adapter/i_o.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      632 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/label_map.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    14700 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/to_python.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-06-27 02:03:53.710295 adapterio-1.6.1/adapterio.egg-info/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/PKG-INFO
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      389 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        1 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)       88 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/requires.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        8 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/top_level.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      103 2023-05-05 11:27:35.000000 adapterio-1.6.1/pyproject.toml
+-rw-r--r--   0 mgrahovac   (502) staff       (20)       38 2023-06-27 02:03:53.711663 adapterio-1.6.1/setup.cfg
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     2779 2023-05-05 11:27:35.000000 adapterio-1.6.1/setup.py
```

### Comparing `adapterio-1.6.0/PKG-INFO` & `adapterio-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapterio
-Version: 1.6.0
+Version: 1.6.1
 Summary: I/O module
 Home-page: https://github.com/LBNL-ETA/Adapter
 Author: Milica Grahovac, Youness Bennani, Thomas Burke, Katie Coughlin, Mohan Ganeshalingam, Akhil Mathur, Evan Neill, Akshay Sharma, Zheng He and Lyra Lan
 License: BSD-3-Clause-LBNL
 Keywords: data,tables,IO for research computation,sql,excel,csv,dataframe,connection
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `adapterio-1.6.0/README.md` & `adapterio-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.0/adapter/comm/excel.py` & `adapterio-1.6.1/adapter/comm/excel.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.0/adapter/comm/sql.py` & `adapterio-1.6.1/adapter/comm/sql.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.0/adapter/comm/tools.py` & `adapterio-1.6.1/adapter/comm/tools.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.0/adapter/i_o.py` & `adapterio-1.6.1/adapter/i_o.py`

 * *Files 0% similar despite different names*

```diff
@@ -896,13 +896,13 @@
         FileNotFoundError: If the input file does not exist.
         EOFError: If the input file is empty.
     """
     if not os.path.exists(in_path):
         raise FileNotFoundError(f"The file {in_path} does not exist.")
 
     with gzip.open(in_path, "rb") as f:
-        py_object = pickle.load(f)
+        py_object = pd.read_pickle(f)
 
     if not py_object:
         raise EOFError("The file is empty.")
 
     return py_object
```

### Comparing `adapterio-1.6.0/adapter/label_map.py` & `adapterio-1.6.1/adapter/label_map.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.0/adapter/to_python.py` & `adapterio-1.6.1/adapter/to_python.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.0/adapterio.egg-info/PKG-INFO` & `adapterio-1.6.1/adapterio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapterio
-Version: 1.6.0
+Version: 1.6.1
 Summary: I/O module
 Home-page: https://github.com/LBNL-ETA/Adapter
 Author: Milica Grahovac, Youness Bennani, Thomas Burke, Katie Coughlin, Mohan Ganeshalingam, Akhil Mathur, Evan Neill, Akshay Sharma, Zheng He and Lyra Lan
 License: BSD-3-Clause-LBNL
 Keywords: data,tables,IO for research computation,sql,excel,csv,dataframe,connection
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `adapterio-1.6.0/setup.py` & `adapterio-1.6.1/setup.py`

 * *Files identical despite different names*

