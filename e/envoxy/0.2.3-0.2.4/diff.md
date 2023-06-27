# Comparing `tmp/envoxy-0.2.3.tar.gz` & `tmp/envoxy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/envoxy-0.2.3.tar", last modified: Thu Jan 26 17:08:02 2023, max compression
+gzip compressed data, was "dist/envoxy-0.2.4.tar", last modified: Tue Jun 27 15:18:20 2023, max compression
```

## Comparing `envoxy-0.2.3.tar` & `envoxy-0.2.4.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:02.000000 envoxy-0.2.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/envoxy.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-26 17:08:01.000000 envoxy-0.2.3/envoxy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 17:08:01.000000 envoxy-0.2.3/envoxy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      268 2023-01-26 17:08:01.000000 envoxy-0.2.3/envoxy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1382 2023-01-26 17:08:01.000000 envoxy-0.2.3/envoxy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     5091 2023-01-26 17:08:01.000000 envoxy-0.2.3/envoxy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2020-01-30 17:54:32.000000 envoxy-0.2.3/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:02.000000 envoxy-0.2.3/src/envoxy/views/
--rw-rw-r--   0 root         (0) root         (0)     1904 2022-09-06 19:19:17.000000 envoxy-0.2.3/src/envoxy/views/containers.py
--rw-rw-r--   0 root         (0) root         (0)     4168 2022-11-17 10:40:18.000000 envoxy-0.2.3/src/envoxy/views/views.py
--rw-r--r--   0 root         (0) root         (0)       44 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/http/
--rw-r--r--   0 root         (0) root         (0)     1427 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/http/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)      128 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/http/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1423 2022-11-17 10:40:18.000000 envoxy-0.2.3/src/envoxy/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/mqtt/
--rw-rw-r--   0 root         (0) root         (0)    13919 2023-01-26 16:40:04.000000 envoxy-0.2.3/src/envoxy/mqtt/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/mqtt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/redis/
--rw-r--r--   0 root         (0) root         (0)     1622 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/redis/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/postgresql/
--rw-rw-r--   0 root         (0) root         (0)     5690 2022-09-06 19:19:17.000000 envoxy-0.2.3/src/envoxy/postgresql/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/postgresql/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      520 2022-11-17 10:40:18.000000 envoxy-0.2.3/src/envoxy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:02.000000 envoxy-0.2.3/src/envoxy/zeromq/
--rw-rw-r--   0 root         (0) root         (0)    18509 2022-11-17 15:57:21.000000 envoxy-0.2.3/src/envoxy/zeromq/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/zeromq/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2933 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/decorators.py
--rw-rw-r--   0 root         (0) root         (0)    17270 2021-11-09 12:43:56.000000 envoxy-0.2.3/src/envoxy/asserts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/couchdb/
--rw-rw-r--   0 root         (0) root         (0)     3244 2022-09-06 19:18:33.000000 envoxy-0.2.3/src/envoxy/couchdb/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/couchdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/cache/
--rw-r--r--   0 root         (0) root         (0)      513 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1813 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/cache/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:02.000000 envoxy-0.2.3/src/envoxy/utils/
--rw-r--r--   0 root         (0) root         (0)      359 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/utils/encoders.py
--rw-r--r--   0 root         (0) root         (0)     2417 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/utils/watchdog.py
--rw-r--r--   0 root         (0) root         (0)      569 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/utils/datetime.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      565 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/utils/cache.py
--rw-r--r--   0 root         (0) root         (0)     7338 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/utils/logs.py
--rw-r--r--   0 root         (0) root         (0)     1388 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/utils/throttle.py
--rw-rw-r--   0 root         (0) root         (0)     1742 2022-11-17 10:40:18.000000 envoxy-0.2.3/src/envoxy/utils/singleton.py
--rw-rw-r--   0 root         (0) root         (0)     1202 2021-11-09 12:43:56.000000 envoxy-0.2.3/src/envoxy/utils/config.py
--rw-r--r--   0 root         (0) root         (0)     1211 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/utils/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/db/
--rw-r--r--   0 root         (0) root         (0)     2934 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/db/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)       46 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/db/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:02.000000 envoxy-0.2.3/src/envoxy/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15506 2021-11-09 12:43:56.000000 envoxy-0.2.3/src/envoxy/tests/test_asserts.py
--rw-r--r--   0 root         (0) root         (0)     1204 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/tests/fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 17:08:01.000000 envoxy-0.2.3/src/envoxy/auth/
--rw-r--r--   0 root         (0) root         (0)     2587 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/auth/backends.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.3/src/envoxy/auth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      216 2022-11-17 15:54:52.000000 envoxy-0.2.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 17:08:02.000000 envoxy-0.2.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4772 2021-11-09 12:43:56.000000 envoxy-0.2.3/README.md
--rw-rw-r--   0 root         (0) root         (0)     1202 2023-01-26 17:03:05.000000 envoxy-0.2.3/setup.py
--rw-r--r--   0 root         (0) root         (0)     5091 2023-01-26 17:08:02.000000 envoxy-0.2.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/envoxy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-27 15:18:20.000000 envoxy-0.2.4/envoxy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 15:18:20.000000 envoxy-0.2.4/envoxy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-27 15:18:20.000000 envoxy-0.2.4/envoxy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-06-27 15:18:20.000000 envoxy-0.2.4/envoxy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-06-27 15:18:20.000000 envoxy-0.2.4/envoxy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2020-01-30 17:54:32.000000 envoxy-0.2.4/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/views/
+-rw-rw-r--   0 root         (0) root         (0)     1848 2023-06-27 09:35:10.000000 envoxy-0.2.4/src/envoxy/views/containers.py
+-rw-rw-r--   0 root         (0) root         (0)     4419 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/views/views.py
+-rw-r--r--   0 root         (0) root         (0)       44 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/http/
+-rw-r--r--   0 root         (0) root         (0)     1427 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/http/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)      128 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/http/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1423 2022-11-17 10:40:18.000000 envoxy-0.2.4/src/envoxy/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/mqtt/
+-rw-rw-r--   0 root         (0) root         (0)    14000 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/mqtt/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/mqtt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/redis/
+-rw-rw-r--   0 root         (0) root         (0)     1865 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/redis/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/postgresql/
+-rw-rw-r--   0 root         (0) root         (0)     5690 2022-09-06 19:19:17.000000 envoxy-0.2.4/src/envoxy/postgresql/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/postgresql/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      520 2022-11-17 10:40:18.000000 envoxy-0.2.4/src/envoxy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/zeromq/
+-rw-rw-r--   0 root         (0) root         (0)    18421 2023-06-27 14:55:49.000000 envoxy-0.2.4/src/envoxy/zeromq/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/zeromq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     3115 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/decorators.py
+-rw-rw-r--   0 root         (0) root         (0)    17506 2023-06-27 15:02:03.000000 envoxy-0.2.4/src/envoxy/asserts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/couchdb/
+-rw-rw-r--   0 root         (0) root         (0)     3271 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/couchdb/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/couchdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/cache/
+-rw-r--r--   0 root         (0) root         (0)      513 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/cache/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1856 2023-06-27 09:44:39.000000 envoxy-0.2.4/src/envoxy/cache/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/utils/
+-rw-rw-r--   0 root         (0) root         (0)      825 2023-06-26 16:48:30.000000 envoxy-0.2.4/src/envoxy/utils/encoders.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/utils/watchdog.py
+-rw-r--r--   0 root         (0) root         (0)      569 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/utils/datetime.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      565 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/utils/cache.py
+-rw-r--r--   0 root         (0) root         (0)     7338 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/utils/logs.py
+-rw-rw-r--   0 root         (0) root         (0)     1397 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/utils/throttle.py
+-rw-rw-r--   0 root         (0) root         (0)     1846 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/utils/singleton.py
+-rw-rw-r--   0 root         (0) root         (0)     1202 2021-11-09 12:43:56.000000 envoxy-0.2.4/src/envoxy/utils/config.py
+-rw-rw-r--   0 root         (0) root         (0)     1237 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/utils/handlers.py
+-rw-rw-r--   0 root         (0) root         (0)     1366 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/utils/profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/db/
+-rw-r--r--   0 root         (0) root         (0)     2934 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/db/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       46 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/db/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15506 2021-11-09 12:43:56.000000 envoxy-0.2.4/src/envoxy/tests/test_asserts.py
+-rw-r--r--   0 root         (0) root         (0)     1204 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/tests/fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 15:18:20.000000 envoxy-0.2.4/src/envoxy/auth/
+-rw-rw-r--   0 root         (0) root         (0)     2619 2023-06-26 16:39:14.000000 envoxy-0.2.4/src/envoxy/auth/backends.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.4/src/envoxy/auth/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      230 2023-06-26 16:39:14.000000 envoxy-0.2.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 15:18:20.000000 envoxy-0.2.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4772 2021-11-09 12:43:56.000000 envoxy-0.2.4/README.md
+-rw-rw-r--   0 root         (0) root         (0)       64 2023-06-26 16:39:14.000000 envoxy-0.2.4/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     1202 2023-06-27 15:03:42.000000 envoxy-0.2.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-06-27 15:18:20.000000 envoxy-0.2.4/PKG-INFO
```

### Comparing `envoxy-0.2.3/envoxy.egg-info/SOURCES.txt` & `envoxy-0.2.4/envoxy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 envoxy.egg-info/PKG-INFO
 envoxy.egg-info/SOURCES.txt
 envoxy.egg-info/dependency_links.txt
 envoxy.egg-info/requires.txt
 envoxy.egg-info/top_level.txt
@@ -37,14 +38,15 @@
 src/envoxy/utils/__init__.py
 src/envoxy/utils/cache.py
 src/envoxy/utils/config.py
 src/envoxy/utils/datetime.py
 src/envoxy/utils/encoders.py
 src/envoxy/utils/handlers.py
 src/envoxy/utils/logs.py
+src/envoxy/utils/profiling.py
 src/envoxy/utils/singleton.py
 src/envoxy/utils/throttle.py
 src/envoxy/utils/watchdog.py
 src/envoxy/views/__init__.py
 src/envoxy/views/containers.py
 src/envoxy/views/views.py
 src/envoxy/zeromq/__init__.py
```

### Comparing `envoxy-0.2.3/envoxy.egg-info/PKG-INFO` & `envoxy-0.2.4/envoxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envoxy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Envoxy Platform Framework
 Home-page: https://github.com/habitio/envoxy
 Author: Matheus (vorjdux) Santos
 Author-email: vorj.dux@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `envoxy-0.2.3/LICENSE` & `envoxy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/views/views.py` & `envoxy-0.2.4/src/envoxy/views/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .containers import Response
 from ..exceptions import ValidationException
 from ..utils.logs import Log
 
 from ..mqtt.dispatcher import Dispatcher as mqttc
 
 REGEX_VAR_PATTERN: str = r'(?P<all>{(?P<var>[^:]+):(?P<type>[^}]+)})'
+COMPILED_REGEX = re.compile(REGEX_VAR_PATTERN)
 
 
 class View(object):
 
     __metaclass__ = None
 
     def __init__(self) -> None:
@@ -29,88 +30,100 @@
     def set_flask(self, app) -> None:
 
         self.__flask_app: Flask = app
 
         _endpoint = getattr(self.__metaclass__, 'endpoint', '')
         _protocols = getattr(self.__metaclass__, 'protocols', [])
         _server = getattr(self.__metaclass__, 'server', '')
-
-        _regex = re.compile(REGEX_VAR_PATTERN)
         
         for _method in self.get_methods():
 
+            _method_attr = getattr(self, _method, 'Not Found')
+
             if 'http' in _protocols:
 
-                if 'http' not in self.protocols: self.protocols.append('http')
+                if 'http' not in self.protocols: 
+                    self.protocols.append('http')
 
                 _flask_endpoint = _endpoint
 
-                for _match in _regex.finditer(_endpoint):
+                for _match in COMPILED_REGEX.finditer(_endpoint):
                     _groups = _match.groupdict()
                     _flask_endpoint = _flask_endpoint.replace(_groups['all'], '<{}:{}>'.format(_groups['type'], _groups['var']))
 
                 self.__flask_app.add_url_rule(
                     _flask_endpoint, 
                     view_func=self._dispatch(_method, _endpoint, 'http'),
                     methods=[_method]
                 )
 
                 Log.system('{} [{}] Added the endpoint "{}" using the method "{}" calling the function "{}"'.format(
                     Log.style.apply('>>>', Log.style.BOLD),
                     Log.style.apply('HTTP', Log.style.GREEN_FG),
                     _endpoint,
                     _method,
-                    getattr(self, _method, 'Not Found')
+                    _method_attr
                 ))
 
             if 'mqtt' in _protocols and _method == "on_event":
 
-                if 'mqtt' not in self.protocols: self.protocols.append('mqtt')
+                if 'mqtt' not in self.protocols: 
+                    self.protocols.append('mqtt')
 
                 Log.system('{} [{}] Subscribing to topic "{}" calling the function "{}"'.format(
                     Log.style.apply('>>>', Log.style.BOLD),
                     Log.style.apply('MQTT', Log.style.GREEN_FG),
                     _endpoint,
                     _method
                 ))
 
-                mqttc.subscribe(_server, _endpoint, getattr(self, _method, 'Not Found'))
+                mqttc.subscribe(_server, _endpoint, _method_attr)
 
     def _dispatch(self, _method, _endpoint, _protocol):
 
         def _wrapper(*args, **kwargs):
             if _protocol == 'http':
                 return self.dispatch(request, _method, _endpoint, *args, **kwargs)
         
         _wrapper.__name__ = '__wrapper__{}__{}__{}'.format(self.__class__.__name__, _method, _protocol)
         
         return _wrapper
 
     def dispatch(self, request, _method, _endpoint, *args, **kwargs):
+        
         kwargs.update({ 'endpoint': _endpoint })
+        
         try:
             return getattr(self, _method)(request, *args, **kwargs)
-
         except Exception as e:
             
-            _error_log_ref = str(uuid.uuid4())
             _code = 0
             _status = 500
 
             if isinstance(e, ValidationException):
-                if 'code' in e.kwargs : _code = e.kwargs['code']
-                if 'status' in e.kwargs: _status = e.kwargs['status']
+                
+                if 'code' in e.kwargs : 
+                    _code = e.kwargs['code']
+                
+                if 'status' in e.kwargs: 
+                    _status = e.kwargs['status']
 
             if request.is_json:
 
-                if _status not in [ 204, '204'] : Log.error(f"ELRC({_error_log_ref}) - Traceback: {traceback.format_exc()}")
+                if _status not in [ 204, '204']:
+                    _error_log_ref = str(uuid.uuid4()) 
+                    Log.error(f"ELRC({_error_log_ref}) - Traceback: {traceback.format_exc()}")
+                
                 _resp =  make_response(jsonify({"error": f"{e} :: ELRC({_error_log_ref})", "code": _code}), _status)
                 _resp.headers['X-Error'] = _code
+                
                 return _resp
 
-            if _status not in [ 204, '204'] : Log.error(f"ELRC({_error_log_ref}) - Traceback: {traceback.format_exc()}")
+            if _status not in [ 204, '204']: 
+                Log.error(f"ELRC({_error_log_ref}) - Traceback: {traceback.format_exc()}")
+            
             return FlaskResponse(str(f"error: {e} :: ELRC({_error_log_ref})"), _status, headers={
                 "X-Error": _code
             })
 
     def cached_response(self, result):
         return Response(result)
```

### Comparing `envoxy-0.2.3/src/envoxy/http/dispatcher.py` & `envoxy-0.2.4/src/envoxy/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/constants.py` & `envoxy-0.2.4/src/envoxy/constants.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/mqtt/dispatcher.py` & `envoxy-0.2.4/src/envoxy/mqtt/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import json
 import threading
 import time
 import uuid
 
 import paho.mqtt.client as paho
 
 from ..constants import SERVER_NAME
 from ..exceptions import ValidationException
 from ..utils.config import Config
 from ..utils.datetime import Now
 from ..utils.logs import Log
 from ..utils.singleton import Singleton
+from ..utils.encoders import envoxy_json_dumps
 
 RC_LIST = {
     0: "Connection successful",
     1: "Connection refused - incorrect protocol version",
     2: "Connection refused - invalid client identifier",
     3: "Connection refused - server unavailable",
     4: "Connection refused - bad username or password",
@@ -289,21 +289,21 @@
                     Log.style.apply('MQTT', Log.style.GREEN_FG),
                     Log.style.apply('{}'.format(topic), Log.style.BLUE_FG)
                 )
                 
                 Log.trace(_message)
 
             if no_envelope:
-                _payload = json.dumps(message)
+                _payload = envoxy_json_dumps(message).decode('utf-8')
 
             else:
-                _payload = json.dumps(message.update({
+                _payload = envoxy_json_dumps(message.update({
                     "headers": headers,
                     "resource": topic
-                }))
+                })).decode('utf-8')
 
             _message = '{} | Message{}'
 
             if Log.is_gte_log_level(Log.VERBOSE):
                 
                 Log.verbose(_message, _payload)
```

### Comparing `envoxy-0.2.3/src/envoxy/redis/client.py` & `envoxy-0.2.4/src/envoxy/redis/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 import redis
-import json
 
 from ..constants import REDIS_DEFAULT_PORT, REDIS_DEFAULT_HOST, REDIS_DEFAULT_DB, REDIS_DEFAULT_TTL
 from ..utils.logs import Log
+from ..utils.encoders import envoxy_json_dumps, envoxy_json_loads
 
 class Client:
 
     _instances = {}
 
     __conn = None
 
     def __init__(self, server_conf):
 
         for _server_key in server_conf.keys():
 
             _conf = server_conf[_server_key]
+            _ttl = _conf.get('ttl', REDIS_DEFAULT_TTL)
+
             self._instances[_server_key] = {
                 'server': _server_key,
-                'conf': _conf
+                'conf': _conf,
+                'ttl': _ttl
             }
 
             self.connect(self._instances[_server_key])
 
     def connect(self, instance):
 
-        config = instance['conf']
+        _config = instance['conf']
 
-        _bind = config.get('bind', '')
-        _db = config.get('db', REDIS_DEFAULT_DB)
-        _ttl = config.get('ttl', REDIS_DEFAULT_TTL)
+        _bind = _config.get('bind', '')
+        _db = _config.get('db', REDIS_DEFAULT_DB)
 
         if ':' in _bind:
             _host, _port = tuple(_bind.split(':'))
         else:
-            _host = config.get('host', REDIS_DEFAULT_HOST)
-            _port = config.get('port', REDIS_DEFAULT_PORT)
+            _host = _config.get('host', REDIS_DEFAULT_HOST)
+            _port = _config.get('port', REDIS_DEFAULT_PORT)
 
         instance['conn'] = redis.Redis(host=_host, port=_port, db=_db)
 
         Log.trace('>>> Successfully connected to REDIS: {}, {}:{}'.format(instance['server'], _host, _port))
 
 
     def get(self, server_key, key):
-        conn = self.__conn if self.__conn is not None else self.get_client(server_key)
+        _conn = self.__conn if self.__conn is not None else self.get_client(server_key)
+
+        _data = _conn.get(key)
+
+        return envoxy_json_loads(_data.encode('utf-8')) if _data else None
 
-        data = conn.get(key)
-        return json.loads(data) if data else None
+    def set(self, server_key, key, value, ttl=None):
+        _instance = self._instances[server_key]
+        
+        _conn = self.__conn if self.__conn is not None else _instance['conn']
 
-    def set(self, server_key, key, value):
-        conn = self.__conn if self.__conn is not None else self.get_client(server_key)
+        _data = envoxy_json_dumps(value).decode('utf-8')
 
-        data = json.dumps(value)
-        return conn.set(key, data)
+        return _conn.set(key, _data, ex=ttl if ttl else _instance['ttl'])
 
     def get_client(self, server_key):
         return self._instances[server_key]['conn']
```

### Comparing `envoxy-0.2.3/src/envoxy/postgresql/client.py` & `envoxy-0.2.4/src/envoxy/postgresql/client.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/__init__.py` & `envoxy-0.2.4/src/envoxy/__init__.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/zeromq/dispatcher.py` & `envoxy-0.2.4/src/envoxy/zeromq/dispatcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,101 @@
 import asyncio
+import queue
 import threading
 import time
 import uuid
 from concurrent.futures import ThreadPoolExecutor
 
 import zmq
 
-from ..asserts import *
+from ..asserts import assertz_integer, assertz_mandatory, assertz_string, assertz_uri
 from ..cache import Cache
-from ..constants import (SERVER_NAME, ZEROMQ_CONTEXT, ZEROMQ_MAX_WORKERS,
-                         ZEROMQ_POLLER_RETRIES, ZEROMQ_POLLIN_TIMEOUT,
-                         ZEROMQ_RETRY_TIMEOUT, Performative)
+from ..constants import SERVER_NAME, ZEROMQ_CONTEXT, ZEROMQ_MAX_WORKERS, ZEROMQ_POLLER_RETRIES, ZEROMQ_POLLIN_TIMEOUT, ZEROMQ_RETRY_TIMEOUT, Performative
 from ..exceptions import ValidationException
 from ..utils.config import Config
 from ..utils.datetime import Now
 from ..utils.logs import Log
 from ..utils.singleton import Singleton
+from ..utils.encoders import envoxy_json_loads, envoxy_json_dumps
 
 
 class NoSocketException(Exception):
     pass
 
+
 class ZMQException(Exception):
     pass
 
+
 class ZMQ(Singleton):
 
-    def __init__(self):
+    _cache = None
+    _instances = {}
+    _contexts = {}
+    _workers = {}
+    _available_workers = queue.Queue()
+    _executor = None
+    _lock = threading.Lock()
 
-        self._cache = None
-        self._instances = {}
-        self._workers = {}
-        self._available_workers = []
-        self._executor = None
-        self._lock = threading.Lock()
+    def __init__(self):
 
         try:
             _workers_conf = Config.get('zmq_workers')
-            self._thread_poll_executor_max_workers = int(_workers_conf.get('thread_poll_executor_max_workers', ZEROMQ_MAX_WORKERS))
+            self._thread_poll_executor_max_workers = int(_workers_conf.get(
+                'thread_poll_executor_max_workers', ZEROMQ_MAX_WORKERS))
         except Exception:
             self._thread_poll_executor_max_workers = ZEROMQ_MAX_WORKERS
 
         try:
             _workers_conf = Config.get('zmq_workers')
-            self._max_workers = int(_workers_conf.get('context_max_workers', ZEROMQ_MAX_WORKERS))
+            self._max_workers = int(_workers_conf.get(
+                'context_max_workers', ZEROMQ_MAX_WORKERS))
         except Exception:
             self._max_workers = ZEROMQ_MAX_WORKERS
 
-        Log.info(f'ZMQ: ThreadPoolExecutor max workers: {self._thread_poll_executor_max_workers}')
+        Log.info(
+            f'ZMQ: ThreadPoolExecutor max workers: {self._thread_poll_executor_max_workers}')
         Log.info(f'ZMQ: Context max workers: {self._max_workers}')
 
         self._server_confs = Config.get('zmq_servers')
 
         if not self._server_confs:
             raise Exception('Error to find ZMQ Servers config')
 
         for _server_key in self._server_confs.keys():
 
             _conf = self._server_confs[_server_key]
 
+            self._contexts[_server_key] = zmq.Context(ZEROMQ_CONTEXT)
+
             self._instances[_server_key] = {
                 'server_key': _server_key,
                 'conf': _conf,
                 'url': f"tcp://{_conf.get('host')}:{_conf.get('port')}"
             }
 
         # Cached Routes
         if Config.get('cache'):
             _cache_instance = Cache()
             self._cache = _cache_instance.get_backend()
-            
+
         for _i in range(self._max_workers):
             self.add_worker(f'zmqc-poller-{_i}')
 
-        self._executor = ThreadPoolExecutor(max_workers=self._thread_poll_executor_max_workers, thread_name_prefix=f'zmqc-worker')
+        self._executor = ThreadPoolExecutor(
+            max_workers=self._thread_poll_executor_max_workers, thread_name_prefix='zmqc-worker')
+
+    def get_available_worker(self):
+        return self._available_workers.get()
 
     def add_worker(self, worker_id):
-        
+
         with self._lock:
 
             self._workers[worker_id] = {
-                'context': zmq.Context(ZEROMQ_CONTEXT),
                 'poller': zmq.Poller(),
                 'socket': None
             }
 
         self.free_worker(worker_id)
 
     def get_or_create_socket(self, server_key, worker_id):
@@ -94,238 +105,256 @@
             _worker = self._workers[worker_id]
 
             _socket = _worker['socket']
 
             if _socket is None or _socket.closed:
 
                 _poller = _worker['poller']
-                
+
                 if _socket is not None:
 
                     try:
                         _poller.unregister(_socket)
                     except Exception:
                         pass
-                        
+
                     try:
                         _socket.close(linger=0)
                     except Exception:
                         pass
-                    
-                _socket = _worker['context'].socket(zmq.REQ)
+
+                _socket = self._contexts[server_key].socket(zmq.REQ)
                 _socket.connect(self._instances[server_key]['url'])
                 _socket.setsockopt(zmq.LINGER, 0)
                 _poller.register(_socket, zmq.POLLIN)
 
                 _worker['socket'] = _socket
 
         return _socket
-
-    def free_worker(self, worker_id, close_socket=False):
-
+    
+    def close_and_unregister_socket(self, worker_id):
+        
         with self._lock:
         
-            if close_socket:
+            _worker = self._workers[worker_id]
+            _socket = _worker['socket']
 
-                _worker = self._workers[worker_id]
-                _socket = _worker['socket']
+            if _socket is not None:
 
-                if _socket is not None:
-                    
-                    try:
-                        _worker['poller'].unregister(_socket)
-                    except Exception:
-                        pass
+                try:
+                    _worker['poller'].unregister(_socket)
+                except Exception:
+                    pass
+                
+                try:
+                    _socket.close(linger=0)
+                except Exception:
+                    pass
+                
+                _worker['socket'] = None
 
-                    try:
-                        _socket.close(linger=0)
-                    except Exception:
-                        pass
-                    
-                    _worker['socket'] = None
-            
-            self._available_workers.append(worker_id)
+    def free_worker(self, worker_id, close_socket=False):
+
+        if close_socket:
+            self.close_and_unregister_socket(worker_id)
+
+        self._available_workers.put(worker_id)
 
     def remove_header(self, response, header):
 
         if 'headers' in response and header in response['headers']:
             response['headers'].pop(header, None)
 
     def remove_keys(self, response, keys):
 
         for _key in keys:
-            
-            if _key in response:
-                response.pop(_key, None)
-    
+            response.pop(_key, None)
+
     def send_and_recv_future(self, server_key, message):
         return self._executor.submit(self.send_and_recv, server_key, message)
 
     def send_and_recv(self, server_key, message):
 
         if Log.is_gte_log_level(Log.DEBUG):
             _start = time.time()
-        
+
         _response = None
         _instance = self._instances[server_key]
 
         _is_in_cached_routes = None
 
         if self._cache:
 
-            if _instance['conf'].get('cached_routes') and (
-                    'X-No-Cache' not in message.get('headers', {}).keys() or message.get('headers', {}).get('X-No-Cache') == False):
+            _cached_routes = _instance['conf'].get('cached_routes') 
+
+            if _cached_routes:
+                
+                _message_headers = message.get('headers', {})
+
+                if 'X-No-Cache' not in _message_headers.keys() or _message_headers.get('X-No-Cache') is False:
+
+                    _performative = message['performative']
+                    _resource = message['resource']
+                    _params = message.get('params')
+
+                    _cached_key = f"{_performative}:{'/'.join(_resource.split('/')[:4])}"
+
+                    _is_in_cached_routes = _cached_routes.get(_cached_key)
+
+                    if _is_in_cached_routes:
 
-                _cached_routes = _instance['conf']['cached_routes']
+                        _cached_response = self._cache.get(
+                            _resource,
+                            _performative,
+                            _params
+                        )
 
-                _cached_key = f"{message['performative']}:{'/'.join(message['resource'].split('/')[:4])}"
+                        if _cached_response:
 
-                _is_in_cached_routes = _cached_routes.get(_cached_key)
+                            if Log.is_gte_log_level(Log.DEBUG):
+
+                                Log.debug(
+                                    f">>> ZMQ::cache::get::cached: {_resource} :: {_performative} :: {_params}")
+
+                                _duration = time.time() - _start
 
-                if _is_in_cached_routes:
-                    
-                    _cached_response = self._cache.get(
-                        message['resource'], 
-                        message['performative'], 
-                        message.get('params')
-                    )
-
-                    if _cached_response:
-                        
-                        if Log.is_gte_log_level(Log.DEBUG):
-                            
-                            Log.debug(f">>> ZMQ::cache::get::cached: {message['resource']} :: {message['performative']} :: {message.get('params')}")
-
-                            _duration = time.time() - _start
-                                
-                            Log.debug(f">>> ZMQ::send_and_recv::time:: {_instance['url']} :: {_duration} :: {message} ")
-                        
-                        return _cached_response
+                                Log.debug(
+                                    f">>> ZMQ::send_and_recv::time:: {_instance['url']} :: {_duration} :: {message} ")
+
+                            return _cached_response
 
         try:
 
             while True:
-    
-                # Test without any lock
-                if not self._available_workers:
-                    time.sleep(0.01)
-                    continue
+
+                _worker_id = self.get_available_worker()
 
                 with self._lock:
-                    
-                    # Check again with lock to make sure that the list is not empty
-                    if not self._available_workers:
-                        continue
+                    _worker = self._workers[_worker_id]
 
-                    _worker_id = self._available_workers.pop()
+                _socket = self.get_or_create_socket(server_key, _worker_id)
 
-                _worker = self._workers[_worker_id]
+                _socket.send_multipart(
+                    [b'', envoxy_json_dumps(message)])
 
-                _socket = self.get_or_create_socket(server_key, _worker_id)
-            
-                _socket.send_multipart([b'', json.dumps(message).encode('utf-8')])
-                    
                 try:
 
                     _poller_attempt = 0
-                    
+
                     while True:
-                        
-                        _socks = dict(_worker['poller'].poll(ZEROMQ_POLLIN_TIMEOUT))
+
+                        _socks = dict(_worker['poller'].poll(
+                            ZEROMQ_POLLIN_TIMEOUT))
 
                         if not _socks:
 
                             _poller_attempt += 1
 
                             if _poller_attempt <= ZEROMQ_POLLER_RETRIES:
                                 continue
                             else:
-                                raise NoSocketException(f'No events received in {(ZEROMQ_POLLIN_TIMEOUT/1000)*ZEROMQ_POLLER_RETRIES} secs on {_instance["url"]}')
+                                raise NoSocketException(
+                                    f'No events received in {(ZEROMQ_POLLIN_TIMEOUT/1000)*ZEROMQ_POLLER_RETRIES} secs on {_instance["url"]}')
 
                         if _socks.get(_socket) == zmq.POLLIN:
-                            
+
                             _recv = _socket.recv_multipart()
 
                             self.free_worker(_worker_id)
-                            
-                            _recv.pop(0) # discard delimiter
-                            _response = json.loads(_recv.pop(0).decode('utf-8')) # actual message
-                            
+
+                            _recv.pop(0)  # discard delimiter
+                            _response = envoxy_json_loads(_recv.pop(0))  # actual message
+
                             self.remove_header(_response, 'X-Cid')
-                            
+
                             self.remove_keys(_response, ['protocol', 'performative'])
 
                             if self._cache and _is_in_cached_routes:
 
+                                _performative = message['performative']
+                                _resource = message['resource']
+                                _params = message.get('params')
+
                                 try:
 
-                                    _status_code = int(_response.get('status', 0))
+                                    _status_code = int(
+                                        _response.get('status', 0))
 
                                     if _status_code >= 200 and _status_code < 300:
 
-                                        _ttl = int(_is_in_cached_routes.get('ttl', 3600))
-                                    
+                                        _ttl = int(
+                                            _is_in_cached_routes.get('ttl', 3600))
+
                                     else:
 
-                                        _ttl = int(_is_in_cached_routes.get('error_ttl', 60))
-                                        
+                                        _ttl = int(
+                                            _is_in_cached_routes.get('error_ttl', 60))
+
                                         if Log.is_gte_log_level(Log.ERROR):
-                                            Log.error(f"ZMQ::cache::set::Error: (state_code: {_status_code}, this cached entry will expire in {_ttl} seconds) {message['resource']} :: {message['performative']} :: {message.get('params')}")
+                                            Log.error(f"ZMQ::cache::set::Error: "
+                                                      f"(state_code: {_status_code}, this cached entry will expire in {_ttl} seconds) "
+                                                      f"{_resource} :: {_performative} :: {_params}"
+                                                      )
 
                                     self._cache.set(
-                                        message['resource'], 
-                                        message['performative'], 
-                                        message.get('params'), 
-                                        _response, 
+                                        _resource,
+                                        _performative,
+                                        _params,
+                                        _response,
                                         _ttl
                                     )
 
                                     if Log.is_gte_log_level(Log.DEBUG):
-                                        Log.debug(f">>> ZMQ::cache::set: {message['resource']} :: {message['performative']} :: {message.get('params')}")
+                                        Log.debug(
+                                            f">>> ZMQ::cache::set: {_resource} :: {_performative} :: {_params}")
 
                                 except Exception as e:
-                                    
+
                                     Log.error(f"ZMQ::cache::set::Error: {e}")
-                            
+
                             if Log.is_gte_log_level(Log.DEBUG):
 
                                 _duration = time.time() - _start
-                                
-                                Log.debug(f">>> ZMQ::send_and_recv::time:: {_instance['url']} :: {_duration} :: {message} ")
+
+                                Log.debug(
+                                    f">>> ZMQ::send_and_recv::time:: {_instance['url']} :: {_duration} :: {message} ")
 
                             return _response
-                        
+
                 except IOError:
-                    
-                    Log.error(f"ZMQ::send_and_recv : Could not connect to ZeroMQ machine: {_instance['url']}")
+
+                    Log.error(
+                        f"ZMQ::send_and_recv : Could not connect to ZeroMQ machine: {_instance['url']}")
 
                     self.free_worker(_worker_id, close_socket=True)
 
                     time.sleep(ZEROMQ_RETRY_TIMEOUT)
 
                     return self.send_and_recv(server_key, message)
-    
+
         except NoSocketException as e:
-           
-            Log.warning(f"ZMQ::send_and_recv : It is not possible to send message using the ZMQ server \"{_instance['url']}\". Error: {e}")
+
+            Log.warning(
+                f"ZMQ::send_and_recv : It is not possible to send message using the ZMQ server \"{_instance['url']}\". Error: {e}")
 
             self.free_worker(_worker_id, close_socket=True)
 
             time.sleep(ZEROMQ_RETRY_TIMEOUT)
-            
+
             return self.send_and_recv(server_key, message)
 
         except Exception as e:
-           
-            Log.warning(f"ZMQ::send_and_recv : Unexpected error. It is not possible to send message using the ZMQ server \"{_instance['url']}\". Error: {e}")
+
+            Log.warning(
+                f"ZMQ::send_and_recv : Unexpected error. It is not possible to send message using the ZMQ server \"{_instance['url']}\". Error: {e}")
 
             self.free_worker(_worker_id, close_socket=True)
 
             time.sleep(ZEROMQ_RETRY_TIMEOUT)
-            
+
             return self.send_and_recv(server_key, message)
 
 
 class Dispatcher():
 
     @staticmethod
     def initialize():
@@ -336,62 +365,63 @@
 
     @staticmethod
     def instance():
         return ZMQ.instance()
 
     @staticmethod
     def generate_headers(client_id=None):
-        
+
         _headers = {
             'Accept': 'application/json',
             'Accept-Charset': 'utf-8',
             'Date': Now.api_format(),
             'User-Agent': SERVER_NAME
         }
-        
+
         if client_id:
             _headers['X-Cid'] = client_id
         else:
             _headers['X-Cid'] = str(uuid.uuid4())
-                
+
         return _headers
 
-    @staticmethod    
+    @staticmethod
     def _get_or_create_eventloop():
-        
+
         try:
-            
             return asyncio.get_event_loop()
+        except RuntimeError as _ex:
+
+            if "There is no current event loop in thread" in str(_ex):
+
+                _loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(_loop)
 
-        except RuntimeError as ex:
-            
-            if "There is no current event loop in thread" in str(ex):
-                
-                loop = asyncio.new_event_loop()
-                asyncio.set_event_loop(loop)
-                
                 return asyncio.get_event_loop()
-            
-            raise ex
-    
+
+            raise _ex
+        except Exception as _ex:
+            Log.error(f"Unexpected error in creating event loop: {_ex}")
+            raise
+
     @staticmethod
     def bulk_requests(request_list):
 
         _loop = Dispatcher._get_or_create_eventloop()
 
         _requests = []
-        
+
         for _request in request_list:
 
             assertz_mandatory(_request, 'server_key')
             assertz_string(_request, 'server_key')
-            
+
             assertz_mandatory(_request, 'performative')
             assertz_integer(_request, 'performative')
-            
+
             assertz_mandatory(_request, 'url')
             assertz_uri(_request, 'url')
 
             _message = {
                 'performative': _request['performative'],
                 'resource': _request['url'],
                 'headers': Dispatcher.generate_headers(),
@@ -399,29 +429,29 @@
                 'payload': _request.get('payload')
             }
 
             if 'headers' in _request and _request.get('headers'):
                 _message['headers'].update(dict(_request['headers']))
 
             _requests.append((_request['server_key'], _message))
-        
+
         if _requests:
 
             _executor = ZMQ.instance()._executor
             _func = ZMQ.instance().send_and_recv
-                
+
             _futures = [
-                _loop.run_in_executor(_executor, _func, _server_key, _message) 
+                _loop.run_in_executor(_executor, _func, _server_key, _message)
                 for _server_key, _message in _requests
             ]
 
             return _loop.run_until_complete(asyncio.gather(*_futures)) if _futures else []
-        
+
         return []
-        
+
     @staticmethod
     def get(server_key, url, params=None, payload=None, headers=None, future=False):
 
         _message = {
             'resource': url,
             'headers': Dispatcher.generate_headers(),
             'params': params,
@@ -435,112 +465,118 @@
         if not future:
             return ZMQ.instance().send_and_recv(server_key, _message)
         else:
             return ZMQ.instance().send_and_recv_future(server_key, _message)
 
     @staticmethod
     def post(server_key, url, params=None, payload=None, headers=None, future=False):
-            
+
         _message = {
             'resource': url,
             'headers': Dispatcher.generate_headers(),
             'params': params,
             'payload': payload,
             'performative': Performative.POST
         }
 
         if headers:
             _message['headers'].update(dict(headers))
-        
+
         if not future:
             return ZMQ.instance().send_and_recv(server_key, _message)
         else:
             return ZMQ.instance().send_and_recv_future(server_key, _message)
 
     @staticmethod
     def put(server_key, url, params=None, payload=None, headers=None, future=False):
-            
+
         _message = {
             'resource': url,
             'headers': Dispatcher.generate_headers(),
             'params': params,
             'payload': payload,
             'performative': Performative.PUT
         }
 
         if headers:
             _message['headers'].update(dict(headers))
-        
+
         if not future:
             return ZMQ.instance().send_and_recv(server_key, _message)
         else:
             return ZMQ.instance().send_and_recv_future(server_key, _message)
 
     @staticmethod
     def patch(server_key, url, params=None, payload=None, headers=None, future=False):
-            
+
         _message = {
             'resource': url,
             'headers': Dispatcher.generate_headers(),
             'params': params,
             'payload': payload,
             'performative': Performative.PATCH
         }
-        
+
         if headers:
             _message['headers'].update(dict(headers))
-        
+
         if not future:
             return ZMQ.instance().send_and_recv(server_key, _message)
         else:
             return ZMQ.instance().send_and_recv_future(server_key, _message)
 
     @staticmethod
     def delete(server_key, url, params=None, payload=None, headers=None, future=False):
-            
+
         _message = {
             'resource': url,
             'headers': Dispatcher.generate_headers(),
             'params': params,
             'payload': payload,
             'performative': Performative.DELETE
         }
 
         if headers:
             _message['headers'].update(dict(headers))
-        
+
         if not future:
             return ZMQ.instance().send_and_recv(server_key, _message)
         else:
             return ZMQ.instance().send_and_recv_future(server_key, _message)
 
     @staticmethod
     def head(server_key, url, params=None, payload=None, headers=None, future=False):
-            
+
         _message = {
             'resource': url,
             'headers': Dispatcher.generate_headers(),
             'params': params,
             'payload': payload,
             'performative': Performative.HEAD
         }
 
         if headers:
             _message['headers'].update(dict(headers))
-        
+
         if not future:
             return ZMQ.instance().send_and_recv(server_key, _message)
         else:
             return ZMQ.instance().send_and_recv_future(server_key, _message)
 
     @staticmethod
     def validate_response(response):
 
         if response is None:
             raise ValidationException("Service Unavailable", code=0, status=503)
+        
+        _status = response.get('status', 0)
+        _payload = response.get('payload', {})
 
-        if response.get('status') not in [200, 201] and ('elements' not in response.get('payload') or '_id' not in response.get('payload')):
-            msg = response.get('payload', {}).get('text', f"Resource error, code: {response['status']}, {response['resource']}")
-            code = response.get('payload', {}).get('code', 0)
-            raise ValidationException(msg, code=code, status=str(response.get('status')))
+        if _status not in [200, 201] \
+                and ('elements' not in _payload or '_id' not in _payload):
+            
+            _msg = _payload.get('text', f"Resource error, code: {_status}, {response['resource']}")
+            _code = _payload.get('code', 0)
+            
+            raise ValidationException(_msg, code=_code, status=str(_status))
 
         return response
```

### Comparing `envoxy-0.2.3/src/envoxy/decorators.py` & `envoxy-0.2.4/src/envoxy/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from functools import wraps
+
+import requests
+
 from .auth.backends import AuthBackendMixin
-from .constants import CACHE_DEFAULT_TTL, GET
 from .cache import Cache
+from .constants import CACHE_DEFAULT_TTL, GET
+from .utils.encoders import envoxy_json_loads
 from .utils.logs import Log
-import requests
-import json
+
 
 def on(**kwargs):
 
     def _decorate(klass):
 
         class Meta:
             pass
@@ -28,18 +31,20 @@
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def __call__(self, func):
 
         @wraps(func)
         def wrapped_func(view, request, *args, **kwargs):
-            if self.kwargs: kwargs.update(**self.kwargs)
+            if self.kwargs:
+                kwargs.update(**self.kwargs)
 
             headers = AuthBackendMixin().authenticate(request, *args, **kwargs)
-            if headers: kwargs.update(**headers)
+            if headers:
+                kwargs.update(**headers)
 
             return func(view, request, *args, **kwargs)
         return wrapped_func
 
 
 class cache(object):
 
@@ -61,53 +66,59 @@
 
             if result:
                 return view.cached_response(result)
 
             response = func(view, request, *args, **kwargs)
 
             if response and not result and response.status_code == requests.codes.ok:
-                self.cache.set(_endpoint, _method, _params, response.get_json(), ttl=self.ttl)
+                self.cache.set(_endpoint, _method, _params,
+                               response.get_json(), ttl=self.ttl)
 
             return response
 
         return wrapped_func
 
 
-
 class log_event(object):
 
     def __init__(self, func):
         self.func = func
 
     def __call__(self, client, userdata, msg, **kwargs):
 
         _message = '{} [{}] {}'.format(
             Log.style.apply('< ON_EVENT', Log.style.BOLD),
             Log.style.apply('MQTT', Log.style.GREEN_FG),
             Log.style.apply('{}'.format(msg.topic), Log.style.BLUE_FG)
         )
+
         Log.trace(_message)
 
-        data = json.loads(msg.payload.decode("utf-8"))
-        _message = '{} | Message{}'.format(_message, data)
+        _data = envoxy_json_loads(msg.payload)
+
+        if Log.is_gte_log_level(Log.VERBOSE):
+
+            _message = '{} | Message{}'.format(_message, _data)
 
-        Log.verbose(_message)
+            Log.verbose(_message)
 
-        return self.func(self.func.__class__, data)
+        return self.func(self.func.__class__, _data)
 
 
 class auth_anonymous_allowed(object):
 
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def __call__(self, func):
 
         @wraps(func)
         def wrapped_func(view, request, *args, **kwargs):
-            if self.kwargs: kwargs.update(**self.kwargs)
+            if self.kwargs:
+                kwargs.update(**self.kwargs)
 
             headers = AuthBackendMixin().anonymous(request, *args, **kwargs)
-            if headers: kwargs.update(**headers)
+            if headers:
+                kwargs.update(**headers)
 
             return func(view, request, *args, **kwargs)
         return wrapped_func
```

### Comparing `envoxy-0.2.3/src/envoxy/asserts.py` & `envoxy-0.2.4/src/envoxy/asserts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+import datetime
+import re
+from inspect import getframeinfo, stack
+from uuid import UUID
+
 from requests import codes as status_codes
 
+from .constants import (EMAIL_REGEX, HASH_REGEX, PHONE_REGEX, TOKEN_REGEX,
+                        URI_REGEX, URL_REGEX)
 from .exceptions import ValidationException
-import json
-import datetime
 from .utils.datetime import Now
-from uuid import UUID
-import re
-from .constants import HASH_REGEX, URI_REGEX, EMAIL_REGEX, PHONE_REGEX, TOKEN_REGEX, URL_REGEX
-from inspect import getframeinfo, stack
+from .utils.encoders import envoxy_json_loads
 
 DEFAULT_STATUS_CODE = status_codes.precondition_failed
 INVALID_TYPE_ERROR_CODE = 1202
 
 
 def assertz(_expression, _error_message, _error_code, _status_code):
     """
     :param _expression: a boolean expression to be validated
     :param _error_message: exception message to be passed as "text" param in payload response
     :param _error_code: internal error code
     :param _status_code: HTTP status code to be replied to the invoking HTTP client
     """
     if not _expression:
-        raise ValidationException(_error_message, code=_error_code, status=_status_code)
+        raise ValidationException(
+            _error_message, code=_error_code, status=_status_code)
+
 
 def assertz_reply(_expression, _error_msg, _error_code, _status_code):
     """
     same as assertz but instead of raising exception will return a dictionary
     :param _expression:
     :param _error_msg:
     :param _status_code:
@@ -42,14 +46,15 @@
             "payload": {
                 "text": _error_msg,
                 "code": _error_code,
                 "assertion_failed": f"{caller.code_context} failed on file {_file}, line {_lineno}"
             }
         }
 
+
 def assertz_call(_expression, _error_msg, _error_code, _status_code, reply=False):
     if not reply:
         return assertz(_expression, _error_msg, _error_code, _status_code)
     else:
         return assertz_reply(_expression, _error_msg, _error_code, _status_code)
 
 
@@ -58,88 +63,96 @@
     Validates if an element is part of another object and value should't be an empty string
     when not given and _element only validates _ob
     """
     if isinstance(_element, str) and not _element:
         return assertz_call(_element, "Key must not be emtpy", 1201, _status_code, reply=reply)
     elif _obj and _element is not None:
         return assertz_call(_element in _obj and _element is not None and _obj[_element] is not None, f"Mandatory: {_element}", _error_code,
-                _status_code, reply=reply)
+                            _status_code, reply=reply)
     else:
         return assertz_call(_obj, f"Mandatory: {_obj}", _error_code, _status_code, reply=reply)
 
 
 def assertz_string(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     try:
         value = _element if key is None else _element[key]
     except KeyError:
         return assertz_call(False, f"Invalid value type: {_element}", _error_code, _status_code, reply=reply)
 
     try:
         return assertz_call(isinstance(value, str), f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
     except (AttributeError, TypeError):
         return assertz_call(False, f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
 
+
 def assertz_integer(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     if isinstance(_element, int) and key is None:
         return assertz_call(_element, f"Invalid value type: {_element}", _error_code, _status_code, reply=reply)
     else:
         return assertz_call(key in _element and isinstance(_element[key], int), f"Invalid value type: {_element[key]}", _error_code,
-                _status_code, reply=reply)
+                            _status_code, reply=reply)
 
 
 def assertz_float(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     if isinstance(_element, float) and key is None:
         return assertz_call(_element, f"Invalid value type: {_element}", _error_code, _status_code, reply=reply)
     else:
         return assertz_call(key in _element and isinstance(_element[key], float), f"Invalid value type: {_element[key]}",
-                _error_code, _status_code, reply=reply)
+                            _error_code, _status_code, reply=reply)
 
 
 def assertz_timestamp(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None or isinstance(_element, datetime.date) or isinstance(_element, datetime.date): return None
+    if _element is None or isinstance(_element, datetime.date) or isinstance(_element, datetime.date):
+        return None
 
     if key is None:
         return assertz_call(Now.to_datetime(_element), f"Invalid value type: {_element}", _error_code, _status_code, reply=reply)
     else:
         return assertz_call(key in _element and Now.to_datetime(_element[key]), f"Invalid value type: {_element[key]}", _error_code,
-                _status_code, reply=reply)
+                            _status_code, reply=reply)
 
 
 def assertz_boolean(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     if isinstance(_element, bool) and key is None:
         return assertz_call(_element in [True, False], f"Invalid value type: {_element}", _error_code, _status_code, reply=reply)
     else:
         return assertz_call(key in _element and isinstance(_element[key], bool), f"Invalid value type: {_element[key]}",
-                _error_code, _status_code, reply=reply)
+                            _error_code, _status_code, reply=reply)
 
 
 def assertz_array(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     try:
         value = _element if key is None else _element[key]
     except KeyError:
         return assertz_call(False, f"Invalid value type: {key}", _error_code, _status_code, reply=reply)
 
     try:
         return assertz_call(isinstance(value, list) and value, f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
     except TypeError:
         return assertz_call(False, f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
 
 
 def assertz_dict(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     try:
         value = _element if key is None else _element[key]
     except KeyError:
         return assertz_call(False, f"Invalid value type: {key}", _error_code, _status_code, reply=reply)
 
     try:
@@ -147,31 +160,31 @@
 
     except TypeError:
 
         return assertz_call(False, f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
 
 
 def assertz_json(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     try:
         value = _element if key is None else _element[key]
     except KeyError:
         return assertz_call(False, f"Invalid value type: {key}", _error_code, _status_code, reply=reply)
 
     try:
-        return assertz_call(json.loads(value), f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
-
-    except (json.JSONDecodeError, TypeError):
-
+        return assertz_call(envoxy_json_loads(value), f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
+    except TypeError:
         return assertz_call(False, f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
 
 
 def assertz_complex(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     msg = ""
 
     try:
         is_json = assertz_json(_element, key, _error_code, _status_code)
     except ValidationException as e:
         is_json = False
@@ -189,15 +202,16 @@
         is_array = False
         msg = str(e)
 
     return assertz_call(None in [is_json, is_dict, is_array], msg, _error_code, _status_code, reply=reply)
 
 
 def assertz_uuid(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     try:
         value = _element if key is None else _element[key]
     except KeyError:
         return assertz_call(False, f"Invalid value type: {key}", _error_code, _status_code, reply=reply)
 
     try:
@@ -205,15 +219,16 @@
 
     except (ValueError, AttributeError, TypeError):
 
         return assertz_call(False, f"Invalid value type: {value}", _error_code, _status_code, reply=reply)
 
 
 def assertz_utf8(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     _error_msg = "Invalid utf-8 encoding"
 
     try:
         value = _element if key is None else _element[key]
     except KeyError:
         return assertz_call(False, _error_msg, _error_code, _status_code, reply=reply)
@@ -222,60 +237,70 @@
         return assertz_call(value.encode(encoding='utf-8'), _error_msg, _error_code, _status_code, reply=reply)
     except (UnicodeEncodeError, AttributeError):
 
         return assertz_call(False, _error_msg, _error_code, _status_code, reply=reply)
 
 
 def assertz_ascii(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     _error_msg = "Invalid ascii encoding"
 
     try:
         value = _element if key is None else _element[key]
     except KeyError:
         return assertz_call(False, _error_msg, _error_code, _status_code, reply=reply)
 
     try:
         return assertz_call(value.encode(encoding='ascii'), _error_msg, _error_code, _status_code, reply=reply)
     except (UnicodeEncodeError, AttributeError):
         return assertz_call(False, _error_msg, _error_code, _status_code, reply=reply)
 
+
 def assertz_regex(regex_expr, _error_msg, _element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     try:
         value = _element if key is None else _element[key]
         assertz_string(value)
 
     except (KeyError, ValidationException):
         return assertz_call(False, _error_msg, _error_code, _status_code, reply=reply)
 
     try:
         return assertz_call(re.match(regex_expr, value).group() == value, _error_msg, _error_code, _status_code)
     except (AttributeError, TypeError):
         return assertz_call(False, _error_msg, _error_code, _status_code, reply=reply)
 
+
 def assertz_hash(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
     return assertz_regex(HASH_REGEX, "Invalid hash", _element, key, _error_code, _status_code, reply=reply)
 
+
 def assertz_token(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
     return assertz_regex(TOKEN_REGEX, "Invalid token", _element, key, _error_code, _status_code, reply=reply)
 
+
 def assertz_uri(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
     return assertz_regex(URI_REGEX, "Invalid uri", _element, key, _error_code, _status_code, reply=reply)
 
+
 def assertz_url(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
     return assertz_regex(URL_REGEX, "Invalid url", _element, key, _error_code, _status_code, reply=reply)
 
+
 def assertz_email(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
     return assertz_regex(EMAIL_REGEX, "Invalid email", _element, key, _error_code, _status_code, reply=reply)
 
+
 def assertz_location(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
-    if _element is None: return None
+    if _element is None:
+        return None
 
     _error_msg = "Invalid location"
 
     try:
         value = _element if key is None else _element[key]
     except KeyError:
         return assertz_call(False, _error_msg, _error_code, _status_code, reply=reply)
@@ -286,30 +311,30 @@
 
             _expression = 'latitude' in value and 'longitude' in value \
                           and (isinstance(value['latitude'], int) or isinstance(value['latitude'], float)) \
                           and (isinstance(value['longitude'], int) or isinstance(value['longitude'], float))
 
         elif isinstance(value, list):
             _expression = len(value) == 2 \
-                          and (isinstance(value[0], int) or isinstance(value[0], float)) \
-                          and (isinstance(value[1], int) or isinstance(value[1], float))
+                and (isinstance(value[0], int) or isinstance(value[0], float)) \
+                and (isinstance(value[1], int) or isinstance(value[1], float))
 
         else:
             raise TypeError
 
         return assertz_call(_expression, _error_msg, _error_code, _status_code, reply=reply)
 
-
     except (AttributeError, TypeError):
         return assertz_call(False, _error_msg, _error_code, _status_code, reply=reply)
 
 
 def assertz_phone(_element, key=None, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
     return assertz_regex(PHONE_REGEX, "Invalid phone", _element, key, _error_code, _status_code, reply=reply)
 
+
 def assertz_intersects(x, y, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
     _expression = set(x).intersection(y)
 
     return assertz_call(_expression, f"No intersection between {x} and {y}", _error_code, _status_code, reply=reply)
 
 
 def assertz_unauthorized(_expression, _error_msg, _error_code=INVALID_TYPE_ERROR_CODE, reply=False):
@@ -319,71 +344,90 @@
 def assertz_valid_values(_expression, _error_msg, _error_code=INVALID_TYPE_ERROR_CODE, _status_code=DEFAULT_STATUS_CODE, reply=False):
     return assertz_call(_expression, _error_msg, _error_code, _status_code, reply=reply)
 
 
 def assertz_mandatory_reply(_element, key, _error_code, _status_code):
     return assertz_mandatory(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_string_reply(_element, key, _error_code, _status_code):
     return assertz_string(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_integer_reply(_element, key, _error_code, _status_code):
     return assertz_integer(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_float_reply(_element, key, _error_code, _status_code):
     return assertz_float(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_timestamp_reply(_element, key, _error_code, _status_code):
     return assertz_timestamp(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_boolean_reply(_element, key, _error_code, _status_code):
     return assertz_boolean(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_complex_reply(_element, key, _error_code, _status_code):
     return assertz_complex(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_dict_reply(_element, key, _error_code, _status_code):
     return assertz_dict(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_json_reply(_element, key, _error_code, _status_code):
     return assertz_json(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_array_reply(_element, key, _error_code, _status_code):
     return assertz_array(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_uuid_reply(_element, key, _error_code, _status_code):
     return assertz_uuid(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_utf8_reply(_element, key, _error_code, _status_code):
     return assertz_utf8(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_ascii_reply(_element, key, _error_code, _status_code):
     return assertz_ascii(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_hash_reply(_element, key, _error_code, _status_code):
     return assertz_hash(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_token_reply(_element, key, _error_code, _status_code):
     return assertz_token(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_uri_reply(_element, key, _error_code, _status_code):
     return assertz_uri(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_email_reply(_element, key, _error_code, _status_code):
     return assertz_email(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_location_reply(_element, key, _error_code, _status_code):
     return assertz_location(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_phone_reply(_element, key, _error_code, _status_code):
     return assertz_phone(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_intersects_reply(_element, key, _error_code, _status_code):
     return assertz_intersects(_element, key, _error_code, _status_code, reply=True)
 
+
 def assertz_unauthorized_reply(_element, key, _error_code):
     return assertz_unauthorized(_element, key, _error_code, reply=True)
 
+
 def assertz_valid_values_reply(_element, key, _error_code, _status_code):
     return assertz_valid_values(_element, key, _error_code, _status_code, reply=True)
-
-
```

### Comparing `envoxy-0.2.3/src/envoxy/couchdb/client.py` & `envoxy-0.2.4/src/envoxy/couchdb/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,16 +71,19 @@
 
         server_key = db_data[0]
         database = db_data[1]
 
         host = self._instances[server_key]['conf']['bind']
         url = '{}/{}'.format(host, database)
 
-        if find: url = f'{url}/_find'
-        if uri: url = f'{url}/{uri}'
+        if find: 
+            url = f'{url}/_find'
+
+        if uri: 
+            url = f'{url}/{uri}'
 
         session = self._get_conn(server_key)
 
         try:
 
             Log.debug('couchdb::{} {}'.format(url, data))
             resp = session.request(method, url, json=data)
```

### Comparing `envoxy-0.2.3/src/envoxy/cache/__init__.py` & `envoxy-0.2.4/src/envoxy/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/cache/redis.py` & `envoxy-0.2.4/src/envoxy/cache/redis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import redis
 import base64
-import json
 
-from ..constants import REDIS_DEFAULT_PORT, REDIS_DEFAULT_HOST, REDIS_DEFAULT_DB, REDIS_DEFAULT_TTL
+import redis
+
+from ..constants import REDIS_DEFAULT_DB, REDIS_DEFAULT_HOST, REDIS_DEFAULT_PORT, REDIS_DEFAULT_TTL
+from ..utils.encoders import envoxy_json_dumps, envoxy_json_loads
+
 
 class RedisCache:
 
     def __init__(self, config):
 
         _bind = config.get('bind', '')
         _db = config.get('db', REDIS_DEFAULT_DB)
@@ -19,35 +21,36 @@
         else:
             _host = config.get('host', REDIS_DEFAULT_HOST)
             _port = config.get('port', REDIS_DEFAULT_PORT)
 
         self.r = redis.Redis(host=_host, port=_port, db=_db)
 
     def _encode_params(self, _json_params):
-        _string_params = json.dumps(_json_params)
-        return base64.urlsafe_b64encode(_string_params.encode()).decode()
+        _bytes_params = envoxy_json_dumps(_json_params)
+        return base64.urlsafe_b64encode(_bytes_params).decode()
 
-    def _decode_params(self, _string_params):
-        return json.loads(base64.urlsafe_b64decode(_string_params.encode()).decode())
+    def _decode_params(self, params):
+        return envoxy_json_loads(base64.urlsafe_b64decode(params).decode())
 
-    def _get_key(self, _endpoint, _method, _params):
+    def _get_key(self, endpoint, method, params):
 
-        b64params = self._encode_params(_params)
-        key = f'{self.key_prefix}:{_endpoint}:{_method}:{b64params}'
-        data = self.r.get(key)
-        return json.loads(data) if data else {}
+        _b64params = self._encode_params(params)
+        _key = f'{self.key_prefix}:{endpoint}:{method}:{_b64params}'
+        _data = self.r.get(_key)
+        return envoxy_json_loads(_data) if _data else {}
 
-    def _set_key(self, _endpoint, _method, _params, _json_data, ttl=None):
+    def _set_key(self, endpoint, method, params, json_data, ttl=None):
 
-        b64params = self._encode_params(_params)
-        key = f'{self.key_prefix}:{_endpoint}:{_method}:{b64params}'
-        data = json.dumps(_json_data)
-        self.r.set(key, data)
+        _b64params = self._encode_params(params)
+        _key = f'{self.key_prefix}:{endpoint}:{method}:{_b64params}'
+        _data = envoxy_json_dumps(json_data)
+        self.r.set(_key, _data)
 
         ttl = ttl if ttl else self.ttl
-        return self.r.expire(key, ttl)
+        
+        return self.r.expire(_key, ttl)
 
-    def get(self, _endpoint, _method, _params):
-        return self._get_key(_endpoint, _method, _params)
+    def get(self, endpoint, method, params):
+        return self._get_key(endpoint, method, params)
 
-    def set(self, _endpoint, _method, _params, _json_data, ttl=None):
-        return self._set_key(_endpoint, _method, _params, _json_data, ttl=ttl)
+    def set(self, endpoint, method, params, json_data, ttl=None):
+        return self._set_key(endpoint, method, params, json_data, ttl=ttl)
```

### Comparing `envoxy-0.2.3/src/envoxy/utils/watchdog.py` & `envoxy-0.2.4/src/envoxy/utils/watchdog.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/utils/datetime.py` & `envoxy-0.2.4/src/envoxy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/utils/cache.py` & `envoxy-0.2.4/src/envoxy/utils/cache.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/utils/logs.py` & `envoxy-0.2.4/src/envoxy/utils/logs.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/utils/throttle.py` & `envoxy-0.2.4/src/envoxy/utils/throttle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import time
 from collections import defaultdict
 from functools import wraps
 
 get_time = time.time
 
-__nop = lambda: None
+def __nop():
+    return None
+
 __throttle_last_time = defaultdict(__nop)
 
 def throttle(duration=1, **kw):
     """ 
     Throttle a function on a duration. Prevent it to be called
     more than once within a period.
     For example:
```

### Comparing `envoxy-0.2.3/src/envoxy/utils/singleton.py` & `envoxy-0.2.4/src/envoxy/utils/singleton.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,30 @@
 
 # A per-thread container implementation of Singleton pattern
 # To be used as mixin or base class
 class SingletonPerThread(object):
 
     # private class instances may not necessarily need name-mangling
     __instances = {}
+    # add a lock
+    __lock = threading.Lock()
 
     @classmethod
     def instance(cls):
-        
         _thread_id = threading.get_ident()
         
-        if _thread_id not in cls.__instances:
-            cls.__instances[_thread_id] = cls()
+        with cls.__lock:
+            if _thread_id not in cls.__instances:
+                cls.__instances[_thread_id] = cls()
         
         return cls.__instances[_thread_id]
 
     @classmethod
     def instance_with_queue(cls, queue_):
         
         _thread_id = threading.get_ident()
         
-        if _thread_id not in cls.__instances:
-            cls.__instances[_thread_id] = cls(queue_=queue_)
+        with cls.__lock:
+            if _thread_id not in cls.__instances:
+                cls.__instances[_thread_id] = cls(queue_=queue_)
         
         return cls.__instances[_thread_id]
```

### Comparing `envoxy-0.2.3/src/envoxy/utils/config.py` & `envoxy-0.2.4/src/envoxy/utils/config.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/utils/handlers.py` & `envoxy-0.2.4/src/envoxy/utils/handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-import json
-
-from requests import Response as RequestsResponse
+from encoders import envoxy_json_dumps
 from flask import Response as FlaskResponse
+from requests import Response as RequestsResponse
 
 
 class Handler:
 
     @staticmethod
     def response(response: RequestsResponse) -> FlaskResponse:
         try:
             return FlaskResponse(response.text, response.status_code, headers=response.headers.items())
         except Exception as e:
             return FlaskResponse({'text': e}, 500)
 
     @staticmethod
     def make_response(object_, status) -> FlaskResponse:
-        
+
         if type(object_) in [dict, list]:
-            return FlaskResponse(json.dumps(object_), status, {'Content-Type': 'application/json'})
+            return FlaskResponse(envoxy_json_dumps(object_), status, {'Content-Type': 'application/json'})
         elif type(object_) in [str]:
             return FlaskResponse(object_, status, {'Content-Type': 'text/html'})
         else:
-            return FlaskResponse(json.dumps({'text':'Error in parsing the response object.'}), 500, {'Content-Type': 'text/html'})
+            return FlaskResponse(envoxy_json_dumps({'text': 'Error in parsing the response object.'}), 500, {'Content-Type': 'text/html'})
 
     @staticmethod
     def freeze(object_):
-        
+
         if isinstance(object_, dict):
             return frozenset((key, Handler.freeze(value)) for key, value in object_.items())
         elif isinstance(object_, list):
             return tuple(Handler.freeze(value) for value in object_)
 
-        return object_
+        return object_
```

### Comparing `envoxy-0.2.3/src/envoxy/db/dispatcher.py` & `envoxy-0.2.4/src/envoxy/db/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/tests/test_asserts.py` & `envoxy-0.2.4/src/envoxy/tests/test_asserts.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/tests/fixtures.py` & `envoxy-0.2.4/src/envoxy/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/src/envoxy/auth/backends.py` & `envoxy-0.2.4/src/envoxy/auth/backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,48 @@
+import importlib
 import re
 import sys
-import importlib
 
 import requests
-import datetime
+
 from ..utils.config import Config
 from ..utils.logs import Log
 
+REGEX_VAR_PATTERN = '{(?P<all>(?P<var>[^:]+):(?P<type>[^}]+))}'
+COMPILED_REGEX_VAR_PATTERN = re.compile(REGEX_VAR_PATTERN)
+
 
 def authenticate_container(credentials):
 
-    auth_url = credentials.get("server")
-    data = {
+    _auth_url = credentials.get("server")
+
+    _data = {
         "client_id": credentials.get("client_id"),
         "client_secret": credentials.get("client_secret"),
         "response_type": credentials.get("response_type"),
         "scope": credentials.get("scope"),
         "state": "active"
     }
 
-    if not "" in data.values() and auth_url:
+    if "" not in _data.values() and _auth_url:
+
         try:
-            resp = requests.get(auth_url, params=data)
-            Log.info("Response >> {}".format(resp.status_code))
+            _resp = requests.get(_auth_url, params=_data)
+            Log.info("Response >> {}".format(_resp.status_code))
         except requests.RequestException as e:
             Log.emergency("Error while performing authorization {}".format(e))
             exit(-10)
 
-        if resp.status_code == requests.codes.ok:
-            return resp.json()
+        if _resp.status_code == requests.codes.ok:
+            return _resp.json()
 
     Log.emergency("Authorization data incomplete")
     exit(-10)
 
+
 def get_auth_module(module_name=None):
     _plugins = Config.plugins()
 
     if 'auth' in _plugins.keys():
 
         if _plugins['auth'] not in sys.path:
             sys.path.append(_plugins['auth'])
@@ -49,28 +55,25 @@
         return Auth
     else:
         from ..auth.backends import Auth
         return Auth
 
     return None
 
-def get_topic(_topic):
 
-    REGEX_VAR_PATTERN = '{(?P<all>(?P<var>[^:]+):(?P<type>[^}]+))}'
-    _regex = re.compile(REGEX_VAR_PATTERN)
+def get_topic(_topic):
 
-    for _match in _regex.finditer(_topic):
+    for _match in COMPILED_REGEX_VAR_PATTERN.finditer(_topic):
         _groups = _match.groupdict()
-        var = _groups['var']
-        _topic = _topic.replace(_groups['all'], f"{var}")
+        _var = _groups['var']
+        _topic = _topic.replace(_groups['all'], f"{_var}")
 
     return _topic
 
 
-
 class AuthBackendMixin:
 
     @property
     def AuthorizationException(self):
         AuthBackend = get_auth_module()
         try:
             return AuthBackend.exception
```

### Comparing `envoxy-0.2.3/README.md` & `envoxy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.3/setup.py` & `envoxy-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return os.path.join(data_dir, path)
 
 with open(find_file('README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='envoxy',
-    version='0.2.3',
+    version='0.2.4',
     description='Envoxy Platform Framework',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Matheus (vorjdux) Santos',
     author_email='vorj.dux@gmail.com',
     url='https://github.com/habitio/envoxy',
     packages=find_packages(where='src/', exclude=("tests", "templates")),
```

### Comparing `envoxy-0.2.3/PKG-INFO` & `envoxy-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envoxy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Envoxy Platform Framework
 Home-page: https://github.com/habitio/envoxy
 Author: Matheus (vorjdux) Santos
 Author-email: vorj.dux@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

