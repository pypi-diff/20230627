# Comparing `tmp/notalib-2.0.0.tar.gz` & `tmp/notalib-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notalib-2.0.0.tar", max compression
+gzip compressed data, was "notalib-2.1.0.tar", max compression
```

## Comparing `notalib-2.0.0.tar` & `notalib-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
--rw-r--r--   0        0        0     1068 2022-12-12 12:38:13.108694 notalib-2.0.0/LICENSE
--rw-r--r--   0        0        0     9341 2022-12-19 09:35:22.248595 notalib-2.0.0/README.md
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/__init__.py
--rw-r--r--   0        0        0      273 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/array.py
--rw-r--r--   0        0        0     1475 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/array_test.py
--rw-r--r--   0        0        0      875 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/combinator.py
--rw-r--r--   0        0        0     3202 2022-12-19 09:35:22.248595 notalib-2.0.0/notalib/date.py
--rw-r--r--   0        0        0     2042 2022-12-19 09:35:22.248595 notalib-2.0.0/notalib/date_test.py
--rw-r--r--   0        0        0      880 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/deprecated.py
--rw-r--r--   0        0        0     1611 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/dict.py
--rw-r--r--   0        0        0     1119 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/dict_test.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/__init__.py
--rw-r--r--   0        0        0     2102 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/auth.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/clickhouse/__init__.py
--rw-r--r--   0        0        0     1685 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/clickhouse/base.py
--rw-r--r--   0        0        0     1002 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/clickhouse/mutations.py
--rw-r--r--   0        0        0     1387 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/clickhouse/profiler.py
--rw-r--r--   0        0        0      796 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/clickhouse/wait.py
--rw-r--r--   0        0        0     1392 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/colorlog.py
--rw-r--r--   0        0        0     1074 2022-12-12 12:38:13.108694 notalib-2.0.0/notalib/django/filterset.py
--rw-r--r--   0        0        0      967 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django/filterset_test.py
--rw-r--r--   0        0        0     1613 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django/formplus.py
--rw-r--r--   0        0        0     1354 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django/formplus_test.py
--rw-r--r--   0        0        0     2298 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django/request_time_middleware.py
--rw-r--r--   0        0        0      998 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django/stream.py
--rw-r--r--   0        0        0      810 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django/stream_test.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django_xauth/__init__.py
--rw-r--r--   0        0        0       89 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django_xauth/apps.py
--rw-r--r--   0        0        0      498 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django_xauth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django_xauth/migrations/__init__.py
--rw-r--r--   0        0        0       97 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django_xauth/models.py
--rw-r--r--   0        0        0      180 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django_xauth/serializers.py
--rw-r--r--   0        0        0      325 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django_xauth/urls.py
--rw-r--r--   0        0        0     1009 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/django_xauth/views.py
--rw-r--r--   0        0        0     8229 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/filterset.py
--rw-r--r--   0        0        0     1858 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/filterset_test.py
--rw-r--r--   0        0        0      303 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/format.py
--rw-r--r--   0        0        0     1920 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/hypertext.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/pandas/__init__.py
--rw-r--r--   0        0        0      973 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/pandas/pandasplus.py
--rw-r--r--   0        0        0     1571 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/pandas/pandasplus_test.py
--rw-r--r--   0        0        0     3304 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/polosa.py
--rw-r--r--   0        0        0     1217 2022-12-12 12:38:13.112694 notalib-2.0.0/notalib/range.py
--rw-r--r--   0        0        0      604 2022-12-12 12:38:13.116694 notalib-2.0.0/notalib/time.py
--rw-r--r--   0        0        0     2214 2022-12-12 12:38:13.116694 notalib-2.0.0/notalib/trendsetter.py
--rw-r--r--   0        0        0       22 2022-12-12 12:38:13.116694 notalib-2.0.0/notalib/utf.py
--rw-r--r--   0        0        0      912 2022-12-19 09:35:22.248595 notalib-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    10548 1970-01-01 00:00:00.000000 notalib-2.0.0/setup.py
--rw-r--r--   0        0        0    10171 1970-01-01 00:00:00.000000 notalib-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-12 12:38:13.108694 notalib-2.1.0/LICENSE
+-rw-r--r--   0        0        0    11440 2023-01-18 09:27:11.485858 notalib-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/__init__.py
+-rw-r--r--   0        0        0      273 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/array.py
+-rw-r--r--   0        0        0     1475 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/array_test.py
+-rw-r--r--   0        0        0      875 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/combinator.py
+-rw-r--r--   0        0        0     3202 2022-12-19 09:40:02.742282 notalib-2.1.0/notalib/date.py
+-rw-r--r--   0        0        0     2042 2022-12-19 09:40:02.742282 notalib-2.1.0/notalib/date_test.py
+-rw-r--r--   0        0        0      880 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/deprecated.py
+-rw-r--r--   0        0        0     2940 2023-01-18 09:17:40.644758 notalib-2.1.0/notalib/dict.py
+-rw-r--r--   0        0        0     2108 2023-01-18 09:17:40.644758 notalib-2.1.0/notalib/dict_test.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/__init__.py
+-rw-r--r--   0        0        0     2102 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/auth.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1685 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/clickhouse/base.py
+-rw-r--r--   0        0        0     1002 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/clickhouse/mutations.py
+-rw-r--r--   0        0        0     1387 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/clickhouse/profiler.py
+-rw-r--r--   0        0        0      796 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/clickhouse/wait.py
+-rw-r--r--   0        0        0     1392 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/colorlog.py
+-rw-r--r--   0        0        0     1074 2022-12-12 12:38:13.108694 notalib-2.1.0/notalib/django/filterset.py
+-rw-r--r--   0        0        0      967 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django/filterset_test.py
+-rw-r--r--   0        0        0     1613 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django/formplus.py
+-rw-r--r--   0        0        0     1354 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django/formplus_test.py
+-rw-r--r--   0        0        0     2298 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django/request_time_middleware.py
+-rw-r--r--   0        0        0      998 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django/stream.py
+-rw-r--r--   0        0        0      810 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django/stream_test.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django_xauth/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-27 09:19:55.956175 notalib-2.1.0/notalib/django_xauth/apps.py
+-rw-r--r--   0        0        0      498 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django_xauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django_xauth/migrations/__init__.py
+-rw-r--r--   0        0        0       97 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django_xauth/models.py
+-rw-r--r--   0        0        0      180 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django_xauth/serializers.py
+-rw-r--r--   0        0        0      325 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django_xauth/urls.py
+-rw-r--r--   0        0        0     1009 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/django_xauth/views.py
+-rw-r--r--   0        0        0     8229 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/filterset.py
+-rw-r--r--   0        0        0     1858 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/filterset_test.py
+-rw-r--r--   0        0        0      303 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/format.py
+-rw-r--r--   0        0        0     1736 2023-01-18 09:17:40.644758 notalib-2.1.0/notalib/git.py
+-rw-r--r--   0        0        0     1920 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/hypertext.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/pandas/__init__.py
+-rw-r--r--   0        0        0      973 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/pandas/pandasplus.py
+-rw-r--r--   0        0        0     1571 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/pandas/pandasplus_test.py
+-rw-r--r--   0        0        0     3304 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/polosa.py
+-rw-r--r--   0        0        0     1217 2022-12-12 12:38:13.112694 notalib-2.1.0/notalib/range.py
+-rw-r--r--   0        0        0      604 2022-12-12 12:38:13.116694 notalib-2.1.0/notalib/time.py
+-rw-r--r--   0        0        0      652 2023-01-18 09:17:40.644758 notalib-2.1.0/notalib/timedelta.py
+-rw-r--r--   0        0        0      925 2023-01-18 09:17:40.644758 notalib-2.1.0/notalib/timedelta_test.py
+-rw-r--r--   0        0        0     2214 2022-12-12 12:38:13.116694 notalib-2.1.0/notalib/trendsetter.py
+-rw-r--r--   0        0        0       22 2022-12-12 12:38:13.116694 notalib-2.1.0/notalib/utf.py
+-rw-r--r--   0        0        0      923 2023-06-27 09:22:00.491330 notalib-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12741 1970-01-01 00:00:00.000000 notalib-2.1.0/setup.py
+-rw-r--r--   0        0        0    12270 1970-01-01 00:00:00.000000 notalib-2.1.0/PKG-INFO
```

### Comparing `notalib-2.0.0/LICENSE` & `notalib-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/README.md` & `notalib-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,70 @@
+Metadata-Version: 2.1
+Name: notalib
+Version: 2.1.0
+Summary: A collection of utility functions & classes
+Home-page: https://github.com/m1kc/notalib
+License: MIT
+Keywords: utility,django,pandas
+Author: m1kc (Max Musatov)
+Author-email: m1kc@yandex.ru
+Requires-Python: >=3.7.3,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: arrow (>=0.14.0,<2.0.0)
+Project-URL: Documentation, https://github.com/m1kc/notalib
+Project-URL: Repository, https://github.com/m1kc/notalib.git
+Description-Content-Type: text/markdown
+
 # notalib [![Django CI](https://github.com/m1kc/notalib/actions/workflows/django.yml/badge.svg)](https://github.com/m1kc/notalib/actions/workflows/django.yml) [![Coverage Status](https://coveralls.io/repos/github/m1kc/notalib/badge.svg?branch=master)](https://coveralls.io/github/m1kc/notalib?branch=master)
 
 Collection of small Python utility functions and classes. Each one was created because I needed it and it didn't exist or I didn't like the existing implementations. 100% of code is used in real-world projects.
 
 (And one day, the documentation is going to be actually good. In the meanwhile, don't hesitate to ask if something's not clear.)
 
+
 ## Install
 
 ```sh
 pip install notalib
 ```
 
 Or with [poetry](https://python-poetry.org/):
 
 ```sh
 poetry add notalib
 ```
 
+
+## Compatibility promise
+
+Version numbers follow the semver rules. Minor releases are backwards-compatible. It should be safe to update, say, from 1.2 to 1.4.
+
+Major releases are not backwards-compatible. If you upgrade, say, from 1.4 to 2.0, read the release notes to see what's changed.
+
+
 ## Maintenance & bugfixes
 
 While I try to fix bugs, add new features, and review any PRs when I have time, there're no promises and no set timeframes, even if a bug is critical. That's a project I do in my free time, free of charge.
 
 If that's not enough for you or you have an urgent request, there are paid maintenance options (bugfixing, features, expedite PR review, 24h security responses). Contact me for prices: m1kc@yandex.ru
 
 Also feel free to just send me money:
 
 * MasterCard: 5559 4925 7484 0297
 * PayPal: [paypal.me/thisism1kc](https://paypal.me/thisism1kc)
 
 Donations are always appreciated, even if you send 10$.
 
+
 ## Constants included
 
 * `notalib.utf.BOM`: contains string `b'\xEF\xBB\xBF'` (UTF-8 little endian byte order mark).
 
 ## Utils included
 
 #### notalib.array.as_chunks :fire:
@@ -99,14 +131,28 @@
 get_week(date2, WeekNumbering.NORMAL)
 # Week(week=52, year=2022)
 
 get_week(date2, WeekNumbering.MATCH_YEAR)
 # Week(week=0, year=2023)
 ```
 
+#### notalib.dict.deep_merge
+
+_:warning: Experimental API. Subject to change. Don't use in production. You've been warned._
+
+Merges two dicts.
+
+Modifies input. Use `copy.deepcopy` to create a deep copy of the original dictionary if you need it.
+
+Accepts three arguments:
+
+* original dict (also target)
+* second dict
+* overwrite=True if you want to overwrite matching paths, overwrite=False to raise an exception on path conflicts (default)
+
 #### notalib.dict.find_field
 #### notalib.dict.find_value
 #### notalib.dict.normalize_dict :fire:
 #### notalib.dict.filter_dict
 
 Filters a dictionary, removing any keys except for the ones you choose.
 
@@ -121,14 +167,33 @@
 filter_dict(src, ["Some", "once"])
 # {'Some': 'BODY', 'once': 'told me'}
 filter_dict(src, [])
 # {}
 ```
 
 #### notalib.format.format_long_list
+#### notalib.timedelta.convert_timedelta
+
+_:warning: Experimental API. Subject to change. Don't use in production. You've been warned._
+
+Converts standard timedelta object to specified formats.
+
+Allowed formats: 's', 'ms'.
+
+```python
+from notalib.timedelta import convert_timedelta
+from datetime import timedelta
+
+td = timedelta(seconds=1, milliseconds=23)
+convert_timedelta(td, 's')
+# 1.023
+convert_timedelta(td, 'ms')
+# 1023
+```
+
 #### notalib.hypertext.strip_tags :fire:
 #### notalib.hypertext.TablePrinter :fire:
 
 Prints an HTML table, row by row, from the given data, using attrs or dictionary keys as columns.
 
 Two ways to use it:
 
@@ -204,14 +269,40 @@
 ...
 with timing:
     do_something()
 ```
 
 #### notalib.trendsetter.Trendsetter :fire:
 
+#### notalib.git.get_current_commit
+
+_:warning: Experimental API. Subject to change. Don't use in production. You've been warned._
+
+Returns short description and hash of last commit of current branch.
+If function is called outside git repo or there are no commits in the history, `None` will be returned.
+
+```python
+from notalib.git import get_current_commit
+
+commit = get_current_commit()
+# Commit(hash='db0e5c1de83f233abef823fd92490727f4ee9d50', short_description='Add timedelta module with convert_timedelta function')
+```
+#### notalib.git.get_last_tag
+
+_:warning: Experimental API. Subject to change. Don't use in production. You've been warned._
+
+Returns last tag label and hash. If function is called outside git repo or there are no tags in the history, `None` will be returned.
+
+```python
+from notalib.git import get_last_tag
+
+tag = get_last_tag()
+# Tag(hash='c4b6e06f57ab4773e2881d286804d4e3141b5195', label='v1.4.0')
+```
+
 ## Pandas-related
 
 #### notalib.pandas.pandasplus.row_to_dict
 #### notalib.pandas.pandasplus.replace_null_objects
 
 Replaces all types of null values in a DataFrame with the given value.
 
@@ -315,7 +406,8 @@
 Waits until all mutations for the given table are complete.
 
 ```python
 # blah blah blah, ALTER TABLE ... UPDATE ...
 wait_result("SOME_DATABASE", "SOME_TABLE_IN_DATABASE")
 # UPDATE complete, continue
 ```
+
```

### Comparing `notalib-2.0.0/notalib/array_test.py` & `notalib-2.1.0/notalib/array_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/combinator.py` & `notalib-2.1.0/notalib/combinator.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/date.py` & `notalib-2.1.0/notalib/date.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/date_test.py` & `notalib-2.1.0/notalib/date_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/deprecated.py` & `notalib-2.1.0/notalib/deprecated.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/auth.py` & `notalib-2.1.0/notalib/django/auth.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/clickhouse/base.py` & `notalib-2.1.0/notalib/django/clickhouse/base.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/clickhouse/mutations.py` & `notalib-2.1.0/notalib/django/clickhouse/mutations.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/clickhouse/profiler.py` & `notalib-2.1.0/notalib/django/clickhouse/profiler.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/clickhouse/wait.py` & `notalib-2.1.0/notalib/django/clickhouse/wait.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/colorlog.py` & `notalib-2.1.0/notalib/django/colorlog.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/filterset.py` & `notalib-2.1.0/notalib/django/filterset.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/filterset_test.py` & `notalib-2.1.0/notalib/django/filterset_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/formplus.py` & `notalib-2.1.0/notalib/django/formplus.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/formplus_test.py` & `notalib-2.1.0/notalib/django/formplus_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/request_time_middleware.py` & `notalib-2.1.0/notalib/django/request_time_middleware.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/stream.py` & `notalib-2.1.0/notalib/django/stream.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django/stream_test.py` & `notalib-2.1.0/notalib/django/stream_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/django_xauth/views.py` & `notalib-2.1.0/notalib/django_xauth/views.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/filterset.py` & `notalib-2.1.0/notalib/filterset.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/filterset_test.py` & `notalib-2.1.0/notalib/filterset_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/hypertext.py` & `notalib-2.1.0/notalib/hypertext.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/pandas/pandasplus.py` & `notalib-2.1.0/notalib/pandas/pandasplus.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/pandas/pandasplus_test.py` & `notalib-2.1.0/notalib/pandas/pandasplus_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/polosa.py` & `notalib-2.1.0/notalib/polosa.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/range.py` & `notalib-2.1.0/notalib/range.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/time.py` & `notalib-2.1.0/notalib/time.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/notalib/trendsetter.py` & `notalib-2.1.0/notalib/trendsetter.py`

 * *Files identical despite different names*

### Comparing `notalib-2.0.0/pyproject.toml` & `notalib-2.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notalib"
-version = "2.0.0"
+version = "2.1.0"
 description = "A collection of utility functions & classes"
 authors = ["m1kc (Max Musatov) <m1kc@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/m1kc/notalib"
 repository = "https://github.com/m1kc/notalib.git"
 documentation = "https://github.com/m1kc/notalib"
@@ -24,15 +24,15 @@
 pytest-cov = "^3.0.0"
 Django = ">=2"
 hypothesis = {extras = ["django", "numpy"], version = "^6.36.1"}
 numpy = "^1.21.1"
 pandas = "^1.1.5"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning",
 ]
```

### Comparing `notalib-2.0.0/setup.py` & `notalib-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 {'': ['*']}
 
 install_requires = \
 ['arrow>=0.14.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'notalib',
-    'version': '2.0.0',
+    'version': '2.1.0',
     'description': 'A collection of utility functions & classes',
-    'long_description': '# notalib [![Django CI](https://github.com/m1kc/notalib/actions/workflows/django.yml/badge.svg)](https://github.com/m1kc/notalib/actions/workflows/django.yml) [![Coverage Status](https://coveralls.io/repos/github/m1kc/notalib/badge.svg?branch=master)](https://coveralls.io/github/m1kc/notalib?branch=master)\n\nCollection of small Python utility functions and classes. Each one was created because I needed it and it didn\'t exist or I didn\'t like the existing implementations. 100% of code is used in real-world projects.\n\n(And one day, the documentation is going to be actually good. In the meanwhile, don\'t hesitate to ask if something\'s not clear.)\n\n## Install\n\n```sh\npip install notalib\n```\n\nOr with [poetry](https://python-poetry.org/):\n\n```sh\npoetry add notalib\n```\n\n## Maintenance & bugfixes\n\nWhile I try to fix bugs, add new features, and review any PRs when I have time, there\'re no promises and no set timeframes, even if a bug is critical. That\'s a project I do in my free time, free of charge.\n\nIf that\'s not enough for you or you have an urgent request, there are paid maintenance options (bugfixing, features, expedite PR review, 24h security responses). Contact me for prices: m1kc@yandex.ru\n\nAlso feel free to just send me money:\n\n* MasterCard: 5559 4925 7484 0297\n* PayPal: [paypal.me/thisism1kc](https://paypal.me/thisism1kc)\n\nDonations are always appreciated, even if you send 10$.\n\n## Constants included\n\n* `notalib.utf.BOM`: contains string `b\'\\xEF\\xBB\\xBF\'` (UTF-8 little endian byte order mark).\n\n## Utils included\n\n#### notalib.array.as_chunks :fire:\n\nIterates over your array in chunks of at most N elements.\n\n```python\nfrom notalib.array import as_chunks\n\narr = [1,2,3,4,5]\nfor chunk in as_chunks(arr, 2):\n    print(chunk)\n# [1,2]\n# [3,4]\n# [5]\n```\n\n#### notalib.array.ensure_iterable :fire:\n\nKeeps iterable things like lists intact, turns single values into single-element lists. Useful for functions that can accept both.\n\n```python\nensure_iterable([1,2,3])  # --> [1,2,3]\nensure_iterable((1,2,3))  # --> (1,2,3)\nensure_iterable(1)        # --> [1]\nensure_iterable(\'smth\')   # --> [\'smth\']\n\ndef my_function(one_or_multiple_args):\n    for arg in ensure_iterable(one_or_multiple_args):\n        ...\n        \nmy_function([\'log\', \'smog\'])\nmy_function(\'dog\')\n```\n\n#### notalib.combinator.Combinator :fire:\n#### notalib.date.parse_month\n#### notalib.date.parse_date\n#### notalib.date.normalize_date :fire:\n#### <s>notalib.date.get_week_number</s>\n\n_Removed in 2.0.0. Use `get_week` instead. If you want the "old" week numbering, use get_week with `WeekNumbering.MATCH_YEAR` and add 1 to week number._\n\n#### notalib.date.get_week\n\nReturns named tuple with week number for the given date. Accepts Python dates and Arrow timestamps.\n\nOptional argument `mode` tells what to do if the week started in previous year:\n\n* WeekNumbering.NORMAL (default): consider it the last week of the previous year\n* WeekNumbering.MATCH_YEAR: consider it 0-th week of current year\n\n```python\nfrom notalib.date import get_week, WeekNumbering\nfrom datetime import date\n\ndate1, date2 = date(2022, 12, 31), date(2023, 1, 1)\nget_week(date1, WeekNumbering.NORMAL)\n# Week(week=52, year=2022)\n\nget_week(date1, WeekNumbering.MATCH_YEAR)\n# Week(week=52, year=2022)\n\nget_week(date2, WeekNumbering.NORMAL)\n# Week(week=52, year=2022)\n\nget_week(date2, WeekNumbering.MATCH_YEAR)\n# Week(week=0, year=2023)\n```\n\n#### notalib.dict.find_field\n#### notalib.dict.find_value\n#### notalib.dict.normalize_dict :fire:\n#### notalib.dict.filter_dict\n\nFilters a dictionary, removing any keys except for the ones you choose.\n\n```python\nfrom notalib.dict import filter_dict\n\nsrc = {\n\t\'Some\': "BODY",\n\t\'once\': "told me",\n\t\'the world\': "is gonna roll me",\n}\nfilter_dict(src, ["Some", "once"])\n# {\'Some\': \'BODY\', \'once\': \'told me\'}\nfilter_dict(src, [])\n# {}\n```\n\n#### notalib.format.format_long_list\n#### notalib.hypertext.strip_tags :fire:\n#### notalib.hypertext.TablePrinter :fire:\n\nPrints an HTML table, row by row, from the given data, using attrs or dictionary keys as columns.\n\nTwo ways to use it:\n\n* Call header() / entry() / footer() manually\n\n```python\nfrom notalib.hypertext import TablePrinter\nt = TablePrinter([\'a\', \'b\'])\nt.header()\n# \'<table><thead><tr><th>a</th><th>b</th></tr></thead><tbody>\'\nt.entry({\'a\': 1, \'b\': 2})\n# \'<tr><td>1</td><td>2</td></tr>\\n\'\nt.entry({\'a\': 11, \'b\': 22})\n# \'<tr><td>11</td><td>22</td></tr>\\n\'\nt.footer()\n# \'</tbody></table>\'\n```\n\n* Pass an iterable to iterator_over()\n\t\n```python\nfrom notalib.hypertext import TablePrinter\nt = TablePrinter([\'a\', \'b\'])\nlist(t.iterator_over([ {\'a\': 11, \'b\': 22} ]))\n# [\'<table><thead><tr><th>a</th><th>b</th></tr></thead><tbody>\',\n#  \'<tr><td>11</td><td>22</td></tr>\\n\',\n#  \'</tbody></table>\']\n```\n\n#### notalib.polosa.polosa :fire: :fire: :fire: :fire: :fire:\n\n```\n18023/2000000   294.8/sec   Processing transaction ID#84378473 (2020-01-04)\n```\n\nThe CLI progress indicator you\'ve always dreamt of: shows current and total if available, measures current speed, can show your comments for each element, makes sure not to slow down your terminal with frequent updates. [See this short demo](https://asciinema.org/a/UI1aOqjQC1KXx303kaVGrxjQp).\n\n_Cheat sheet_\n\n```python\n## Basic usage\nwith polosa() as p:\n    p.tick()\n# 467344   201.2/sec\n\n## Specify total number of elements:\nwith polosa(total=1337) as p:\n# 26/1337   1.2/sec\n\n## Print something useful about every element:\np.tick(caption=my_order.time_created)\n# 1723910/2000000   319231.2/sec   2020-01-01 15:37:00\n```\n\n#### notalib.range.Range\n#### notalib.time.Timing :fire:\n\nMeasures time spent on executing your code. Killer feature: it can be used as a reusable context.\n\n```python\ntiming = Timing()\n...\nwith timing:\n    do_something()\n# That\'s it, do something with the measurement\nlog(f\'Operation took {timing.result} sec\')\n```\n\nIf you just want to print measurements into console, there\'s a shorthand:\n\n```python\ntiming = Timing(auto_print=True)\n...\nwith timing:\n    do_something()\n```\n\n#### notalib.trendsetter.Trendsetter :fire:\n\n## Pandas-related\n\n#### notalib.pandas.pandasplus.row_to_dict\n#### notalib.pandas.pandasplus.replace_null_objects\n\nReplaces all types of null values in a DataFrame with the given value.\n\n```python\ndf = pd.DataFrame({\'A\': [pd.NA, pd.NaT, \'SomeVal\', None]})\nnew_df = replace_null_objects(df, "Hello, notalib!")\nnew_df\n#                  A\n# 0  Hello, notalib!\n# 1  Hello, notalib!\n# 2          SomeVal\n# 3  Hello, notalib!\n```\n\n## Django-related\n\n#### notalib.django.auth.StaticBackend\n#### notalib.django.auth.SettingsBackend\n\n#### notalib.django.xauth\n\nEndpoints for easier authentication in APIs. Requires Django REST framework.\n\nProvides endpoints:\n\n* `/xauth/check` — returns code 200 if client is authenticated (or global permissions are set to AllowAny), 403 if not\n* `/xauth/auth-post` — authenticates a client; accepts two POST parameters `username` and `password`; returns code 200 on success and 403 on failure\n\nHow to use:\n\n1. Make sure Django REST framework is installed.\n2. Add `\'notalib.django_xauth\'` to INSTALLED_APPS.\n3. Run `manage.py migrate django_xauth` (doesn\'t actually change your DB).\n4. Add something like this to your urls.py: `path(\'xauth/\', include(\'notalib.django_xauth.urls\')),`\n\n#### notalib.django.colorlog.ColorFormatter\n#### notalib.django.filterset :fire:\n#### notalib.django.formplus.MonthField\n#### notalib.django.formplus.ChoiceWithDefault\n#### notalib.django.formplus.IntegerArrayField\n#### notalib.django.formplus.StringArrayField\n#### notalib.django.formplus.MonthArrayField\n#### notalib.django.request_time_middleware.RequestTimeLoggingMiddleware\n#### notalib.django.stream.stream_json\n\nStream all elements of iterable object as JSON array using the StreamingHttpResponse class. Unlike DRF\'s Response class, it can handle arrays of any size.\n\n```python\nclass SomeViewSet(...):\n    ...\n    \n    def list(self, request, *args, **kwargs):\n        ...\n        return stream_json(data)\n```\n\n## Django/Clickhouse\n\n_Stage: alpha_\n\nRequired packages: `clickhouse-sqlalchemy`\n\nRequired two django.settings variables:\n\n* **CLICKHOUSE_URL** — database URL\n* **CLICKHOUSE_PROFILE** — dump all queries and their timing to console, true/false\n\n#### notalib.django.clickhouse.base.get_connection\n#### notalib.django.clickhouse.base.get_database_name\n#### notalib.django.clickhouse.base.Query\n\nA wrapper for SQLAlchemy\'s `select` with some useful postprocessing options.\n\n* `execute` — no postprocessing\n* `execute_val` — returns single value\n* `execute_list` — returns single column as list\n* `execute_kv` — returns dict, first column becomes keys, second column becomes values\n* `execute_na` — returns number of affected rows\n\nUsage example:\n\n```python\nq = Query(\n    select([ SomeTable.c.notalib ])\n)\nq.execute_list()\n# ["Example", "OOOOO", "my", "defence", ...]\n```\n\n#### notalib.django.clickhouse.mutations.get_mutations_in_progress_count\n\nReturns the number of mutations in progress for the specified table.\n\n```python\nget_mutations_in_progress_count("SOME_DATABASE", "SOME_TABLE_IN_DATABASE")\n# 5\n```\n\n#### notalib.django.clickhouse.wait.wait_result :fire:\n\nWaits until all mutations for the given table are complete.\n\n```python\n# blah blah blah, ALTER TABLE ... UPDATE ...\nwait_result("SOME_DATABASE", "SOME_TABLE_IN_DATABASE")\n# UPDATE complete, continue\n```\n',
+    'long_description': '# notalib [![Django CI](https://github.com/m1kc/notalib/actions/workflows/django.yml/badge.svg)](https://github.com/m1kc/notalib/actions/workflows/django.yml) [![Coverage Status](https://coveralls.io/repos/github/m1kc/notalib/badge.svg?branch=master)](https://coveralls.io/github/m1kc/notalib?branch=master)\n\nCollection of small Python utility functions and classes. Each one was created because I needed it and it didn\'t exist or I didn\'t like the existing implementations. 100% of code is used in real-world projects.\n\n(And one day, the documentation is going to be actually good. In the meanwhile, don\'t hesitate to ask if something\'s not clear.)\n\n\n## Install\n\n```sh\npip install notalib\n```\n\nOr with [poetry](https://python-poetry.org/):\n\n```sh\npoetry add notalib\n```\n\n\n## Compatibility promise\n\nVersion numbers follow the semver rules. Minor releases are backwards-compatible. It should be safe to update, say, from 1.2 to 1.4.\n\nMajor releases are not backwards-compatible. If you upgrade, say, from 1.4 to 2.0, read the release notes to see what\'s changed.\n\n\n## Maintenance & bugfixes\n\nWhile I try to fix bugs, add new features, and review any PRs when I have time, there\'re no promises and no set timeframes, even if a bug is critical. That\'s a project I do in my free time, free of charge.\n\nIf that\'s not enough for you or you have an urgent request, there are paid maintenance options (bugfixing, features, expedite PR review, 24h security responses). Contact me for prices: m1kc@yandex.ru\n\nAlso feel free to just send me money:\n\n* MasterCard: 5559 4925 7484 0297\n* PayPal: [paypal.me/thisism1kc](https://paypal.me/thisism1kc)\n\nDonations are always appreciated, even if you send 10$.\n\n\n## Constants included\n\n* `notalib.utf.BOM`: contains string `b\'\\xEF\\xBB\\xBF\'` (UTF-8 little endian byte order mark).\n\n## Utils included\n\n#### notalib.array.as_chunks :fire:\n\nIterates over your array in chunks of at most N elements.\n\n```python\nfrom notalib.array import as_chunks\n\narr = [1,2,3,4,5]\nfor chunk in as_chunks(arr, 2):\n    print(chunk)\n# [1,2]\n# [3,4]\n# [5]\n```\n\n#### notalib.array.ensure_iterable :fire:\n\nKeeps iterable things like lists intact, turns single values into single-element lists. Useful for functions that can accept both.\n\n```python\nensure_iterable([1,2,3])  # --> [1,2,3]\nensure_iterable((1,2,3))  # --> (1,2,3)\nensure_iterable(1)        # --> [1]\nensure_iterable(\'smth\')   # --> [\'smth\']\n\ndef my_function(one_or_multiple_args):\n    for arg in ensure_iterable(one_or_multiple_args):\n        ...\n        \nmy_function([\'log\', \'smog\'])\nmy_function(\'dog\')\n```\n\n#### notalib.combinator.Combinator :fire:\n#### notalib.date.parse_month\n#### notalib.date.parse_date\n#### notalib.date.normalize_date :fire:\n#### <s>notalib.date.get_week_number</s>\n\n_Removed in 2.0.0. Use `get_week` instead. If you want the "old" week numbering, use get_week with `WeekNumbering.MATCH_YEAR` and add 1 to week number._\n\n#### notalib.date.get_week\n\nReturns named tuple with week number for the given date. Accepts Python dates and Arrow timestamps.\n\nOptional argument `mode` tells what to do if the week started in previous year:\n\n* WeekNumbering.NORMAL (default): consider it the last week of the previous year\n* WeekNumbering.MATCH_YEAR: consider it 0-th week of current year\n\n```python\nfrom notalib.date import get_week, WeekNumbering\nfrom datetime import date\n\ndate1, date2 = date(2022, 12, 31), date(2023, 1, 1)\nget_week(date1, WeekNumbering.NORMAL)\n# Week(week=52, year=2022)\n\nget_week(date1, WeekNumbering.MATCH_YEAR)\n# Week(week=52, year=2022)\n\nget_week(date2, WeekNumbering.NORMAL)\n# Week(week=52, year=2022)\n\nget_week(date2, WeekNumbering.MATCH_YEAR)\n# Week(week=0, year=2023)\n```\n\n#### notalib.dict.deep_merge\n\n_:warning: Experimental API. Subject to change. Don\'t use in production. You\'ve been warned._\n\nMerges two dicts.\n\nModifies input. Use `copy.deepcopy` to create a deep copy of the original dictionary if you need it.\n\nAccepts three arguments:\n\n* original dict (also target)\n* second dict\n* overwrite=True if you want to overwrite matching paths, overwrite=False to raise an exception on path conflicts (default)\n\n#### notalib.dict.find_field\n#### notalib.dict.find_value\n#### notalib.dict.normalize_dict :fire:\n#### notalib.dict.filter_dict\n\nFilters a dictionary, removing any keys except for the ones you choose.\n\n```python\nfrom notalib.dict import filter_dict\n\nsrc = {\n\t\'Some\': "BODY",\n\t\'once\': "told me",\n\t\'the world\': "is gonna roll me",\n}\nfilter_dict(src, ["Some", "once"])\n# {\'Some\': \'BODY\', \'once\': \'told me\'}\nfilter_dict(src, [])\n# {}\n```\n\n#### notalib.format.format_long_list\n#### notalib.timedelta.convert_timedelta\n\n_:warning: Experimental API. Subject to change. Don\'t use in production. You\'ve been warned._\n\nConverts standard timedelta object to specified formats.\n\nAllowed formats: \'s\', \'ms\'.\n\n```python\nfrom notalib.timedelta import convert_timedelta\nfrom datetime import timedelta\n\ntd = timedelta(seconds=1, milliseconds=23)\nconvert_timedelta(td, \'s\')\n# 1.023\nconvert_timedelta(td, \'ms\')\n# 1023\n```\n\n#### notalib.hypertext.strip_tags :fire:\n#### notalib.hypertext.TablePrinter :fire:\n\nPrints an HTML table, row by row, from the given data, using attrs or dictionary keys as columns.\n\nTwo ways to use it:\n\n* Call header() / entry() / footer() manually\n\n```python\nfrom notalib.hypertext import TablePrinter\nt = TablePrinter([\'a\', \'b\'])\nt.header()\n# \'<table><thead><tr><th>a</th><th>b</th></tr></thead><tbody>\'\nt.entry({\'a\': 1, \'b\': 2})\n# \'<tr><td>1</td><td>2</td></tr>\\n\'\nt.entry({\'a\': 11, \'b\': 22})\n# \'<tr><td>11</td><td>22</td></tr>\\n\'\nt.footer()\n# \'</tbody></table>\'\n```\n\n* Pass an iterable to iterator_over()\n\t\n```python\nfrom notalib.hypertext import TablePrinter\nt = TablePrinter([\'a\', \'b\'])\nlist(t.iterator_over([ {\'a\': 11, \'b\': 22} ]))\n# [\'<table><thead><tr><th>a</th><th>b</th></tr></thead><tbody>\',\n#  \'<tr><td>11</td><td>22</td></tr>\\n\',\n#  \'</tbody></table>\']\n```\n\n#### notalib.polosa.polosa :fire: :fire: :fire: :fire: :fire:\n\n```\n18023/2000000   294.8/sec   Processing transaction ID#84378473 (2020-01-04)\n```\n\nThe CLI progress indicator you\'ve always dreamt of: shows current and total if available, measures current speed, can show your comments for each element, makes sure not to slow down your terminal with frequent updates. [See this short demo](https://asciinema.org/a/UI1aOqjQC1KXx303kaVGrxjQp).\n\n_Cheat sheet_\n\n```python\n## Basic usage\nwith polosa() as p:\n    p.tick()\n# 467344   201.2/sec\n\n## Specify total number of elements:\nwith polosa(total=1337) as p:\n# 26/1337   1.2/sec\n\n## Print something useful about every element:\np.tick(caption=my_order.time_created)\n# 1723910/2000000   319231.2/sec   2020-01-01 15:37:00\n```\n\n#### notalib.range.Range\n#### notalib.time.Timing :fire:\n\nMeasures time spent on executing your code. Killer feature: it can be used as a reusable context.\n\n```python\ntiming = Timing()\n...\nwith timing:\n    do_something()\n# That\'s it, do something with the measurement\nlog(f\'Operation took {timing.result} sec\')\n```\n\nIf you just want to print measurements into console, there\'s a shorthand:\n\n```python\ntiming = Timing(auto_print=True)\n...\nwith timing:\n    do_something()\n```\n\n#### notalib.trendsetter.Trendsetter :fire:\n\n#### notalib.git.get_current_commit\n\n_:warning: Experimental API. Subject to change. Don\'t use in production. You\'ve been warned._\n\nReturns short description and hash of last commit of current branch.\nIf function is called outside git repo or there are no commits in the history, `None` will be returned.\n\n```python\nfrom notalib.git import get_current_commit\n\ncommit = get_current_commit()\n# Commit(hash=\'db0e5c1de83f233abef823fd92490727f4ee9d50\', short_description=\'Add timedelta module with convert_timedelta function\')\n```\n#### notalib.git.get_last_tag\n\n_:warning: Experimental API. Subject to change. Don\'t use in production. You\'ve been warned._\n\nReturns last tag label and hash. If function is called outside git repo or there are no tags in the history, `None` will be returned.\n\n```python\nfrom notalib.git import get_last_tag\n\ntag = get_last_tag()\n# Tag(hash=\'c4b6e06f57ab4773e2881d286804d4e3141b5195\', label=\'v1.4.0\')\n```\n\n## Pandas-related\n\n#### notalib.pandas.pandasplus.row_to_dict\n#### notalib.pandas.pandasplus.replace_null_objects\n\nReplaces all types of null values in a DataFrame with the given value.\n\n```python\ndf = pd.DataFrame({\'A\': [pd.NA, pd.NaT, \'SomeVal\', None]})\nnew_df = replace_null_objects(df, "Hello, notalib!")\nnew_df\n#                  A\n# 0  Hello, notalib!\n# 1  Hello, notalib!\n# 2          SomeVal\n# 3  Hello, notalib!\n```\n\n## Django-related\n\n#### notalib.django.auth.StaticBackend\n#### notalib.django.auth.SettingsBackend\n\n#### notalib.django.xauth\n\nEndpoints for easier authentication in APIs. Requires Django REST framework.\n\nProvides endpoints:\n\n* `/xauth/check` — returns code 200 if client is authenticated (or global permissions are set to AllowAny), 403 if not\n* `/xauth/auth-post` — authenticates a client; accepts two POST parameters `username` and `password`; returns code 200 on success and 403 on failure\n\nHow to use:\n\n1. Make sure Django REST framework is installed.\n2. Add `\'notalib.django_xauth\'` to INSTALLED_APPS.\n3. Run `manage.py migrate django_xauth` (doesn\'t actually change your DB).\n4. Add something like this to your urls.py: `path(\'xauth/\', include(\'notalib.django_xauth.urls\')),`\n\n#### notalib.django.colorlog.ColorFormatter\n#### notalib.django.filterset :fire:\n#### notalib.django.formplus.MonthField\n#### notalib.django.formplus.ChoiceWithDefault\n#### notalib.django.formplus.IntegerArrayField\n#### notalib.django.formplus.StringArrayField\n#### notalib.django.formplus.MonthArrayField\n#### notalib.django.request_time_middleware.RequestTimeLoggingMiddleware\n#### notalib.django.stream.stream_json\n\nStream all elements of iterable object as JSON array using the StreamingHttpResponse class. Unlike DRF\'s Response class, it can handle arrays of any size.\n\n```python\nclass SomeViewSet(...):\n    ...\n    \n    def list(self, request, *args, **kwargs):\n        ...\n        return stream_json(data)\n```\n\n## Django/Clickhouse\n\n_Stage: alpha_\n\nRequired packages: `clickhouse-sqlalchemy`\n\nRequired two django.settings variables:\n\n* **CLICKHOUSE_URL** — database URL\n* **CLICKHOUSE_PROFILE** — dump all queries and their timing to console, true/false\n\n#### notalib.django.clickhouse.base.get_connection\n#### notalib.django.clickhouse.base.get_database_name\n#### notalib.django.clickhouse.base.Query\n\nA wrapper for SQLAlchemy\'s `select` with some useful postprocessing options.\n\n* `execute` — no postprocessing\n* `execute_val` — returns single value\n* `execute_list` — returns single column as list\n* `execute_kv` — returns dict, first column becomes keys, second column becomes values\n* `execute_na` — returns number of affected rows\n\nUsage example:\n\n```python\nq = Query(\n    select([ SomeTable.c.notalib ])\n)\nq.execute_list()\n# ["Example", "OOOOO", "my", "defence", ...]\n```\n\n#### notalib.django.clickhouse.mutations.get_mutations_in_progress_count\n\nReturns the number of mutations in progress for the specified table.\n\n```python\nget_mutations_in_progress_count("SOME_DATABASE", "SOME_TABLE_IN_DATABASE")\n# 5\n```\n\n#### notalib.django.clickhouse.wait.wait_result :fire:\n\nWaits until all mutations for the given table are complete.\n\n```python\n# blah blah blah, ALTER TABLE ... UPDATE ...\nwait_result("SOME_DATABASE", "SOME_TABLE_IN_DATABASE")\n# UPDATE complete, continue\n```\n',
     'author': 'm1kc (Max Musatov)',
     'author_email': 'm1kc@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/m1kc/notalib',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `notalib-2.0.0/PKG-INFO` & `notalib-2.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,48 @@
-Metadata-Version: 2.1
-Name: notalib
-Version: 2.0.0
-Summary: A collection of utility functions & classes
-Home-page: https://github.com/m1kc/notalib
-License: MIT
-Keywords: utility,django,pandas
-Author: m1kc (Max Musatov)
-Author-email: m1kc@yandex.ru
-Requires-Python: >=3.7.3,<4.0.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: arrow (>=0.14.0,<2.0.0)
-Project-URL: Documentation, https://github.com/m1kc/notalib
-Project-URL: Repository, https://github.com/m1kc/notalib.git
-Description-Content-Type: text/markdown
-
 # notalib [![Django CI](https://github.com/m1kc/notalib/actions/workflows/django.yml/badge.svg)](https://github.com/m1kc/notalib/actions/workflows/django.yml) [![Coverage Status](https://coveralls.io/repos/github/m1kc/notalib/badge.svg?branch=master)](https://coveralls.io/github/m1kc/notalib?branch=master)
 
 Collection of small Python utility functions and classes. Each one was created because I needed it and it didn't exist or I didn't like the existing implementations. 100% of code is used in real-world projects.
 
 (And one day, the documentation is going to be actually good. In the meanwhile, don't hesitate to ask if something's not clear.)
 
+
 ## Install
 
 ```sh
 pip install notalib
 ```
 
 Or with [poetry](https://python-poetry.org/):
 
 ```sh
 poetry add notalib
 ```
 
+
+## Compatibility promise
+
+Version numbers follow the semver rules. Minor releases are backwards-compatible. It should be safe to update, say, from 1.2 to 1.4.
+
+Major releases are not backwards-compatible. If you upgrade, say, from 1.4 to 2.0, read the release notes to see what's changed.
+
+
 ## Maintenance & bugfixes
 
 While I try to fix bugs, add new features, and review any PRs when I have time, there're no promises and no set timeframes, even if a bug is critical. That's a project I do in my free time, free of charge.
 
 If that's not enough for you or you have an urgent request, there are paid maintenance options (bugfixing, features, expedite PR review, 24h security responses). Contact me for prices: m1kc@yandex.ru
 
 Also feel free to just send me money:
 
 * MasterCard: 5559 4925 7484 0297
 * PayPal: [paypal.me/thisism1kc](https://paypal.me/thisism1kc)
 
 Donations are always appreciated, even if you send 10$.
 
+
 ## Constants included
 
 * `notalib.utf.BOM`: contains string `b'\xEF\xBB\xBF'` (UTF-8 little endian byte order mark).
 
 ## Utils included
 
 #### notalib.array.as_chunks :fire:
@@ -121,14 +109,28 @@
 get_week(date2, WeekNumbering.NORMAL)
 # Week(week=52, year=2022)
 
 get_week(date2, WeekNumbering.MATCH_YEAR)
 # Week(week=0, year=2023)
 ```
 
+#### notalib.dict.deep_merge
+
+_:warning: Experimental API. Subject to change. Don't use in production. You've been warned._
+
+Merges two dicts.
+
+Modifies input. Use `copy.deepcopy` to create a deep copy of the original dictionary if you need it.
+
+Accepts three arguments:
+
+* original dict (also target)
+* second dict
+* overwrite=True if you want to overwrite matching paths, overwrite=False to raise an exception on path conflicts (default)
+
 #### notalib.dict.find_field
 #### notalib.dict.find_value
 #### notalib.dict.normalize_dict :fire:
 #### notalib.dict.filter_dict
 
 Filters a dictionary, removing any keys except for the ones you choose.
 
@@ -143,14 +145,33 @@
 filter_dict(src, ["Some", "once"])
 # {'Some': 'BODY', 'once': 'told me'}
 filter_dict(src, [])
 # {}
 ```
 
 #### notalib.format.format_long_list
+#### notalib.timedelta.convert_timedelta
+
+_:warning: Experimental API. Subject to change. Don't use in production. You've been warned._
+
+Converts standard timedelta object to specified formats.
+
+Allowed formats: 's', 'ms'.
+
+```python
+from notalib.timedelta import convert_timedelta
+from datetime import timedelta
+
+td = timedelta(seconds=1, milliseconds=23)
+convert_timedelta(td, 's')
+# 1.023
+convert_timedelta(td, 'ms')
+# 1023
+```
+
 #### notalib.hypertext.strip_tags :fire:
 #### notalib.hypertext.TablePrinter :fire:
 
 Prints an HTML table, row by row, from the given data, using attrs or dictionary keys as columns.
 
 Two ways to use it:
 
@@ -226,14 +247,40 @@
 ...
 with timing:
     do_something()
 ```
 
 #### notalib.trendsetter.Trendsetter :fire:
 
+#### notalib.git.get_current_commit
+
+_:warning: Experimental API. Subject to change. Don't use in production. You've been warned._
+
+Returns short description and hash of last commit of current branch.
+If function is called outside git repo or there are no commits in the history, `None` will be returned.
+
+```python
+from notalib.git import get_current_commit
+
+commit = get_current_commit()
+# Commit(hash='db0e5c1de83f233abef823fd92490727f4ee9d50', short_description='Add timedelta module with convert_timedelta function')
+```
+#### notalib.git.get_last_tag
+
+_:warning: Experimental API. Subject to change. Don't use in production. You've been warned._
+
+Returns last tag label and hash. If function is called outside git repo or there are no tags in the history, `None` will be returned.
+
+```python
+from notalib.git import get_last_tag
+
+tag = get_last_tag()
+# Tag(hash='c4b6e06f57ab4773e2881d286804d4e3141b5195', label='v1.4.0')
+```
+
 ## Pandas-related
 
 #### notalib.pandas.pandasplus.row_to_dict
 #### notalib.pandas.pandasplus.replace_null_objects
 
 Replaces all types of null values in a DataFrame with the given value.
 
@@ -337,8 +384,7 @@
 Waits until all mutations for the given table are complete.
 
 ```python
 # blah blah blah, ALTER TABLE ... UPDATE ...
 wait_result("SOME_DATABASE", "SOME_TABLE_IN_DATABASE")
 # UPDATE complete, continue
 ```
-
```

