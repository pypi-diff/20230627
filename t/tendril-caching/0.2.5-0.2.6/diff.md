# Comparing `tmp/tendril-caching-0.2.5.tar.gz` & `tmp/tendril-caching-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-caching-0.2.5.tar", last modified: Mon Jun 26 13:25:03 2023, max compression
+gzip compressed data, was "tendril-caching-0.2.6.tar", last modified: Tue Jun 27 11:09:47 2023, max compression
```

## Comparing `tendril-caching-0.2.5.tar` & `tendril-caching-0.2.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.744602 tendril-caching-0.2.5/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.744602 tendril-caching-0.2.5/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-caching-0.2.5/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      903 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-06-26 13:25:03.752602 tendril-caching-0.2.5/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3133 2022-11-29 09:11:32.000000 tendril-caching-0.2.5/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.744602 tendril-caching-0.2.5/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:20.000000 tendril-caching-0.2.5/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-caching-0.2.5/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      863 2023-06-26 13:20:44.000000 tendril-caching-0.2.5/src/tendril/apiserver/routers/tokens.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/src/tendril/caching/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      449 2022-11-29 14:28:12.000000 tendril-caching-0.2.5/src/tendril/caching/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/src/tendril/caching/providers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:53:59.000000 tendril-caching-0.2.5/src/tendril/caching/providers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      272 2022-11-29 13:57:11.000000 tendril-caching-0.2.5/src/tendril/caching/providers/dummy.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1910 2022-11-29 14:11:44.000000 tendril-caching-0.2.5/src/tendril/caching/providers/redis.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4512 2023-06-26 13:24:26.000000 tendril-caching-0.2.5/src/tendril/caching/tokens.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2349 2023-06-25 19:47:22.000000 tendril-caching-0.2.5/src/tendril/caching/transit.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-caching-0.2.5/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1689 2023-06-26 10:43:35.000000 tendril-caching-0.2.5/src/tendril/config/caching.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/src/tendril_caching.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-06-26 13:25:03.000000 tendril-caching-0.2.5/src/tendril_caching.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1035 2023-06-26 13:25:03.000000 tendril-caching-0.2.5/src/tendril_caching.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-06-26 13:25:03.000000 tendril-caching-0.2.5/src/tendril_caching.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      503 2023-06-26 13:25:03.000000 tendril-caching-0.2.5/src/tendril_caching.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-06-26 13:25:03.000000 tendril-caching-0.2.5/src/tendril_caching.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:25:03.748602 tendril-caching-0.2.5/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-11-29 08:29:31.000000 tendril-caching-0.2.5/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-caching-0.2.6/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      903 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3133 2022-11-29 09:11:32.000000 tendril-caching-0.2.6/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.340193 tendril-caching-0.2.6/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:20.000000 tendril-caching-0.2.6/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-caching-0.2.6/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      863 2023-06-26 13:20:44.000000 tendril-caching-0.2.6/src/tendril/apiserver/routers/tokens.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/src/tendril/caching/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      449 2022-11-29 14:28:12.000000 tendril-caching-0.2.6/src/tendril/caching/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/src/tendril/caching/providers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:53:59.000000 tendril-caching-0.2.6/src/tendril/caching/providers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      272 2022-11-29 13:57:11.000000 tendril-caching-0.2.6/src/tendril/caching/providers/dummy.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1910 2022-11-29 14:11:44.000000 tendril-caching-0.2.6/src/tendril/caching/providers/redis.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4450 2023-06-27 11:00:52.000000 tendril-caching-0.2.6/src/tendril/caching/tokens.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2349 2023-06-25 19:47:22.000000 tendril-caching-0.2.6/src/tendril/caching/transit.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-caching-0.2.6/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1689 2023-06-26 10:43:35.000000 tendril-caching-0.2.6/src/tendril/config/caching.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/src/tendril_caching.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-06-27 11:09:47.000000 tendril-caching-0.2.6/src/tendril_caching.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1035 2023-06-27 11:09:47.000000 tendril-caching-0.2.6/src/tendril_caching.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-06-27 11:09:47.000000 tendril-caching-0.2.6/src/tendril_caching.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      503 2023-06-27 11:09:47.000000 tendril-caching-0.2.6/src/tendril_caching.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-06-27 11:09:47.000000 tendril-caching-0.2.6/src/tendril_caching.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-27 11:09:47.344193 tendril-caching-0.2.6/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-11-29 08:29:31.000000 tendril-caching-0.2.6/tox.ini
```

### Comparing `tendril-caching-0.2.5/.gitignore` & `tendril-caching-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/.readthedocs.yml` & `tendril-caching-0.2.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/.travis.yml` & `tendril-caching-0.2.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/LICENSE` & `tendril-caching-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/PKG-INFO` & `tendril-caching-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-caching
-Version: 0.2.5
+Version: 0.2.6
 Summary: Caching Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-caching
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-caching.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-caching/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-caching
```

### Comparing `tendril-caching-0.2.5/README.rst` & `tendril-caching-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/Makefile` & `tendril-caching-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/_static/custom.css` & `tendril-caching-0.2.6/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/_static/favicon.ico` & `tendril-caching-0.2.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/_static/logo.png` & `tendril-caching-0.2.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/_static/logo_packed.png` & `tendril-caching-0.2.6/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/_templates/about.html` & `tendril-caching-0.2.6/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/conf.py` & `tendril-caching-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/index.rst` & `tendril-caching-0.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/docs/installation.rst` & `tendril-caching-0.2.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/setup.py` & `tendril-caching-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/src/tendril/apiserver/routers/tokens.py` & `tendril-caching-0.2.6/src/tendril/apiserver/routers/tokens.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/src/tendril/caching/providers/redis.py` & `tendril-caching-0.2.6/src/tendril/caching/providers/redis.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/src/tendril/caching/tokens.py` & `tendril-caching-0.2.6/src/tendril/caching/tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,16 +102,14 @@
     cache_key = _cache_key(namespace=namespace, key=key)
     logger.info(f"Creating token {cache_key}")
     params = {
         'metadata': metadata,
         'id': key
     }
     if user:
-        if not isinstance(user, int):
-            raise TypeError("Expecting an integer user reference")
         params['user'] = user
     if current:
         params['current'] = current
     if progress_max:
         progress = TokenProgressTModel(
             max=progress_max, done=0
         )
@@ -123,27 +121,30 @@
 
 def read(namespace, key, tmodel=GenericTokenTModel):
     return _read(_cache_key(namespace=namespace, key=key),
                  tmodel=tmodel)
 
 
 def update(namespace, key,
-           state: TokenStatus=None, current: str=None, done: int=None, max: int=None,
-           metadata=None, metadata_strategy='update', ttl=None, tmodel=GenericTokenTModel):
+           state: TokenStatus = None,
+           current: str = None,
+           done: int = None, max: int = None,
+           metadata=None, metadata_strategy='update',
+           ttl=None, tmodel=GenericTokenTModel):
     cache_key = _cache_key(namespace, key)
     data: GenericTokenTModel = _read(cache_key, tmodel=tmodel)
     if state:
         data.state = state
     if current:
         data.current = current
     if done:
         data.progress.done = done
     if max:
         data.progress.max = max
-    if metadata and metadata_strategy=='update':
+    if metadata and metadata_strategy == 'update':
         data.metadata = data.metadata.update(metadata)
     return _write(cache_key, data, ex=ttl)
 
 
 def close(namespace, key, failed=False, ttl=300,
           tmodel=GenericTokenTModel):
     if failed:
```

### Comparing `tendril-caching-0.2.5/src/tendril/caching/transit.py` & `tendril-caching-0.2.6/src/tendril/caching/transit.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/src/tendril/config/__init__.py` & `tendril-caching-0.2.6/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/src/tendril/config/caching.py` & `tendril-caching-0.2.6/src/tendril/config/caching.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/src/tendril_caching.egg-info/PKG-INFO` & `tendril-caching-0.2.6/src/tendril_caching.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-caching
-Version: 0.2.5
+Version: 0.2.6
 Summary: Caching Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-caching
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-caching.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-caching/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-caching
```

### Comparing `tendril-caching-0.2.5/src/tendril_caching.egg-info/SOURCES.txt` & `tendril-caching-0.2.6/src/tendril_caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/tests/coveralls.py` & `tendril-caching-0.2.6/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.5/tox.ini` & `tendril-caching-0.2.6/tox.ini`

 * *Files identical despite different names*

