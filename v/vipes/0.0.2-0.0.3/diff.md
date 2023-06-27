# Comparing `tmp/vipes-0.0.2.tar.gz` & `tmp/vipes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipes-0.0.2.tar", last modified: Mon Jun 26 23:55:09 2023, max compression
+gzip compressed data, was "vipes-0.0.3.tar", last modified: Tue Jun 27 00:04:13 2023, max compression
```

## Comparing `vipes-0.0.2.tar` & `vipes-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-26 23:55:09.350901 vipes-0.0.2/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)     1067 2023-06-26 20:30:07.000000 vipes-0.0.2/LICENSE
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-26 23:55:09.350758 vipes-0.0.2/PKG-INFO
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      437 2023-06-26 22:18:09.000000 vipes-0.0.2/README.md
--rw-r--r--   0 jhonaguiar   (501) staff       (20)       38 2023-06-26 23:55:09.350937 vipes-0.0.2/setup.cfg
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      702 2023-06-26 23:55:06.000000 vipes-0.0.2/setup.py
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-26 23:55:09.350593 vipes-0.0.2/vipes.egg-info/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/PKG-INFO
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      174 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/SOURCES.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/dependency_links.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)       46 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/entry_points.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/top_level.txt
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:04:13.520237 vipes-0.0.3/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)     1067 2023-06-26 20:30:07.000000 vipes-0.0.3/LICENSE
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:04:13.520084 vipes-0.0.3/PKG-INFO
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      437 2023-06-26 22:18:09.000000 vipes-0.0.3/README.md
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)       38 2023-06-27 00:04:13.520274 vipes-0.0.3/setup.cfg
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      699 2023-06-27 00:02:18.000000 vipes-0.0.3/setup.py
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-27 00:04:13.519792 vipes-0.0.3/vipes.egg-info/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/PKG-INFO
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      174 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/SOURCES.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/dependency_links.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)       43 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/entry_points.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-27 00:04:13.000000 vipes-0.0.3/vipes.egg-info/top_level.txt
```

### Comparing `vipes-0.0.2/LICENSE` & `vipes-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vipes-0.0.2/PKG-INFO` & `vipes-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipes
-Version: 0.0.2
+Version: 0.0.3
 Summary: The most reliable script manager for crossplatform projects
 Home-page: https://github.com/flobbun/vipes
 Author: Jhon
 Keywords: script,manager,crossplatform,configuration
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `vipes-0.0.2/setup.py` & `vipes-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vipes',
-    version='0.0.2',
+    version='0.0.3',
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
-        vipes=vipes.__main__:main
+        vipes=vipes.vipes:main
     ''',
     include_package_data=False
 )
```

### Comparing `vipes-0.0.2/vipes.egg-info/PKG-INFO` & `vipes-0.0.3/vipes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipes
-Version: 0.0.2
+Version: 0.0.3
 Summary: The most reliable script manager for crossplatform projects
 Home-page: https://github.com/flobbun/vipes
 Author: Jhon
 Keywords: script,manager,crossplatform,configuration
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

