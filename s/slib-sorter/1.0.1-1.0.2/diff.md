# Comparing `tmp/slib-sorter-1.0.1.tar.gz` & `tmp/slib-sorter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.0.1.tar", last modified: Tue Jun 27 12:04:58 2023, max compression
+gzip compressed data, was "slib-sorter-1.0.2.tar", last modified: Tue Jun 27 12:22:51 2023, max compression
```

## Comparing `slib-sorter-1.0.1.tar` & `slib-sorter-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:04:58.938591 slib-sorter-1.0.1/
--rw-rw-rw-   0        0        0    11558 2023-06-27 11:10:13.000000 slib-sorter-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      262 2023-06-27 12:04:58.937605 slib-sorter-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-06-27 11:10:13.000000 slib-sorter-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 12:04:58.938591 slib-sorter-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      544 2023-06-27 12:02:44.000000 slib-sorter-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:04:58.936617 slib-sorter-1.0.1/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0      262 2023-06-27 12:04:58.000000 slib-sorter-1.0.1/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-27 12:04:58.000000 slib-sorter-1.0.1/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:04:58.000000 slib-sorter-1.0.1/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-27 12:04:58.000000 slib-sorter-1.0.1/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 12:04:58.000000 slib-sorter-1.0.1/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:04:58.000000 slib-sorter-1.0.1/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 12:22:51.627789 slib-sorter-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-27 11:10:13.000000 slib-sorter-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      262 2023-06-27 12:22:51.627789 slib-sorter-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-06-27 11:10:13.000000 slib-sorter-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:22:51.627789 slib-sorter-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      544 2023-06-27 12:22:02.000000 slib-sorter-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:22:51.626766 slib-sorter-1.0.2/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-06-27 12:22:51.000000 slib-sorter-1.0.2/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-27 12:22:51.000000 slib-sorter-1.0.2/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:22:51.000000 slib-sorter-1.0.2/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-27 12:22:51.000000 slib-sorter-1.0.2/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 12:22:51.000000 slib-sorter-1.0.2/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:22:51.000000 slib-sorter-1.0.2/slib_sorter.egg-info/top_level.txt
```

### Comparing `slib-sorter-1.0.1/LICENSE` & `slib-sorter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.0.1/README.md` & `slib-sorter-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.0.1/setup.py` & `slib-sorter-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="slib-sorter",
-    version="1.0.1",
+    version="1.0.2",
     readme = "README.md",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "slib-sorter = slib_sorter.__main__:main",
         ]
     },
```

