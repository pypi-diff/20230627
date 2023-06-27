# Comparing `tmp/autoclicker_geo-0.0.3.tar.gz` & `tmp/autoclicker_geo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoclicker_geo-0.0.3.tar", last modified: Tue Jun 27 17:04:27 2023, max compression
+gzip compressed data, was "autoclicker_geo-0.0.4.tar", last modified: Tue Jun 27 17:16:04 2023, max compression
```

## Comparing `autoclicker_geo-0.0.3.tar` & `autoclicker_geo-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 17:04:27.647363 autoclicker_geo-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-27 16:29:17.000000 autoclicker_geo-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1160 2023-06-27 17:04:27.647363 autoclicker_geo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-06-27 17:00:07.000000 autoclicker_geo-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 17:04:27.644371 autoclicker_geo-0.0.3/autoclicker_geo.egg-info/
--rw-rw-rw-   0        0        0     1160 2023-06-27 17:04:27.000000 autoclicker_geo-0.0.3/autoclicker_geo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-27 17:04:27.000000 autoclicker_geo-0.0.3/autoclicker_geo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 17:04:27.000000 autoclicker_geo-0.0.3/autoclicker_geo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 17:04:27.000000 autoclicker_geo-0.0.3/autoclicker_geo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-27 17:04:27.000000 autoclicker_geo-0.0.3/autoclicker_geo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 17:04:27.648359 autoclicker_geo-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-06-27 17:04:20.000000 autoclicker_geo-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:04:27.646365 autoclicker_geo-0.0.3/src/
--rw-rw-rw-   0        0        0       35 2023-06-27 16:17:16.000000 autoclicker_geo-0.0.3/src/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-06-27 16:59:01.000000 autoclicker_geo-0.0.3/src/autoclicker.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:16:04.274156 autoclicker_geo-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 16:29:17.000000 autoclicker_geo-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1160 2023-06-27 17:16:04.272899 autoclicker_geo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-06-27 17:00:07.000000 autoclicker_geo-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:16:04.270384 autoclicker_geo-0.0.4/autoclicker_geo.egg-info/
+-rw-rw-rw-   0        0        0     1160 2023-06-27 17:16:04.000000 autoclicker_geo-0.0.4/autoclicker_geo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-27 17:16:04.000000 autoclicker_geo-0.0.4/autoclicker_geo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:16:04.000000 autoclicker_geo-0.0.4/autoclicker_geo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 17:16:04.000000 autoclicker_geo-0.0.4/autoclicker_geo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-27 17:16:04.000000 autoclicker_geo-0.0.4/autoclicker_geo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:16:04.274156 autoclicker_geo-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-06-27 17:15:06.000000 autoclicker_geo-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:16:04.272899 autoclicker_geo-0.0.4/src/
+-rw-rw-rw-   0        0        0       35 2023-06-27 16:17:16.000000 autoclicker_geo-0.0.4/src/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-06-27 16:59:01.000000 autoclicker_geo-0.0.4/src/autoclicker.py
```

### Comparing `autoclicker_geo-0.0.3/LICENSE` & `autoclicker_geo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autoclicker_geo-0.0.3/PKG-INFO` & `autoclicker_geo-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoclicker_geo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple autoclicker for python
 Author: Geo
 Author-email: <geocraft31@gamil.com>
 Keywords: python,autoclicker
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autoclicker_geo-0.0.3/README.md` & `autoclicker_geo-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `autoclicker_geo-0.0.3/autoclicker_geo.egg-info/PKG-INFO` & `autoclicker_geo-0.0.4/autoclicker_geo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoclicker-geo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple autoclicker for python
 Author: Geo
 Author-email: <geocraft31@gamil.com>
 Keywords: python,autoclicker
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autoclicker_geo-0.0.3/setup.py` & `autoclicker_geo-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Simple autoclicker for python'
 LONGDESCRIPTION = 'Simple autoclicker for python long description'
 
 # Setting up
 setup(
     name="autoclicker_geo",
     version=VERSION,
```

### Comparing `autoclicker_geo-0.0.3/src/autoclicker.py` & `autoclicker_geo-0.0.4/src/autoclicker.py`

 * *Files identical despite different names*

