# Comparing `tmp/djangorestsearch-0.8.9.tar.gz` & `tmp/djangorestsearch-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangorestsearch-0.8.9.tar", last modified: Tue Aug 25 11:44:21 2020, max compression
+gzip compressed data, was "djangorestsearch-0.9.0.tar", last modified: Wed Sep  1 15:33:17 2021, max compression
```

## Comparing `djangorestsearch-0.8.9.tar` & `djangorestsearch-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 sharky    (1000) sharky    (1000)        0 2020-08-25 11:44:21.233814 djangorestsearch-0.8.9/
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1297 2019-07-25 22:56:46.000000 djangorestsearch-0.8.9/LICENSE
--rw-r--r--   0 sharky    (1000) sharky    (1000)       96 2019-07-25 22:56:46.000000 djangorestsearch-0.8.9/MANIFEST.in
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1828 2020-08-25 11:44:21.233814 djangorestsearch-0.8.9/PKG-INFO
--rw-r--r--   0 sharky    (1000) sharky    (1000)      900 2020-04-14 12:11:48.000000 djangorestsearch-0.8.9/README.rst
-drwxr-xr-x   0 sharky    (1000) sharky    (1000)        0 2020-08-25 11:44:21.233814 djangorestsearch-0.8.9/djangorestsearch.egg-info/
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1828 2020-08-25 11:44:21.000000 djangorestsearch-0.8.9/djangorestsearch.egg-info/PKG-INFO
--rw-r--r--   0 sharky    (1000) sharky    (1000)      434 2020-08-25 11:44:21.000000 djangorestsearch-0.8.9/djangorestsearch.egg-info/SOURCES.txt
--rw-r--r--   0 sharky    (1000) sharky    (1000)        1 2020-08-25 11:44:21.000000 djangorestsearch-0.8.9/djangorestsearch.egg-info/dependency_links.txt
--rw-r--r--   0 sharky    (1000) sharky    (1000)       53 2020-08-25 11:44:21.000000 djangorestsearch-0.8.9/djangorestsearch.egg-info/requires.txt
--rw-r--r--   0 sharky    (1000) sharky    (1000)       12 2020-08-25 11:44:21.000000 djangorestsearch-0.8.9/djangorestsearch.egg-info/top_level.txt
-drwxr-xr-x   0 sharky    (1000) sharky    (1000)        0 2020-08-25 11:44:21.233814 djangorestsearch-0.8.9/rest_search/
--rw-r--r--   0 sharky    (1000) sharky    (1000)     2573 2020-04-13 08:31:51.000000 djangorestsearch-0.8.9/rest_search/__init__.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)      357 2020-04-13 08:31:51.000000 djangorestsearch-0.8.9/rest_search/decorators.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1163 2020-04-13 08:31:51.000000 djangorestsearch-0.8.9/rest_search/forms.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1865 2020-04-13 08:31:51.000000 djangorestsearch-0.8.9/rest_search/indexers.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)      329 2020-04-13 08:31:51.000000 djangorestsearch-0.8.9/rest_search/middleware.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)     2482 2020-08-25 11:31:00.000000 djangorestsearch-0.8.9/rest_search/schemas.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)     3486 2020-04-13 08:31:51.000000 djangorestsearch-0.8.9/rest_search/tasks.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)     2108 2020-04-13 14:15:39.000000 djangorestsearch-0.8.9/rest_search/views.py
--rw-r--r--   0 sharky    (1000) sharky    (1000)      225 2020-08-25 11:44:21.233814 djangorestsearch-0.8.9/setup.cfg
--rw-r--r--   0 sharky    (1000) sharky    (1000)     1005 2020-08-25 11:39:37.000000 djangorestsearch-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 15:33:17.015626 djangorestsearch-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-09-01 15:33:17.015626 djangorestsearch-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-09-01 15:33:17.015626 djangorestsearch-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1542 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 15:33:17.015626 djangorestsearch-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 15:33:17.015626 djangorestsearch-0.9.0/src/djangorestsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-09-01 15:33:16.000000 djangorestsearch-0.9.0/src/djangorestsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2021-09-01 15:33:16.000000 djangorestsearch-0.9.0/src/djangorestsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-01 15:33:16.000000 djangorestsearch-0.9.0/src/djangorestsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-09-01 15:33:16.000000 djangorestsearch-0.9.0/src/djangorestsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-01 15:33:16.000000 djangorestsearch-0.9.0/src/djangorestsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 15:33:17.015626 djangorestsearch-0.9.0/src/rest_search/
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/about.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1163 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1865 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/indexers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3486 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2469 2021-09-01 15:33:14.000000 djangorestsearch-0.9.0/src/rest_search/views.py
```

### Comparing `djangorestsearch-0.8.9/LICENSE` & `djangorestsearch-0.9.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # License
 
-Copyright (c) 2016-2017, Wemap SAS
+Copyright (c) 2016-2021, Wemap SAS
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer.
```

### Comparing `djangorestsearch-0.8.9/PKG-INFO` & `djangorestsearch-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangorestsearch
-Version: 0.8.9
+Version: 0.9.0
 Summary: ElasticSearch integration for Django.
 Home-page: https://github.com/wemap/django-rest-search
 Author: Jeremy Lainé
 Author-email: jeremy@getwemap.com
 License: BSD
 Description: Django REST Search
         ==================
@@ -32,11 +32,12 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: dev
```

### Comparing `djangorestsearch-0.8.9/README.rst` & `djangorestsearch-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `djangorestsearch-0.8.9/djangorestsearch.egg-info/PKG-INFO` & `djangorestsearch-0.9.0/src/djangorestsearch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangorestsearch
-Version: 0.8.9
+Version: 0.9.0
 Summary: ElasticSearch integration for Django.
 Home-page: https://github.com/wemap/django-rest-search
 Author: Jeremy Lainé
 Author-email: jeremy@getwemap.com
 License: BSD
 Description: Django REST Search
         ==================
@@ -32,11 +32,12 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: dev
```

### Comparing `djangorestsearch-0.8.9/rest_search/__init__.py` & `djangorestsearch-0.9.0/src/rest_search/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from threading import local
 
 from aws_requests_auth.aws_auth import AWSRequestsAuth
 from django.conf import settings
 from elasticsearch import Elasticsearch, RequestsHttpConnection
 
+from .about import __version__  # noqa
+
 DEFAULT_INDEX_SETTINGS = {
     "analysis": {
         "analyzer": {
             "default": {
                 "tokenizer": "standard",
                 "filter": ["standard", "lowercase", "asciifolding"],
             }
```

### Comparing `djangorestsearch-0.8.9/rest_search/forms.py` & `djangorestsearch-0.9.0/src/rest_search/forms.py`

 * *Files identical despite different names*

### Comparing `djangorestsearch-0.8.9/rest_search/indexers.py` & `djangorestsearch-0.9.0/src/rest_search/indexers.py`

 * *Files identical despite different names*

### Comparing `djangorestsearch-0.8.9/rest_search/schemas.py` & `djangorestsearch-0.9.0/src/rest_search/schemas.py`

 * *Files identical despite different names*

### Comparing `djangorestsearch-0.8.9/rest_search/tasks.py` & `djangorestsearch-0.9.0/src/rest_search/tasks.py`

 * *Files identical despite different names*

### Comparing `djangorestsearch-0.8.9/rest_search/views.py` & `djangorestsearch-0.9.0/src/rest_search/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,35 +19,49 @@
     def get_schema_operation_parameters(self, view):
         return get_form_schema_operation_parameters(view.form_class)
 
 
 class SearchAPIView(APIView):
     filter_backends = (SearchFilterBackend,)
 
+    def _get_total(self, total):
+        if isinstance(total, dict):
+            # for ES >= 7
+            # hits.total is now an object in the search response
+            return total["value"]
+        else:
+            # for ES < 7
+            return total
+
     def get(self, request, *args, **kwargs):
         query = self.get_query()
         sort = self.get_sort()
 
         pagination = LimitOffsetPagination()
         pagination.default_limit = 20
         pagination.limit = pagination.get_limit(request)
         pagination.offset = pagination.get_offset(request)
         pagination.request = request
 
-        body = {"query": query, "size": pagination.limit, "from": pagination.offset}
+        body = {
+            "track_total_hits": True,
+            "query": query,
+            "size": pagination.limit,
+            "from": pagination.offset,
+        }
         if sort:
             body["sort"] = sort
 
         # execute elasticsearch query
         indexer = self.get_indexer()
         res = indexer.search(body=body)
 
         # map back to expected format
         items = list(indexer.map_results(res["hits"]["hits"]))
-        pagination.count = res["hits"]["total"]
+        pagination.count = self._get_total(res["hits"]["total"])
         return pagination.get_paginated_response(items)
 
     def get_indexer(self):
         return self.indexer_class()
 
     def get_query(self):
         """
```

