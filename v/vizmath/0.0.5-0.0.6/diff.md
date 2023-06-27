# Comparing `tmp/vizmath-0.0.5.tar.gz` & `tmp/vizmath-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vizmath-0.0.5.tar", last modified: Tue Jun 27 04:00:04 2023, max compression
+gzip compressed data, was "dist\vizmath-0.0.6.tar", last modified: Tue Jun 27 04:17:56 2023, max compression
```

## Comparing `vizmath-0.0.5.tar` & `vizmath-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 04:00:04.000000 vizmath-0.0.5/
--rw-rw-rw-   0        0        0      517 2023-06-27 04:00:04.000000 vizmath-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-27 01:09:47.000000 vizmath-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 04:00:04.000000 vizmath-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-06-27 03:58:40.000000 vizmath-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 04:00:04.000000 vizmath-0.0.5/vizmath/
--rw-rw-rw-   0        0        0       67 2023-06-27 03:58:45.000000 vizmath-0.0.5/vizmath/__init__.py
--rw-rw-rw-   0        0        0    22127 2023-06-27 03:59:17.000000 vizmath-0.0.5/vizmath/vizmath.py
-drwxrwxrwx   0        0        0        0 2023-06-27 04:00:04.000000 vizmath-0.0.5/vizmath.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-27 04:00:04.000000 vizmath-0.0.5/vizmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-27 04:00:04.000000 vizmath-0.0.5/vizmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 04:00:04.000000 vizmath-0.0.5/vizmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-27 04:00:04.000000 vizmath-0.0.5/vizmath.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-27 04:00:04.000000 vizmath-0.0.5/vizmath.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 04:17:56.000000 vizmath-0.0.6/
+-rw-rw-rw-   0        0        0      517 2023-06-27 04:17:56.000000 vizmath-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-27 01:09:47.000000 vizmath-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 04:17:56.000000 vizmath-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-06-27 04:17:08.000000 vizmath-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:17:56.000000 vizmath-0.0.6/vizmath/
+-rw-rw-rw-   0        0        0       67 2023-06-27 04:16:47.000000 vizmath-0.0.6/vizmath/__init__.py
+-rw-rw-rw-   0        0        0    22178 2023-06-27 04:16:35.000000 vizmath-0.0.6/vizmath/vizmath.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:17:56.000000 vizmath-0.0.6/vizmath.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-06-27 04:17:55.000000 vizmath-0.0.6/vizmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-27 04:17:55.000000 vizmath-0.0.6/vizmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 04:17:55.000000 vizmath-0.0.6/vizmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-27 04:17:55.000000 vizmath-0.0.6/vizmath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 04:17:55.000000 vizmath-0.0.6/vizmath.egg-info/top_level.txt
```

### Comparing `vizmath-0.0.5/PKG-INFO` & `vizmath-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vizmath
-Version: 0.0.5
+Version: 0.0.6
 Summary: Visualization math toolkit.
 Home-page: https://github.com/nickgerend/vizmath
 Author: Nick Gerend
 Author-email: nickgerend@gmail.com
 License: MIT
 Description: # Welcome to vizmath
```

### Comparing `vizmath-0.0.5/setup.py` & `vizmath-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools as st
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="vizmath",
-    version="0.0.5",
+    version="0.0.6",
     description="Visualization math toolkit.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/nickgerend/vizmath",
     author="Nick Gerend",
     author_email="nickgerend@gmail.com",
     license="MIT",
```

### Comparing `vizmath-0.0.5/vizmath/vizmath.py` & `vizmath-0.0.6/vizmath/vizmath.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,16 +415,17 @@
         Zout_x0 = np.concatenate([Zout1_x0, Zout2_x0])
         Zout_y0 = np.concatenate([Zout1_y0, Zout2_y0])
 
         zip(Yout,Xout,Zout,Zout_x0,Zout_y0)
 
 class points:
 
-    viz=[]
-    df = pd.DataFrame()
+    def __init__(self):
+            self.viz=[]
+            self.df = pd.DataFrame()
 
     class point:
 
         def __init__(self, id=None, x=0.0, y=0.0, path=0, kwargs=None):
             self.id = id
             self.x = x
             self.y = y
```

### Comparing `vizmath-0.0.5/vizmath.egg-info/PKG-INFO` & `vizmath-0.0.6/vizmath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vizmath
-Version: 0.0.5
+Version: 0.0.6
 Summary: Visualization math toolkit.
 Home-page: https://github.com/nickgerend/vizmath
 Author: Nick Gerend
 Author-email: nickgerend@gmail.com
 License: MIT
 Description: # Welcome to vizmath
```

