# Comparing `tmp/django-mptt2-0.1.1.tar.gz` & `tmp/django-mptt2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mptt2-0.1.1.tar", last modified: Thu Jun  8 07:09:44 2023, max compression
+gzip compressed data, was "django-mptt2-0.2.0.tar", last modified: Tue Jun 27 09:36:34 2023, max compression
```

## Comparing `django-mptt2-0.1.1.tar` & `django-mptt2-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/django_mptt2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/mptt2/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/mptt2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/query.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.592146 django-mptt2-0.2.0/django_mptt2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-27 09:36:34.000000 django-mptt2-0.2.0/django_mptt2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 09:36:34.000000 django-mptt2-0.2.0/django_mptt2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:36:34.000000 django-mptt2-0.2.0/django_mptt2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:36:34.000000 django-mptt2-0.2.0/django_mptt2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 09:36:34.000000 django-mptt2-0.2.0/django_mptt2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:36:34.000000 django-mptt2-0.2.0/django_mptt2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.592146 django-mptt2-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.592146 django-mptt2-0.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/source/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/source/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/source/docstrings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/docs/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/mptt2/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.588146 django-mptt2-0.2.0/mptt2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.588146 django-mptt2-0.2.0/mptt2/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/mptt2/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/mptt2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.592146 django-mptt2-0.2.0/mptt2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/mptt2/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/templates/admin/mptt_change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/templates/admin/mptt_change_list_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/templates/admin/mptt_draggable_change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/mptt2/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/mptt2/templatetags/mptt_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:36:34.596146 django-mptt2-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/tests/tests_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/tests/tests_admin_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41385 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/tests/tests_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/tests/tests_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-27 09:36:30.000000 django-mptt2-0.2.0/tests/tests_query.py
```

### Comparing `django-mptt2-0.1.1/LICENSE` & `django-mptt2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mptt2-0.1.1/PKG-INFO` & `django-mptt2-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: django-mptt2
-Version: 0.1.1
-Summary: Utilities for implementing a modified pre-order traversal tree (nested sets) in django.
-Home-page: https://github.com/jokiefer/django-mptt2
+Version: 0.2.0
+Summary: Utilities for implementing Modified Preorder Tree Traversal with your Django Models and working with trees of Model instances.
+Home-page: https://github.com/jokiefer/django-mptt2/
 Author: Jonas Kiefer
 Author-email: jonas.kiefer@live.com
-License: MIT
-Platform: UNKNOWN
+License: MIT-License
+Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: tests
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/django-mptt2/badge/?version=latest
     :target: https://django-mptt2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://badge.fury.io/py/django-mptt2.svg
@@ -83,8 +86,7 @@
     metal.insert_at(target=rock) # it will become the last child from rock 
 
     alternative = Genre(name="Alternative")
     alternative.insert_at(target=rock) # it will become the last child from rock, the right sibling of metal
 
 
 For full usage description, please read the tutorial section of our `documentation <https://django-mptt2.rtfd.io>`_.
-
```

### Comparing `django-mptt2-0.1.1/README.rst` & `django-mptt2-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-mptt2-0.1.1/django_mptt2.egg-info/PKG-INFO` & `django-mptt2-0.2.0/django_mptt2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: django-mptt2
-Version: 0.1.1
-Summary: Utilities for implementing a modified pre-order traversal tree (nested sets) in django.
-Home-page: https://github.com/jokiefer/django-mptt2
+Version: 0.2.0
+Summary: Utilities for implementing Modified Preorder Tree Traversal with your Django Models and working with trees of Model instances.
+Home-page: https://github.com/jokiefer/django-mptt2/
 Author: Jonas Kiefer
 Author-email: jonas.kiefer@live.com
-License: MIT
-Platform: UNKNOWN
+License: MIT-License
+Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: tests
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/django-mptt2/badge/?version=latest
     :target: https://django-mptt2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://badge.fury.io/py/django-mptt2.svg
@@ -83,8 +86,7 @@
     metal.insert_at(target=rock) # it will become the last child from rock 
 
     alternative = Genre(name="Alternative")
     alternative.insert_at(target=rock) # it will become the last child from rock, the right sibling of metal
 
 
 For full usage description, please read the tutorial section of our `documentation <https://django-mptt2.rtfd.io>`_.
-
```

### Comparing `django-mptt2-0.1.1/mptt2/expressions.py` & `django-mptt2-0.2.0/mptt2/expressions.py`

 * *Files identical despite different names*

### Comparing `django-mptt2-0.1.1/mptt2/managers.py` & `django-mptt2-0.2.0/mptt2/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 from django.db.models.query import QuerySet
 from django.db.transaction import atomic
 from django.utils.translation import gettext as _
 
 from mptt2.enums import Position
 from mptt2.exceptions import InvalidInsert, InvalidMove
 from mptt2.expressions import Depth, Left, Right
-from mptt2.query import (DescendantsQuery, RightSiblingsWithDescendants,
-                         RootQuery, SameNodeQuery, TreeQuerySet)
+from mptt2.query import (AncestorsQuery, DescendantsQuery,
+                         RightSiblingsWithDescendants, RootQuery,
+                         SameNodeQuery, TreeQuerySet)
 
 
 class TreeManager(Manager):
 
-    def get_queryset(self) -> QuerySet[TreeQuerySet]:
-        return TreeQuerySet(self.model, using=self._db)
+    queryset_class = TreeQuerySet
+
+    def get_queryset(self) -> QuerySet[queryset_class]:
+        return self.queryset_class(self.model, using=self._db)
 
     def _calculate_node_mptt_values_for_insert(self, node, target, position):
         node.mptt_tree = target.mptt_tree
         if position == Position.LAST_CHILD:
             node.mptt_parent = target
             node.mptt_depth = target.mptt_depth + 1
             node.mptt_lft = target.mptt_rgt
@@ -43,28 +46,29 @@
             node.mptt_rgt = target.mptt_rgt + 2
 
     def _calculate_filter_for_insert(self, target, position):
         if position in [Position.LAST_CHILD, Position.RIGHT]:
             return (
                 RootQuery(of=target) |
                 RightSiblingsWithDescendants(
-                    of=target, include_self=True if position == Position.LAST_CHILD else False)
+                    of=target, include_self=True if position == Position.LAST_CHILD else False)  |
+                AncestorsQuery(of=target)
             )
         else:
             return (
                 RootQuery(of=target) |
                 DescendantsQuery(of=target, include_self=True) |
                 RightSiblingsWithDescendants(of=target)
             )
 
     def _calculate_conditional_update_for_insert(self, target, position) -> Dict:
         condition = ~RootQuery(of=target)
 
         if position in [Position.LAST_CHILD, Position.FIRST_CHILD]:
-            condition &= ~SameNodeQuery(of=target)
+            condition &= ~SameNodeQuery(of=target) & ~ AncestorsQuery(of=target)
 
         return {
             "mptt_lft": Case(
                 When(
                     condition=condition,
                     then=Left() + 2
                 ),
@@ -260,7 +264,8 @@
         )
 
         node.mptt_lft = new_left
         node.mptt_rgt = new_right
         node.mptt_depth -= depth_change
         node.mptt_parent = parent
         node.save()
+        return node
```

### Comparing `django-mptt2-0.1.1/mptt2/models.py` & `django-mptt2-0.2.0/mptt2/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from django.db.models import Model
-from django.db.models.constraints import CheckConstraint
+from django.db.models.constraints import CheckConstraint, UniqueConstraint
 from django.db.models.deletion import CASCADE
 from django.db.models.expressions import F
 from django.db.models.fields import PositiveIntegerField
 from django.db.models.fields.related import ForeignKey
 from django.db.models.indexes import Index
 from django.db.models.query import Q, QuerySet
 from django.db.transaction import atomic
 from django.utils.translation import gettext as _
 
 from mptt2.compatibility import violation_error_message_kwargs
 from mptt2.enums import Position
 from mptt2.managers import TreeManager
-from mptt2.query import (AncestorsQuery, ChildrenQuery, DescendantsQuery,
-                         FamilyQuery, RootQuery, SiblingsQuery)
+from mptt2.query import (
+    AncestorsQuery,
+    ChildrenQuery,
+    DescendantsQuery,
+    FamilyQuery,
+    RootQuery,
+    SiblingsQuery,
+)
 
 
 class Tree(Model):
     """Simple Tree model to generate simple tree id's by the database to support thread safe inserting new tree's"""
     pass
 
 
@@ -51,16 +57,17 @@
         help_text=_("The parent of this node"),
     )
     mptt_tree = ForeignKey(
         to=Tree,
         on_delete=CASCADE,
         verbose_name=_("tree"),
         help_text=_("The unique tree, where this node is part of"),
-        related_name="nodes",
-        related_query_name="node"
+        related_name="%(app_label)s_%(class)s_nodes",
+        related_query_name="%(app_label)s_%(class)s_node",
+        editable=False
     )
     mptt_lft = PositiveIntegerField(
         editable=False,
         verbose_name=_("left"),
         help_text=_("The left value of the node")
     )
     mptt_rgt = PositiveIntegerField(
@@ -81,17 +88,19 @@
         ordering = ["mptt_tree_id", "mptt_lft"]
         indexes = [
             Index(fields=("mptt_tree_id", "mptt_lft", "mptt_rgt"))
         ]
         constraints = [
             CheckConstraint(
                 check=Q(mptt_rgt__gt=F("mptt_lft")),
-                name="rgt_gt_lft",
+                name="%(app_label)s_%(class)s_rgt_gt_lft",
                 **violation_error_message_kwargs()
-            )
+            ),
+            # TODO: add unique constraint for lft and rgt fields
+            # UniqueConstraint(fields=["mptt_tree_id", "mptt_lft"], name="unique_lft")
         ]
 
     def __str__(self) -> str:
         """returns pk | tree | lft | rgt"""
         return f"pk {self.pk} | tree {self.mptt_tree_id} | lft {self.mptt_lft} | rgt {self.mptt_rgt}"
 
     @atomic
@@ -230,15 +239,15 @@
     def is_leaf_node(self) -> bool:
         """returns true if this is a leaf node without children"""
         return (self.mptt_rgt - self.mptt_lft) // 2 == 0
 
     @ property
     def has_leafs(self) -> bool:
         """returns true if this node has leafs (descendants)"""
-        return self.mptt_rgt - self.mptt_lft > 0
+        return self.mptt_rgt - self.mptt_lft > 1
 
     @ property
     def descendant_count(self) -> int:
         """returns the descendant count"""
         if self.mptt_rgt is None:
             # node not saved yet
             return 0
```

### Comparing `django-mptt2-0.1.1/mptt2/query.py` & `django-mptt2-0.2.0/mptt2/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any, Dict, Tuple
 
 from django.db.models.expressions import CombinedExpression, F, OuterRef
 from django.db.models.query import QuerySet
 from django.db.models.query_utils import Q
 
 
 class ConvertableQuery(Q):
@@ -158,9 +158,13 @@
             "mptt_rgt__lte" if include_self else "mptt_rgt__lt": of.mptt_rgt
         }
         super().__init__(*args, **kwargs, **query_kwargs)
 
 
 class TreeQuerySet(QuerySet):
 
+    def delete(self):
+        # TODO: if this function is called, we need to analyze the nodes of the queryset first and update the tree(s).
+        raise NotImplementedError("Delete MPTT nodes in bulk is not supported for now. Please delete a single node. All descendants will also be deleted as well.")
+
     def with_descendant_count(self):
         self.annotate(descendant_count=F("mptt_rgt") - F("mptt_lft") // 2)
```

