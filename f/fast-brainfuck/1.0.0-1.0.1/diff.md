# Comparing `tmp/fast-brainfuck-1.0.0.tar.gz` & `tmp/fast-brainfuck-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fast-brainfuck-1.0.0.tar", last modified: Tue Jun 27 14:27:49 2023, max compression
+gzip compressed data, was "dist\fast-brainfuck-1.0.1.tar", last modified: Tue Jun 27 14:36:17 2023, max compression
```

## Comparing `fast-brainfuck-1.0.0.tar` & `fast-brainfuck-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 14:27:49.099532 fast-brainfuck-1.0.0/
--rw-rw-rw-   0        0        0     3143 2023-06-27 14:27:49.099532 fast-brainfuck-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2023-06-27 14:27:06.000000 fast-brainfuck-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 14:27:49.097951 fast-brainfuck-1.0.0/fast_brainfuck.egg-info/
--rw-rw-rw-   0        0        0     3143 2023-06-27 14:27:49.000000 fast-brainfuck-1.0.0/fast_brainfuck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-27 14:27:49.000000 fast-brainfuck-1.0.0/fast_brainfuck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 14:27:49.000000 fast-brainfuck-1.0.0/fast_brainfuck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-27 14:27:49.000000 fast-brainfuck-1.0.0/fast_brainfuck.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-06-27 14:27:49.000000 fast-brainfuck-1.0.0/fast_brainfuck.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 14:27:49.000000 fast-brainfuck-1.0.0/fast_brainfuck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3950 2023-06-27 13:41:59.000000 fast-brainfuck-1.0.0/fastbf.py
--rw-rw-rw-   0        0        0       42 2023-06-27 14:27:49.099532 fast-brainfuck-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-06-27 14:26:29.000000 fast-brainfuck-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:36:17.789626 fast-brainfuck-1.0.1/
+-rw-rw-rw-   0        0        0     3143 2023-06-27 14:36:17.789626 fast-brainfuck-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1936 2023-06-27 14:27:06.000000 fast-brainfuck-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 14:36:17.789626 fast-brainfuck-1.0.1/fast_brainfuck.egg-info/
+-rw-rw-rw-   0        0        0     3143 2023-06-27 14:36:17.000000 fast-brainfuck-1.0.1/fast_brainfuck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-27 14:36:17.000000 fast-brainfuck-1.0.1/fast_brainfuck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 14:36:17.000000 fast-brainfuck-1.0.1/fast_brainfuck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-27 14:36:17.000000 fast-brainfuck-1.0.1/fast_brainfuck.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-06-27 14:36:17.000000 fast-brainfuck-1.0.1/fast_brainfuck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 14:36:17.000000 fast-brainfuck-1.0.1/fast_brainfuck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3950 2023-06-27 13:41:59.000000 fast-brainfuck-1.0.1/fastbf.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 14:36:17.789626 fast-brainfuck-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-06-27 14:36:09.000000 fast-brainfuck-1.0.1/setup.py
```

### Comparing `fast-brainfuck-1.0.0/PKG-INFO` & `fast-brainfuck-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-brainfuck
-Version: 1.0.0
+Version: 1.0.1
 Summary: Brainfuck "compiler" for Python (fast)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
         ### This is a very fast brainfuck "compiler".
```

### Comparing `fast-brainfuck-1.0.0/README.md` & `fast-brainfuck-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fast-brainfuck-1.0.0/fast_brainfuck.egg-info/PKG-INFO` & `fast-brainfuck-1.0.1/fast_brainfuck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-brainfuck
-Version: 1.0.0
+Version: 1.0.1
 Summary: Brainfuck "compiler" for Python (fast)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
         ### This is a very fast brainfuck "compiler".
```

### Comparing `fast-brainfuck-1.0.0/fastbf.py` & `fast-brainfuck-1.0.1/fastbf.py`

 * *Files identical despite different names*

### Comparing `fast-brainfuck-1.0.0/setup.py` & `fast-brainfuck-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 def readme():
     with open('README.md','r') as f:
         return f.read()
 setup(
     name='fast-brainfuck',
     py_modules=['fastbf'],
-    version='1.0.0',
+    version='1.0.1',
     entry_points={
         'console_scripts':[
             'fastbf=fastbf:_fastbf_inter'
         ]
     },
     description='Brainfuck "compiler" for Python (fast)',
     long_description=readme(),
```

