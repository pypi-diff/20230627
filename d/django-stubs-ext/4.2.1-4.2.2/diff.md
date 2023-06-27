# Comparing `tmp/django-stubs-ext-4.2.1.tar.gz` & `tmp/django-stubs-ext-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stubs-ext-4.2.1.tar", last modified: Fri Jun  2 14:11:07 2023, max compression
+gzip compressed data, was "django-stubs-ext-4.2.2.tar", last modified: Tue Jun 27 17:50:47 2023, max compression
```

## Comparing `django-stubs-ext-4.2.1.tar` & `django-stubs-ext-4.2.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/LICENSE.md
--rw-r--r--   0 marti     (1000) marti      (121)     3565 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     2496 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.161298 django-stubs-ext-4.2.1/django_stubs_ext/
--rw-r--r--   0 marti     (1000) marti      (121)      535 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)      620 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/aliases.py
--rw-r--r--   0 marti     (1000) marti      (121)      693 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/annotations.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/django_stubs_ext/db/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/django_stubs_ext/db/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     1886 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/django_stubs_ext/db/models.py
--rw-r--r--   0 marti     (1000) marti      (121)     3660 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/patch.py
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/py.typed
--rw-r--r--   0 marti     (1000) marti      (121)      236 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/django_stubs_ext/types.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)     3565 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)      508 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)       25 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       17 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/top_level.txt
--rw-r--r--   0 marti     (1000) marti      (121)       38 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/setup.cfg
--rwxr-xr-x   0 marti     (1000) marti      (121)     1777 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/setup.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/tests/
--rw-r--r--   0 marti     (1000) marti      (121)      169 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/tests/test_aliases.py
--rw-r--r--   0 marti     (1000) marti      (121)     3928 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/tests/test_monkeypatching.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:50:47.533976 django-stubs-ext-4.2.2/
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.2/LICENSE.md
+-rw-r--r--   0 marti     (1000) marti      (121)     3448 2023-06-27 17:50:47.533976 django-stubs-ext-4.2.2/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     2496 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.2/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:50:47.530643 django-stubs-ext-4.2.2/django_stubs_ext/
+-rw-r--r--   0 marti     (1000) marti      (121)      535 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.2/django_stubs_ext/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)      620 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.2/django_stubs_ext/aliases.py
+-rw-r--r--   0 marti     (1000) marti      (121)      693 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.2/django_stubs_ext/annotations.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:50:47.533976 django-stubs-ext-4.2.2/django_stubs_ext/db/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.2/django_stubs_ext/db/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1886 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.2/django_stubs_ext/db/models.py
+-rw-r--r--   0 marti     (1000) marti      (121)      978 2023-06-27 17:49:10.000000 django-stubs-ext-4.2.2/django_stubs_ext/db/router.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3753 2023-06-27 17:49:10.000000 django-stubs-ext-4.2.2/django_stubs_ext/patch.py
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.2/django_stubs_ext/py.typed
+-rw-r--r--   0 marti     (1000) marti      (121)      236 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.2/django_stubs_ext/types.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:50:47.533976 django-stubs-ext-4.2.2/django_stubs_ext.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)     3448 2023-06-27 17:50:47.000000 django-stubs-ext-4.2.2/django_stubs_ext.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)      538 2023-06-27 17:50:47.000000 django-stubs-ext-4.2.2/django_stubs_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-27 17:50:47.000000 django-stubs-ext-4.2.2/django_stubs_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       25 2023-06-27 17:50:47.000000 django-stubs-ext-4.2.2/django_stubs_ext.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       17 2023-06-27 17:50:47.000000 django-stubs-ext-4.2.2/django_stubs_ext.egg-info/top_level.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       38 2023-06-27 17:50:47.533976 django-stubs-ext-4.2.2/setup.cfg
+-rwxr-xr-x   0 marti     (1000) marti      (121)     1663 2023-06-27 17:49:10.000000 django-stubs-ext-4.2.2/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:50:47.533976 django-stubs-ext-4.2.2/tests/
+-rw-r--r--   0 marti     (1000) marti      (121)      169 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.2/tests/test_aliases.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3928 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.2/tests/test_monkeypatching.py
```

### Comparing `django-stubs-ext-4.2.1/LICENSE.md` & `django-stubs-ext-4.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.1/PKG-INFO` & `django-stubs-ext-4.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 4.2.1
+Version: 4.2.2
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
 Author-email: 3nki.nam.shub@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -13,17 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `django-stubs-ext-4.2.1/README.md` & `django-stubs-ext-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.1/django_stubs_ext/__init__.py` & `django-stubs-ext-4.2.2/django_stubs_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.1/django_stubs_ext/aliases.py` & `django-stubs-ext-4.2.2/django_stubs_ext/aliases.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.1/django_stubs_ext/annotations.py` & `django-stubs-ext-4.2.2/django_stubs_ext/annotations.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.1/django_stubs_ext/db/models.py` & `django-stubs-ext-4.2.2/django_stubs_ext/db/models.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.1/django_stubs_ext/patch.py` & `django-stubs-ext-4.2.2/django_stubs_ext/patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from django import VERSION
 from django.contrib.admin import ModelAdmin
 from django.contrib.admin.options import BaseModelAdmin
 from django.contrib.sitemaps import Sitemap
 from django.contrib.syndication.views import Feed
 from django.core.files.utils import FileProxyMixin
 from django.core.paginator import Paginator
+from django.db.models.expressions import ExpressionWrapper
 from django.db.models.fields import Field
 from django.db.models.fields.related import ForeignKey
 from django.db.models.lookups import Lookup
 from django.db.models.manager import BaseManager
 from django.db.models.query import QuerySet
 from django.forms.formsets import BaseFormSet
 from django.forms.models import BaseModelForm, BaseModelFormSet
@@ -62,14 +63,15 @@
     MPGeneric(BaseModelForm),
     MPGeneric(BaseModelFormSet),
     MPGeneric(Feed),
     MPGeneric(Sitemap),
     MPGeneric(FileProxyMixin),
     MPGeneric(Lookup),
     MPGeneric(BaseConnectionHandler),
+    MPGeneric(ExpressionWrapper),
     # These types do have native `__class_getitem__` method since django 3.1:
     MPGeneric(QuerySet, (3, 1)),
     MPGeneric(BaseManager, (3, 1)),
     # These types do have native `__class_getitem__` method since django 4.1:
     MPGeneric(ForeignKey, (4, 1)),
 ]
```

### Comparing `django-stubs-ext-4.2.1/django_stubs_ext.egg-info/PKG-INFO` & `django-stubs-ext-4.2.2/django_stubs_ext.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 4.2.1
+Version: 4.2.2
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
 Author-email: 3nki.nam.shub@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -13,17 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `django-stubs-ext-4.2.1/setup.py` & `django-stubs-ext-4.2.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "typing-extensions",
 ]
 
 # NB! For clarity, keep version major.minor.patch in sync with django-stubs.
 # It's fine to skip django-stubs-ext releases, but when doing a release, update this to newest django-stubs version.
 setup(
     name="django-stubs-ext",
-    version="4.2.1",
+    version="4.2.2",
     description="Monkey-patching and extensions for django-stubs",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Simula Proxy",
@@ -36,17 +36,14 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
     ],
     project_urls={
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
```

### Comparing `django-stubs-ext-4.2.1/tests/test_monkeypatching.py` & `django-stubs-ext-4.2.2/tests/test_monkeypatching.py`

 * *Files identical despite different names*

