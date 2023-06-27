# Comparing `tmp/ambition-utils-3.1.0.tar.gz` & `tmp/ambition-utils-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ambition-utils-3.1.0.tar", last modified: Wed Mar 15 19:41:35 2023, max compression
+gzip compressed data, was "ambition-utils-3.1.1.tar", last modified: Tue Jun 27 19:04:41 2023, max compression
```

## Comparing `ambition-utils-3.1.0.tar` & `ambition-utils-3.1.1.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils.egg-info/
--rw-r--r--   0 jared     (1000) jared     (1000)     3016 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        1 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       15 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/top_level.txt
--rw-r--r--   0 jared     (1000) jared     (1000)     2390 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)      287 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/requires.txt
--rw-r--r--   0 jared     (1000) jared     (1000)     1075 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/LICENSE
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/tests/
--rw-rw-r--   0 jared     (1000) jared     (1000)     3144 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/sql_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)    16240 2020-05-08 15:58:44.000000 ambition-utils-3.1.0/ambition_utils/tests/form_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     3435 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/time_helper_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      190 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/apps.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      364 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/tests/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)      685 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/migrations/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      489 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       74 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2556 2023-03-15 19:41:28.000000 ambition-utils-3.1.0/ambition_utils/tests/field_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)    13636 2021-03-10 18:52:40.000000 ambition-utils-3.1.0/ambition_utils/forms.py
--rw-r--r--   0 jared     (1000) jared     (1000)     7349 2020-05-08 15:58:44.000000 ambition-utils-3.1.0/ambition_utils/sql.py
--rw-r--r--   0 jared     (1000) jared     (1000)      138 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/apps.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/tests/
--rw-r--r--   0 jared     (1000) jared     (1000)     4399 2022-05-25 19:46:46.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/tests/lock_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/tests/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     3782 2022-05-25 18:18:33.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/lock.py
--rw-r--r--   0 jared     (1000) jared     (1000)      875 2022-05-25 17:51:38.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/
--rw-r--r--   0 jared     (1000) jared     (1000)      581 2022-05-25 17:54:45.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
--rw-r--r--   0 jared     (1000) jared     (1000)      434 2020-05-08 15:58:44.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      487 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/0001_initial.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2059 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/fields.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/transaction/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/transaction/tests/
--rw-r--r--   0 jared     (1000) jared     (1000)     2023 2021-03-11 16:47:27.000000 ambition-utils-3.1.0/ambition_utils/transaction/tests/durable_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2021-03-10 18:52:40.000000 ambition-utils-3.1.0/ambition_utils/transaction/tests/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2261 2021-03-10 18:52:40.000000 ambition-utils-3.1.0/ambition_utils/transaction/decorators.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2666 2021-03-11 15:49:49.000000 ambition-utils-3.1.0/ambition_utils/transaction/utils.py
--rw-r--r--   0 jared     (1000) jared     (1000)       46 2021-03-10 18:52:40.000000 ambition-utils-3.1.0/ambition_utils/transaction/__init__.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/anomaly/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/
--rw-rw-r--   0 jared     (1000) jared     (1000)      202 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/apps.py
--rw-r--r--   0 jared     (1000) jared     (1000)      928 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/models.py
--rw-r--r--   0 jared     (1000) jared     (1000)     6036 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/anomaly_tests.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/migrations/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2748 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       76 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     9808 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/anomaly/models.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/anomaly/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)       38 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/urls.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       22 2023-03-15 19:41:28.000000 ambition-utils-3.1.0/ambition_utils/version.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/rrule/
--rw-r--r--   0 jared     (1000) jared     (1000)      389 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/rrule/handler.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/
--rw-rw-r--   0 jared     (1000) jared     (1000)    16189 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/form_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      200 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/apps.py
--rw-rw-r--   0 jared     (1000) jared     (1000)    54228 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/model_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      713 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/migrations/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     1005 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       72 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     8681 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/forms.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      162 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/apps.py
--rw-r--r--   0 jared     (1000) jared     (1000)      127 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/rrule/constants.py
--rw-rw-r--   0 jared     (1000) jared     (1000)    16920 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)      936 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
--rw-r--r--   0 jared     (1000) jared     (1000)      415 2020-05-08 15:58:44.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1071 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       61 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      112 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/__init__.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/activity/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/activity/tests/
--rw-r--r--   0 jared     (1000) jared     (1000)     2785 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/tests/task_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)      229 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/tests/model_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/tests/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     4446 2023-03-15 18:34:46.000000 ambition-utils-3.1.0/ambition_utils/activity/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/activity/migrations/
--rw-r--r--   0 jared     (1000) jared     (1000)     1696 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/migrations/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2271 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/migrations/0001_initial.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2799 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/tasks.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     4765 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/time_helpers.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/requirements/
--rw-rw-r--   0 jared     (1000) jared     (1000)      113 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/requirements/requirements-testing.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)      168 2023-03-15 19:41:28.000000 ambition-utils-3.1.0/requirements/requirements.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       31 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/requirements/docs.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)     1990 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/setup.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      252 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/setup.cfg
--rw-r--r--   0 jared     (1000) jared     (1000)     1114 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/README.rst
--rw-r--r--   0 jared     (1000) jared     (1000)       68 2018-12-06 16:50:17.000000 ambition-utils-3.1.0/MANIFEST.in
--rw-rw-r--   0 jared     (1000) jared     (1000)     2390 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/PKG-INFO
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.318690 ambition-utils-3.1.1/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       68 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1975 2023-06-27 19:04:41.318690 ambition-utils-3.1.1/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1114 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.306691 ambition-utils-3.1.1/ambition_utils/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.310690 ambition-utils-3.1.1/ambition_utils/activity/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/activity/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.310690 ambition-utils-3.1.1/ambition_utils/activity/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2231 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/activity/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1656 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/activity/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4446 2023-06-26 19:14:11.000000 ambition-utils-3.1.1/ambition_utils/activity/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2737 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/activity/tasks.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.310690 ambition-utils-3.1.1/ambition_utils/activity/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/activity/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      229 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/activity/tests/model_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2794 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/activity/tests/task_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.310690 ambition-utils-3.1.1/ambition_utils/anomaly/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/anomaly/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     9762 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/anomaly/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.310690 ambition-utils-3.1.1/ambition_utils/anomaly/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/anomaly/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6036 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/anomaly/tests/anomaly_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      202 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/anomaly/tests/apps.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.310690 ambition-utils-3.1.1/ambition_utils/anomaly/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2644 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/anomaly/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/anomaly/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      928 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/anomaly/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      138 2023-01-06 21:50:12.000000 ambition-utils-3.1.1/ambition_utils/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2059 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/fields.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    13636 2022-02-17 21:55:47.000000 ambition-utils-3.1.1/ambition_utils/forms.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.310690 ambition-utils-3.1.1/ambition_utils/postgres_lock/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3782 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/lock.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.314690 ambition-utils-3.1.1/ambition_utils/postgres_lock/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      487 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      434 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      581 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      875 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.314690 ambition-utils-3.1.1/ambition_utils/postgres_lock/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4399 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/postgres_lock/tests/lock_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.314690 ambition-utils-3.1.1/ambition_utils/rrule/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/rrule/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      162 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/rrule/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      127 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/rrule/constants.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     9796 2023-06-26 21:32:04.000000 ambition-utils-3.1.1/ambition_utils/rrule/forms.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      389 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/rrule/handler.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.314690 ambition-utils-3.1.1/ambition_utils/rrule/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      927 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/rrule/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      415 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      936 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      486 2023-06-26 21:32:04.000000 ambition-utils-3.1.1/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/rrule/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    18818 2023-06-26 21:54:12.000000 ambition-utils-3.1.1/ambition_utils/rrule/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.314690 ambition-utils-3.1.1/ambition_utils/rrule/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/rrule/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      200 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/rrule/tests/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    17567 2023-06-26 21:32:04.000000 ambition-utils-3.1.1/ambition_utils/rrule/tests/form_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.314690 ambition-utils-3.1.1/ambition_utils/rrule/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1005 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/rrule/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/rrule/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    56586 2023-06-26 21:32:04.000000 ambition-utils-3.1.1/ambition_utils/rrule/tests/model_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      713 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/rrule/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7349 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/sql.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.318690 ambition-utils-3.1.1/ambition_utils/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      190 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/tests/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2556 2023-06-26 21:33:07.000000 ambition-utils-3.1.1/ambition_utils/tests/field_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    16249 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/tests/form_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.318690 ambition-utils-3.1.1/ambition_utils/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      489 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      685 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      364 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3144 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/tests/sql_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3435 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/tests/time_helper_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4765 2023-01-24 18:43:16.000000 ambition-utils-3.1.1/ambition_utils/time_helpers.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.318690 ambition-utils-3.1.1/ambition_utils/transaction/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       46 2022-02-17 21:55:47.000000 ambition-utils-3.1.1/ambition_utils/transaction/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2261 2022-02-17 21:55:47.000000 ambition-utils-3.1.1/ambition_utils/transaction/decorators.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.318690 ambition-utils-3.1.1/ambition_utils/transaction/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-17 21:55:47.000000 ambition-utils-3.1.1/ambition_utils/transaction/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2032 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/ambition_utils/transaction/tests/durable_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2666 2022-02-17 21:55:47.000000 ambition-utils-3.1.1/ambition_utils/transaction/utils.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/ambition_utils/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-26 21:32:17.000000 ambition-utils-3.1.1/ambition_utils/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.310690 ambition-utils-3.1.1/ambition_utils.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1975 2023-06-27 19:04:41.000000 ambition-utils-3.1.1/ambition_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3085 2023-06-27 19:04:41.000000 ambition-utils-3.1.1/ambition_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-27 19:04:41.000000 ambition-utils-3.1.1/ambition_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      262 2023-06-27 19:04:41.000000 ambition-utils-3.1.1/ambition_utils.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       15 2023-06-27 19:04:41.000000 ambition-utils-3.1.1/ambition_utils.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 19:04:41.318690 ambition-utils-3.1.1/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2022-02-11 17:04:09.000000 ambition-utils-3.1.1/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       96 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      160 2023-06-26 21:33:07.000000 ambition-utils-3.1.1/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      252 2023-06-27 19:04:41.318690 ambition-utils-3.1.1/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1914 2023-06-26 21:29:57.000000 ambition-utils-3.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ambition-utils-3.1.0/ambition_utils.egg-info/SOURCES.txt` & `ambition-utils-3.1.1/ambition_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 ambition_utils/rrule/constants.py
 ambition_utils/rrule/forms.py
 ambition_utils/rrule/handler.py
 ambition_utils/rrule/models.py
 ambition_utils/rrule/migrations/0001_initial.py
 ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
 ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
+ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
 ambition_utils/rrule/migrations/__init__.py
 ambition_utils/rrule/tests/__init__.py
 ambition_utils/rrule/tests/apps.py
 ambition_utils/rrule/tests/form_tests.py
 ambition_utils/rrule/tests/model_tests.py
 ambition_utils/rrule/tests/models.py
 ambition_utils/rrule/tests/migrations/0001_initial.py
```

### Comparing `ambition-utils-3.1.0/ambition_utils.egg-info/PKG-INFO` & `ambition-utils-3.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.0
+Version: 3.1.1
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/ambition-utils.png
-           :target: https://travis-ci.org/ambitioninc/ambition-utils
-        
-        .. image:: https://coveralls.io/repos/ambitioninc/ambition-utils/badge.png?branch=develop
-            :target: https://coveralls.io/r/ambitioninc/ambition-utils?branch=develop
-        
-        .. image:: https://pypip.in/v/ambition-utils/badge.png
-            :target: https://crate.io/packages/ambition-utils/
-            :alt: Latest PyPI version
-        
-        .. image:: https://pypip.in/d/ambition-utils/badge.png
-            :target: https://crate.io/packages/ambition-utils/
-        
-        
-        Requirements
-        ------------
-        * Python 3.6+
-        * Django 1.11+
-        * Postgres 9.5+
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install ambition-utils
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/ambition-utils.git
-        
-        Documentation
-        -------------
-        
-        Note: As of version 0.5.0, this project only supports Python3.6+
-        If you need Python2 support, pin to `ambition-utils==0.4.0`
-        
-        Full documentation is available at http://ambition-utils.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-        
 Keywords: django,database,query,sql,postgres,upsert
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Provides-Extra: dev
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/ambition-utils.png
+   :target: https://travis-ci.org/ambitioninc/ambition-utils
+
+.. image:: https://coveralls.io/repos/ambitioninc/ambition-utils/badge.png?branch=develop
+    :target: https://coveralls.io/r/ambitioninc/ambition-utils?branch=develop
+
+.. image:: https://pypip.in/v/ambition-utils/badge.png
+    :target: https://crate.io/packages/ambition-utils/
+    :alt: Latest PyPI version
+
+.. image:: https://pypip.in/d/ambition-utils/badge.png
+    :target: https://crate.io/packages/ambition-utils/
+
+
+Requirements
+------------
+* Python 3.6+
+* Django 1.11+
+* Postgres 9.5+
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install ambition-utils
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/ambition-utils.git
+
+Documentation
+-------------
+
+Note: As of version 0.5.0, this project only supports Python3.6+
+If you need Python2 support, pin to `ambition-utils==0.4.0`
+
+Full documentation is available at http://ambition-utils.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `ambition-utils-3.1.0/LICENSE` & `ambition-utils-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/tests/sql_tests.py` & `ambition-utils-3.1.1/ambition_utils/tests/sql_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/tests/form_tests.py` & `ambition-utils-3.1.1/ambition_utils/tests/form_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django import forms
 from django.core.exceptions import ValidationError
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.test import TestCase
-from mock import MagicMock
+from unittest.mock import MagicMock
 
 from ambition_utils.forms import NestedFormMixin, NestedFormConfig
 from ambition_utils.tests.models import FakeModel
 
 
 class BadFormNoSave(NestedFormMixin, forms.Form):
     pass
```

### Comparing `ambition-utils-3.1.0/ambition_utils/tests/time_helper_tests.py` & `ambition-utils-3.1.1/ambition_utils/tests/time_helper_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/tests/migrations/0002_auto_20230124_1754.py` & `ambition-utils-3.1.1/ambition_utils/tests/migrations/0002_auto_20230124_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/tests/field_tests.py` & `ambition-utils-3.1.1/ambition_utils/tests/field_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/forms.py` & `ambition-utils-3.1.1/ambition_utils/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/sql.py` & `ambition-utils-3.1.1/ambition_utils/sql.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/postgres_lock/tests/lock_tests.py` & `ambition-utils-3.1.1/ambition_utils/postgres_lock/tests/lock_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/postgres_lock/lock.py` & `ambition-utils-3.1.1/ambition_utils/postgres_lock/lock.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/postgres_lock/models.py` & `ambition-utils-3.1.1/ambition_utils/postgres_lock/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py` & `ambition-utils-3.1.1/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/fields.py` & `ambition-utils-3.1.1/ambition_utils/fields.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/transaction/tests/durable_tests.py` & `ambition-utils-3.1.1/ambition_utils/transaction/tests/durable_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import transaction, utils
 from django.test.testcases import TestCase
-from mock import patch
+from unittest.mock import patch
 
 from ambition_utils.transaction import durable
 from ambition_utils.transaction import decorators
 from ambition_utils.transaction.utils import DurableResetAtomicForTestingPatcher
 
 
 class DurableTests(TestCase):
```

### Comparing `ambition-utils-3.1.0/ambition_utils/transaction/decorators.py` & `ambition-utils-3.1.1/ambition_utils/transaction/decorators.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/transaction/utils.py` & `ambition-utils-3.1.1/ambition_utils/transaction/utils.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/anomaly/tests/models.py` & `ambition-utils-3.1.1/ambition_utils/anomaly/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/anomaly/tests/anomaly_tests.py` & `ambition-utils-3.1.1/ambition_utils/anomaly/tests/anomaly_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/anomaly/tests/migrations/0001_initial.py` & `ambition-utils-3.1.1/ambition_utils/anomaly/tests/migrations/0001_initial.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Generated by Django 2.2.28 on 2023-01-06 21:15
 
-import django.contrib.postgres.fields.jsonb
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
@@ -20,15 +19,15 @@
             ],
         ),
         migrations.CreateModel(
             name='IncrementalAnomaly',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('uid', models.CharField(max_length=256, unique=True)),
-                ('blob', django.contrib.postgres.fields.jsonb.JSONField(default=dict, null=True)),
+                ('blob', models.JSONField(default=dict, null=True)),
                 ('percentile_low', models.FloatField(null=True)),
                 ('percentile_high', models.FloatField(null=True)),
                 ('delta', models.FloatField(default=0.01, null=True)),
                 ('K', models.FloatField(default=25, null=True)),
                 ('threshold_low', models.FloatField(db_index=True, null=True)),
                 ('threshold_high', models.FloatField(db_index=True, null=True)),
                 ('num_values_ingested', models.IntegerField(default=0)),
@@ -40,15 +39,15 @@
             },
         ),
         migrations.CreateModel(
             name='NonIncrementalAnomaly',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('uid', models.CharField(max_length=256, unique=True)),
-                ('blob', django.contrib.postgres.fields.jsonb.JSONField(default=dict, null=True)),
+                ('blob', models.JSONField(default=dict, null=True)),
                 ('percentile_low', models.FloatField(null=True)),
                 ('percentile_high', models.FloatField(null=True)),
                 ('delta', models.FloatField(default=0.01, null=True)),
                 ('K', models.FloatField(default=25, null=True)),
                 ('threshold_low', models.FloatField(db_index=True, null=True)),
                 ('threshold_high', models.FloatField(db_index=True, null=True)),
                 ('num_values_ingested', models.IntegerField(default=0)),
```

### Comparing `ambition-utils-3.1.0/ambition_utils/anomaly/models.py` & `ambition-utils-3.1.1/ambition_utils/anomaly/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import datetime
 import sys
 from numbers import Number
 from typing import Union, Iterable, List
 
 
 from django.db import models
-from django.contrib.postgres.fields import JSONField
 from django.utils.functional import cached_property
 import fleming
 from tdigest import TDigest
 
 from manager_utils import ManagerUtilsManager, ManagerUtilsQuerySet
 
 
@@ -63,15 +62,15 @@
     class Meta:
         abstract = True
 
     # unique id to identify this anomaly detector
     uid = models.CharField(max_length=256, unique=True)
 
     # JSON blob to persist the state of the tdigest
-    blob = JSONField(default=dict, null=True)
+    blob = models.JSONField(default=dict, null=True)
 
     # User defined percentiles below and above which an anomaly will happen
     percentile_low = models.FloatField(null=True)
     percentile_high = models.FloatField(null=True)
 
     # These configure the accuracy/space tradeoff for the t-digest state
     delta = models.FloatField(default=.01, null=True)
```

### Comparing `ambition-utils-3.1.0/ambition_utils/rrule/tests/form_tests.py` & `ambition-utils-3.1.1/ambition_utils/rrule/tests/form_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import json
 
 from dateutil import rrule
 from django.test import TestCase
 from freezegun import freeze_time
 
 from ambition_utils.rrule.constants import RecurrenceEnds
 from ambition_utils.rrule.forms import RecurrenceForm
@@ -113,14 +114,15 @@
             'byminute': 0,
             'bynweekday': [],
             'byweekday': [],
             'count': None,
             'repeat_by': '',
             'until': None,
             'rrule': None,
+            'rrule_exclusion': None
         })
 
     def test_missing_after_occurrences_count(self):
         data = {
             'freq': rrule.DAILY,
             'interval': 4,
             'dtstart': '6/1/2017',
@@ -484,7 +486,40 @@
         form = RecurrenceForm(data=data)
         self.assertTrue(form.is_valid())
         rrule_model = form.save(
             occurrence_handler_path='ambition_utils.rrule.handler.OccurrenceHandler',
         )
         self.assertEqual(RRule.objects.count(), 1)
         self.assertEqual(rrule_model.next_occurrence, datetime.datetime(2017, 6, 7))
+
+    def test_exclusion_rule(self):
+        exclusion_data = {
+            'freq': rrule.MONTHLY,
+            'interval': 1,
+            'dtstart': '6/1/2023',
+            'byhour': '0',
+            'bysetpos': 2,
+            'bynweekday': json.dumps([[0, 2]]),
+            'ends': RecurrenceEnds.NEVER,
+            'repeat_by': 'DAY_OF_THE_WEEK_START'
+        }
+        data = {
+            'freq': rrule.WEEKLY,
+            'interval': 1,
+            'dtstart': '6/1/2023',
+            'byhour': '0',
+            'byweekday': json.dumps([0]),
+            'time_zone': 'UTC',
+            'ends': RecurrenceEnds.NEVER,
+            'rrule_exclusion': json.dumps(exclusion_data)
+        }
+        form = RecurrenceForm(data=data)
+        self.assertTrue(form.is_valid())
+        rrule_model = form.save()
+        self.assertEqual(
+            rrule_model.get_dates(num_dates=10),
+            [datetime.datetime(2023, 6, 5, 0, 0), datetime.datetime(2023, 6, 19, 0, 0),
+             datetime.datetime(2023, 6, 26, 0, 0), datetime.datetime(2023, 7, 3, 0, 0),
+             datetime.datetime(2023, 7, 17, 0, 0), datetime.datetime(2023, 7, 24, 0, 0),
+             datetime.datetime(2023, 7, 31, 0, 0), datetime.datetime(2023, 8, 7, 0, 0),
+             datetime.datetime(2023, 8, 21, 0, 0), datetime.datetime(2023, 8, 28, 0, 0)]
+        )
```

### Comparing `ambition-utils-3.1.0/ambition_utils/rrule/tests/model_tests.py` & `ambition-utils-3.1.1/ambition_utils/rrule/tests/model_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1418,7 +1418,60 @@
             [
                 datetime.datetime(2022, 10, 28, 7),
                 datetime.datetime(2022, 10, 29, 7),
                 datetime.datetime(2022, 10, 30, 8),
                 datetime.datetime(2022, 10, 31, 8),
             ]
         )
+
+
+class RRuleWithExclusionTest(TestCase):
+    def test_exclusion(self):
+        weekly_program = Program.objects.create(name='Weekly Program')
+        weekly_rrule = RRule.objects.create(
+            rrule_params={
+                'freq': rrule.DAILY,
+                'interval': 1,
+                'dtstart': datetime.datetime(2023, 6, 1),
+                'byweekday': 0,
+            },
+            rrule_exclusion_params={
+                'freq': rrule.MONTHLY,
+                'interval': 1,
+                'dtstart': datetime.datetime(2023, 6, 1),
+                'bysetpos': 2,
+                'byweekday': 0
+            },
+            related_object=weekly_program,
+            related_object_handler_name='handle_start_recurrence',
+        )
+        monthly_program = Program.objects.create(name='Monthly Program')
+        monthly_rrule = RRule.objects.create(
+            rrule_params={
+                'freq': rrule.MONTHLY,
+                'interval': 1,
+                'dtstart': datetime.datetime(2023, 6, 1),
+                'bysetpos': 2,
+                'byweekday': 0
+            },
+            related_object=monthly_program,
+            related_object_handler_name='handle_start_recurrence',
+        )
+
+        weekly_dates = weekly_rrule.get_dates(num_dates=10)
+        monthly_dates = monthly_rrule.get_dates(num_dates=10)
+        self.assertEqual(
+            weekly_dates,
+            [datetime.datetime(2023, 6, 5, 0, 0), datetime.datetime(2023, 6, 19, 0, 0),
+             datetime.datetime(2023, 6, 26, 0, 0), datetime.datetime(2023, 7, 3, 0, 0),
+             datetime.datetime(2023, 7, 17, 0, 0), datetime.datetime(2023, 7, 24, 0, 0),
+             datetime.datetime(2023, 7, 31, 0, 0), datetime.datetime(2023, 8, 7, 0, 0),
+             datetime.datetime(2023, 8, 21, 0, 0), datetime.datetime(2023, 8, 28, 0, 0)]
+        )
+        self.assertEqual(
+            monthly_dates,
+            [datetime.datetime(2023, 6, 12, 0, 0), datetime.datetime(2023, 7, 10, 0, 0),
+             datetime.datetime(2023, 8, 14, 0, 0), datetime.datetime(2023, 9, 11, 0, 0),
+             datetime.datetime(2023, 10, 9, 0, 0), datetime.datetime(2023, 11, 13, 0, 0),
+             datetime.datetime(2023, 12, 11, 0, 0), datetime.datetime(2024, 1, 8, 0, 0),
+             datetime.datetime(2024, 2, 12, 0, 0), datetime.datetime(2024, 3, 11, 0, 0)]
+        )
```

### Comparing `ambition-utils-3.1.0/ambition_utils/rrule/tests/models.py` & `ambition-utils-3.1.1/ambition_utils/rrule/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/rrule/tests/migrations/0001_initial.py` & `ambition-utils-3.1.1/ambition_utils/rrule/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/rrule/forms.py` & `ambition-utils-3.1.1/ambition_utils/rrule/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,20 +30,19 @@
     ('DAY_OF_THE_WEEK_START', 'Day of the week counting from the beginning of the month'),
     ('DAY_OF_THE_WEEK_END', 'Day of the week counting backwards from the end of the month'),
     # ('FIRST_DAY_OF_MONTH', 'First day of Month'),
     ('DAY_OF_THE_MONTH_END', 'Last day of Month'),
 )
 
 
-class RecurrenceForm(forms.Form):
+class RRuleForm(forms.Form):
     """
     Handles submission of data for populating rrule objects. The field names are based on the rrule
     params defined here http://dateutil.readthedocs.io/en/stable/rrule.html
     """
-    rrule = forms.ModelChoiceField(queryset=RRule.objects.all(), required=False)
 
     # Date from which the recurrence will be started from. This might not always be the first recurrence in the series
     dtstart = forms.DateField(
         error_messages={'required': 'Starts on is required'},
     )
 
     # The hour for each recurrence (0-23)
@@ -84,32 +83,25 @@
     # Number of times the recurrence will occur. Only required if ends is set to AFTER
     count = forms.IntegerField(required=False)
 
     # Date when the recurrence will end. Only required if ends is set to ON. The 'until' date might not be the last
     # recurrence date
     until = forms.DateField(required=False)
 
-    def __init__(self, *args, **kwargs):
-        # Remove the instance param if it exists. Model forms will try to pass this, but it isn't used here and will
-        # cause the base form init to fail
-        kwargs.pop('instance', None)
-
-        super(RecurrenceForm, self).__init__(*args, **kwargs)
-
     def clean_freq(self):
         """
         Make sure the frequency is an integer
         """
         return int(self.data.get('freq', -1))
 
     def clean(self):
         """
         Perform additional form validation based on submitted params
         """
-        cleaned_data = super(RecurrenceForm, self).clean()
+        cleaned_data = super().clean()
 
         if self.errors:
             return cleaned_data
 
         # Check if count is required
         if self.cleaned_data['ends'] == RecurrenceEnds.AFTER and not self.cleaned_data['count']:
             raise ValidationError('Number of occurrences is required')
@@ -168,18 +160,15 @@
         try:
             value = json.loads(self.data.get('bynweekday', '[]'))
         except ValueError:
             pass
 
         return value
 
-    def save(self, **kwargs):
-        """
-        Saves the RRule model and returns it
-        """
+    def get_rrule_params_from_cleaned_data(self):
         rrule_freq = self.cleaned_data['freq']
         start_date = self.cleaned_data['dtstart']
 
         # Convert date to datetime
         start_datetime = datetime.combine(start_date, datetime.min.time())
 
         # Build params for rrule object
@@ -212,27 +201,72 @@
                 params['bymonthday'] = start_datetime.day
             elif self.cleaned_data.get('repeat_by') == 'DAY_OF_THE_MONTH_END':
                 params['bymonthday'] = -1
             else:
                 params['byweekday'] = self.cleaned_data['bynweekday'][0][0]
                 params['bysetpos'] = self.cleaned_data['bynweekday'][0][1]
 
+        # Return the params
+        return params
+
+
+class RecurrenceForm(RRuleForm):
+    """
+    Converts rrule options into an rrule model
+    """
+
+    # Optional rrule object that we are modifying
+    rrule = forms.ModelChoiceField(queryset=RRule.objects.all(), required=False)
+
+    # Optional rrule exclusion params
+    rrule_exclusion = forms.CharField(required=False)
+
+    def __init__(self, *args, **kwargs):
+        # Remove the instance param if it exists. Model forms will try to pass this, but it isn't used here and will
+        # cause the base form init to fail
+        kwargs.pop('instance', None)
+
+        super(RecurrenceForm, self).__init__(*args, **kwargs)
+
+    def clean_rrule_exclusion(self):
+        # Get the value from data
+        rrule_exclusion = self.cleaned_data.get('rrule_exclusion')
+        if not rrule_exclusion:
+            return None
+
+        # Parse the exclusion options
+        rrule_exclusion = json.loads(rrule_exclusion)
+        rrule_exclusion['time_zone'] = self.cleaned_data['time_zone']
+
+        # Validate the options
+        rrule_exclusion_form = RRuleForm(data=rrule_exclusion)
+        if not rrule_exclusion_form.is_valid():
+            raise ValidationError('Exclusion options invalid')
+
+        # Return the exclusion params
+        return rrule_exclusion_form.get_rrule_params_from_cleaned_data()
+
+    def save(self, **kwargs):
+        """
+        Saves the RRule model and returns it
+        """
         # Keep track if this is an existing rrule that needs occurrence updated
         need_to_refresh_next_recurrence = False
 
         # Get the rrule model from the cleaned data
         rrule_model = self.cleaned_data.get('rrule')
         if rrule_model:
             need_to_refresh_next_recurrence = True
         else:
             # Use the recurrence passed into save kwargs
             rrule_model = kwargs.get('recurrence') or RRule()
 
         # Create or update the rule
-        rrule_model.rrule_params = params
+        rrule_model.rrule_params = self.get_rrule_params_from_cleaned_data()
+        rrule_model.rrule_exclusion_params = self.cleaned_data.get('rrule_exclusion')
         rrule_model.time_zone = self.cleaned_data.get('time_zone')
         for key, value in kwargs.items():
             if hasattr(rrule_model, key):
                 # This try except is because some field names might be reverse foreign key relationships
                 try:
                     setattr(rrule_model, key, value)
                 except TypeError:  # pragma: no cover
```

### Comparing `ambition-utils-3.1.0/ambition_utils/rrule/models.py` & `ambition-utils-3.1.1/ambition_utils/rrule/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 from datetime import datetime, timedelta
 from dateutil import parser
-from dateutil.rrule import rrule
+from dateutil.rrule import rrule, rruleset
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
-from django.contrib.postgres.fields import JSONField
 from django.db import models, transaction
 from django.utils.module_loading import import_string
 from fleming import fleming
 from manager_utils import bulk_update
 from timezone_field import TimeZoneField
 from typing import List
 import copy
@@ -103,18 +102,21 @@
 
 class RRule(models.Model):
     """
     Model that will hold rrule details and generate recurrences to be handled by the supplied handler
     """
 
     # Params used to generate the rrule
-    rrule_params = JSONField()
+    rrule_params = models.JSONField()
+
+    # Optional params used to generate the rrule exclusion
+    rrule_exclusion_params = models.JSONField(default=None, blank=True, null=True)
 
     # Any meta data associated with the object that created this rule
-    meta_data = JSONField(default=dict)
+    meta_data = models.JSONField(default=dict)
 
     # The timezone all dates should be converted to
     time_zone = TimeZoneField(default='UTC')
 
     # The last occurrence date that was handled
     last_occurrence = models.DateTimeField(null=True, default=None)
 
@@ -133,14 +135,17 @@
     # The name of the method to call on the related_object when the recurrence has expired
     related_object_handler_name = models.TextField(default=None, null=True, blank=True)
 
     # Custom object manager
     objects = RRuleManager()
 
     def get_time_zone_object(self):
+        """
+        Returns the time zone object from pytz
+        """
         if self.time_zone is None:
             return pytz.utc
 
         # There is a test for this but it still doesn't hit this block
         if isinstance(self.time_zone, str):  # pragma: no cover
             return pytz.timezone(self.time_zone)
 
@@ -154,21 +159,50 @@
         """
         try:
             handler_class = import_string(self.occurrence_handler_path)()
             return handler_class
         except:
             return None
 
+    def get_rrule_set(self):
+        """
+        Returns the rrule set that will combine the rrule and optional exclusion rrule
+        """
+        rrule_set = rruleset()
+        rrule_set.rrule(self.get_rrule())
+        rrule_exclusion = self.get_rrule_exclusion()
+        if rrule_exclusion:
+            rrule_set.exrule(rrule_exclusion)
+        return rrule_set
+
     def get_rrule(self):
         """
         Builds the rrule object by restoring all the params.
+        """
+        return self.get_rrule_from_params(self.rrule_params)
+
+    def get_rrule_exclusion(self):
+        """
+        Builds the rrule exclusion object by restoring all the params.
+        :rtype: rrule
+        """
+        return self.get_rrule_from_params(self.rrule_exclusion_params)
+
+    def get_rrule_from_params(self, params):
+        """
+        Creates an rrule object from a dict of rrule params. Returns None if no params exists.
         The dtstart param will be converted to local time if it is set.
         :rtype: rrule
         """
-        params = copy.deepcopy(self.rrule_params)
+        # Check for none or empty
+        if not params:
+            return None
+
+        # Create a deep copy because we will manipulate
+        params = copy.deepcopy(params)
 
         # Convert next scheduled from utc back to time zone
         if params.get('dtstart') and not hasattr(params.get('dtstart'), 'date'):
             params['dtstart'] = parser.parse(params['dtstart'])
 
         # Convert until date from utc back to time zone
         if params.get('until') and not hasattr(params.get('until'), 'date'):
@@ -186,38 +220,38 @@
         :param last_occurrence: The last occurrence that was generated
         :param force: If the next occurrence is none, force the rrule to generate another
         :rtype: rrule or None
         """
         # Get the last occurrence
         last_occurrence = last_occurrence or self.last_occurrence or datetime.utcnow()
 
-        # Get the rule
-        rule = self.get_rrule()
+        # Get the rule set
+        rule_set = self.get_rrule_set()
 
         # Convert to local time zone for getting next occurrence, otherwise time zones ahead of utc will return the same
         last_occurrence = fleming.convert_to_tz(last_occurrence, self.get_time_zone_object(), return_naive=True)
 
         # Generate the next occurrence
-        next_occurrence = rule.after(last_occurrence)
+        next_occurrence = rule_set.after(last_occurrence)
 
         # If next occurrence is none and force is true, force the rrule to generate another date
         if next_occurrence is None and force:
             # Keep a reference to the original rrule_params
             original_rrule_params = {}
             original_rrule_params.update(self.rrule_params)
 
             # Remove any limiting params
             self.rrule_params.pop('count', None)
             self.rrule_params.pop('until', None)
 
-            # Refetch the rule
-            rule = self.get_rrule()
+            # Refetch the rule set
+            rule_set = self.get_rrule_set()
 
             # Generate the next occurrence
-            next_occurrence = rule.after(last_occurrence)
+            next_occurrence = rule_set.after(last_occurrence)
 
             # Restore the rrule params
             self.rrule_params = original_rrule_params
 
         # If there is a next occurrence, convert to utc
         if next_occurrence:
             next_occurrence = self.convert_to_utc(next_occurrence)
@@ -280,83 +314,107 @@
         else:
             self.next_occurrence = next_occurrence
 
     def pre_save_hooks(self):
         self.set_date_objects()
 
     def set_date_objects(self):
-        # Check if this is a new rrule object
-        if self.pk is None:
-            # Convert next scheduled from utc back to time zone
-            if self.rrule_params.get('dtstart') and not hasattr(self.rrule_params.get('dtstart'), 'date'):
-                self.rrule_params['dtstart'] = parser.parse(self.rrule_params['dtstart'])
+        """
+        Ensure that all the date keys are properly set on all rrule params
+        """
 
-            # Convert until date from utc back to time zone
-            if self.rrule_params.get('until') and not hasattr(self.rrule_params.get('until'), 'date'):
-                self.rrule_params['until'] = parser.parse(self.rrule_params['until'])
+        # Convert the rrule and exclusion rrule params to properly set date keys
+        is_new = self.pk is None
+        self.set_date_objects_for_params(self.rrule_params, is_new=is_new)
+        self.set_date_objects_for_params(self.rrule_exclusion_params, is_new=is_new)
 
+        # Check if this is a new rrule object
+        if is_new:
             # Get the first scheduled time according to the rrule (this converts from utc back to local time)
-            self.next_occurrence = self.get_rrule()[0]
+            self.next_occurrence = self.get_rrule_set()[0]
 
             # Convert back to utc before saving
             self.next_occurrence = self.convert_to_utc(self.next_occurrence)
 
+    def set_date_objects_for_params(self, params, is_new=False):
+        """
+        Give an rrule params object, ensure that the date keys are properly set and properly converted to strings
+        """
+        # Check for no params
+        if not params:
+            return params
+
+        # Check if this is a new rrule object
+        if is_new:
+            # Convert next scheduled from utc back to time zone
+            if params.get('dtstart') and not hasattr(params.get('dtstart'), 'date'):
+                params['dtstart'] = parser.parse(params['dtstart'])
+
+            # Convert until date from utc back to time zone
+            if params.get('until') and not hasattr(params.get('until'), 'date'):
+                params['until'] = parser.parse(params['until'])
+
         # Serialize the datetime objects if they exist
-        if self.rrule_params.get('dtstart') and hasattr(self.rrule_params.get('dtstart'), 'date'):
-            self.rrule_params['dtstart'] = self.rrule_params['dtstart'].strftime('%Y-%m-%d %H:%M:%S')
+        if params.get('dtstart') and hasattr(params.get('dtstart'), 'date'):
+            params['dtstart'] = params['dtstart'].strftime('%Y-%m-%d %H:%M:%S')
 
-        if self.rrule_params.get('until') and hasattr(self.rrule_params.get('until'), 'date'):
-            self.rrule_params['until'] = self.rrule_params['until'].strftime('%Y-%m-%d %H:%M:%S')
+        if params.get('until') and hasattr(params.get('until'), 'date'):
+            params['until'] = params['until'].strftime('%Y-%m-%d %H:%M:%S')
 
     def save(self, *args, **kwargs):
         """
         Saves the rrule model to the database. If this is a new object, the first next_scheduled time is
         determined and set. The `dtstart` and `until` objects will be safely encoded as strings if they are
         datetime objects.
         """
+
+        # Run any pre save hooks
         self.pre_save_hooks()
 
         # Call the parent save method
         super().save(*args, **kwargs)
 
     def get_dates(self, num_dates=20, start_date=None) -> List[datetime]:
         """
         Return a list of datetime objects the recurrence will generate, after the start date (if defined).
         :param num_dates: The maximum number of dates to calculate. Will stop at passed start_date
         :param start_date: The optional start date to begin generating dates after
         :return: A list of datetime objects
         """
+
+        # Assert that we have dates
         assert num_dates > 0
 
+        # Ensure that pre save hooks have been run
         self.pre_save_hooks()
 
+        # Generate the dates
         dates = []
-
         try:
             # Capture the rule's first date for use in RRule.after() in the loop.
-            rule = self.get_rrule()
+            rule_set = self.get_rrule_set()
 
             # Evaluate if the first date should be retained.
-            d = self.convert_to_utc(rule[0])
+            d = self.convert_to_utc(rule_set[0])
             if not start_date or d > start_date:
                 dates.append(d)
 
             # Continue evaluating and appending dates to satisfy desired number,
             # retaining date for evaluation in the next iteration.
             while len(dates) < num_dates:
                 d = self.get_next_occurrence(last_occurrence=d)
                 if d:
                     if not start_date or d > start_date:
                         dates.append(d)
                 else:
                     break
-
         except Exception:  # pragma: no cover
             pass
 
+        # Return the generated dates
         return dates
 
     def generate_dates(self, num_dates=20):
         """
         DEPRECATED. Replaced by get_dates.
         Return a list of the next num_dates datetimes of the recurrence.
         """
@@ -367,17 +425,15 @@
         """
         Creates a clone of itself.
         """
 
         # Clear id to force a new object.
         clone = copy.deepcopy(self)
         clone.id = None
-
         clone.save()
-
         return clone
 
     def clone_with_day_offset(self, day_offset: int) -> RRule:
         """
         Creates a clone of a passed RRule object offset by a specified number of days
         :param day_offset: The number of days to offset the clone's start date. Can be negative.
         """
```

### Comparing `ambition-utils-3.1.0/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py` & `ambition-utils-3.1.1/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/rrule/migrations/0001_initial.py` & `ambition-utils-3.1.1/ambition_utils/rrule/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.11.7 on 2017-12-28 17:08
-from __future__ import unicode_literals
 
-import django.contrib.postgres.fields.jsonb
 from django.db import migrations, models
 import timezone_field.fields
 
 
 class Migration(migrations.Migration):
 
     initial = True
@@ -15,16 +13,16 @@
     ]
 
     operations = [
         migrations.CreateModel(
             name='RRule',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('rrule_params', django.contrib.postgres.fields.jsonb.JSONField()),
-                ('meta_data', django.contrib.postgres.fields.jsonb.JSONField(default=dict)),
+                ('rrule_params', models.JSONField()),
+                ('meta_data', models.JSONField(default=dict)),
                 ('time_zone', timezone_field.fields.TimeZoneField(default=b'UTC')),
                 ('last_occurrence', models.DateTimeField(default=None, null=True)),
                 ('next_occurrence', models.DateTimeField(default=None, null=True)),
                 ('occurrence_handler_path', models.CharField(max_length=500)),
             ],
         ),
     ]
```

### Comparing `ambition-utils-3.1.0/ambition_utils/activity/tests/task_tests.py` & `ambition-utils-3.1.1/ambition_utils/activity/tests/task_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from celery import Celery
 from django.test import TestCase
-from mock import patch
+from unittest.mock import patch
 from uuid import uuid4
 
 from ambition_utils.activity.tasks import ActivityManagedTaskMixin, track_activity
 from ambition_utils.activity.models import Activity, ActivityGroup, ActivityStatus, ActivityGroupStatus
 
 test_application = Celery('task_tests')
```

### Comparing `ambition-utils-3.1.0/ambition_utils/activity/models.py` & `ambition-utils-3.1.1/ambition_utils/activity/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/ambition_utils/activity/migrations/0002_auto_20180427_1819.py` & `ambition-utils-3.1.1/ambition_utils/activity/migrations/0002_auto_20180427_1819.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.11.10 on 2018-04-27 18:19
-from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `ambition-utils-3.1.0/ambition_utils/activity/migrations/0001_initial.py` & `ambition-utils-3.1.1/ambition_utils/activity/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.11.10 on 2018-04-03 18:09
-from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 import uuid
 
 
 class Migration(migrations.Migration):
```

### Comparing `ambition-utils-3.1.0/ambition_utils/activity/tasks.py` & `ambition-utils-3.1.1/ambition_utils/activity/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from django.contrib.contenttypes.models import ContentType
 from functools import wraps
 from inspect import getmembers
-from six import reraise
-from sys import exc_info
 
 from ambition_utils.activity.models import Activity, ActivityGroup
 
 
 def decorate_activity(fn, activity):
     """
     Decorator to wrap function call with activity state management
@@ -17,15 +15,15 @@
         set_active()
         try:
             ret_val = fn(*args, **kwargs)
             activity.success()
             return ret_val
         except Exception as e:
             activity.failure(str(e))
-            reraise(*exc_info())
+            raise e
     return decorator
 
 
 def track_activity(fn):
     """
     decorator to add state to method which indicates that its progress should be tracked through activities
     """
```

### Comparing `ambition-utils-3.1.0/ambition_utils/time_helpers.py` & `ambition-utils-3.1.1/ambition_utils/time_helpers.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/setup.py` & `ambition-utils-3.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -40,20 +40,18 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     license='MIT',
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={'dev': tests_require},
     test_suite='run_tests.run_tests',
     include_package_data=True,
```

### Comparing `ambition-utils-3.1.0/README.rst` & `ambition-utils-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.0/PKG-INFO` & `ambition-utils-3.1.1/ambition_utils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.0
+Version: 3.1.1
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/ambition-utils.png
-           :target: https://travis-ci.org/ambitioninc/ambition-utils
-        
-        .. image:: https://coveralls.io/repos/ambitioninc/ambition-utils/badge.png?branch=develop
-            :target: https://coveralls.io/r/ambitioninc/ambition-utils?branch=develop
-        
-        .. image:: https://pypip.in/v/ambition-utils/badge.png
-            :target: https://crate.io/packages/ambition-utils/
-            :alt: Latest PyPI version
-        
-        .. image:: https://pypip.in/d/ambition-utils/badge.png
-            :target: https://crate.io/packages/ambition-utils/
-        
-        
-        Requirements
-        ------------
-        * Python 3.6+
-        * Django 1.11+
-        * Postgres 9.5+
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install ambition-utils
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/ambition-utils.git
-        
-        Documentation
-        -------------
-        
-        Note: As of version 0.5.0, this project only supports Python3.6+
-        If you need Python2 support, pin to `ambition-utils==0.4.0`
-        
-        Full documentation is available at http://ambition-utils.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-        
 Keywords: django,database,query,sql,postgres,upsert
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Provides-Extra: dev
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/ambition-utils.png
+   :target: https://travis-ci.org/ambitioninc/ambition-utils
+
+.. image:: https://coveralls.io/repos/ambitioninc/ambition-utils/badge.png?branch=develop
+    :target: https://coveralls.io/r/ambitioninc/ambition-utils?branch=develop
+
+.. image:: https://pypip.in/v/ambition-utils/badge.png
+    :target: https://crate.io/packages/ambition-utils/
+    :alt: Latest PyPI version
+
+.. image:: https://pypip.in/d/ambition-utils/badge.png
+    :target: https://crate.io/packages/ambition-utils/
+
+
+Requirements
+------------
+* Python 3.6+
+* Django 1.11+
+* Postgres 9.5+
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install ambition-utils
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/ambition-utils.git
+
+Documentation
+-------------
+
+Note: As of version 0.5.0, this project only supports Python3.6+
+If you need Python2 support, pin to `ambition-utils==0.4.0`
+
+Full documentation is available at http://ambition-utils.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

