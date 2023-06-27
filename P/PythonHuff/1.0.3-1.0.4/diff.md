# Comparing `tmp/PythonHuff-1.0.3.tar.gz` & `tmp/PythonHuff-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PythonHuff-1.0.3.tar", last modified: Mon Jun 26 14:12:00 2023, max compression
+gzip compressed data, was "dist\PythonHuff-1.0.4.tar", last modified: Tue Jun 27 08:19:02 2023, max compression
```

## Comparing `PythonHuff-1.0.3.tar` & `PythonHuff-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 14:12:00.236091 PythonHuff-1.0.3/
--rw-rw-rw-   0        0        0     1480 2023-06-26 14:12:00.236091 PythonHuff-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 14:12:00.236091 PythonHuff-1.0.3/PythonHuff.egg-info/
--rw-rw-rw-   0        0        0     1480 2023-06-26 14:12:00.000000 PythonHuff-1.0.3/PythonHuff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-06-26 14:12:00.000000 PythonHuff-1.0.3/PythonHuff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 14:12:00.000000 PythonHuff-1.0.3/PythonHuff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-26 14:12:00.000000 PythonHuff-1.0.3/PythonHuff.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 14:12:00.000000 PythonHuff-1.0.3/PythonHuff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      864 2023-06-26 09:45:17.000000 PythonHuff-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 14:12:00.236091 PythonHuff-1.0.3/pyhuff/
--rw-rw-rw-   0        0        0     4195 2023-06-26 14:11:48.000000 PythonHuff-1.0.3/pyhuff/__init__.py
--rw-rw-rw-   0        0        0     2452 2023-06-26 08:39:21.000000 PythonHuff-1.0.3/pyhuff/classes.py
--rw-rw-rw-   0        0        0       42 2023-06-26 14:12:00.236091 PythonHuff-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-06-26 14:11:52.000000 PythonHuff-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:19:02.815929 PythonHuff-1.0.4/
+-rw-rw-rw-   0        0        0     1480 2023-06-27 08:19:02.800301 PythonHuff-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 08:19:02.800301 PythonHuff-1.0.4/PythonHuff.egg-info/
+-rw-rw-rw-   0        0        0     1480 2023-06-27 08:19:02.000000 PythonHuff-1.0.4/PythonHuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-06-27 08:19:02.000000 PythonHuff-1.0.4/PythonHuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:19:02.000000 PythonHuff-1.0.4/PythonHuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-27 08:19:02.000000 PythonHuff-1.0.4/PythonHuff.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 08:19:02.000000 PythonHuff-1.0.4/PythonHuff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      864 2023-06-26 09:45:17.000000 PythonHuff-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 08:19:02.800301 PythonHuff-1.0.4/pyhuff/
+-rw-rw-rw-   0        0        0     4195 2023-06-26 14:11:48.000000 PythonHuff-1.0.4/pyhuff/__init__.py
+-rw-rw-rw-   0        0        0     2452 2023-06-26 08:39:21.000000 PythonHuff-1.0.4/pyhuff/classes.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:19:02.815929 PythonHuff-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-06-27 08:18:45.000000 PythonHuff-1.0.4/setup.py
```

### Comparing `PythonHuff-1.0.3/PKG-INFO` & `PythonHuff-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonHuff
-Version: 1.0.3
+Version: 1.0.4
 Summary: Huffman compression and decompression (Pure Python implementation)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
         ### Usage
         ```python
```

### Comparing `PythonHuff-1.0.3/PythonHuff.egg-info/PKG-INFO` & `PythonHuff-1.0.4/PythonHuff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonHuff
-Version: 1.0.3
+Version: 1.0.4
 Summary: Huffman compression and decompression (Pure Python implementation)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
         ### Usage
         ```python
```

### Comparing `PythonHuff-1.0.3/README.md` & `PythonHuff-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PythonHuff-1.0.3/pyhuff/__init__.py` & `PythonHuff-1.0.4/pyhuff/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonHuff-1.0.3/pyhuff/classes.py` & `PythonHuff-1.0.4/pyhuff/classes.py`

 * *Files identical despite different names*

### Comparing `PythonHuff-1.0.3/setup.py` & `PythonHuff-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 def readme():
     with open('README.md','r') as f:
         return f.read()
 setup(
     name='PythonHuff',
-    version='1.0.3',
+    version='1.0.4',
     packages=['pyhuff'],
     description='Huffman compression and decompression (Pure Python implementation)',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords=['huffman','compression','decompression','algorithm'],
     classifiers=[
         'Programming Language :: Python :: 3',
```

