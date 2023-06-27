# Comparing `tmp/incantoos-1.0.3.tar.gz` & `tmp/incantoos-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incantoos-1.0.3.tar", last modified: Mon Jun 26 23:17:53 2023, max compression
+gzip compressed data, was "incantoos-1.0.4.tar", last modified: Tue Jun 27 03:34:33 2023, max compression
```

## Comparing `incantoos-1.0.3.tar` & `incantoos-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:17:53.214888 incantoos-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 23:17:43.000000 incantoos-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-26 23:17:53.214888 incantoos-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 23:17:43.000000 incantoos-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:17:53.214888 incantoos-1.0.3/incantoos/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 23:17:43.000000 incantoos-1.0.3/incantoos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:17:53.214888 incantoos-1.0.3/incantoos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-26 23:17:53.000000 incantoos-1.0.3/incantoos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-26 23:17:53.000000 incantoos-1.0.3/incantoos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:17:53.000000 incantoos-1.0.3/incantoos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 23:17:53.000000 incantoos-1.0.3/incantoos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 23:17:53.214888 incantoos-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 23:17:43.000000 incantoos-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:34:33.953731 incantoos-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 03:34:22.000000 incantoos-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 03:34:33.953731 incantoos-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-27 03:34:22.000000 incantoos-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:34:33.953731 incantoos-1.0.4/incantoos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-27 03:34:22.000000 incantoos-1.0.4/incantoos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:34:33.953731 incantoos-1.0.4/incantoos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 03:34:33.000000 incantoos-1.0.4/incantoos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 03:34:33.000000 incantoos-1.0.4/incantoos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:34:33.000000 incantoos-1.0.4/incantoos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 03:34:33.000000 incantoos-1.0.4/incantoos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 03:34:33.953731 incantoos-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-27 03:34:22.000000 incantoos-1.0.4/setup.py
```

### Comparing `incantoos-1.0.3/LICENSE` & `incantoos-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `incantoos-1.0.3/PKG-INFO` & `incantoos-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incantoos
-Version: 1.0.3
+Version: 1.0.4
 Summary: IncantoOS Is a wrapper related to OS functions that can be put into a smaller faster function
 Home-page: https://github.com/NinoTheMeano/incantoos
 Author: NinoTheMeano
 Author-email: ninosdeveloping@gmail.com
 Project-URL: Discord, https://discord.com/users/255125932447236096
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -36,12 +36,19 @@
 ```
 
 Prints the current system time.
 ```py
     incantoos.nowtime()
 ```
 
-Gives you a 8 character ID Ex. ("944b-fq8d")
+
 ```py
-    incantoos.ranid()
+    class ids
+
+    ids.fourdashfour()
+        Gives you a 8 character ID Ex. ("944b-fq8d")
+
+    ids.ranid(amount : int)
+        Gives you a randomized id of the specified amount
+        
 ```
```

### Comparing `incantoos-1.0.3/incantoos.egg-info/PKG-INFO` & `incantoos-1.0.4/incantoos.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incantoos
-Version: 1.0.3
+Version: 1.0.4
 Summary: IncantoOS Is a wrapper related to OS functions that can be put into a smaller faster function
 Home-page: https://github.com/NinoTheMeano/incantoos
 Author: NinoTheMeano
 Author-email: ninosdeveloping@gmail.com
 Project-URL: Discord, https://discord.com/users/255125932447236096
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -36,12 +36,19 @@
 ```
 
 Prints the current system time.
 ```py
     incantoos.nowtime()
 ```
 
-Gives you a 8 character ID Ex. ("944b-fq8d")
+
 ```py
-    incantoos.ranid()
+    class ids
+
+    ids.fourdashfour()
+        Gives you a 8 character ID Ex. ("944b-fq8d")
+
+    ids.ranid(amount : int)
+        Gives you a randomized id of the specified amount
+        
 ```
```

### Comparing `incantoos-1.0.3/setup.py` & `incantoos-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup_info = {
     "name": "incantoos",
-    "version": "1.0.3",
+    "version": "1.0.4",
     "author": "NinoTheMeano",
     "author_email": "ninosdeveloping@gmail.com",
     "description": "IncantoOS Is a wrapper related to OS functions that can be put into a smaller faster function",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "url": "https://github.com/NinoTheMeano/incantoos",
     "packages": setuptools.find_packages(),
```

