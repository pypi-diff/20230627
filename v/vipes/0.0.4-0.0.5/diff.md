# Comparing `tmp/vipes-0.0.4.tar.gz` & `tmp/vipes-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipes-0.0.4.tar", last modified: Tue Jun 27 00:12:45 2023, max compression
+gzip compressed data, was "vipes-0.0.5.tar", last modified: Tue Jun 27 00:17:39 2023, max compression
```

## Comparing `vipes-0.0.4.tar` & `vipes-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:12:45.443639 vipes-0.0.4/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)     1067 2023-06-26 20:30:07.000000 vipes-0.0.4/LICENSE
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:12:45.443469 vipes-0.0.4/PKG-INFO
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      437 2023-06-26 22:18:09.000000 vipes-0.0.4/README.md
--rw-r--r--   0 jhonaguiar   (501) staff       (20)       38 2023-06-27 00:12:45.443694 vipes-0.0.4/setup.cfg
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      699 2023-06-27 00:12:34.000000 vipes-0.0.4/setup.py
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:12:45.442350 vipes-0.0.4/vipes/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:09:01.000000 vipes-0.0.4/vipes/__init__.py
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      604 2023-06-26 19:40:18.000000 vipes-0.0.4/vipes/__main__.py
--rw-r--r--   0 jhonaguiar   (501) staff       (20)     1176 2023-06-26 19:18:43.000000 vipes-0.0.4/vipes/interpreter.py
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:12:45.443239 vipes-0.0.4/vipes.egg-info/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/PKG-INFO
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      231 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/SOURCES.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/dependency_links.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)       43 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/entry_points.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        6 2023-06-27 00:12:45.000000 vipes-0.0.4/vipes.egg-info/top_level.txt
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:17:39.752632 vipes-0.0.5/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)     1067 2023-06-26 20:30:07.000000 vipes-0.0.5/LICENSE
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:17:39.752481 vipes-0.0.5/PKG-INFO
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      437 2023-06-26 22:18:09.000000 vipes-0.0.5/README.md
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)       38 2023-06-27 00:17:39.752670 vipes-0.0.5/setup.cfg
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      697 2023-06-27 00:17:26.000000 vipes-0.0.5/setup.py
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:17:39.751763 vipes-0.0.5/vipes/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:09:01.000000 vipes-0.0.5/vipes/__init__.py
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      604 2023-06-26 19:40:18.000000 vipes-0.0.5/vipes/cli.py
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)     1176 2023-06-26 19:18:43.000000 vipes-0.0.5/vipes/interpreter.py
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:17:39.752300 vipes-0.0.5/vipes.egg-info/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:17:39.000000 vipes-0.0.5/vipes.egg-info/PKG-INFO
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      226 2023-06-27 00:17:39.000000 vipes-0.0.5/vipes.egg-info/SOURCES.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-27 00:17:39.000000 vipes-0.0.5/vipes.egg-info/dependency_links.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)       41 2023-06-27 00:17:39.000000 vipes-0.0.5/vipes.egg-info/entry_points.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        6 2023-06-27 00:17:39.000000 vipes-0.0.5/vipes.egg-info/top_level.txt
```

### Comparing `vipes-0.0.4/LICENSE` & `vipes-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vipes-0.0.4/PKG-INFO` & `vipes-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipes
-Version: 0.0.4
+Version: 0.0.5
 Summary: The most reliable script manager for crossplatform projects
 Home-page: https://github.com/flobbun/vipes
 Author: Jhon
 Keywords: script,manager,crossplatform,configuration
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `vipes-0.0.4/setup.py` & `vipes-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vipes',
-    version='0.0.4',
+    version='0.0.5',
     author='Jhon',
     description='The most reliable script manager for crossplatform projects',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/flobbun/vipes',
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Operating System :: OS Independent',
     ],
     keywords=['script', 'manager', 'crossplatform', 'configuration'],
     packages=find_packages(),
     python_requires='>=3.7',
     entry_points='''
         [console_scripts]
-        vipes=vipes.vipes:main
+        vipes=vipes.cli:main
     ''',
     include_package_data=False
 )
```

### Comparing `vipes-0.0.4/vipes/__main__.py` & `vipes-0.0.5/vipes/cli.py`

 * *Files identical despite different names*

### Comparing `vipes-0.0.4/vipes/interpreter.py` & `vipes-0.0.5/vipes/interpreter.py`

 * *Files identical despite different names*

### Comparing `vipes-0.0.4/vipes.egg-info/PKG-INFO` & `vipes-0.0.5/vipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipes
-Version: 0.0.4
+Version: 0.0.5
 Summary: The most reliable script manager for crossplatform projects
 Home-page: https://github.com/flobbun/vipes
 Author: Jhon
 Keywords: script,manager,crossplatform,configuration
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

