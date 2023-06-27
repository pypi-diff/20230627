# Comparing `tmp/yplib-1.8.3.tar.gz` & `tmp/yplib-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.8.3.tar", last modified: Tue Jun 27 01:46:02 2023, max compression
+gzip compressed data, was "dist\yplib-1.8.4.tar", last modified: Tue Jun 27 08:02:58 2023, max compression
```

## Comparing `yplib-1.8.3.tar` & `yplib-1.8.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 01:46:02.520671 yplib-1.8.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-27 01:46:02.520671 yplib-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 01:46:02.520671 yplib-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-27 01:45:24.000000 yplib-1.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:46:02.516619 yplib-1.8.3/yplib/
--rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-1.8.3/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-1.8.3/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.3/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.3/yplib/http_util.py
--rw-rw-rw-   0        0        0    26791 2023-06-27 01:45:16.000000 yplib-1.8.3/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.3/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:46:02.520114 yplib-1.8.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-27 01:46:02.000000 yplib-1.8.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-27 01:46:02.000000 yplib-1.8.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 01:46:02.000000 yplib-1.8.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-27 01:46:02.000000 yplib-1.8.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 08:02:58.188740 yplib-1.8.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-27 08:02:58.188740 yplib-1.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:02:58.189281 yplib-1.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-27 08:02:53.000000 yplib-1.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:02:58.185728 yplib-1.8.4/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-1.8.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-1.8.4/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.4/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.4/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26791 2023-06-27 01:45:16.000000 yplib-1.8.4/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-27 08:02:47.000000 yplib-1.8.4/yplib/mail.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.4/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:02:58.188067 yplib-1.8.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-27 08:02:57.000000 yplib-1.8.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-27 08:02:58.000000 yplib-1.8.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:02:57.000000 yplib-1.8.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 08:02:58.000000 yplib-1.8.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.8.3/LICENSE` & `yplib-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.8.3/setup.py` & `yplib-1.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.8.3",
+  version="1.8.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.8.3/yplib/chart.py` & `yplib-1.8.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.3/yplib/chart_html.py` & `yplib-1.8.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.3/yplib/db.py` & `yplib-1.8.4/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.3/yplib/file.py` & `yplib-1.8.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.3/yplib/http_util.py` & `yplib-1.8.4/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.3/yplib/index.py` & `yplib-1.8.4/yplib/index.py`

 * *Files identical despite different names*

