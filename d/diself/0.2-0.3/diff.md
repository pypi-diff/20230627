# Comparing `tmp/diself-0.2.tar.gz` & `tmp/diself-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diself-0.2.tar", last modified: Mon Jun 26 23:16:47 2023, max compression
+gzip compressed data, was "diself-0.3.tar", last modified: Mon Jun 26 23:21:35 2023, max compression
```

## Comparing `diself-0.2.tar` & `diself-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 23:16:47.598401 diself-0.2/
--rw-rw-rw-   0        0        0     1065 2023-06-26 22:08:08.000000 diself-0.2/LICENSE
--rw-rw-rw-   0        0        0     3201 2023-06-26 23:16:47.597401 diself-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2826 2023-06-26 23:10:20.000000 diself-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 23:16:47.592402 diself-0.2/diself/
--rw-rw-rw-   0        0        0        0 2023-06-26 18:32:05.000000 diself-0.2/diself/__init__.py
--rw-rw-rw-   0        0        0     4081 2023-06-26 22:56:31.000000 diself-0.2/diself/diself.py
-drwxrwxrwx   0        0        0        0 2023-06-26 23:16:47.596401 diself-0.2/diself.egg-info/
--rw-rw-rw-   0        0        0     3201 2023-06-26 23:16:47.000000 diself-0.2/diself.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-26 23:16:47.000000 diself-0.2/diself.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 23:16:47.000000 diself-0.2/diself.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-26 23:16:47.000000 diself-0.2/diself.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 23:16:47.000000 diself-0.2/diself.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 23:16:47.598401 diself-0.2/setup.cfg
--rw-rw-rw-   0        0        0      451 2023-06-26 23:16:36.000000 diself-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:21:35.088954 diself-0.3/
+-rw-rw-rw-   0        0        0     1065 2023-06-26 22:08:08.000000 diself-0.3/LICENSE
+-rw-rw-rw-   0        0        0     3201 2023-06-26 23:21:35.088954 diself-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2826 2023-06-26 23:10:20.000000 diself-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 23:21:35.083953 diself-0.3/diself/
+-rw-rw-rw-   0        0        0       13 2023-06-26 23:21:04.000000 diself-0.3/diself/__init__.py
+-rw-rw-rw-   0        0        0     4081 2023-06-26 22:56:31.000000 diself-0.3/diself/diself.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:21:35.087953 diself-0.3/diself.egg-info/
+-rw-rw-rw-   0        0        0     3201 2023-06-26 23:21:35.000000 diself-0.3/diself.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-26 23:21:35.000000 diself-0.3/diself.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 23:21:35.000000 diself-0.3/diself.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-26 23:21:35.000000 diself-0.3/diself.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 23:21:35.000000 diself-0.3/diself.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 23:21:35.089954 diself-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      451 2023-06-26 23:21:29.000000 diself-0.3/setup.py
```

### Comparing `diself-0.2/LICENSE` & `diself-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `diself-0.2/PKG-INFO` & `diself-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diself
-Version: 0.2
+Version: 0.3
 Summary: A python module like discord.py but for selfbot
 Home-page: https://github.com/lululepu/diself
 Author: Lululepu
 Author-email: a.no.qsdf@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `diself-0.2/README.md` & `diself-0.3/README.md`

 * *Files identical despite different names*

### Comparing `diself-0.2/diself/diself.py` & `diself-0.3/diself/diself.py`

 * *Files identical despite different names*

### Comparing `diself-0.2/diself.egg-info/PKG-INFO` & `diself-0.3/diself.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diself
-Version: 0.2
+Version: 0.3
 Summary: A python module like discord.py but for selfbot
 Home-page: https://github.com/lululepu/diself
 Author: Lululepu
 Author-email: a.no.qsdf@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

