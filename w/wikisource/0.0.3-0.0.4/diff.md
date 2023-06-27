# Comparing `tmp/wikisource-0.0.3.tar.gz` & `tmp/wikisource-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikisource-0.0.3.tar", last modified: Tue Jun 27 10:13:22 2023, max compression
+gzip compressed data, was "wikisource-0.0.4.tar", last modified: Tue Jun 27 10:19:40 2023, max compression
```

## Comparing `wikisource-0.0.3.tar` & `wikisource-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 10:13:22.665979 wikisource-0.0.3/
--rw-r--r--   0 mathieu    (501) staff       (20)     1074 2023-06-27 09:07:24.000000 wikisource-0.0.3/LICENSE
--rw-r--r--   0 mathieu    (501) staff       (20)      382 2023-06-27 10:13:22.666019 wikisource-0.0.3/PKG-INFO
--rw-r--r--   0 mathieu    (501) staff       (20)     1014 2023-06-27 09:19:30.000000 wikisource-0.0.3/README.md
--rw-r--r--   0 mathieu    (501) staff       (20)      433 2023-06-27 09:59:41.000000 wikisource-0.0.3/pyproject.toml
--rw-r--r--   0 mathieu    (501) staff       (20)      108 2023-06-27 10:13:22.666180 wikisource-0.0.3/setup.cfg
--rw-r--r--   0 mathieu    (501) staff       (20)       38 2023-06-26 17:06:58.000000 wikisource-0.0.3/setup.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 10:13:22.664489 wikisource-0.0.3/tests/
--rw-r--r--   0 mathieu    (501) staff       (20)      765 2023-06-27 09:02:51.000000 wikisource-0.0.3/tests/test_chapter.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2214 2023-06-27 09:02:55.000000 wikisource-0.0.3/tests/test_collection.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2819 2023-06-27 09:02:57.000000 wikisource-0.0.3/tests/test_wikisource.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 10:13:22.665182 wikisource-0.0.3/wikisource/
--rw-r--r--   0 mathieu    (501) staff       (20)        0 2023-06-26 17:07:46.000000 wikisource-0.0.3/wikisource/__init__.py
--rw-r--r--   0 mathieu    (501) staff       (20)     1888 2023-06-26 22:49:59.000000 wikisource-0.0.3/wikisource/chapter.py
--rw-r--r--   0 mathieu    (501) staff       (20)      748 2023-06-27 10:13:11.000000 wikisource-0.0.3/wikisource/cli.py
--rw-r--r--   0 mathieu    (501) staff       (20)      962 2023-06-26 23:04:54.000000 wikisource-0.0.3/wikisource/collection.py
--rw-r--r--   0 mathieu    (501) staff       (20)      355 2023-06-26 23:08:19.000000 wikisource-0.0.3/wikisource/paragraph.py
--rw-r--r--   0 mathieu    (501) staff       (20)     3225 2023-06-26 23:04:30.000000 wikisource-0.0.3/wikisource/source.py
--rw-r--r--   0 mathieu    (501) staff       (20)      238 2023-06-26 22:08:48.000000 wikisource-0.0.3/wikisource/webpage.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 10:13:22.665890 wikisource-0.0.3/wikisource.egg-info/
--rw-r--r--   0 mathieu    (501) staff       (20)      382 2023-06-27 10:13:22.000000 wikisource-0.0.3/wikisource.egg-info/PKG-INFO
--rw-r--r--   0 mathieu    (501) staff       (20)      484 2023-06-27 10:13:22.000000 wikisource-0.0.3/wikisource.egg-info/SOURCES.txt
--rw-r--r--   0 mathieu    (501) staff       (20)        1 2023-06-27 10:13:22.000000 wikisource-0.0.3/wikisource.egg-info/dependency_links.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       44 2023-06-27 10:13:22.000000 wikisource-0.0.3/wikisource.egg-info/entry_points.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       13 2023-06-27 10:13:22.000000 wikisource-0.0.3/wikisource.egg-info/requires.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       11 2023-06-27 10:13:22.000000 wikisource-0.0.3/wikisource.egg-info/top_level.txt
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 10:19:40.913113 wikisource-0.0.4/
+-rw-r--r--   0 mathieu    (501) staff       (20)     1074 2023-06-27 09:07:24.000000 wikisource-0.0.4/LICENSE
+-rw-r--r--   0 mathieu    (501) staff       (20)      382 2023-06-27 10:19:40.913161 wikisource-0.0.4/PKG-INFO
+-rw-r--r--   0 mathieu    (501) staff       (20)     1014 2023-06-27 09:19:30.000000 wikisource-0.0.4/README.md
+-rw-r--r--   0 mathieu    (501) staff       (20)      433 2023-06-27 10:13:45.000000 wikisource-0.0.4/pyproject.toml
+-rw-r--r--   0 mathieu    (501) staff       (20)      108 2023-06-27 10:19:40.913333 wikisource-0.0.4/setup.cfg
+-rw-r--r--   0 mathieu    (501) staff       (20)       38 2023-06-26 17:06:58.000000 wikisource-0.0.4/setup.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 10:19:40.911463 wikisource-0.0.4/tests/
+-rw-r--r--   0 mathieu    (501) staff       (20)      765 2023-06-27 09:02:51.000000 wikisource-0.0.4/tests/test_chapter.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2214 2023-06-27 09:02:55.000000 wikisource-0.0.4/tests/test_collection.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2819 2023-06-27 09:02:57.000000 wikisource-0.0.4/tests/test_wikisource.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 10:19:40.912262 wikisource-0.0.4/wikisource/
+-rw-r--r--   0 mathieu    (501) staff       (20)        0 2023-06-26 17:07:46.000000 wikisource-0.0.4/wikisource/__init__.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     1888 2023-06-26 22:49:59.000000 wikisource-0.0.4/wikisource/chapter.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      878 2023-06-27 10:18:02.000000 wikisource-0.0.4/wikisource/cli.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      962 2023-06-26 23:04:54.000000 wikisource-0.0.4/wikisource/collection.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      355 2023-06-26 23:08:19.000000 wikisource-0.0.4/wikisource/paragraph.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     3225 2023-06-26 23:04:30.000000 wikisource-0.0.4/wikisource/source.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      238 2023-06-26 22:08:48.000000 wikisource-0.0.4/wikisource/webpage.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 10:19:40.913012 wikisource-0.0.4/wikisource.egg-info/
+-rw-r--r--   0 mathieu    (501) staff       (20)      382 2023-06-27 10:19:40.000000 wikisource-0.0.4/wikisource.egg-info/PKG-INFO
+-rw-r--r--   0 mathieu    (501) staff       (20)      484 2023-06-27 10:19:40.000000 wikisource-0.0.4/wikisource.egg-info/SOURCES.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)        1 2023-06-27 10:19:40.000000 wikisource-0.0.4/wikisource.egg-info/dependency_links.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       44 2023-06-27 10:19:40.000000 wikisource-0.0.4/wikisource.egg-info/entry_points.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       13 2023-06-27 10:19:40.000000 wikisource-0.0.4/wikisource.egg-info/requires.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       11 2023-06-27 10:19:40.000000 wikisource-0.0.4/wikisource.egg-info/top_level.txt
```

### Comparing `wikisource-0.0.3/LICENSE` & `wikisource-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.3/README.md` & `wikisource-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.3/tests/test_chapter.py` & `wikisource-0.0.4/tests/test_chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.3/tests/test_collection.py` & `wikisource-0.0.4/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.3/tests/test_wikisource.py` & `wikisource-0.0.4/tests/test_wikisource.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.3/wikisource/chapter.py` & `wikisource-0.0.4/wikisource/chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.3/wikisource/collection.py` & `wikisource-0.0.4/wikisource/collection.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.3/wikisource/source.py` & `wikisource-0.0.4/wikisource/source.py`

 * *Files identical despite different names*

