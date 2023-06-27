# Comparing `tmp/vipes-0.0.3.tar.gz` & `tmp/vipes-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipes-0.0.3.tar", last modified: Tue Jun 27 00:04:13 2023, max compression
+gzip compressed data, was "vipes-0.0.4.tar", last modified: Tue Jun 27 00:12:45 2023, max compression
```

## Comparing `vipes-0.0.3.tar` & `vipes-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:04:13.520237 vipes-0.0.3/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)     1067 2023-06-26 20:30:07.000000 vipes-0.0.3/LICENSE
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:04:13.520084 vipes-0.0.3/PKG-INFO
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      437 2023-06-26 22:18:09.000000 vipes-0.0.3/README.md
--rw-r--r--   0 jhonaguiar   (501) staff       (20)       38 2023-06-27 00:04:13.520274 vipes-0.0.3/setup.cfg
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      699 2023-06-27 00:02:18.000000 vipes-0.0.3/setup.py
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:04:13.519792 vipes-0.0.3/vipes.egg-info/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/PKG-INFO
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      174 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/SOURCES.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/dependency_links.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)       43 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/entry_points.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/top_level.txt
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:12:45.443639 vipes-0.0.4/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)     1067 2023-06-26 20:30:07.000000 vipes-0.0.4/LICENSE
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:12:45.443469 vipes-0.0.4/PKG-INFO
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      437 2023-06-26 22:18:09.000000 vipes-0.0.4/README.md
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)       38 2023-06-27 00:12:45.443694 vipes-0.0.4/setup.cfg
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      699 2023-06-27 00:12:34.000000 vipes-0.0.4/setup.py
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:12:45.442350 vipes-0.0.4/vipes/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:09:01.000000 vipes-0.0.4/vipes/__init__.py
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      604 2023-06-26 19:40:18.000000 vipes-0.0.4/vipes/__main__.py
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)     1176 2023-06-26 19:18:43.000000 vipes-0.0.4/vipes/interpreter.py
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:12:45.443239 vipes-0.0.4/vipes.egg-info/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/PKG-INFO
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      231 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/SOURCES.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/dependency_links.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)       43 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/entry_points.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        6 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/top_level.txt
```

### Comparing `vipes-0.0.3/LICENSE` & `vipes-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vipes-0.0.3/PKG-INFO` & `vipes-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipes
-Version: 0.0.3
+Version: 0.0.4
 Summary: The most reliable script manager for crossplatform projects
 Home-page: https://github.com/flobbun/vipes
 Author: Jhon
 Keywords: script,manager,crossplatform,configuration
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `vipes-0.0.3/setup.py` & `vipes-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vipes',
-    version='0.0.3',
+    version='0.0.4',
     author='Jhon',
     description='The most reliable script manager for crossplatform projects',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/flobbun/vipes',
     classifiers=[
         'Programming Language :: Python :: 3.7',
```

### Comparing `vipes-0.0.3/vipes.egg-info/PKG-INFO` & `vipes-0.0.4/vipes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipes
-Version: 0.0.3
+Version: 0.0.4
 Summary: The most reliable script manager for crossplatform projects
 Home-page: https://github.com/flobbun/vipes
 Author: Jhon
 Keywords: script,manager,crossplatform,configuration
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

