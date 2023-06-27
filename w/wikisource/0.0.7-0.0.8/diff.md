# Comparing `tmp/wikisource-0.0.7.tar.gz` & `tmp/wikisource-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikisource-0.0.7.tar", last modified: Tue Jun 27 11:58:17 2023, max compression
+gzip compressed data, was "wikisource-0.0.8.tar", last modified: Tue Jun 27 12:00:35 2023, max compression
```

## Comparing `wikisource-0.0.7.tar` & `wikisource-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:58:17.050253 wikisource-0.0.7/
--rw-r--r--   0 mathieu    (501) staff       (20)     1074 2023-06-27 09:07:24.000000 wikisource-0.0.7/LICENSE
--rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 11:58:17.050308 wikisource-0.0.7/PKG-INFO
--rw-r--r--   0 mathieu    (501) staff       (20)     1014 2023-06-27 09:19:30.000000 wikisource-0.0.7/README.md
--rw-r--r--   0 mathieu    (501) staff       (20)      421 2023-06-27 11:57:50.000000 wikisource-0.0.7/pyproject.toml
--rw-r--r--   0 mathieu    (501) staff       (20)      108 2023-06-27 11:58:17.050506 wikisource-0.0.7/setup.cfg
--rw-r--r--   0 mathieu    (501) staff       (20)       38 2023-06-27 11:27:10.000000 wikisource-0.0.7/setup.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:58:17.046825 wikisource-0.0.7/tests/
--rw-r--r--   0 mathieu    (501) staff       (20)      765 2023-06-27 09:02:51.000000 wikisource-0.0.7/tests/test_chapter.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2214 2023-06-27 09:02:55.000000 wikisource-0.0.7/tests/test_collection.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2819 2023-06-27 09:02:57.000000 wikisource-0.0.7/tests/test_wikisource.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:58:17.049188 wikisource-0.0.7/wikisource/
--rw-r--r--   0 mathieu    (501) staff       (20)        0 2023-06-26 17:07:46.000000 wikisource-0.0.7/wikisource/__init__.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2565 2023-06-27 11:57:45.000000 wikisource-0.0.7/wikisource/chapter.py
--rw-r--r--   0 mathieu    (501) staff       (20)      878 2023-06-27 10:18:02.000000 wikisource-0.0.7/wikisource/cli.py
--rw-r--r--   0 mathieu    (501) staff       (20)     1923 2023-06-27 11:47:08.000000 wikisource-0.0.7/wikisource/collection.py
--rw-r--r--   0 mathieu    (501) staff       (20)      607 2023-06-27 11:47:37.000000 wikisource-0.0.7/wikisource/paragraph.py
--rw-r--r--   0 mathieu    (501) staff       (20)     4262 2023-06-27 11:57:33.000000 wikisource-0.0.7/wikisource/source.py
--rw-r--r--   0 mathieu    (501) staff       (20)      454 2023-06-27 11:50:30.000000 wikisource-0.0.7/wikisource/webpage.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:58:17.050142 wikisource-0.0.7/wikisource.egg-info/
--rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 11:58:17.000000 wikisource-0.0.7/wikisource.egg-info/PKG-INFO
--rw-r--r--   0 mathieu    (501) staff       (20)      484 2023-06-27 11:58:17.000000 wikisource-0.0.7/wikisource.egg-info/SOURCES.txt
--rw-r--r--   0 mathieu    (501) staff       (20)        1 2023-06-27 11:58:17.000000 wikisource-0.0.7/wikisource.egg-info/dependency_links.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       44 2023-06-27 11:58:17.000000 wikisource-0.0.7/wikisource.egg-info/entry_points.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       13 2023-06-27 11:58:17.000000 wikisource-0.0.7/wikisource.egg-info/requires.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       11 2023-06-27 11:58:17.000000 wikisource-0.0.7/wikisource.egg-info/top_level.txt
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 12:00:35.160277 wikisource-0.0.8/
+-rw-r--r--   0 mathieu    (501) staff       (20)     1074 2023-06-27 09:07:24.000000 wikisource-0.0.8/LICENSE
+-rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 12:00:35.160323 wikisource-0.0.8/PKG-INFO
+-rw-r--r--   0 mathieu    (501) staff       (20)     1014 2023-06-27 09:19:30.000000 wikisource-0.0.8/README.md
+-rw-r--r--   0 mathieu    (501) staff       (20)      421 2023-06-27 12:00:26.000000 wikisource-0.0.8/pyproject.toml
+-rw-r--r--   0 mathieu    (501) staff       (20)      108 2023-06-27 12:00:35.160503 wikisource-0.0.8/setup.cfg
+-rw-r--r--   0 mathieu    (501) staff       (20)       38 2023-06-27 11:27:10.000000 wikisource-0.0.8/setup.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 12:00:35.158257 wikisource-0.0.8/tests/
+-rw-r--r--   0 mathieu    (501) staff       (20)      765 2023-06-27 09:02:51.000000 wikisource-0.0.8/tests/test_chapter.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2214 2023-06-27 09:02:55.000000 wikisource-0.0.8/tests/test_collection.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2819 2023-06-27 09:02:57.000000 wikisource-0.0.8/tests/test_wikisource.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 12:00:35.159324 wikisource-0.0.8/wikisource/
+-rw-r--r--   0 mathieu    (501) staff       (20)        0 2023-06-26 17:07:46.000000 wikisource-0.0.8/wikisource/__init__.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2565 2023-06-27 11:57:45.000000 wikisource-0.0.8/wikisource/chapter.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      878 2023-06-27 10:18:02.000000 wikisource-0.0.8/wikisource/cli.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     1923 2023-06-27 11:47:08.000000 wikisource-0.0.8/wikisource/collection.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      607 2023-06-27 11:47:37.000000 wikisource-0.0.8/wikisource/paragraph.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     4261 2023-06-27 12:00:09.000000 wikisource-0.0.8/wikisource/source.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      454 2023-06-27 11:50:30.000000 wikisource-0.0.8/wikisource/webpage.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 12:00:35.160190 wikisource-0.0.8/wikisource.egg-info/
+-rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/PKG-INFO
+-rw-r--r--   0 mathieu    (501) staff       (20)      484 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/SOURCES.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)        1 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/dependency_links.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       44 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/entry_points.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       13 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/requires.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       11 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/top_level.txt
```

### Comparing `wikisource-0.0.7/LICENSE` & `wikisource-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/PKG-INFO` & `wikisource-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikisource
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to search in books available on wikisource.org
 Author-email: "Mathieu G." <mathieu6700417@gmail.com>
 Project-URL: Homepage, https://github.com/mathieu6700417/wikisource
 Project-URL: Bug Tracker, https://github.com/mathieu6700417/wikisource/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wikisource-0.0.7/README.md` & `wikisource-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/tests/test_chapter.py` & `wikisource-0.0.8/tests/test_chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/tests/test_collection.py` & `wikisource-0.0.8/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/tests/test_wikisource.py` & `wikisource-0.0.8/tests/test_wikisource.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/wikisource/chapter.py` & `wikisource-0.0.8/wikisource/chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/wikisource/cli.py` & `wikisource-0.0.8/wikisource/cli.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/wikisource/collection.py` & `wikisource-0.0.8/wikisource/collection.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/wikisource/paragraph.py` & `wikisource-0.0.8/wikisource/paragraph.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.7/wikisource/source.py` & `wikisource-0.0.8/wikisource/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re, os
 import requests
 from bs4 import BeautifulSoup
 from .chapter import Chapter
 from .webpage import WebPage
 import json
 from dataclasses import dataclass
-from typings import Optional
+from typing import Optional
 
 @dataclass
 class ChapterLink:
     title: str
     url: str
```

### Comparing `wikisource-0.0.7/wikisource.egg-info/PKG-INFO` & `wikisource-0.0.8/wikisource.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikisource
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to search in books available on wikisource.org
 Author-email: "Mathieu G." <mathieu6700417@gmail.com>
 Project-URL: Homepage, https://github.com/mathieu6700417/wikisource
 Project-URL: Bug Tracker, https://github.com/mathieu6700417/wikisource/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

