# Comparing `tmp/telexy.mars-1.23.621.tar.gz` & `tmp/telexy.mars-1.23.626.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telexy.mars-1.23.621.tar", last modified: Wed Jun 21 19:14:16 2023, max compression
+gzip compressed data, was "telexy.mars-1.23.626.tar", last modified: Mon Jun 26 22:48:52 2023, max compression
```

## Comparing `telexy.mars-1.23.621.tar` & `telexy.mars-1.23.626.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 19:14:16.615999 telexy.mars-1.23.621/
--rw-rw-rw-   0        0        0     1076 2023-06-21 19:06:45.000000 telexy.mars-1.23.621/LICENSE.txt
--rw-rw-rw-   0        0        0      478 2023-06-21 19:14:16.615000 telexy.mars-1.23.621/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 19:14:16.599484 telexy.mars-1.23.621/mars/
--rw-rw-rw-   0        0        0       23 2023-06-21 19:06:45.000000 telexy.mars-1.23.621/mars/__init__.py
--rw-rw-rw-   0        0        0      939 2023-06-21 19:13:46.000000 telexy.mars-1.23.621/mars/__main__.py
--rw-rw-rw-   0        0        0     1859 2023-06-21 19:09:15.000000 telexy.mars-1.23.621/mars/registry.py
--rw-rw-rw-   0        0        0       42 2023-06-21 19:14:16.615999 telexy.mars-1.23.621/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-06-21 19:09:35.000000 telexy.mars-1.23.621/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 19:14:16.612998 telexy.mars-1.23.621/telexy.mars.egg-info/
--rw-rw-rw-   0        0        0      478 2023-06-21 19:14:16.000000 telexy.mars-1.23.621/telexy.mars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-21 19:14:16.000000 telexy.mars-1.23.621/telexy.mars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 19:14:16.000000 telexy.mars-1.23.621/telexy.mars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-21 19:14:16.000000 telexy.mars-1.23.621/telexy.mars.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-21 19:14:16.000000 telexy.mars-1.23.621/telexy.mars.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 22:48:52.226575 telexy.mars-1.23.626/
+-rw-rw-rw-   0        0        0     1076 2023-06-21 19:06:45.000000 telexy.mars-1.23.626/LICENSE.txt
+-rw-rw-rw-   0        0        0      419 2023-06-26 22:48:52.225577 telexy.mars-1.23.626/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-06-21 19:13:15.000000 telexy.mars-1.23.626/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 22:48:52.216576 telexy.mars-1.23.626/mars/
+-rw-rw-rw-   0        0        0       23 2023-06-21 19:06:45.000000 telexy.mars-1.23.626/mars/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-06-21 19:13:46.000000 telexy.mars-1.23.626/mars/__main__.py
+-rw-rw-rw-   0        0        0     1859 2023-06-21 19:09:15.000000 telexy.mars-1.23.626/mars/registry.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 22:48:52.226575 telexy.mars-1.23.626/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-06-26 22:48:27.000000 telexy.mars-1.23.626/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:48:52.224576 telexy.mars-1.23.626/telexy.mars.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-26 22:48:52.000000 telexy.mars-1.23.626/telexy.mars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-26 22:48:52.000000 telexy.mars-1.23.626/telexy.mars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 22:48:52.000000 telexy.mars-1.23.626/telexy.mars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-26 22:48:52.000000 telexy.mars-1.23.626/telexy.mars.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 22:48:52.000000 telexy.mars-1.23.626/telexy.mars.egg-info/top_level.txt
```

### Comparing `telexy.mars-1.23.621/LICENSE.txt` & `telexy.mars-1.23.626/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `telexy.mars-1.23.621/mars/__main__.py` & `telexy.mars-1.23.626/mars/__main__.py`

 * *Files identical despite different names*

### Comparing `telexy.mars-1.23.621/mars/registry.py` & `telexy.mars-1.23.626/mars/registry.py`

 * *Files identical despite different names*

### Comparing `telexy.mars-1.23.621/setup.py` & `telexy.mars-1.23.626/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #To build/publish, use following commands
-#python3 setup.py sdist bdist_wheel - for build
+#python3 python3 -m build - for build
 #python3 -m twine upload dist/* - for publish
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="telexy.mars",                     # This is the name of the package
-    version="1.23.621",                        # The initial release version
+    version="1.23.626",                        # The initial release version
     author="Telexy",                     # Full name of the author
     author_email="support@telexy.com", # Full email of author
     description="Mars Inference server",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
```

