# Comparing `tmp/mercury-sync-0.3.5.tar.gz` & `tmp/mercury-sync-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.3.5.tar", last modified: Sun Jun 25 08:00:16 2023, max compression
+gzip compressed data, was "mercury-sync-0.3.6.tar", last modified: Tue Jun 27 18:50:05 2023, max compression
```

## Comparing `mercury-sync-0.3.5.tar` & `mercury-sync-0.3.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    41512 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/service/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.608969 mercury-sync-0.3.6/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.608969 mercury-sync-0.3.6/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.608969 mercury-sync-0.3.6/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22566 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.608969 mercury-sync-0.3.6/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.608969 mercury-sync-0.3.6/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/models/ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39747 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/service/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:50:05.608969 mercury-sync-0.3.6/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-27 18:50:05.000000 mercury-sync-0.3.6/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-27 18:50:05.000000 mercury-sync-0.3.6/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:50:05.000000 mercury-sync-0.3.6/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 18:50:05.000000 mercury-sync-0.3.6/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 18:50:05.000000 mercury-sync-0.3.6/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:50:05.612969 mercury-sync-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-27 18:50:01.000000 mercury-sync-0.3.6/setup.py
```

### Comparing `mercury-sync-0.3.5/LICENSE` & `mercury-sync-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/PKG-INFO` & `mercury-sync-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.5
+Version: 0.3.6
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.5/README.md` & `mercury-sync-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.3.6/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,14 +302,32 @@
                 asyncio.sleep(self._cleanup_interval)
             )
 
             await self._sleep_task
 
             for pending in list(self._pending_responses):
                 if pending.done() or pending.cancelled():
+
+                    try:
+                        await pending
+
+                    except (
+                        ConnectionAbortedError,
+                        ConnectionRefusedError,
+                        ConnectionResetError,
+                        asyncio.CancelledError,
+                        asyncio.InvalidStateError,
+                        RuntimeError
+                    ):
+                        await self.close()
+                        await self.connect_async(
+                            cert_path=self._client_cert_path,
+                            key_path=self._client_key_path
+                        )
+
                     self._pending_responses.pop()
 
     async def send(
         self, 
         event_name: bytes,
         data: bytes, 
         address: Tuple[str, int]
@@ -726,14 +744,17 @@
         compressed = self._compressor.compress(encrypted_message)
 
         transport.write(compressed)
         
     async def close(self) -> None:
         self._stream = False
         self._running = False
+
+        for client in self._client_transports.values():\
+            client.abort()
         
         if self._cleanup_task:
             self._cleanup_task.cancel()
             if self._cleanup_task.cancelled() is False:
                 try:
                     self._sleep_task.cancel()
                     if not self._sleep_task.cancelled():
```

### Comparing `mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.3.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.3.6/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.3.6/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         self._decompressor: Union[zstandard.ZstdDecompressor, None] = None
         
         self._running = False
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._sleep_task: Union[asyncio.Task, None] = None
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
         self._max_concurrency = env.MERCURY_SYNC_MAX_CONCURRENCY
+        self.udp_socket: Union[socket.socket, None] = None
 
     def connect(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None,
         worker_socket: Optional[socket.socket]=None
     ) -> None:
@@ -89,40 +90,40 @@
 
         self._semaphore = asyncio.Semaphore(self._max_concurrency)
 
         self._compressor = zstandard.ZstdCompressor()
         self._decompressor = zstandard.ZstdDecompressor()
 
         if worker_socket is None:
-            udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
-            udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            udp_socket.bind((
+            self.udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+            self.udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self.udp_socket.bind((
                 self.host,
                 self.port
             ))
 
-            udp_socket.setblocking(False)
+            self.udp_socket.setblocking(False)
 
         else:
-            udp_socket = worker_socket
+            self.udp_socket = worker_socket
 
 
         if cert_path and key_path:
             self._udp_ssl_context = self._create_udp_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path,
             )
 
-            udp_socket = self._udp_ssl_context.wrap_socket(udp_socket)
+            self.udp_socket = self._udp_ssl_context.wrap_socket(self.udp_socket)
 
         server = self._loop.create_datagram_endpoint(
             lambda: MercurySyncUDPProtocol(
                 self.read
             ),
-            sock=udp_socket
+            sock=self.udp_socket
         )
 
         transport, _ = self._loop.run_until_complete(server)
         self._transport = transport
 
         self._cleanup_task = self._loop.create_task(self._cleanup())
 
@@ -154,40 +155,40 @@
 
         self._semaphore = asyncio.Semaphore(self._max_concurrency)
 
         self._compressor = zstandard.ZstdCompressor()
         self._decompressor = zstandard.ZstdDecompressor()
 
         if worker_socket is None:
-            udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
-            udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            udp_socket.bind((
+            self.udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+            self.udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self.udp_socket.bind((
                 self.host,
                 self.port
             ))
 
-            udp_socket.setblocking(False)
+            self.udp_socket.setblocking(False)
 
         else:
-            udp_socket = worker_socket
+            self.udp_socket = worker_socket
 
 
         if cert_path and key_path:
             self._udp_ssl_context = self._create_udp_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path,
             )
 
-            udp_socket = self._udp_ssl_context.wrap_socket(udp_socket)
+            self.udp_socket = self._udp_ssl_context.wrap_socket(self.udp_socket)
 
         server = self._loop.create_datagram_endpoint(
             lambda: MercurySyncUDPProtocol(
                 self.read
             ),
-            sock=udp_socket
+            sock=self.udp_socket
         )
 
         transport, _ = await server
         self._transport = transport
 
         self._cleanup_task = self._loop.create_task(self._cleanup())
 
@@ -222,14 +223,31 @@
                 asyncio.sleep(self._cleanup_interval)
             )
 
             await self._sleep_task
 
             for pending in list(self._pending_responses):
                 if pending.done() or pending.cancelled():
+                    try:
+                        await pending
+
+                    except (
+                        ConnectionAbortedError,
+                        ConnectionRefusedError,
+                        ConnectionResetError,
+                        asyncio.CancelledError,
+                        asyncio.InvalidStateError
+                    ):
+                        await self.close()
+                        await self.connect_async(
+                            cert_path=self._udp_cert_path,
+                            key_path=self._udp_key_path
+                        )
+                    
+
                     self._pending_responses.pop()
     
     async def send(
         self, 
         event_name: str,
         data: Any, 
         addr: Tuple[str, int]
@@ -431,14 +449,15 @@
 
             encrypted_message = self._encryptor.encrypt(item)
             compressed = self._compressor.compress(encrypted_message)
             self._transport.sendto(compressed, addr)
 
     async def close(self) -> None:
         self._running = False
+        self._transport.abort()
         
         if self._cleanup_task:
             self._cleanup_task.cancel()
             if self._cleanup_task.cancelled() is False:
                 try:
                     self._sleep_task.cancel()
                     if not self._sleep_task.cancelled():
```

### Comparing `mercury-sync-0.3.5/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.3.6/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.3.6/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/env/env.py` & `mercury-sync-0.3.6/mercury_sync/env/env.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 )
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
+    MERCURY_SYNC_UDP_SYNC_INTERVAL: StrictStr='5s'
     MERCURY_SYNC_TCP_CONNECT_RETRIES: StrictInt=3
     MERCURY_SYNC_BOOT_WAIT: StrictStr='3s'
     MERCURY_SYNC_MAX_TIME_IDLE: StrictStr='10s'
     MERCURY_SYNC_IDLE_REBOOT_TIMEOUT: StrictStr='10s'
+    MERCURY_SYNC_POLL_RETRIES: StrictInt=3
     MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD=3
-    MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=2
+    MERCURY_SYNC_MAX_POLL_MULTIPLIER: StrictInt=5
+    MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=4
     MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=7
     MERCURY_SYNC_INITIAL_NODES_COUNT: StrictInt=3
     MERCURY_SYNC_HEALTH_CHECK_TIMEOUT: StrictStr='0.2s'
     MERCURY_SYNC_REGISTRATION_TIMEOUT: StrictStr='1m'
     MERCURY_SYNC_HEALTH_POLL_INTERVAL: StrictFloat='0.2s'
     MERCURY_SYNC_INDIRECT_CHECK_NODES: StrictInt=3
     MERCURY_SYNC_CLEANUP_INTERVAL: StrictStr='10s'
     MERCURY_SYNC_MAX_CONCURRENCY: StrictInt=2048
     MERCURY_SYNC_AUTH_SECRET: StrictStr
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
+            'MERCURY_SYNC_UDP_SYNC_INTERVAL': str,
+            'MERCURY_SYNC_POLL_RETRIES': int,
+            'MERCURY_SYNC_MAX_POLL_MULTIPLIER': int,
             'MERCURY_SYNC_TCP_CONNECT_RETRIES': int,
             'MERCURY_SYNC_MAX_TIME_IDLE': str,
             'MERCURY_SYNC_IDLE_REBOOT_TIMEOUT': str,
             'MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD': int,
             'MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER': int,
             'MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER': int,
             'MERCURY_SYNC_INITIAL_NODES_COUNT': int,
```

### Comparing `mercury-sync-0.3.5/mercury_sync/env/load_env.py` & `mercury-sync-0.3.6/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/env/time_parser.py` & `mercury-sync-0.3.6/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.3.6/mercury_sync/hooks/client_hook.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from mercury_sync.service import Service
 from mercury_sync.service.controller import Controller
 from typing import Union
 
 
 def client(
     call_name: str, 
-    as_tcp: bool=False
+    as_tcp: bool=False,
+    retries: int=3
 ):
 
     def wraps(func):
 
         func.client_only = True
         func.target = call_name
```

### Comparing `mercury-sync-0.3.5/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.3.6/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/service/controller.py` & `mercury-sync-0.3.6/mercury_sync/service/controller.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/service/monitor.py` & `mercury-sync-0.3.6/mercury_sync/service/monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,35 +69,38 @@
         self._registered: Dict[int, Tuple[str, int]] = {}
         self._running = False
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
         self._poll_interval = TimeParser(env.MERCURY_SYNC_HEALTH_POLL_INTERVAL).time
         self._poll_timeout = TimeParser(env.MERCURY_SYNC_HEALTH_CHECK_TIMEOUT).time
         self._reboot_timeout = TimeParser(env.MERCURY_SYNC_IDLE_REBOOT_TIMEOUT).time
         self._max_time_idle = TimeParser(env.MERCURY_SYNC_MAX_TIME_IDLE).time
-        self._tcp_sync_interval = 1
-        self._sync_interval = 1
+        self._poll_retries = env.MERCURY_SYNC_MAX_POLL_MULTIPLIER
+        self._sync_interval = TimeParser(env.MERCURY_SYNC_UDP_SYNC_INTERVAL).time
 
         self._check_nodes_count = env.MERCURY_SYNC_INDIRECT_CHECK_NODES
 
         self.min_suspect_multiplier = env.MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER
         self.max_suspect_multiplier = env.MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER 
         self._min_suspect_node_count = env.MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD
+        self._max_poll_multiplier = env.MERCURY_SYNC_MAX_POLL_MULTIPLIER
         self._local_health_multiplier = 0
-        self._confirmed_suspicions: Dict[Tuple[str, int], int] = {}
+
+        self._confirmed_suspicions: Dict[Tuple[str, int], int] = defaultdict(lambda: 0)
         self._waiter: Optional[asyncio.Future] = None
 
         self._tasks_queue: Deque[asyncio.Task] = deque()
         self._degraded_nodes: Deque[Tuple[str, int]] = deque()
         self._suspect_nodes: Deque[Tuple[str, int]] = deque()
 
         self._degraded_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
         self._suspect_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
+        self._latest_update: Dict[Tuple[str,int], int] = {}
 
         self._local_health_monitor: Union[asyncio.Task, None] = None
-        self._udp_sync_task: Union[asyncio.Task, None] = None
+        self._sync_task: Union[asyncio.Task, None] = None
         self._tcp_sync_task: Union[asyncio.Task, None] = None
 
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._investigating_nodes: Dict[Tuple[str, int], Dict[Tuple[str, int]]] = defaultdict(dict)
         self._node_statuses: Dict[Tuple[str, int], HealthStatus] = {}
 
         self.bootstrap_host: Union[str, None] = None
@@ -105,59 +108,77 @@
 
         self._healthy_statuses = [
             'waiting',
             'healthy'
         ]
 
         self._unhealthy_statuses = [
-            'degraded',
             'suspect',
             'failed'
         ]
 
     @server()
     async def update_node_status(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
-    
+        
         update_node_host = healthcheck.source_host
         update_node_port = healthcheck.source_port
         update_status = healthcheck.status
 
         if healthcheck.target_host and healthcheck.target_port:
             update_node_host = healthcheck.target_host
             update_node_port = healthcheck.target_port
 
         if healthcheck.target_status:
             update_status = healthcheck.target_status
         
-        node_exists = self._node_statuses.get((
+        local_status = self._node_statuses.get((
             update_node_host,
             update_node_port
-        )) is not None
+        ))
 
-        if update_node_host != self.host and update_node_port != self.port and node_exists:
 
-            self._node_statuses[(update_node_host, update_node_port)] = update_status
+        target_last_updated: Union[int, None] = healthcheck.target_last_updated
+        local_last_updated: Union[int, None] = self._latest_update.get((
+            update_node_host,
+            update_node_port
+        ), 0)
+
+        not_self = update_node_host != self.host and update_node_port != self.port
 
-        elif update_node_host != self.host and update_node_port != self.port:
+        if not_self and local_status in self._unhealthy_statuses:
+
+            await self.refresh_clients(
+                HealthCheck(
+                    host=update_node_host,
+                    port=update_node_port,
+                    source_host=self.host,
+                    source_port=self.port,
+                    status=update_status,
+                    error=healthcheck.error
+                )
+            )
+
+        elif not_self and local_status is None:
 
             await self.extend_client(
                 HealthCheck(
                     host=update_node_host,
                     port=update_node_port,
                     source_host=self.host,
                     source_port=self.port,
                     status=self.status,
                     error=healthcheck.error
                 )
             )
 
+        if target_last_updated > local_last_updated:
             self._node_statuses[(update_node_host, update_node_port)] = update_status
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
@@ -170,33 +191,19 @@
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         
         source_host = healthcheck.source_host
         source_port = healthcheck.source_port
 
-        target_host = healthcheck.target_host
-        target_port = healthcheck.target_port
-
         if self.status == 'healthy':
-            self._tasks_queue.append(
-                asyncio.create_task(
-                    self.push_status_update(
-                        host=target_host,
-                        port=target_port,
-                        health_status=self.status,
-                        error_context=self.error_context
-                    )
-                )
-            )
-
             self._local_health_multiplier = min(
-                self._local_health_multiplier + 1, 
-                self.max_suspect_multiplier
-            )
+                self._local_health_multiplier, 
+                self._max_poll_multiplier
+            ) + 1
 
         return HealthCheck(
             host=source_host,
             port=source_port,
             source_host=self.host,
             source_port=self.port,
             status=self.status
@@ -220,145 +227,71 @@
             investigation_update = self._acknowledge_indirect_probe(
                 source_host,
                 source_port,
                 target_host,
                 target_port
             )
 
-
-            indirect_probe = asyncio.wait_for(
-                self.push_health_update(
-                    target_host,
-                    target_port,
-                    self.status,
-                    error_context=healthcheck.error
-                ),
-                timeout=self._poll_timeout * (self._local_health_multiplier + 1)
+            indirect_probe = self._run_healthcheck(
+                target_host,
+                target_port
             )
 
             for task in asyncio.as_completed([
                 investigation_update,
                 indirect_probe
             ]):
-                result: Union[Tuple[int, HealthCheck], None] = await task
-
-                if isinstance(result, tuple):
+                await task
 
-                    self._local_health_multiplier = max(
-                        self._local_health_multiplier - 1, 
-                        0
-                    )
-
-                    _, response = result
-
-                    self._node_statuses[(target_host, target_port)]  = response.status
+                self._local_health_multiplier = max(
+                    self._local_health_multiplier - 1, 
+                    0
+                )
 
-                    # We've received a refutation
-                    return HealthCheck(
-                        host=healthcheck.source_host,
-                        port=healthcheck.source_port,
-                        target_status=response.status,   
-                        source_host=response.source_host,
-                        source_port=response.source_port,
-                        status=response.status,
-                        error=response.error
-                    )
+            # We've received a refutation
+            return HealthCheck(
+                host=healthcheck.source_host,
+                port=healthcheck.source_port,
+                target_status=self._node_statuses.get((target_host, target_port)),   
+                source_host=target_host,
+                source_port=target_port,
+                status=self.status,
+                error=self.error_context
+            )
 
         except asyncio.TimeoutError:
-
             self._local_health_multiplier = min(
-                self._local_health_multiplier + 1, 
-                self.max_suspect_multiplier
-            )
-
-            node_status = self._node_statuses.get((target_host, target_port)) 
-
-            if node_status not in self._unhealthy_statuses or node_status is None:
-                self._node_statuses[(target_host, target_port)] = 'degraded'
-
-                self._degraded_nodes.append((
-                    target_host,
-                    target_port
-                ))
-
-                self._degraded_tasks[(target_host, target_port)] = asyncio.create_task(
-                    self._probe_timed_out_node()
-                )
+                self._local_health_multiplier, 
+                self._max_poll_multiplier
+            ) + 1
 
             # Our suspicion is correct!
             return HealthCheck(
                 host=healthcheck.source_host,
                 port=healthcheck.source_port,
                 source_host=target_host,
                 source_port=target_port,
-                target_status=healthcheck.status, 
+                target_status='suspect', 
                 status=self.status
             )
-        
-    @server()
-    async def register_new_node(
-        self,
-        shard_id: int,
-        healthcheck: HealthCheck
-    ) -> Call[HealthCheck]:
-        source_host = healthcheck.source_host
-        source_port = healthcheck.source_port
-
-        not_self = source_host != self.host and source_port != self.port
-        
-        if not_self:
-
-            suspect_tasks = dict(self._suspect_tasks)
-            suspect_task = suspect_tasks.get((source_host, source_port))
-
-            if suspect_task:
-                await cancel(suspect_task)
-                del suspect_tasks[(source_host, source_port)]
-                
-                self._suspect_tasks = suspect_tasks
-
-
-            local_node_status = self._node_statuses.get((source_host, source_port))
-
-            if local_node_status is None:
-            
-                await self.extend_client(
-                    HealthCheck(
-                        host=source_host,
-                        port=source_port,
-                        source_host=self.host,
-                        source_port=self.port,
-                        status=healthcheck.status,
-                        error=healthcheck.error
-                    )
-                )
-
-            self._node_statuses[(source_host, source_port)] =  'healthy'
-
-        return HealthCheck(
-            host=source_host,
-            port=source_port,
-            source_host=self.host,
-            source_port=self.port,
-            error=self.error_context,
-            status=self.status
-        )
     
     @server()
     async def update_acknowledged(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
-        
         source_host = healthcheck.source_host
         source_port = healthcheck.source_port
         target_host = healthcheck.target_host
         target_port = healthcheck.target_port
 
+        if self._investigating_nodes.get((target_host, target_port)) is None:
+            self._investigating_nodes[(target_host, target_port)] = {}
+
         self._investigating_nodes[(target_host, target_port)].update({
             (source_host, source_port): healthcheck.status
         })
 
         return HealthCheck(
             host=source_host,
             port=source_port,
@@ -369,67 +302,69 @@
         
     @server()
     async def register_health_update(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
-        
+            
         source_host = healthcheck.source_host
         source_port = healthcheck.source_port
 
         target_host = healthcheck.target_host
         target_port = healthcheck.target_port
 
-        if target_host and target_port: 
-            self._node_statuses[(target_host, target_port)] = healthcheck.target_status
-
         local_node_status = self._node_statuses.get((source_host, source_port))
 
         suspect_tasks = dict(self._suspect_tasks)
         suspect_task = suspect_tasks.pop((source_host, source_port), None)
 
         if suspect_task:
-            await cancel(suspect_task)
+            self._tasks_queue.append(
+                asyncio.create_task(
+                    cancel(suspect_task)
+                )
+            )
+
+            del self._suspect_tasks[(source_host, source_port)]
 
             self._suspect_tasks = suspect_tasks
 
-        status_unhealthy = local_node_status == 'failed' or local_node_status == 'suspect'
-            
-        if local_node_status is None or status_unhealthy:
-            
-            monitoring = [
-                address for address, status in self._node_statuses.items() if status == 'healthy'
-            ]
-
-            await asyncio.gather(*[
-                self.push_new_node(
-                    host,
-                    port,
-                    source_host,
-                    source_port,
-                    healthcheck.status,
-                    error_context=healthcheck.error
-                ) for host, port in monitoring
-            ])
 
         if local_node_status is None:
 
             await self.extend_client(
                 HealthCheck(
                     host=source_host,
                     port=source_port,
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
                     error=healthcheck.error
                 )
             )
 
+        elif local_node_status in self._unhealthy_statuses:
+            await self.refresh_clients(
+                HealthCheck(
+                    host=source_host,
+                    port=source_port,
+                    source_host=self.host,
+                    source_port=self.port,
+                    status=healthcheck.status,
+                    error=healthcheck.error
+                )
+            )
+    
+
         self._node_statuses[(source_host, source_port)] = healthcheck.status
+        self._latest_update[(source_host, source_port)] = Snowflake.parse(shard_id).timestamp
+
+        if target_host and target_port: 
+            self._node_statuses[(target_host, target_port)] = healthcheck.target_status
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
             source_status=local_node_status,
@@ -487,47 +422,90 @@
             target_host=target_host,
             target_port=target_port,
             target_status=target_status,
             error=error_context,
             status=health_status
         )
     
-    @client('register_new_node')
-    async def push_new_node(
-        self,
-        host: str,
+    async def _run_tcp_healthcheck(
+        self, 
+        host: str, 
         port: int,
-        source_host: str,
-        source_port: int,
-        health_status: HealthStatus,
-        error_context: Optional[str]=None
-    ) -> Call[HealthCheck]:
-        return HealthCheck(
-            host=host,
-            port=port,
-            source_host=source_host,
-            source_port=source_port,
-            error=error_context,
-            status=health_status
-        )
+        target_host: Optional[str]=None,
+        target_port: Optional[str]=None
+    ) -> Union[Tuple[int, HealthCheck], None]:
+        
+        shard_id: Union[int, None] = None
+        healthcheck: Union[HealthCheck, None] = None
+
+        for _ in range(self._poll_retries):
+
+            try:
+
+                response: Tuple[int, HealthCheck] = await asyncio.wait_for(
+                    self.push_tcp_health_update(
+                        host,
+                        port,
+                        self.status,
+                        target_host=target_host,
+                        target_port=target_port,
+                        error_context=self.error_context
+                    ),
+                    timeout=self._poll_timeout * (self._local_health_multiplier + 1)
+                )
+
+                shard_id, healthcheck = response
+                source_host, source_port = healthcheck.source_host, healthcheck.source_port
+
+                self._node_statuses[(source_host, source_port)] = healthcheck.status
+
+                self._local_health_multiplier = max(
+                    0, 
+                    self._local_health_multiplier - 1
+                )
+
+                return shard_id, healthcheck
+
+            except asyncio.TimeoutError:
+                self._local_health_multiplier = min(
+                    self._local_health_multiplier, 
+                    self._max_poll_multiplier
+                ) + 1
+                
+        check_host = host
+        check_port = port
+
+        if target_host and target_port:
+            check_host = target_host
+            check_port = target_port
+
+        if healthcheck is None and self._node_statuses.get((check_host, check_port)) == 'healthy':
+            self._node_statuses[(check_host, check_port)] = 'suspect'
+
+            self._suspect_nodes.append((
+                check_host,
+                check_port
+            ))
+
+            self._suspect_tasks[(host, port)] = asyncio.create_task(
+                self._start_suspect_monitor()
+            )
+
+        return shard_id, healthcheck
     
     @client('update_acknowledged')
     async def push_acknowledge_check(
         self,
         host: str,
         port: int,
         target_host: str,
         target_port: int,
         health_status: HealthStatus,
-        timeout: float,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
-        
-        await asyncio.sleep(0.8 * timeout)
-
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             target_host=target_host,
             target_port=target_port,
@@ -566,24 +544,32 @@
         health_status: HealthStatus,
         target_host: Optional[str]=None,
         target_port: Optional[int]=None,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
         
         target_status: Union[HealthStatus, None] = None
+        target_last_updated: Union[int,  None] = self._latest_update.get(
+            (host, port), 0
+        )
+
         if target_host and target_port:
             target_status = self._node_statuses.get((target_host, target_port))
+            target_last_updated = self._latest_update.get(
+                (target_host, target_port), 0
+            )
 
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             target_host=target_host,
             target_port=target_port,
+            target_last_updated=target_last_updated,
             target_status=target_status,
             status=health_status,
             error=error_context
         )
     
     @client('update_node_status', as_tcp=True)
     async def push_tcp_status_update(
@@ -613,24 +599,20 @@
         )
     
     @client('update_as_suspect')
     async def push_suspect_update(
         self,
         host: str,
         port: int,
-        target_host: str,
-        target_port: int,
         health_status: HealthStatus,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
         return HealthCheck(
             host=host,
             port=port,
-            target_host=target_host,
-            target_port=target_port,
             source_host=self.host,
             source_port=self.port,
             status=health_status,
             error=error_context
         )
     
     async def start(self):
@@ -673,49 +655,47 @@
             self.start_health_monitor()
         )
         
         self.confirmation_task = asyncio.create_task(
             self.cleanup_pending_checks()
         )
 
-        self._udp_sync_task = asyncio.create_task(
+        self._sync_task = asyncio.create_task(
             self._run_state_sync()
         )
 
     def _calculate_min_suspect_timeout(self):
-        nodes_count = len({
-            address: status for address, status in self._node_statuses.items() if status != 'failed'
-        }) + 1
+        nodes_count = len(self._node_statuses) + 1
 
-        poll_timeout = self._poll_timeout * (self._local_health_multiplier + 1)
+        poll_interval = self._poll_interval * (self._local_health_multiplier + 1)
 
         return round(
-            self.min_suspect_multiplier * math.log10(nodes_count) * poll_timeout,
-            4
+            self.min_suspect_multiplier * math.log10(nodes_count) * poll_interval,
+            2
         )
 
     def _calculate_max_suspect_timeout(self, min_suspect_timeout: float):
         
         return round(
             self.max_suspect_multiplier * min_suspect_timeout,
-            4
+            2
         )
 
     def _calculate_suspicion_timeout(
         self,
         suspect_node_address: Tuple[str, int]
     ):
 
         min_suspect_timeout = self._calculate_min_suspect_timeout()
         
         max_suspect_timeout = self._calculate_max_suspect_timeout(min_suspect_timeout)
 
         confirmed_suspect_count = max(
             0,
-            self._confirmed_suspicions[suspect_node_address] - 1
+            self._confirmed_suspicions[suspect_node_address]
         )
 
         timeout_modifier = math.log(
             confirmed_suspect_count + 1
         )/math.log(self._min_suspect_node_count + 1)
 
         timeout_difference = max_suspect_timeout - min_suspect_timeout
@@ -729,298 +709,234 @@
         self,
         host: str,
         port: int,
         target_host: str,
         target_port: int
     ):
         try:
-            
             timeout = self._poll_timeout * (self._local_health_multiplier + 1)
             response: Tuple[int, HealthCheck] = await asyncio.wait_for(
                 self.push_acknowledge_check(
                     host,
                     port,
                     target_host,
                     target_port,
                     self.status,
-                    timeout,
                     error_context=self.error_context
                 ),
                 timeout=timeout
             )
 
             _, healthcheck = response
+
             source_host, source_port = healthcheck.source_host, healthcheck.source_port
 
             self._node_statuses[(source_host, source_port)] = healthcheck.status
 
             self._local_health_multiplier = max(
                 0, 
                 self._local_health_multiplier - 1
             )
 
         except asyncio.TimeoutError:
             self._local_health_multiplier = min(
-                self._local_health_multiplier + 1, 
-                self.max_suspect_multiplier
-            )
-
-            node_status = self._node_statuses.get((host, port)) 
+                self._local_health_multiplier, 
+                self._max_poll_multiplier
+            ) + 1
 
-            if node_status and node_status not in self._unhealthy_statuses:
-                self._node_statuses[(host, port)] = 'degraded'
+            if self._node_statuses.get((host, port)) == 'healthy':
+                self._node_statuses[(host, port)] = 'suspect'
 
-                self._degraded_nodes.append((
+                self._suspect_nodes.append((
                     host,
                     port
                 ))
 
-                self._degraded_tasks[(host, port)] = asyncio.create_task(
-                    self._probe_timed_out_node()
+                self._suspect_tasks[(host, port)] = asyncio.create_task(
+                    self._start_suspect_monitor()
                 )
 
     async def _run_healthcheck(
         self, 
         host: str, 
         port: int,
         target_host: Optional[str]=None,
         target_port: Optional[str]=None
-    ):
-
-        try:
-
-            response: Tuple[int, HealthCheck] = await asyncio.wait_for(
-                self.push_health_update(
-                    host,
-                    port,
-                    self.status,
-                    target_host=target_host,
-                    target_port=target_port,
-                    error_context=self.error_context
-                ),
-                timeout=self._poll_timeout * (self._local_health_multiplier + 1)
-            )
-
-            _, healthcheck = response
-            source_host, source_port = healthcheck.source_host, healthcheck.source_port
-
-            self._node_statuses[(source_host, source_port)] = healthcheck.status
-
-            self._local_health_multiplier = max(
-                0, 
-                self._local_health_multiplier - 1
-            )
+    ) -> Union[Tuple[int, HealthCheck], None]:
+        
+        shard_id: Union[int, None] = None
+        healthcheck: Union[HealthCheck, None] = None
 
-        except asyncio.TimeoutError:
-            self._local_health_multiplier = min(
-                self._local_health_multiplier + 1, 
-                self.max_suspect_multiplier
-            )
+        for _ in range(self._poll_retries):
 
-            if self._node_statuses[(host, port)] not in self._unhealthy_statuses:
-                self._node_statuses[(host, port)] = 'degraded'
+            try:
 
-                self._degraded_nodes.append((
-                    host,
-                    port
-                ))
-
-                self._degraded_tasks[(host, port)] = asyncio.create_task(
-                    self._probe_timed_out_node()
+                response: Tuple[int, HealthCheck] = await asyncio.wait_for(
+                    self.push_health_update(
+                        host,
+                        port,
+                        self.status,
+                        target_host=target_host,
+                        target_port=target_port,
+                        error_context=self.error_context
+                    ),
+                    timeout=self._poll_timeout * (self._local_health_multiplier + 1)
                 )
 
-    async def _probe_timed_out_node(self):
-        
-        suspect_host, suspect_port = self._degraded_nodes.pop()
-        
-        confirmation_members = self._get_confirmation_members()
-
-        healthchecks, suspect_count = await self._request_indirect_probe(
-            suspect_host,
-            suspect_port,
-            confirmation_members
-        )
-
-        self._confirmed_suspicions[(suspect_host, suspect_port)] = len([
-            check for _, check in healthchecks if check.target_status == 'suspect'
-        ])
-
-        indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
-        self._local_health_multiplier = max(
-            0,
-            self._local_health_multiplier - indirect_ack_count
-        )
+                shard_id, healthcheck = response
+                source_host, source_port = healthcheck.source_host, healthcheck.source_port
 
+                self._node_statuses[(source_host, source_port)] = healthcheck.status
 
-        missing_ack_count = len(confirmation_members) - indirect_ack_count
-        
-        next_health_multiplier = self._local_health_multiplier + missing_ack_count - indirect_ack_count
-        if next_health_multiplier < 0:
-            self._local_health_multiplier = 0
+                self._local_health_multiplier = max(
+                    0, 
+                    self._local_health_multiplier - 1
+                )
 
-        else:
-            self._local_health_multiplier = min(
-                next_health_multiplier, 
-                self.max_suspect_multiplier
-            )
+                return shard_id, healthcheck
 
-        confirmation_members_count = len(confirmation_members)
+            except asyncio.TimeoutError:
+                self._local_health_multiplier = min(
+                    self._local_health_multiplier, 
+                    self._max_poll_multiplier
+                ) + 1
 
-        if suspect_count >= confirmation_members_count:
+        check_host = host
+        check_port = port
 
-            self._node_statuses[(suspect_host, suspect_port)] = 'suspect'
+        if target_host and target_port:
+            check_host = target_host
+            check_port = target_port
 
-            self._tasks_queue.append(
-                asyncio.create_task(
-                    self._push_suspect_update(
-                        host=suspect_host,
-                        port=suspect_port,
-                        target_host=suspect_host,
-                        target_port=suspect_port,
-                        health_status=self.status,
-                        error_context=self.error_context
-                    )
-                )
-            )
+        if healthcheck is None and self._node_statuses.get((check_host, check_port)) == 'healthy':
+            self._node_statuses[(check_host, check_port)] = 'suspect'
 
-            self._suspect_nodes.append((suspect_host, suspect_port))
+            self._suspect_nodes.append((
+                check_host,
+                check_port
+            ))
 
-            self._suspect_tasks[(suspect_host, suspect_port)] = asyncio.create_task(
+            self._suspect_tasks[(host, port)] = asyncio.create_task(
                 self._start_suspect_monitor()
             )
 
-        else:
-            self._node_statuses[(suspect_host, suspect_port)] = 'healthy' 
-            self.status = 'healthy'
-
-        if self._investigating_nodes.get((suspect_host, suspect_port)):
-            del self._investigating_nodes[(suspect_host, suspect_port)]
+        return shard_id, healthcheck
 
     async def _start_suspect_monitor(self):
 
-        elapsed = 0
-        start = time.monotonic()
-
-    
         if len(self._suspect_nodes) < 1:
             return
         
         address = self._suspect_nodes.pop()
         suspect_host, suspect_port = address
-
-        confirmation_task = self._degraded_tasks.get((suspect_host, suspect_port))
-        if confirmation_task:
-            await cancel(confirmation_task)
-            confirmation_task.cancel()
-
-        node_status = self._node_statuses[(suspect_host, suspect_port)]
         
         suspicion_timeout = self._calculate_suspicion_timeout(address)
 
-        while elapsed < suspicion_timeout and node_status == 'suspect':
+
+        elapsed = 0
+        start = time.monotonic()
+
+        while elapsed < suspicion_timeout and self._node_statuses[(suspect_host, suspect_port)] == 'suspect':
 
             self._tasks_queue.append(
                 asyncio.create_task(
                     self._push_suspect_update(
                         host=suspect_host,
                         port=suspect_port,
-                        target_host=suspect_host,
-                        target_port=suspect_port,
                         health_status=self.status,
                         error_context=self.error_context
                     )
                 )
             )
                 
-            confirmation_members = self._get_confirmation_members()
+            confirmation_members = self._get_confirmation_members((
+                suspect_host,
+                suspect_port
+            ))
 
-            healthchecks, suspect_count = await self._request_indirect_probe(
+            suspect_count = await self._request_indirect_probe(
                 suspect_host,
                 suspect_port,
                 confirmation_members
             )
 
-            self._confirmed_suspicions[(suspect_host, suspect_port)] = len([
-                check for _, check in healthchecks if check.target_status == 'suspect'
-            ])
-            
-            indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
-            self._local_health_multiplier = max(
+            self._confirmed_suspicions[(suspect_host, suspect_port)] += max(
                 0,
-                self._local_health_multiplier - indirect_ack_count
+                suspect_count - 1
             )
 
+            indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
 
             missing_ack_count = len(confirmation_members) - indirect_ack_count
-            
+
             next_health_multiplier = self._local_health_multiplier + missing_ack_count - indirect_ack_count
             if next_health_multiplier < 0:
                 self._local_health_multiplier = 0
 
             else:
                 self._local_health_multiplier = min(
                     next_health_multiplier, 
-                    self.max_suspect_multiplier
-                )
+                    self._max_poll_multiplier
+                ) + 1
 
             confirmation_members_count = len(confirmation_members)
 
             if suspect_count < confirmation_members_count:
                 # We had a majority confirmation the node was healthy.
+                self._investigating_nodes[(suspect_host, suspect_port)] = {}
+                self._confirmed_suspicions[(suspect_host, suspect_port)] = 0
 
                 self._node_statuses[(suspect_host, suspect_port)] = 'healthy'
 
-                await self._propagate_state_update(
-                    suspect_host,
-                    suspect_port
-                )
-
-            if self._investigating_nodes.get((suspect_host, suspect_port)):
-                del self._investigating_nodes[(suspect_host, suspect_port)]
-
+                break
+            
             await asyncio.sleep(
                 self._poll_interval * (self._local_health_multiplier + 1)
             ) 
 
             elapsed = time.monotonic() - start
-
             suspicion_timeout = self._calculate_suspicion_timeout(address)
 
         if self._node_statuses[(suspect_host, suspect_port)] == 'suspect':
             self._node_statuses[(suspect_host, suspect_port)] = 'failed'
+        
+        self._investigating_nodes[(suspect_host, suspect_port)] = {}
+        self._confirmed_suspicions[(suspect_host, suspect_port)] = 0
             
-    def _get_confirmation_members(self) -> List[Tuple[str, int]]:
+    def _get_confirmation_members(self, suspect_address: Tuple[str, int]) -> List[Tuple[str, int]]:
+
         confirmation_members = [
-            address for address, status in self._node_statuses.items() if status in self._healthy_statuses
+            address for address in self._node_statuses.keys() if address != suspect_address
         ]
 
         confirmation_members_count = len(confirmation_members)
 
+        if self._check_nodes_count > confirmation_members_count:
+            self._check_nodes_count = confirmation_members_count
+            
         confirmation_members = random.sample(
             confirmation_members, 
-            confirmation_members_count
+            self._check_nodes_count
         )
 
         return confirmation_members
 
     async def _request_indirect_probe(
         self,
         host: str,
         port: int,
         confirmation_members: List[Tuple[str, int]]
     ) -> Tuple[List[Call[HealthCheck]], int]:
 
         if len(confirmation_members) < 1:
             requested_checks = [
                 asyncio.create_task(
-                    self.push_tcp_health_update(
+                    self._run_tcp_healthcheck(
                         host,
-                        port,
-                        self.status,
-                        error_context=self.error_context
+                        port
                     )
                 )
             ]
         
         else:
             requested_checks = [
                 asyncio.create_task(
@@ -1033,31 +949,47 @@
                         error_context=self.error_context
                     )
                 ) for node_host, node_port in confirmation_members
             ]
 
             requested_checks.append(
                 asyncio.create_task(
-                    self.push_tcp_health_update(
+                    self._run_tcp_healthcheck(
                         host,
-                        port,
-                        self.status,
-                        error_context=self.error_context
+                        port
                     )
                 )
             )
 
         check_tasks: Tuple[List[asyncio.Task], List[asyncio.Task]] = await asyncio.wait(
             requested_checks, 
             timeout=self._poll_timeout * (self._local_health_multiplier + 1)
         )
 
         completed, pending = check_tasks
 
-        healthchecks: List[Call[HealthCheck]]  = await asyncio.gather(*completed)
+        results: List[Call[HealthCheck]]  = await asyncio.gather(
+            *completed,
+            return_exceptions=True
+        )
+
+        healthchecks = [
+            result for result in results if isinstance(
+                result,
+                tuple
+            )
+        ]
+
+        errors = [
+            result for result in results if isinstance(
+                result,
+                tuple
+            ) is False
+        ]
+
         sorted_checks: List[Call[HealthCheck]] = list(sorted(
             healthchecks,
             key=lambda check: Snowflake.parse(
                 Snowflake.parse(check[0]).timestamp
             ).timestamp
         ))
 
@@ -1070,36 +1002,40 @@
 
         healthy = [
             (
                 shard_id,
                 check
             ) for shard_id, check in sorted_checks if check.target_status == 'healthy'
         ]
+            
+        if len(healthy) < 1:
+            suspect_count = len(suspect) + len(pending) + len(errors)
 
-        suspect_checks: List[Call[HealthCheck]] = []
-        for suspect_shard_id, suspect_check in suspect:
+        else:
+            suspect_checks: List[Call[HealthCheck]] = []
+            for suspect_shard_id, suspect_check in suspect:
 
-            newer_count = 0
-            for healthy_shard_id, _ in healthy:
-                if suspect_shard_id > healthy_shard_id:
-                    newer_count += 1
-
-            if newer_count >= len(healthy):
-                suspect_checks.append((
-                    suspect_shard_id,
-                    suspect_check
-                ))
+                newer_count = 0
+                for healthy_shard_id, _ in healthy:
+                    if suspect_shard_id > healthy_shard_id:
+                        newer_count += 1
+
+                if newer_count >= len(healthy):
+                    suspect_checks.append((
+                        suspect_shard_id,
+                        suspect_check
+                    ))
 
-        suspect_count = len(suspect_checks) + len(pending)
+            suspect_count = len(suspect_checks) + len(pending) + len(errors)
         
         await asyncio.gather(*[
             cancel(pending_check) for pending_check in pending
         ])
 
-        return healthchecks, suspect_count
+        return suspect_count
     
     async def _propagate_state_update(
         self,
         target_host: str,
         target_port: int
     ):
         monitoring = [
@@ -1116,46 +1052,38 @@
             )
 
     async def run_forever(self):
         self._waiter = asyncio.Future()
         await self._waiter
 
     async def start_health_monitor(self):
-        
-        monitor_idx = 0
 
         while self._running:
 
-            monitors = [
-                address for address, status in self._node_statuses.items() if status == 'healthy'
-            ]
+            monitors = list(self._node_statuses.keys())
 
             host: Union[str, None] = None
             port: Union[int, None] = None
 
             monitors_count = len(monitors)
 
             if monitors_count > 0:
+                host, port = random.choice(monitors)
 
-                monitor_idx = monitor_idx%monitors_count
-                host, port = monitors[monitor_idx]
-
-            if self._node_statuses.get((host, port)):
+            if self._node_statuses.get((host, port)) == 'healthy':
         
                 self._tasks_queue.append(
                     asyncio.create_task(
                         self._run_healthcheck(
                             host,
                             port
                         )
                     )
                 )
 
-            monitor_idx += 1
-
             await asyncio.sleep(
                 self._poll_interval * (self._local_health_multiplier + 1)
             )
 
     async def _run_state_sync(self):
         while self._running:
 
@@ -1172,86 +1100,96 @@
                         self._push_state_to_node(
                             host=host,
                             port=port
                         )
                     ) for host, port in monitors
                 ])
 
-                self._tasks_queue.extend([
-                    asyncio.create_task(
-                        self._push_state_to_node_tcp(
-                            host=host,
-                            port=port
-                        )
-                    ) for host, port in monitors
-                ])
-
-                self._sync_interval = round(
-                    math.log10(active_nodes_count + 1),
-                    2
-                ) * (active_nodes_count + 1)
-
             await asyncio.sleep(
-                max(
-                    self._sync_interval,
-                    1
-                )
+                self._sync_interval
             )
 
     async def _push_state_to_node(
         self,
         host: str,
         port: int
     ):
-        await asyncio.gather(*[
+        
+        updates = [
             self._push_status_update(
                 host=host,
                 port=port,
                 target_host=node_host,
                 target_port=node_port
-            ) for node_host, node_port in self._node_statuses
-        ])
+            ) for node_host, node_port in self._node_statuses if self._node_statuses.get((
+                node_host,
+                node_port
+            )) == 'healthy' and host != node_host and port != node_port
+        ]
+
+        if len(updates) > 0:
+            await asyncio.gather(*updates)
 
     async def _push_state_to_node_tcp(
         self,
         host: str,
         port: int
     ):
-        await asyncio.gather(*[
-            self._push_tcp_status_update(
-                host=host,
-                port=port,
-                target_host=node_host,
-                target_port=node_port
-            ) for node_host, node_port in self._node_statuses
-        ])
+        
+        if self._node_statuses.get((host, port)) != 'failed':
+            await asyncio.gather(*[
+                self._push_tcp_status_update(
+                    host=host,
+                    port=port,
+                    target_host=node_host,
+                    target_port=node_port
+                ) for node_host, node_port in self._node_statuses
+            ])
 
     async def _push_status_update(
         self,
         host: str,
         port: int,
         target_host: Optional[str]=None,
         target_port: Optional[int]=None
-    ):
+    ) -> Tuple[
+            Union[int, None], 
+            Union[HealthCheck, None]
+        ]:
         
-        try:
+        shard_id: Union[int, None] = None
+        healthcheck: Union[HealthCheck, None] = None
 
-            await asyncio.wait_for(
-                self.push_status_update(
-                    host=host,
-                    port=port,
-                    target_host=target_host,
-                    target_port=target_port,
-                    health_status=self.status
-                ),
-                timeout=self._poll_timeout * (self._local_health_multiplier + 1)
-            )
+        for _ in range(self._poll_retries):
 
-        except asyncio.TimeoutError:
-            pass
+            try:
+
+                response: Tuple[int, HealthCheck] = await asyncio.wait_for(
+                    self.push_status_update(
+                        host,
+                        port,
+                        self.status,
+                        target_host=target_host,
+                        target_port=target_port,
+                        error_context=self.error_context
+                    ),
+                    timeout=self._poll_timeout * (self._local_health_multiplier + 1)
+                )
+
+                shard_id, healthcheck = response
+                source_host, source_port = healthcheck.source_host, healthcheck.source_port
+
+                self._node_statuses[(source_host, source_port)] = healthcheck.status
+
+                return shard_id, healthcheck
+
+            except asyncio.TimeoutError:
+                pass
+
+        return shard_id, healthcheck
 
     async def _push_tcp_status_update(
         self,
         host: str,
         port: int,
         target_host: Optional[str]=None,
         target_port: Optional[int]=None
@@ -1273,42 +1211,52 @@
         except asyncio.TimeoutError:
             pass
 
     async def _push_suspect_update(
         self,
         host: str,
         port: int,
-        target_host: str,
-        target_port: int,
         health_status: HealthStatus,
         error_context: Optional[str]=None
     ):
         
         try:
-            await asyncio.wait_for(
+            response: Tuple[int, HealthCheck] = await asyncio.wait_for(
                 self.push_suspect_update(
                     host=host,
                     port=port,
-                    target_host=target_host,
-                    target_port=target_port,
                     health_status=health_status,
                     error_context=error_context
                 ),
                 timeout=self._poll_timeout * (self._local_health_multiplier + 1)
             )
 
+            _, healthcheck = response
+
+            self._node_statuses[(host, port)] = healthcheck.status
+
         except asyncio.TimeoutError:
             pass
 
     async def cleanup_pending_checks(self):
 
         while self._running:
 
             for pending_check in list(self._tasks_queue):
                 if pending_check.done() or pending_check.cancelled():
+                    try:
+                        await pending_check
+
+                    except (
+                        ConnectionRefusedError,
+                        ConnectionAbortedError,
+                        ConnectionResetError
+                    ):
+                        pass
+
                     self._tasks_queue.remove(pending_check)
 
             await asyncio.sleep(self._cleanup_interval)
     
     async def shutdown(self):
         self._running = False
         self._local_health_monitor.cancel()
@@ -1321,15 +1269,15 @@
             cancel(remote_check) for remote_check in self._healthchecks.values()
         ])
 
         await cancel(self._local_health_monitor)
         
         await cancel(self._cleanup_task)
 
-        await cancel(self._udp_sync_task)
+        await cancel(self._sync_task)
 
         await self.close()
 
     async def soft_shutdown(self):
         await asyncio.gather(*[
             cancel(check) for check in self._tasks_queue
         ])
```

### Comparing `mercury-sync-0.3.5/mercury_sync/service/service.py` & `mercury-sync-0.3.6/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.3.6/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.3.6/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.3.6/mercury_sync.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.5
+Version: 0.3.6
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.5/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.3.6/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.5/setup.py` & `mercury-sync-0.3.6/setup.py`

 * *Files identical despite different names*

