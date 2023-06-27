# Comparing `tmp/pyfigtree-1.0.tar.gz` & `tmp/pyfigtree-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfigtree-1.0.tar", last modified: Tue Jun 27 13:13:41 2023, max compression
+gzip compressed data, was "pyfigtree-1.0.1.tar", last modified: Tue Jun 27 13:34:11 2023, max compression
```

## Comparing `pyfigtree-1.0.tar` & `pyfigtree-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 plumail   (1000) plumail   (1000)        0 2023-06-27 13:13:41.831405 pyfigtree-1.0/
--rw-r--r--   0 plumail   (1000) plumail   (1000)    18026 2023-06-27 12:46:15.000000 pyfigtree-1.0/LICENSE
--rw-r--r--   0 plumail   (1000) plumail   (1000)     4244 2023-06-27 13:13:41.831405 pyfigtree-1.0/PKG-INFO
--rw-r--r--   0 plumail   (1000) plumail   (1000)     3935 2023-06-27 12:48:51.000000 pyfigtree-1.0/README.md
-drwxr-xr-x   0 plumail   (1000) plumail   (1000)        0 2023-06-27 13:13:41.831405 pyfigtree-1.0/pyfigtree/
--rw-r--r--   0 plumail   (1000) plumail   (1000)       30 2023-06-27 12:44:44.000000 pyfigtree-1.0/pyfigtree/__init__.py
-drwxr-xr-x   0 plumail   (1000) plumail   (1000)        0 2023-06-27 13:13:41.831405 pyfigtree-1.0/pyfigtree/lib/
--rwxr-xr-x   0 plumail   (1000) plumail   (1000)    87120 2023-06-27 12:52:22.000000 pyfigtree-1.0/pyfigtree/lib/libann_figtree_version.so
--rwxr-xr-x   0 plumail   (1000) plumail   (1000)    82416 2023-06-27 12:52:22.000000 pyfigtree-1.0/pyfigtree/lib/libfigtree.so
--rw-r--r--   0 plumail   (1000) plumail   (1000)    21129 2023-06-27 13:09:34.000000 pyfigtree-1.0/pyfigtree/pyfigtree.py
-drwxr-xr-x   0 plumail   (1000) plumail   (1000)        0 2023-06-27 13:13:41.831405 pyfigtree-1.0/pyfigtree.egg-info/
--rw-r--r--   0 plumail   (1000) plumail   (1000)     4244 2023-06-27 13:13:41.000000 pyfigtree-1.0/pyfigtree.egg-info/PKG-INFO
--rw-r--r--   0 plumail   (1000) plumail   (1000)      286 2023-06-27 13:13:41.000000 pyfigtree-1.0/pyfigtree.egg-info/SOURCES.txt
--rw-r--r--   0 plumail   (1000) plumail   (1000)        1 2023-06-27 13:13:41.000000 pyfigtree-1.0/pyfigtree.egg-info/dependency_links.txt
--rw-r--r--   0 plumail   (1000) plumail   (1000)       10 2023-06-27 13:13:41.000000 pyfigtree-1.0/pyfigtree.egg-info/top_level.txt
--rw-r--r--   0 plumail   (1000) plumail   (1000)       81 2023-06-27 12:17:03.000000 pyfigtree-1.0/pyproject.toml
--rw-r--r--   0 plumail   (1000) plumail   (1000)       38 2023-06-27 13:13:41.831405 pyfigtree-1.0/setup.cfg
--rwxr-xr-x   0 plumail   (1000) plumail   (1000)     1323 2023-06-27 13:13:31.000000 pyfigtree-1.0/setup.py
+drwxr-xr-x   0 plumail   (1000) plumail   (1000)        0 2023-06-27 13:34:11.911405 pyfigtree-1.0.1/
+-rw-r--r--   0 plumail   (1000) plumail   (1000)    18026 2023-06-27 12:46:15.000000 pyfigtree-1.0.1/LICENSE
+-rw-r--r--   0 plumail   (1000) plumail   (1000)     4246 2023-06-27 13:34:11.911405 pyfigtree-1.0.1/PKG-INFO
+-rw-r--r--   0 plumail   (1000) plumail   (1000)     3935 2023-06-27 12:48:51.000000 pyfigtree-1.0.1/README.md
+drwxr-xr-x   0 plumail   (1000) plumail   (1000)        0 2023-06-27 13:34:11.911405 pyfigtree-1.0.1/pyfigtree/
+-rw-r--r--   0 plumail   (1000) plumail   (1000)       30 2023-06-27 12:44:44.000000 pyfigtree-1.0.1/pyfigtree/__init__.py
+drwxr-xr-x   0 plumail   (1000) plumail   (1000)        0 2023-06-27 13:34:11.911405 pyfigtree-1.0.1/pyfigtree/lib/
+-rwxr-xr-x   0 plumail   (1000) plumail   (1000)    87120 2023-06-27 12:52:22.000000 pyfigtree-1.0.1/pyfigtree/lib/libann_figtree_version.so
+-rwxr-xr-x   0 plumail   (1000) plumail   (1000)    82416 2023-06-27 12:52:22.000000 pyfigtree-1.0.1/pyfigtree/lib/libfigtree.so
+-rw-r--r--   0 plumail   (1000) plumail   (1000)    21129 2023-06-27 13:09:34.000000 pyfigtree-1.0.1/pyfigtree/pyfigtree.py
+drwxr-xr-x   0 plumail   (1000) plumail   (1000)        0 2023-06-27 13:34:11.911405 pyfigtree-1.0.1/pyfigtree.egg-info/
+-rw-r--r--   0 plumail   (1000) plumail   (1000)     4246 2023-06-27 13:34:11.000000 pyfigtree-1.0.1/pyfigtree.egg-info/PKG-INFO
+-rw-r--r--   0 plumail   (1000) plumail   (1000)      318 2023-06-27 13:34:11.000000 pyfigtree-1.0.1/pyfigtree.egg-info/SOURCES.txt
+-rw-r--r--   0 plumail   (1000) plumail   (1000)        1 2023-06-27 13:34:11.000000 pyfigtree-1.0.1/pyfigtree.egg-info/dependency_links.txt
+-rw-r--r--   0 plumail   (1000) plumail   (1000)        6 2023-06-27 13:34:11.000000 pyfigtree-1.0.1/pyfigtree.egg-info/requires.txt
+-rw-r--r--   0 plumail   (1000) plumail   (1000)       10 2023-06-27 13:34:11.000000 pyfigtree-1.0.1/pyfigtree.egg-info/top_level.txt
+-rw-r--r--   0 plumail   (1000) plumail   (1000)       81 2023-06-27 12:17:03.000000 pyfigtree-1.0.1/pyproject.toml
+-rw-r--r--   0 plumail   (1000) plumail   (1000)       38 2023-06-27 13:34:11.911405 pyfigtree-1.0.1/setup.cfg
+-rwxr-xr-x   0 plumail   (1000) plumail   (1000)     1358 2023-06-27 13:32:42.000000 pyfigtree-1.0.1/setup.py
```

### Comparing `pyfigtree-1.0/LICENSE` & `pyfigtree-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfigtree-1.0/PKG-INFO` & `pyfigtree-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfigtree
-Version: 1.0
+Version: 1.0.1
 Summary: Python ctypes wrapper of the figtree library for fast Gaussian summation
 Home-page: https://github.com/fredRos/pyfigtree
 Author: Frederik Beaujean
 Author-email: Frederik.Beaujean@lmu.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyfigtree-1.0/README.md` & `pyfigtree-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfigtree-1.0/pyfigtree/lib/libann_figtree_version.so` & `pyfigtree-1.0.1/pyfigtree/lib/libann_figtree_version.so`

 * *Files identical despite different names*

### Comparing `pyfigtree-1.0/pyfigtree/lib/libfigtree.so` & `pyfigtree-1.0.1/pyfigtree/lib/libfigtree.so`

 * *Files identical despite different names*

### Comparing `pyfigtree-1.0/pyfigtree/pyfigtree.py` & `pyfigtree-1.0.1/pyfigtree/pyfigtree.py`

 * *Files identical despite different names*

### Comparing `pyfigtree-1.0/pyfigtree.egg-info/PKG-INFO` & `pyfigtree-1.0.1/pyfigtree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfigtree
-Version: 1.0
+Version: 1.0.1
 Summary: Python ctypes wrapper of the figtree library for fast Gaussian summation
 Home-page: https://github.com/fredRos/pyfigtree
 Author: Frederik Beaujean
 Author-email: Frederik.Beaujean@lmu.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyfigtree-1.0/setup.py` & `pyfigtree-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,12 +29,14 @@
     # optional, the contents of README.md that were read earlier
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # See class BinaryDistribution that was defined earlier
     distclass=BinaryDistribution,
 
-    version='1.0',
+    install_requires=["numpy"],
+
+    version='1.0.1',
     author="Frederik Beaujean",
     author_email="Frederik.Beaujean@lmu.de",
     url="https://github.com/fredRos/pyfigtree"
 )
```

