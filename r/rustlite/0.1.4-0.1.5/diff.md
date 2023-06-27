# Comparing `tmp/rustlite-0.1.4.tar.gz` & `tmp/rustlite-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustlite-0.1.4.tar", last modified: Tue Jun 27 08:18:44 2023, max compression
+gzip compressed data, was "rustlite-0.1.5.tar", last modified: Tue Jun 27 08:33:32 2023, max compression
```

## Comparing `rustlite-0.1.4.tar` & `rustlite-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:18:44.158654 rustlite-0.1.4/
--rw-rw-rw-   0        0        0      978 2023-06-27 08:18:44.158069 rustlite-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-06-27 08:07:58.000000 rustlite-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 08:18:44.144532 rustlite-0.1.4/rustlite/
--rw-rw-rw-   0        0        0       58 2023-06-26 20:35:57.000000 rustlite-0.1.4/rustlite/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-06-27 08:15:30.000000 rustlite-0.1.4/rustlite/enumerable.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:18:44.156055 rustlite-0.1.4/rustlite.egg-info/
--rw-rw-rw-   0        0        0      978 2023-06-27 08:18:44.000000 rustlite-0.1.4/rustlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-27 08:18:44.000000 rustlite-0.1.4/rustlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:18:44.000000 rustlite-0.1.4/rustlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 08:18:44.000000 rustlite-0.1.4/rustlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 08:18:44.159161 rustlite-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-06-27 08:18:21.000000 rustlite-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:33:32.578824 rustlite-0.1.5/
+-rw-rw-rw-   0        0        0      930 2023-06-27 08:33:32.577790 rustlite-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-06-27 08:32:59.000000 rustlite-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 08:33:32.566291 rustlite-0.1.5/rustlite/
+-rw-rw-rw-   0        0        0       58 2023-06-27 08:32:45.000000 rustlite-0.1.5/rustlite/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-06-27 08:15:30.000000 rustlite-0.1.5/rustlite/enumerable.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:33:32.577285 rustlite-0.1.5/rustlite.egg-info/
+-rw-rw-rw-   0        0        0      930 2023-06-27 08:33:32.000000 rustlite-0.1.5/rustlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-27 08:33:32.000000 rustlite-0.1.5/rustlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:33:32.000000 rustlite-0.1.5/rustlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 08:33:32.000000 rustlite-0.1.5/rustlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:33:32.578824 rustlite-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-06-27 08:33:27.000000 rustlite-0.1.5/setup.py
```

### Comparing `rustlite-0.1.4/PKG-INFO` & `rustlite-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustlite
-Version: 0.1.4
+Version: 0.1.5
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,14 +21,13 @@
 ```python
 ## create iterator for even integers squared
 even_integers = Iter[int](range(100)) \
     .filter(lambda x: x % 2 == 0) \
     .map(lambda x: x ** 2)
 
 ## to evaluate into a list use
-basic_list = even_integers.collect(list)
-smart_list = even_integers.to_list()
+my_list = even_integers.to_list()
 
 ## The smart list will allow the usage of iterator notation again by
-times2_iter = smart_list.iter() \
+times2_iter = my_list.iter() \
     .map(lambda x: x * 2)
 ```
```

### Comparing `rustlite-0.1.4/rustlite/enumerable.py` & `rustlite-0.1.5/rustlite/enumerable.py`

 * *Files identical despite different names*

### Comparing `rustlite-0.1.4/rustlite.egg-info/PKG-INFO` & `rustlite-0.1.5/rustlite.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustlite
-Version: 0.1.4
+Version: 0.1.5
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,14 +21,13 @@
 ```python
 ## create iterator for even integers squared
 even_integers = Iter[int](range(100)) \
     .filter(lambda x: x % 2 == 0) \
     .map(lambda x: x ** 2)
 
 ## to evaluate into a list use
-basic_list = even_integers.collect(list)
-smart_list = even_integers.to_list()
+my_list = even_integers.to_list()
 
 ## The smart list will allow the usage of iterator notation again by
-times2_iter = smart_list.iter() \
+times2_iter = my_list.iter() \
     .map(lambda x: x * 2)
 ```
```

