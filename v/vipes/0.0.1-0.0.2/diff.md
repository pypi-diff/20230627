# Comparing `tmp/vipes-0.0.1.tar.gz` & `tmp/vipes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipes-0.0.1.tar", last modified: Mon Jun 26 22:20:12 2023, max compression
+gzip compressed data, was "vipes-0.0.2.tar", last modified: Mon Jun 26 23:55:09 2023, max compression
```

## Comparing `vipes-0.0.1.tar` & `vipes-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-26 22:20:12.193027 vipes-0.0.1/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)     1067 2023-06-26 20:30:07.000000 vipes-0.0.1/LICENSE
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      692 2023-06-26 22:20:12.192882 vipes-0.0.1/PKG-INFO
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      437 2023-06-26 22:18:09.000000 vipes-0.0.1/README.md
--rw-r--r--   0 jhonaguiar   (501) staff       (20)       38 2023-06-26 22:20:12.193063 vipes-0.0.1/setup.cfg
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      416 2023-06-26 22:17:36.000000 vipes-0.0.1/setup.py
-drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-26 22:20:12.192706 vipes-0.0.1/vipes.egg-info/
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      692 2023-06-26 22:20:12.000000 vipes-0.0.1/vipes.egg-info/PKG-INFO
--rw-r--r--   0 jhonaguiar   (501) staff       (20)      142 2023-06-26 22:20:12.000000 vipes-0.0.1/vipes.egg-info/SOURCES.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-26 22:20:12.000000 vipes-0.0.1/vipes.egg-info/dependency_links.txt
--rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-26 22:20:12.000000 vipes-0.0.1/vipes.egg-info/top_level.txt
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-26 23:55:09.350901 vipes-0.0.2/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)     1067 2023-06-26 20:30:07.000000 vipes-0.0.2/LICENSE
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-26 23:55:09.350758 vipes-0.0.2/PKG-INFO
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      437 2023-06-26 22:18:09.000000 vipes-0.0.2/README.md
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)       38 2023-06-26 23:55:09.350937 vipes-0.0.2/setup.cfg
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      702 2023-06-26 23:55:06.000000 vipes-0.0.2/setup.py
+drwxr-xr-x   0 jhonaguiar   (501) staff       (20)        0 2023-06-26 23:55:09.350593 vipes-0.0.2/vipes.egg-info/
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      848 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/PKG-INFO
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)      174 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/SOURCES.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/dependency_links.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)       46 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/entry_points.txt
+-rw-r--r--   0 jhonaguiar   (501) staff       (20)        1 2023-06-26 23:55:09.000000 vipes-0.0.2/vipes.egg-info/top_level.txt
```

### Comparing `vipes-0.0.1/LICENSE` & `vipes-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vipes-0.0.1/PKG-INFO` & `vipes-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: vipes
-Version: 0.0.1
+Version: 0.0.2
 Summary: The most reliable script manager for crossplatform projects
-Home-page: https://github.com/flobbun
+Home-page: https://github.com/flobbun/vipes
 Author: Jhon
+Keywords: script,manager,crossplatform,configuration
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vipes
 
 ## What is Vipes?
```

### Comparing `vipes-0.0.1/vipes.egg-info/PKG-INFO` & `vipes-0.0.2/vipes.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: vipes
-Version: 0.0.1
+Version: 0.0.2
 Summary: The most reliable script manager for crossplatform projects
-Home-page: https://github.com/flobbun
+Home-page: https://github.com/flobbun/vipes
 Author: Jhon
+Keywords: script,manager,crossplatform,configuration
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vipes
 
 ## What is Vipes?
```

