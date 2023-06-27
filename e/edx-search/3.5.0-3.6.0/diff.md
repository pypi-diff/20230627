# Comparing `tmp/edx-search-3.5.0.tar.gz` & `tmp/edx-search-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-search-3.5.0.tar", last modified: Mon Apr 10 15:16:14 2023, max compression
+gzip compressed data, was "edx-search-3.6.0.tar", last modified: Tue Jun 27 12:01:56 2023, max compression
```

## Comparing `edx-search-3.5.0.tar` & `edx-search-3.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 15:16:05.000000 edx-search-3.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-04-10 15:16:05.000000 edx-search-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-10 15:16:05.000000 edx-search-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-10 15:16:14.820492 edx-search-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12575 2023-04-10 15:16:05.000000 edx-search-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.816492 edx-search-3.5.0/edx_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-10 15:16:14.000000 edx-search-3.5.0/edx_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/edxsearch/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-04-10 15:16:05.000000 edx-search-3.5.0/edxsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-04-10 15:16:05.000000 edx-search-3.5.0/edxsearch/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-04-10 15:16:05.000000 edx-search-3.5.0/edxsearch/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-04-10 15:16:05.000000 edx-search-3.5.0/edxsearch/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-04-10 15:16:05.000000 edx-search-3.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-10 15:16:05.000000 edx-search-3.5.0/requirements/testing.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/search/
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    22812 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/elastic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/filter_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)      877 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/initializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6055 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/result_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/search_engine_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:14.820492 edx-search-3.5.0/search/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14988 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/mock_search_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)    15779 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_course_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_course_discovery_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    10533 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_engines.py
--rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_mock_search_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)    14297 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_search_result_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)    20485 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7137 2023-04-10 15:16:05.000000 edx-search-3.5.0/search/views.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 15:16:14.824492 edx-search-3.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2470 2023-04-10 15:16:05.000000 edx-search-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:01:56.637252 edx-search-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-27 12:01:50.000000 edx-search-3.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-06-27 12:01:50.000000 edx-search-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-27 12:01:50.000000 edx-search-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-27 12:01:56.637252 edx-search-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12575 2023-06-27 12:01:50.000000 edx-search-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:01:56.633252 edx-search-3.6.0/edx_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-27 12:01:56.000000 edx-search-3.6.0/edx_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-06-27 12:01:56.000000 edx-search-3.6.0/edx_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 12:01:56.000000 edx-search-3.6.0/edx_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-27 12:01:56.000000 edx-search-3.6.0/edx_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-27 12:01:56.000000 edx-search-3.6.0/edx_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:01:56.637252 edx-search-3.6.0/edxsearch/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-27 12:01:50.000000 edx-search-3.6.0/edxsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-06-27 12:01:50.000000 edx-search-3.6.0/edxsearch/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-06-27 12:01:50.000000 edx-search-3.6.0/edxsearch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-27 12:01:50.000000 edx-search-3.6.0/edxsearch/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:01:56.637252 edx-search-3.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-06-27 12:01:50.000000 edx-search-3.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-27 12:01:50.000000 edx-search-3.6.0/requirements/testing.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:01:56.637252 edx-search-3.6.0/search/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22812 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/filter_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6055 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/result_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/search_engine_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:01:56.637252 edx-search-3.6.0/search/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14988 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/mock_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15779 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/test_course_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/test_course_discovery_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10533 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/test_engines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/test_mock_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14297 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/test_search_result_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20485 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-06-27 12:01:50.000000 edx-search-3.6.0/search/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 12:01:56.637252 edx-search-3.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2546 2023-06-27 12:01:50.000000 edx-search-3.6.0/setup.py
```

### Comparing `edx-search-3.5.0/LICENSE` & `edx-search-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/PKG-INFO` & `edx-search-3.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-search
-Version: 3.5.0
+Version: 3.6.0
 Summary: Search and index routines for index access
 Home-page: https://github.com/openedx/edx-search
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,12 +16,14 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 License-File: AUTHORS
 
 UNKNOWN
```

### Comparing `edx-search-3.5.0/README.md` & `edx-search-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/edx_search.egg-info/PKG-INFO` & `edx-search-3.6.0/edx_search.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-search
-Version: 3.5.0
+Version: 3.6.0
 Summary: Search and index routines for index access
 Home-page: https://github.com/openedx/edx-search
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,12 +16,14 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 License-File: AUTHORS
 
 UNKNOWN
```

### Comparing `edx-search-3.5.0/edx_search.egg-info/SOURCES.txt` & `edx-search-3.6.0/edx_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/edxsearch/settings.py` & `edx-search-3.6.0/edxsearch/settings.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/requirements/base.in` & `edx-search-3.6.0/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/api.py` & `edx-search-3.6.0/search/api.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/elastic.py` & `edx-search-3.6.0/search/elastic.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/filter_generator.py` & `edx-search-3.6.0/search/filter_generator.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/initializer.py` & `edx-search-3.6.0/search/initializer.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/result_processor.py` & `edx-search-3.6.0/search/result_processor.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/search_engine_base.py` & `edx-search-3.6.0/search/search_engine_base.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/mock_search_engine.py` & `edx-search-3.6.0/search/tests/mock_search_engine.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/test_course_discovery.py` & `edx-search-3.6.0/search/tests/test_course_discovery.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/test_course_discovery_views.py` & `edx-search-3.6.0/search/tests/test_course_discovery_views.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/test_engines.py` & `edx-search-3.6.0/search/tests/test_engines.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/test_mock_search_engine.py` & `edx-search-3.6.0/search/tests/test_mock_search_engine.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/test_search_result_processor.py` & `edx-search-3.6.0/search/tests/test_search_result_processor.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/test_views.py` & `edx-search-3.6.0/search/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/tests.py` & `edx-search-3.6.0/search/tests/tests.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/tests/utils.py` & `edx-search-3.6.0/search/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/utils.py` & `edx-search-3.6.0/search/utils.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.5.0/search/views.py` & `edx-search-3.6.0/search/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This contains just the url entry points to use if desired, which currently has only one
 # pylint: disable=too-few-public-methods
 
 import logging
 
 from django.conf import settings
 from django.http import JsonResponse
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.views.decorators.http import require_POST
 
 from eventtracking import tracker as track
 from .api import perform_search, course_discovery_search, course_discovery_filter_fields
 from .initializer import SearchInitializer
 
 # log appears to be standard name used for logger
```

### Comparing `edx-search-3.5.0/setup.py` & `edx-search-3.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,11 +66,13 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.8',
         'Framework :: Django',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
     ],
     packages=['search', 'search.tests', 'edxsearch'],
     install_requires=load_requirements('requirements/base.in')
 )
```

