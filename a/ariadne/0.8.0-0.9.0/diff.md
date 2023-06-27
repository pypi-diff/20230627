# Comparing `tmp/ariadne-0.8.0.tar.gz` & `tmp/ariadne-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ariadne-0.8.0.tar", last modified: Mon Nov 25 18:22:31 2019, max compression
+gzip compressed data, was "dist/ariadne-0.9.0.tar", last modified: Wed Dec 11 17:31:19 2019, max compression
```

## Comparing `ariadne-0.8.0.tar` & `ariadne-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-11-25 18:22:31.000000 ariadne-0.8.0/
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1512 2018-11-04 15:35:34.000000 ariadne-0.8.0/LICENSE
--rw-r--r--   0 rafalpiton   (501) staff       (20)      126 2019-05-23 14:11:33.000000 ariadne-0.8.0/MANIFEST.in
--rw-r--r--   0 rafalpiton   (501) staff       (20)     6753 2019-11-25 18:22:31.000000 ariadne-0.8.0/PKG-INFO
--rw-r--r--   0 rafalpiton   (501) staff       (20)     4946 2019-11-25 18:20:21.000000 ariadne-0.8.0/README.md
-drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne/
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1846 2019-08-22 13:05:11.000000 ariadne-0.8.0/ariadne/__init__.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)    12237 2019-08-09 16:21:25.000000 ariadne-0.8.0/ariadne/asgi.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1945 2019-06-24 08:50:18.000000 ariadne-0.8.0/ariadne/constants.py
-drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne/contrib/
--rw-r--r--   0 rafalpiton   (501) staff       (20)        0 2019-05-13 15:38:50.000000 ariadne-0.8.0/ariadne/contrib/__init__.py
-drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne/contrib/django/
--rw-r--r--   0 rafalpiton   (501) staff       (20)       65 2019-05-13 15:38:50.000000 ariadne-0.8.0/ariadne/contrib/django/__init__.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)      155 2019-05-13 15:38:50.000000 ariadne-0.8.0/ariadne/contrib/django/apps.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1676 2019-05-13 15:38:50.000000 ariadne-0.8.0/ariadne/contrib/django/scalars.py
-drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne/contrib/django/templates/
-drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne/contrib/django/templates/ariadne/
--rw-r--r--   0 rafalpiton   (501) staff       (20)    19195 2019-05-13 15:38:50.000000 ariadne-0.8.0/ariadne/contrib/django/templates/ariadne/graphql_playground.html
--rw-r--r--   0 rafalpiton   (501) staff       (20)     4403 2019-06-28 16:07:11.000000 ariadne-0.8.0/ariadne/contrib/django/views.py
-drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne/contrib/tracing/
--rw-r--r--   0 rafalpiton   (501) staff       (20)        0 2019-08-09 16:21:25.000000 ariadne-0.8.0/ariadne/contrib/tracing/__init__.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     3447 2019-10-02 08:57:36.000000 ariadne-0.8.0/ariadne/contrib/tracing/apollotracing.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     3587 2019-09-23 16:25:44.000000 ariadne-0.8.0/ariadne/contrib/tracing/opentracing.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)      800 2019-08-09 16:21:25.000000 ariadne-0.8.0/ariadne/contrib/tracing/utils.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1879 2019-06-14 17:33:25.000000 ariadne-0.8.0/ariadne/enums.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)      758 2019-08-12 10:18:03.000000 ariadne-0.8.0/ariadne/exceptions.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1907 2019-11-25 11:38:43.000000 ariadne-0.8.0/ariadne/executable_schema.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1617 2019-10-02 08:57:36.000000 ariadne-0.8.0/ariadne/extensions.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     3495 2019-06-24 08:50:18.000000 ariadne-0.8.0/ariadne/file_uploads.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1456 2019-08-12 15:01:10.000000 ariadne-0.8.0/ariadne/format_error.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)    11090 2019-10-02 08:57:36.000000 ariadne-0.8.0/ariadne/graphql.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     2036 2019-05-07 11:16:47.000000 ariadne-0.8.0/ariadne/interfaces.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)      947 2019-11-22 16:35:14.000000 ariadne-0.8.0/ariadne/load_schema.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)      432 2019-05-13 13:01:30.000000 ariadne-0.8.0/ariadne/logger.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     2653 2019-06-24 08:50:18.000000 ariadne-0.8.0/ariadne/objects.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)        0 2019-05-17 13:23:04.000000 ariadne-0.8.0/ariadne/py.typed
--rw-r--r--   0 rafalpiton   (501) staff       (20)     2182 2019-07-25 11:42:25.000000 ariadne-0.8.0/ariadne/resolvers.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     3049 2019-11-25 11:38:43.000000 ariadne-0.8.0/ariadne/scalars.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)    20974 2019-11-25 11:38:43.000000 ariadne-0.8.0/ariadne/schema_visitor.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1689 2019-05-10 14:32:07.000000 ariadne-0.8.0/ariadne/subscriptions.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1764 2019-10-02 08:57:36.000000 ariadne-0.8.0/ariadne/types.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1372 2019-05-07 11:16:47.000000 ariadne-0.8.0/ariadne/unions.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1391 2019-07-19 15:20:22.000000 ariadne-0.8.0/ariadne/utils.py
--rw-r--r--   0 rafalpiton   (501) staff       (20)     8823 2019-09-13 11:30:54.000000 ariadne-0.8.0/ariadne/wsgi.py
-drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne.egg-info/
--rw-r--r--   0 rafalpiton   (501) staff       (20)     6753 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne.egg-info/PKG-INFO
--rw-r--r--   0 rafalpiton   (501) staff       (20)     1068 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne.egg-info/SOURCES.txt
--rw-r--r--   0 rafalpiton   (501) staff       (20)        1 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne.egg-info/dependency_links.txt
--rw-r--r--   0 rafalpiton   (501) staff       (20)        1 2019-05-23 14:12:40.000000 ariadne-0.8.0/ariadne.egg-info/not-zip-safe
--rw-r--r--   0 rafalpiton   (501) staff       (20)      109 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne.egg-info/requires.txt
--rw-r--r--   0 rafalpiton   (501) staff       (20)        8 2019-11-25 18:22:31.000000 ariadne-0.8.0/ariadne.egg-info/top_level.txt
--rw-r--r--   0 rafalpiton   (501) staff       (20)       38 2019-11-25 18:22:31.000000 ariadne-0.8.0/setup.cfg
--rwxr-xr-x   0 rafalpiton   (501) staff       (20)     1301 2019-11-25 18:03:21.000000 ariadne-0.8.0/setup.py
+drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-12-11 17:31:19.000000 ariadne-0.9.0/
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1512 2018-11-04 15:35:34.000000 ariadne-0.9.0/LICENSE
+-rw-r--r--   0 rafalpiton   (501) staff       (20)      126 2019-05-23 14:11:33.000000 ariadne-0.9.0/MANIFEST.in
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     6753 2019-12-11 17:31:19.000000 ariadne-0.9.0/PKG-INFO
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     4946 2019-11-25 18:20:21.000000 ariadne-0.9.0/README.md
+drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-12-11 17:31:19.000000 ariadne-0.9.0/ariadne/
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1846 2019-08-22 13:05:11.000000 ariadne-0.9.0/ariadne/__init__.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)    12237 2019-08-09 16:21:25.000000 ariadne-0.9.0/ariadne/asgi.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1945 2019-06-24 08:50:18.000000 ariadne-0.9.0/ariadne/constants.py
+drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-12-11 17:31:19.000000 ariadne-0.9.0/ariadne/contrib/
+-rw-r--r--   0 rafalpiton   (501) staff       (20)        0 2019-05-13 15:38:50.000000 ariadne-0.9.0/ariadne/contrib/__init__.py
+drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-12-11 17:31:19.000000 ariadne-0.9.0/ariadne/contrib/django/
+-rw-r--r--   0 rafalpiton   (501) staff       (20)       65 2019-05-13 15:38:50.000000 ariadne-0.9.0/ariadne/contrib/django/__init__.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)      155 2019-05-13 15:38:50.000000 ariadne-0.9.0/ariadne/contrib/django/apps.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1676 2019-05-13 15:38:50.000000 ariadne-0.9.0/ariadne/contrib/django/scalars.py
+drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-12-11 17:31:19.000000 ariadne-0.9.0/ariadne/contrib/django/templates/
+drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-12-11 17:31:19.000000 ariadne-0.9.0/ariadne/contrib/django/templates/ariadne/
+-rw-r--r--   0 rafalpiton   (501) staff       (20)    19195 2019-05-13 15:38:50.000000 ariadne-0.9.0/ariadne/contrib/django/templates/ariadne/graphql_playground.html
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     4403 2019-06-28 16:07:11.000000 ariadne-0.9.0/ariadne/contrib/django/views.py
+drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-12-11 17:31:19.000000 ariadne-0.9.0/ariadne/contrib/tracing/
+-rw-r--r--   0 rafalpiton   (501) staff       (20)        0 2019-08-09 16:21:25.000000 ariadne-0.9.0/ariadne/contrib/tracing/__init__.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     3447 2019-10-02 08:57:36.000000 ariadne-0.9.0/ariadne/contrib/tracing/apollotracing.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     3587 2019-09-23 16:25:44.000000 ariadne-0.9.0/ariadne/contrib/tracing/opentracing.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)      800 2019-08-09 16:21:25.000000 ariadne-0.9.0/ariadne/contrib/tracing/utils.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1879 2019-06-14 17:33:25.000000 ariadne-0.9.0/ariadne/enums.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)      758 2019-08-12 10:18:03.000000 ariadne-0.9.0/ariadne/exceptions.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1907 2019-11-25 11:38:43.000000 ariadne-0.9.0/ariadne/executable_schema.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1617 2019-10-02 08:57:36.000000 ariadne-0.9.0/ariadne/extensions.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     3495 2019-06-24 08:50:18.000000 ariadne-0.9.0/ariadne/file_uploads.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1456 2019-08-12 15:01:10.000000 ariadne-0.9.0/ariadne/format_error.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)    11090 2019-10-02 08:57:36.000000 ariadne-0.9.0/ariadne/graphql.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     2036 2019-05-07 11:16:47.000000 ariadne-0.9.0/ariadne/interfaces.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)      947 2019-11-22 16:35:14.000000 ariadne-0.9.0/ariadne/load_schema.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)      432 2019-05-13 13:01:30.000000 ariadne-0.9.0/ariadne/logger.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     2653 2019-06-24 08:50:18.000000 ariadne-0.9.0/ariadne/objects.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)        0 2019-05-17 13:23:04.000000 ariadne-0.9.0/ariadne/py.typed
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     2182 2019-07-25 11:42:25.000000 ariadne-0.9.0/ariadne/resolvers.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     3049 2019-11-25 11:38:43.000000 ariadne-0.9.0/ariadne/scalars.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)    20974 2019-11-25 11:38:43.000000 ariadne-0.9.0/ariadne/schema_visitor.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1689 2019-05-10 14:32:07.000000 ariadne-0.9.0/ariadne/subscriptions.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1764 2019-10-02 08:57:36.000000 ariadne-0.9.0/ariadne/types.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1372 2019-05-07 11:16:47.000000 ariadne-0.9.0/ariadne/unions.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1391 2019-07-19 15:20:22.000000 ariadne-0.9.0/ariadne/utils.py
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     8823 2019-09-13 11:30:54.000000 ariadne-0.9.0/ariadne/wsgi.py
+drwxr-xr-x   0 rafalpiton   (501) staff       (20)        0 2019-12-11 17:31:19.000000 ariadne-0.9.0/ariadne.egg-info/
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     6753 2019-12-11 17:31:18.000000 ariadne-0.9.0/ariadne.egg-info/PKG-INFO
+-rw-r--r--   0 rafalpiton   (501) staff       (20)     1068 2019-12-11 17:31:18.000000 ariadne-0.9.0/ariadne.egg-info/SOURCES.txt
+-rw-r--r--   0 rafalpiton   (501) staff       (20)        1 2019-12-11 17:31:18.000000 ariadne-0.9.0/ariadne.egg-info/dependency_links.txt
+-rw-r--r--   0 rafalpiton   (501) staff       (20)        1 2019-05-23 14:12:40.000000 ariadne-0.9.0/ariadne.egg-info/not-zip-safe
+-rw-r--r--   0 rafalpiton   (501) staff       (20)      105 2019-12-11 17:31:18.000000 ariadne-0.9.0/ariadne.egg-info/requires.txt
+-rw-r--r--   0 rafalpiton   (501) staff       (20)        8 2019-12-11 17:31:18.000000 ariadne-0.9.0/ariadne.egg-info/top_level.txt
+-rw-r--r--   0 rafalpiton   (501) staff       (20)       38 2019-12-11 17:31:19.000000 ariadne-0.9.0/setup.cfg
+-rwxr-xr-x   0 rafalpiton   (501) staff       (20)     1297 2019-12-11 17:22:24.000000 ariadne-0.9.0/setup.py
```

### Comparing `ariadne-0.8.0/LICENSE` & `ariadne-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/PKG-INFO` & `ariadne-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariadne
-Version: 0.8.0
+Version: 0.9.0
 Summary: Ariadne is a Python library for implementing GraphQL servers.
 Home-page: https://github.com/mirumee/ariadne
 Author: Mirumee Software
 Author-email: hello@mirumee.com
 License: BSD
 Description: [![Ariadne](https://ariadnegraphql.org/img/logo-horizontal-sm.png)](https://ariadnegraphql.org)
```

### Comparing `ariadne-0.8.0/README.md` & `ariadne-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/__init__.py` & `ariadne-0.9.0/ariadne/__init__.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/asgi.py` & `ariadne-0.9.0/ariadne/asgi.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/constants.py` & `ariadne-0.9.0/ariadne/constants.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/contrib/django/scalars.py` & `ariadne-0.9.0/ariadne/contrib/django/scalars.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/contrib/django/templates/ariadne/graphql_playground.html` & `ariadne-0.9.0/ariadne/contrib/django/templates/ariadne/graphql_playground.html`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/contrib/django/views.py` & `ariadne-0.9.0/ariadne/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/contrib/tracing/apollotracing.py` & `ariadne-0.9.0/ariadne/contrib/tracing/apollotracing.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/contrib/tracing/opentracing.py` & `ariadne-0.9.0/ariadne/contrib/tracing/opentracing.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/contrib/tracing/utils.py` & `ariadne-0.9.0/ariadne/contrib/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/enums.py` & `ariadne-0.9.0/ariadne/enums.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/exceptions.py` & `ariadne-0.9.0/ariadne/exceptions.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/executable_schema.py` & `ariadne-0.9.0/ariadne/executable_schema.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/extensions.py` & `ariadne-0.9.0/ariadne/extensions.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/file_uploads.py` & `ariadne-0.9.0/ariadne/file_uploads.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/format_error.py` & `ariadne-0.9.0/ariadne/format_error.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/graphql.py` & `ariadne-0.9.0/ariadne/graphql.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/interfaces.py` & `ariadne-0.9.0/ariadne/interfaces.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/load_schema.py` & `ariadne-0.9.0/ariadne/load_schema.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/objects.py` & `ariadne-0.9.0/ariadne/objects.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/resolvers.py` & `ariadne-0.9.0/ariadne/resolvers.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/scalars.py` & `ariadne-0.9.0/ariadne/scalars.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/schema_visitor.py` & `ariadne-0.9.0/ariadne/schema_visitor.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/subscriptions.py` & `ariadne-0.9.0/ariadne/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/types.py` & `ariadne-0.9.0/ariadne/types.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/unions.py` & `ariadne-0.9.0/ariadne/unions.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/utils.py` & `ariadne-0.9.0/ariadne/utils.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne/wsgi.py` & `ariadne-0.9.0/ariadne/wsgi.py`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/ariadne.egg-info/PKG-INFO` & `ariadne-0.9.0/ariadne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariadne
-Version: 0.8.0
+Version: 0.9.0
 Summary: Ariadne is a Python library for implementing GraphQL servers.
 Home-page: https://github.com/mirumee/ariadne
 Author: Mirumee Software
 Author-email: hello@mirumee.com
 License: BSD
 Description: [![Ariadne](https://ariadnegraphql.org/img/logo-horizontal-sm.png)](https://ariadnegraphql.org)
```

### Comparing `ariadne-0.8.0/ariadne.egg-info/SOURCES.txt` & `ariadne-0.9.0/ariadne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ariadne-0.8.0/setup.py` & `ariadne-0.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,20 +22,20 @@
     name="ariadne",
     author="Mirumee Software",
     author_email="hello@mirumee.com",
     description="Ariadne is a Python library for implementing GraphQL servers.",
     long_description=README,
     long_description_content_type="text/markdown",
     license="BSD",
-    version="0.8.0",
+    version="0.9.0",
     url="https://github.com/mirumee/ariadne",
     packages=["ariadne"],
     include_package_data=True,
     install_requires=[
-        "graphql-core-next<3.0.0",
+        "graphql-core>=3.0.0",
         "starlette<0.14",
         "typing_extensions>=3.6.0",
     ],
     extras_require={"asgi-file-uploads": ["python-multipart>=0.0.5"]},
     classifiers=CLASSIFIERS,
     platforms=["any"],
     zip_safe=False,
```

