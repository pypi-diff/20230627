# Comparing `tmp/autoclicker_geo-0.0.1.tar.gz` & `tmp/autoclicker_geo-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoclicker_geo-0.0.1.tar", last modified: Tue Jun 27 16:27:44 2023, max compression
+gzip compressed data, was "autoclicker_geo-0.0.10.tar", last modified: Tue Jun 27 16:31:38 2023, max compression
```

## Comparing `autoclicker_geo-0.0.1.tar` & `autoclicker_geo-0.0.10.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 16:27:44.021580 autoclicker_geo-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-27 16:27:44.008628 autoclicker_geo-0.0.1/Autoclicker_geo/
--rw-rw-rw-   0        0        0       35 2023-06-27 16:17:16.000000 autoclicker_geo-0.0.1/Autoclicker_geo/__init__.py
--rw-rw-rw-   0        0        0     1186 2023-06-27 15:52:37.000000 autoclicker_geo-0.0.1/Autoclicker_geo/autoclicker.py
--rw-rw-rw-   0        0        0        0 2023-06-27 16:14:56.000000 autoclicker_geo-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      490 2023-06-27 16:27:44.021580 autoclicker_geo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-27 16:14:03.000000 autoclicker_geo-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 16:27:44.020580 autoclicker_geo-0.0.1/autoclicker_geo.egg-info/
--rw-rw-rw-   0        0        0      490 2023-06-27 16:27:43.000000 autoclicker_geo-0.0.1/autoclicker_geo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-06-27 16:27:43.000000 autoclicker_geo-0.0.1/autoclicker_geo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 16:27:43.000000 autoclicker_geo-0.0.1/autoclicker_geo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 16:27:43.000000 autoclicker_geo-0.0.1/autoclicker_geo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 16:27:43.000000 autoclicker_geo-0.0.1/autoclicker_geo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 16:27:44.022578 autoclicker_geo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-06-27 16:27:31.000000 autoclicker_geo-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:31:38.718702 autoclicker_geo-0.0.10/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 16:29:17.000000 autoclicker_geo-0.0.10/LICENSE
+-rw-rw-rw-   0        0        0      551 2023-06-27 16:31:38.718702 autoclicker_geo-0.0.10/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-27 16:29:22.000000 autoclicker_geo-0.0.10/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 16:31:38.716196 autoclicker_geo-0.0.10/autoclicker_geo.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-06-27 16:31:38.000000 autoclicker_geo-0.0.10/autoclicker_geo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-27 16:31:38.000000 autoclicker_geo-0.0.10/autoclicker_geo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 16:31:38.000000 autoclicker_geo-0.0.10/autoclicker_geo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 16:31:38.000000 autoclicker_geo-0.0.10/autoclicker_geo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-27 16:31:38.000000 autoclicker_geo-0.0.10/autoclicker_geo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 16:31:38.719715 autoclicker_geo-0.0.10/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-06-27 16:31:36.000000 autoclicker_geo-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:31:38.717194 autoclicker_geo-0.0.10/src/
+-rw-rw-rw-   0        0        0       35 2023-06-27 16:17:16.000000 autoclicker_geo-0.0.10/src/__init__.py
+-rw-rw-rw-   0        0        0     1186 2023-06-27 15:52:37.000000 autoclicker_geo-0.0.10/src/autoclicker.py
```

### Comparing `autoclicker_geo-0.0.1/Autoclicker_geo/autoclicker.py` & `autoclicker_geo-0.0.10/src/autoclicker.py`

 * *Files identical despite different names*

### Comparing `autoclicker_geo-0.0.1/setup.py` & `autoclicker_geo-0.0.10/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+VERSION = '0.0.10'
 DESCRIPTION = 'Simple autoclicker for python'
+LONGDESCRIPTION = 'Simple autoclicker for python long description'
 
 # Setting up
 setup(
     name="autoclicker_geo",
     version=VERSION,
     author="Geo",
     author_email="<geocraft31@gamil.com>",
     description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
     packages=find_packages(),
     install_requires=['pynput', 'six'],
     keywords=['python', 'autoclicker'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

