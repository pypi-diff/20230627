# Comparing `tmp/ambition-utils-3.1.2.tar.gz` & `tmp/ambition-utils-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambition-utils-3.1.2.tar", last modified: Tue Jun 27 20:59:20 2023, max compression
+gzip compressed data, was "ambition-utils-3.1.3.tar", last modified: Tue Jun 27 21:02:41 2023, max compression
```

## Comparing `ambition-utils-3.1.2.tar` & `ambition-utils-3.1.3.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/LICENSE
--rw-rw-r--   0 wes       (1000) wes       (1000)       68 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/MANIFEST.in
--rw-rw-r--   0 wes       (1000) wes       (1000)     1975 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1114 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/README.rst
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.006524 ambition-utils-3.1.2/ambition_utils/
--rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.006524 ambition-utils-3.1.2/ambition_utils/activity/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/activity/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.006524 ambition-utils-3.1.2/ambition_utils/activity/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     2231 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/activity/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1656 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/activity/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4446 2023-06-26 19:14:11.000000 ambition-utils-3.1.2/ambition_utils/activity/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2737 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/activity/tasks.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/activity/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/activity/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      229 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/activity/tests/model_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2794 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/activity/tests/task_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/anomaly/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/anomaly/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     9762 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/anomaly/models.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/anomaly/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/anomaly/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     6036 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/anomaly/tests/anomaly_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      202 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/anomaly/tests/apps.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/anomaly/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     2644 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/anomaly/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/anomaly/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      928 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/anomaly/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      138 2023-01-06 21:50:12.000000 ambition-utils-3.1.2/ambition_utils/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2059 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/fields.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    13636 2022-02-17 21:55:47.000000 ambition-utils-3.1.2/ambition_utils/forms.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/postgres_lock/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3782 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/lock.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/postgres_lock/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)      487 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      434 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      581 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      875 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/models.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/postgres_lock/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4399 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/postgres_lock/tests/lock_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/rrule/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/rrule/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      162 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/rrule/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      127 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/rrule/constants.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     9796 2023-06-26 21:32:04.000000 ambition-utils-3.1.2/ambition_utils/rrule/forms.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      389 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/rrule/handler.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.010524 ambition-utils-3.1.2/ambition_utils/rrule/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)      927 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/rrule/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      415 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      936 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      486 2023-06-26 21:32:04.000000 ambition-utils-3.1.2/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/rrule/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    18819 2023-06-27 20:55:38.000000 ambition-utils-3.1.2/ambition_utils/rrule/models.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/ambition_utils/rrule/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/rrule/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      200 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/rrule/tests/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    17567 2023-06-26 21:32:04.000000 ambition-utils-3.1.2/ambition_utils/rrule/tests/form_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/ambition_utils/rrule/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1005 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/rrule/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/rrule/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    56586 2023-06-26 21:32:04.000000 ambition-utils-3.1.2/ambition_utils/rrule/tests/model_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      713 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/rrule/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7349 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/sql.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/ambition_utils/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      190 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/tests/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2556 2023-06-26 21:33:07.000000 ambition-utils-3.1.2/ambition_utils/tests/field_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    16249 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/tests/form_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/ambition_utils/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)      489 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      685 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      364 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3144 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/tests/sql_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3435 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/tests/time_helper_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4765 2023-01-24 18:43:16.000000 ambition-utils-3.1.2/ambition_utils/time_helpers.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/ambition_utils/transaction/
--rw-rw-r--   0 wes       (1000) wes       (1000)       46 2022-02-17 21:55:47.000000 ambition-utils-3.1.2/ambition_utils/transaction/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2261 2022-02-17 21:55:47.000000 ambition-utils-3.1.2/ambition_utils/transaction/decorators.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/ambition_utils/transaction/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-17 21:55:47.000000 ambition-utils-3.1.2/ambition_utils/transaction/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2032 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/ambition_utils/transaction/tests/durable_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2666 2022-02-17 21:55:47.000000 ambition-utils-3.1.2/ambition_utils/transaction/utils.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/ambition_utils/urls.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-27 20:57:16.000000 ambition-utils-3.1.2/ambition_utils/version.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.006524 ambition-utils-3.1.2/ambition_utils.egg-info/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1975 2023-06-27 20:59:19.000000 ambition-utils-3.1.2/ambition_utils.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     3085 2023-06-27 20:59:20.000000 ambition-utils-3.1.2/ambition_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-27 20:59:19.000000 ambition-utils-3.1.2/ambition_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      262 2023-06-27 20:59:19.000000 ambition-utils-3.1.2/ambition_utils.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       15 2023-06-27 20:59:19.000000 ambition-utils-3.1.2/ambition_utils.egg-info/top_level.txt
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/requirements/
--rw-rw-r--   0 wes       (1000) wes       (1000)       31 2022-02-11 17:04:09.000000 ambition-utils-3.1.2/requirements/docs.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       96 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/requirements/requirements-testing.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      160 2023-06-26 21:33:07.000000 ambition-utils-3.1.2/requirements/requirements.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      252 2023-06-27 20:59:20.014524 ambition-utils-3.1.2/setup.cfg
--rw-rw-r--   0 wes       (1000) wes       (1000)     1914 2023-06-26 21:29:57.000000 ambition-utils-3.1.2/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.359197 ambition-utils-3.1.3/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       68 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1975 2023-06-27 21:02:41.359197 ambition-utils-3.1.3/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1114 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.351197 ambition-utils-3.1.3/ambition_utils/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/activity/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/activity/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/activity/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2231 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/activity/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1656 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/activity/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4446 2023-06-26 19:14:11.000000 ambition-utils-3.1.3/ambition_utils/activity/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2737 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/activity/tasks.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/activity/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/activity/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      229 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/activity/tests/model_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2794 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/activity/tests/task_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/anomaly/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/anomaly/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     9762 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/anomaly/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/anomaly/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/anomaly/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6036 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/anomaly/tests/anomaly_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      202 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/anomaly/tests/apps.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/anomaly/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2644 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/anomaly/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/anomaly/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      928 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/anomaly/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      138 2023-01-06 21:50:12.000000 ambition-utils-3.1.3/ambition_utils/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2059 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/fields.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    13636 2022-02-17 21:55:47.000000 ambition-utils-3.1.3/ambition_utils/forms.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/postgres_lock/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3782 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/lock.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/postgres_lock/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      487 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      434 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      581 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      875 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/postgres_lock/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4399 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/postgres_lock/tests/lock_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/rrule/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/rrule/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      162 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/rrule/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      127 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/rrule/constants.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     9796 2023-06-26 21:32:04.000000 ambition-utils-3.1.3/ambition_utils/rrule/forms.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      389 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/rrule/handler.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/rrule/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      927 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/rrule/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      415 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      936 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      486 2023-06-26 21:32:04.000000 ambition-utils-3.1.3/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/rrule/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    18825 2023-06-27 21:01:00.000000 ambition-utils-3.1.3/ambition_utils/rrule/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/rrule/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/rrule/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      200 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/rrule/tests/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    17567 2023-06-26 21:32:04.000000 ambition-utils-3.1.3/ambition_utils/rrule/tests/form_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/rrule/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1005 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/rrule/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/rrule/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    56586 2023-06-26 21:32:04.000000 ambition-utils-3.1.3/ambition_utils/rrule/tests/model_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      713 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/rrule/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7349 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/sql.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.355197 ambition-utils-3.1.3/ambition_utils/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      190 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/tests/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2556 2023-06-26 21:33:07.000000 ambition-utils-3.1.3/ambition_utils/tests/field_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    16249 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/tests/form_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.359197 ambition-utils-3.1.3/ambition_utils/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      489 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      685 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      364 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3144 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/tests/sql_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3435 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/tests/time_helper_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4765 2023-01-24 18:43:16.000000 ambition-utils-3.1.3/ambition_utils/time_helpers.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.359197 ambition-utils-3.1.3/ambition_utils/transaction/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       46 2022-02-17 21:55:47.000000 ambition-utils-3.1.3/ambition_utils/transaction/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2261 2022-02-17 21:55:47.000000 ambition-utils-3.1.3/ambition_utils/transaction/decorators.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.359197 ambition-utils-3.1.3/ambition_utils/transaction/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-17 21:55:47.000000 ambition-utils-3.1.3/ambition_utils/transaction/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2032 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/ambition_utils/transaction/tests/durable_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2666 2022-02-17 21:55:47.000000 ambition-utils-3.1.3/ambition_utils/transaction/utils.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/ambition_utils/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-27 21:00:35.000000 ambition-utils-3.1.3/ambition_utils/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.351197 ambition-utils-3.1.3/ambition_utils.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1975 2023-06-27 21:02:41.000000 ambition-utils-3.1.3/ambition_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3085 2023-06-27 21:02:41.000000 ambition-utils-3.1.3/ambition_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-27 21:02:41.000000 ambition-utils-3.1.3/ambition_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      262 2023-06-27 21:02:41.000000 ambition-utils-3.1.3/ambition_utils.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       15 2023-06-27 21:02:41.000000 ambition-utils-3.1.3/ambition_utils.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 21:02:41.359197 ambition-utils-3.1.3/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2022-02-11 17:04:09.000000 ambition-utils-3.1.3/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       96 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      160 2023-06-26 21:33:07.000000 ambition-utils-3.1.3/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      252 2023-06-27 21:02:41.359197 ambition-utils-3.1.3/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1914 2023-06-26 21:29:57.000000 ambition-utils-3.1.3/setup.py
```

### Comparing `ambition-utils-3.1.2/LICENSE` & `ambition-utils-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/PKG-INFO` & `ambition-utils-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.2
+Version: 3.1.3
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Keywords: django,database,query,sql,postgres,upsert
 Classifier: Programming Language :: Python
```

### Comparing `ambition-utils-3.1.2/README.rst` & `ambition-utils-3.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/activity/migrations/0001_initial.py` & `ambition-utils-3.1.3/ambition_utils/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/activity/migrations/0002_auto_20180427_1819.py` & `ambition-utils-3.1.3/ambition_utils/activity/migrations/0002_auto_20180427_1819.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/activity/models.py` & `ambition-utils-3.1.3/ambition_utils/activity/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/activity/tasks.py` & `ambition-utils-3.1.3/ambition_utils/activity/tasks.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/activity/tests/task_tests.py` & `ambition-utils-3.1.3/ambition_utils/activity/tests/task_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/anomaly/models.py` & `ambition-utils-3.1.3/ambition_utils/anomaly/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/anomaly/tests/anomaly_tests.py` & `ambition-utils-3.1.3/ambition_utils/anomaly/tests/anomaly_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/anomaly/tests/migrations/0001_initial.py` & `ambition-utils-3.1.3/ambition_utils/anomaly/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/anomaly/tests/models.py` & `ambition-utils-3.1.3/ambition_utils/anomaly/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/fields.py` & `ambition-utils-3.1.3/ambition_utils/fields.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/forms.py` & `ambition-utils-3.1.3/ambition_utils/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/postgres_lock/lock.py` & `ambition-utils-3.1.3/ambition_utils/postgres_lock/lock.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py` & `ambition-utils-3.1.3/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/postgres_lock/models.py` & `ambition-utils-3.1.3/ambition_utils/postgres_lock/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/postgres_lock/tests/lock_tests.py` & `ambition-utils-3.1.3/ambition_utils/postgres_lock/tests/lock_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/rrule/forms.py` & `ambition-utils-3.1.3/ambition_utils/rrule/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/rrule/migrations/0001_initial.py` & `ambition-utils-3.1.3/ambition_utils/rrule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py` & `ambition-utils-3.1.3/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/rrule/models.py` & `ambition-utils-3.1.3/ambition_utils/rrule/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dateutil.rrule import rrule, rruleset
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.db import models, transaction
 from django.utils.module_loading import import_string
 from fleming import fleming
 from manager_utils import bulk_update
-from ambition.fields import TimeZoneField
+from ambition_utils.fields import TimeZoneField
 from typing import List
 import copy
 import pytz
 import logging
 
 LOG = logging.getLogger(__name__)
```

### Comparing `ambition-utils-3.1.2/ambition_utils/rrule/tests/form_tests.py` & `ambition-utils-3.1.3/ambition_utils/rrule/tests/form_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/rrule/tests/migrations/0001_initial.py` & `ambition-utils-3.1.3/ambition_utils/rrule/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/rrule/tests/model_tests.py` & `ambition-utils-3.1.3/ambition_utils/rrule/tests/model_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/rrule/tests/models.py` & `ambition-utils-3.1.3/ambition_utils/rrule/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/sql.py` & `ambition-utils-3.1.3/ambition_utils/sql.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/tests/field_tests.py` & `ambition-utils-3.1.3/ambition_utils/tests/field_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/tests/form_tests.py` & `ambition-utils-3.1.3/ambition_utils/tests/form_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/tests/migrations/0002_auto_20230124_1754.py` & `ambition-utils-3.1.3/ambition_utils/tests/migrations/0002_auto_20230124_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/tests/sql_tests.py` & `ambition-utils-3.1.3/ambition_utils/tests/sql_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/tests/time_helper_tests.py` & `ambition-utils-3.1.3/ambition_utils/tests/time_helper_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/time_helpers.py` & `ambition-utils-3.1.3/ambition_utils/time_helpers.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/transaction/decorators.py` & `ambition-utils-3.1.3/ambition_utils/transaction/decorators.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/transaction/tests/durable_tests.py` & `ambition-utils-3.1.3/ambition_utils/transaction/tests/durable_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils/transaction/utils.py` & `ambition-utils-3.1.3/ambition_utils/transaction/utils.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/ambition_utils.egg-info/PKG-INFO` & `ambition-utils-3.1.3/ambition_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.2
+Version: 3.1.3
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Keywords: django,database,query,sql,postgres,upsert
 Classifier: Programming Language :: Python
```

### Comparing `ambition-utils-3.1.2/ambition_utils.egg-info/SOURCES.txt` & `ambition-utils-3.1.3/ambition_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.2/setup.py` & `ambition-utils-3.1.3/setup.py`

 * *Files identical despite different names*

