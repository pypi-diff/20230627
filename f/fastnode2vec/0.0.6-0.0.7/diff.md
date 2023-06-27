# Comparing `tmp/fastnode2vec-0.0.6.tar.gz` & `tmp/fastnode2vec-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastnode2vec-0.0.6.tar", last modified: Sat Mar 26 22:32:30 2022, max compression
+gzip compressed data, was "fastnode2vec-0.0.7.tar", last modified: Tue Jun 27 09:50:33 2023, max compression
```

## Comparing `fastnode2vec-0.0.6.tar` & `fastnode2vec-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2022-03-26 22:32:30.031933 fastnode2vec-0.0.6/
--rw-r--r--   0 louisabraham   (501) staff       (20)     1070 2021-05-23 20:42:53.000000 fastnode2vec-0.0.6/LICENSE
--rw-r--r--   0 louisabraham   (501) staff       (20)     2853 2022-03-26 22:32:30.031718 fastnode2vec-0.0.6/PKG-INFO
--rw-r--r--   0 louisabraham   (501) staff       (20)     2451 2022-03-26 22:31:22.000000 fastnode2vec-0.0.6/README.md
-drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2022-03-26 22:32:30.030477 fastnode2vec-0.0.6/fastnode2vec/
--rw-r--r--   0 louisabraham   (501) staff       (20)       89 2021-05-23 20:42:53.000000 fastnode2vec-0.0.6/fastnode2vec/__init__.py
--rw-r--r--   0 louisabraham   (501) staff       (20)     1315 2021-05-23 20:42:53.000000 fastnode2vec-0.0.6/fastnode2vec/build_graph.py
--rw-r--r--   0 louisabraham   (501) staff       (20)     1640 2021-05-23 20:42:53.000000 fastnode2vec-0.0.6/fastnode2vec/cli.py
--rw-r--r--   0 louisabraham   (501) staff       (20)     4883 2022-03-26 22:31:26.000000 fastnode2vec-0.0.6/fastnode2vec/graph.py
--rw-r--r--   0 louisabraham   (501) staff       (20)     2446 2022-03-26 22:24:36.000000 fastnode2vec-0.0.6/fastnode2vec/node2vec.py
-drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2022-03-26 22:32:30.031496 fastnode2vec-0.0.6/fastnode2vec.egg-info/
--rw-r--r--   0 louisabraham   (501) staff       (20)     2853 2022-03-26 22:32:29.000000 fastnode2vec-0.0.6/fastnode2vec.egg-info/PKG-INFO
--rw-r--r--   0 louisabraham   (501) staff       (20)      364 2022-03-26 22:32:29.000000 fastnode2vec-0.0.6/fastnode2vec.egg-info/SOURCES.txt
--rw-r--r--   0 louisabraham   (501) staff       (20)        1 2022-03-26 22:32:29.000000 fastnode2vec-0.0.6/fastnode2vec.egg-info/dependency_links.txt
--rw-r--r--   0 louisabraham   (501) staff       (20)       60 2022-03-26 22:32:29.000000 fastnode2vec-0.0.6/fastnode2vec.egg-info/entry_points.txt
--rw-r--r--   0 louisabraham   (501) staff       (20)       30 2022-03-26 22:32:29.000000 fastnode2vec-0.0.6/fastnode2vec.egg-info/requires.txt
--rw-r--r--   0 louisabraham   (501) staff       (20)       13 2022-03-26 22:32:29.000000 fastnode2vec-0.0.6/fastnode2vec.egg-info/top_level.txt
--rw-r--r--   0 louisabraham   (501) staff       (20)       38 2022-03-26 22:32:30.031999 fastnode2vec-0.0.6/setup.cfg
--rw-r--r--   0 louisabraham   (501) staff       (20)      790 2022-03-26 22:31:48.000000 fastnode2vec-0.0.6/setup.py
+drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2023-06-27 09:50:33.031015 fastnode2vec-0.0.7/
+-rw-r--r--   0 louisabraham   (501) staff       (20)     1070 2021-05-23 20:42:53.000000 fastnode2vec-0.0.7/LICENSE
+-rw-r--r--   0 louisabraham   (501) staff       (20)     2839 2023-06-27 09:50:33.030760 fastnode2vec-0.0.7/PKG-INFO
+-rw-r--r--   0 louisabraham   (501) staff       (20)     2457 2023-05-13 09:44:05.000000 fastnode2vec-0.0.7/README.md
+drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2023-06-27 09:50:33.029171 fastnode2vec-0.0.7/fastnode2vec/
+-rw-r--r--   0 louisabraham   (501) staff       (20)       89 2021-05-23 20:42:53.000000 fastnode2vec-0.0.7/fastnode2vec/__init__.py
+-rw-r--r--   0 louisabraham   (501) staff       (20)     1315 2021-05-23 20:42:53.000000 fastnode2vec-0.0.7/fastnode2vec/build_graph.py
+-rw-r--r--   0 louisabraham   (501) staff       (20)     1640 2021-05-23 20:42:53.000000 fastnode2vec-0.0.7/fastnode2vec/cli.py
+-rw-r--r--   0 louisabraham   (501) staff       (20)     6721 2023-05-13 09:44:19.000000 fastnode2vec-0.0.7/fastnode2vec/graph.py
+-rw-r--r--   0 louisabraham   (501) staff       (20)     7123 2023-06-27 09:49:25.000000 fastnode2vec-0.0.7/fastnode2vec/node2vec.py
+drwxr-xr-x   0 louisabraham   (501) staff       (20)        0 2023-06-27 09:50:33.030513 fastnode2vec-0.0.7/fastnode2vec.egg-info/
+-rw-r--r--   0 louisabraham   (501) staff       (20)     2839 2023-06-27 09:50:32.000000 fastnode2vec-0.0.7/fastnode2vec.egg-info/PKG-INFO
+-rw-r--r--   0 louisabraham   (501) staff       (20)      364 2023-06-27 09:50:32.000000 fastnode2vec-0.0.7/fastnode2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 louisabraham   (501) staff       (20)        1 2023-06-27 09:50:32.000000 fastnode2vec-0.0.7/fastnode2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 louisabraham   (501) staff       (20)       59 2023-06-27 09:50:32.000000 fastnode2vec-0.0.7/fastnode2vec.egg-info/entry_points.txt
+-rw-r--r--   0 louisabraham   (501) staff       (20)       30 2023-06-27 09:50:32.000000 fastnode2vec-0.0.7/fastnode2vec.egg-info/requires.txt
+-rw-r--r--   0 louisabraham   (501) staff       (20)       13 2023-06-27 09:50:32.000000 fastnode2vec-0.0.7/fastnode2vec.egg-info/top_level.txt
+-rw-r--r--   0 louisabraham   (501) staff       (20)       38 2023-06-27 09:50:33.031084 fastnode2vec-0.0.7/setup.cfg
+-rw-r--r--   0 louisabraham   (501) staff       (20)      791 2023-06-27 09:50:06.000000 fastnode2vec-0.0.7/setup.py
```

### Comparing `fastnode2vec-0.0.6/LICENSE` & `fastnode2vec-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastnode2vec-0.0.6/PKG-INFO` & `fastnode2vec-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fastnode2vec
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fast implementation of node2vec
 Home-page: https://github.com/louisabraham/fastnode2vec
 Author: Louis Abraham
 Author-email: louis.abraham@yahoo.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Downloads](https://pepy.tech/badge/fastnode2vec)](https://pepy.tech/project/fastnode2vec) [![PyPI
 version](https://badge.fury.io/py/fastnode2vec.svg)](https://badge.fury.io/py/fastnode2vec)
@@ -90,12 +89,10 @@
 ```
 @software{fastnode2vec,
   author       = {Louis Abraham},
   title        = {fastnode2vec},
   year         = 2020,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.3902632},
-  url          = {https://doi.org/10.5281/zenodo.3902632}
+  url          = {https://github.com/louisabraham/fastnode2vec}
 }
 ```
-
-
```

### Comparing `fastnode2vec-0.0.6/README.md` & `fastnode2vec-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -144,11 +144,11 @@
 000008f0: 7665 637d 2c0a 2020 7965 6172 2020 2020  vec},.  year    
 00000900: 2020 2020 203d 2032 3032 302c 0a20 2070       = 2020,.  p
 00000910: 7562 6c69 7368 6572 2020 2020 3d20 7b5a  ublisher    = {Z
 00000920: 656e 6f64 6f7d 2c0a 2020 646f 6920 2020  enodo},.  doi   
 00000930: 2020 2020 2020 203d 207b 3130 2e35 3238         = {10.528
 00000940: 312f 7a65 6e6f 646f 2e33 3930 3236 3332  1/zenodo.3902632
 00000950: 7d2c 0a20 2075 726c 2020 2020 2020 2020  },.  url        
-00000960: 2020 3d20 7b68 7474 7073 3a2f 2f64 6f69    = {https://doi
-00000970: 2e6f 7267 2f31 302e 3532 3831 2f7a 656e  .org/10.5281/zen
-00000980: 6f64 6f2e 3339 3032 3633 327d 0a7d 0a60  odo.3902632}.}.`
-00000990: 6060 0a                                  ``.
+00000960: 2020 3d20 7b68 7474 7073 3a2f 2f67 6974    = {https://git
+00000970: 6875 622e 636f 6d2f 6c6f 7569 7361 6272  hub.com/louisabr
+00000980: 6168 616d 2f66 6173 746e 6f64 6532 7665  aham/fastnode2ve
+00000990: 637d 0a7d 0a60 6060 0a                   c}.}.```.
```

### Comparing `fastnode2vec-0.0.6/fastnode2vec/build_graph.py` & `fastnode2vec-0.0.7/fastnode2vec/build_graph.py`

 * *Files identical despite different names*

### Comparing `fastnode2vec-0.0.6/fastnode2vec/cli.py` & `fastnode2vec-0.0.7/fastnode2vec/cli.py`

 * *Files identical despite different names*

### Comparing `fastnode2vec-0.0.6/fastnode2vec.egg-info/PKG-INFO` & `fastnode2vec-0.0.7/fastnode2vec.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fastnode2vec
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fast implementation of node2vec
 Home-page: https://github.com/louisabraham/fastnode2vec
 Author: Louis Abraham
 Author-email: louis.abraham@yahoo.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Downloads](https://pepy.tech/badge/fastnode2vec)](https://pepy.tech/project/fastnode2vec) [![PyPI
 version](https://badge.fury.io/py/fastnode2vec.svg)](https://badge.fury.io/py/fastnode2vec)
@@ -90,12 +89,10 @@
 ```
 @software{fastnode2vec,
   author       = {Louis Abraham},
   title        = {fastnode2vec},
   year         = 2020,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.3902632},
-  url          = {https://doi.org/10.5281/zenodo.3902632}
+  url          = {https://github.com/louisabraham/fastnode2vec}
 }
 ```
-
-
```

### Comparing `fastnode2vec-0.0.6/setup.py` & `fastnode2vec-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python3
 
 import os
+
 from setuptools import setup
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="fastnode2vec",
-    version="0.0.6",
+    version="0.0.7",
     author="Louis Abraham",
     license="MIT",
     author_email="louis.abraham@yahoo.fr",
     description="Fast implementation of node2vec",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/louisabraham/fastnode2vec",
```

