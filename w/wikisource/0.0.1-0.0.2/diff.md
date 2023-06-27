# Comparing `tmp/wikisource-0.0.1.tar.gz` & `tmp/wikisource-0.0.2.tar.gz`

## Comparing `wikisource-0.0.1.tar` & `wikisource-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 wikisource-0.0.1/README.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wikisource-0.0.1/setup.cfg
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 wikisource-0.0.1/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikisource-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 wikisource-0.0.1/tests/test_chapter.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 wikisource-0.0.1/tests/test_collection.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 wikisource-0.0.1/tests/test_wikisource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikisource-0.0.1/wikisource/__init__.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 wikisource-0.0.1/wikisource/chapter.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 wikisource-0.0.1/wikisource/collection.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wikisource-0.0.1/wikisource/paragraph.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 wikisource-0.0.1/wikisource/source.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 wikisource-0.0.1/wikisource/webpage.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 wikisource-0.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 wikisource-0.0.1/LICENSE
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wikisource-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wikisource-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 wikisource-0.0.2/README.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wikisource-0.0.2/setup.cfg
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 wikisource-0.0.2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikisource-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 wikisource-0.0.2/tests/test_chapter.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 wikisource-0.0.2/tests/test_collection.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 wikisource-0.0.2/tests/test_wikisource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikisource-0.0.2/wikisource/__init__.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 wikisource-0.0.2/wikisource/chapter.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 wikisource-0.0.2/wikisource/collection.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wikisource-0.0.2/wikisource/paragraph.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 wikisource-0.0.2/wikisource/source.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 wikisource-0.0.2/wikisource/webpage.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 wikisource-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 wikisource-0.0.2/LICENSE
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 wikisource-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wikisource-0.0.2/PKG-INFO
```

### Comparing `wikisource-0.0.1/README.md` & `wikisource-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# WikiCorpus
+# WikiSource
 
-WikiCorpus is a python package to help search the [Wikisource Books](https://wikisource.org/wiki/Main_Page)
+wikisource is a python package to help search the [Wikisource Books](https://wikisource.org/wiki/Main_Page)
 
 It offers a few classes to help find sentences in a book, or in a book collection. 
 
 For example, to search in a book for a specific string
 
 ```
 from wikisource import WikiSource
```

### Comparing `wikisource-0.0.1/tests/test_chapter.py` & `wikisource-0.0.2/tests/test_chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.1/tests/test_collection.py` & `wikisource-0.0.2/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.1/tests/test_wikisource.py` & `wikisource-0.0.2/tests/test_wikisource.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.1/wikisource/chapter.py` & `wikisource-0.0.2/wikisource/chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.1/wikisource/collection.py` & `wikisource-0.0.2/wikisource/collection.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.1/wikisource/source.py` & `wikisource-0.0.2/wikisource/source.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.1/LICENSE` & `wikisource-0.0.2/LICENSE`

 * *Files identical despite different names*

