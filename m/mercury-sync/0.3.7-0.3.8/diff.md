# Comparing `tmp/mercury-sync-0.3.7.tar.gz` & `tmp/mercury-sync-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.3.7.tar", last modified: Tue Jun 27 18:51:04 2023, max compression
+gzip compressed data, was "mercury-sync-0.3.8.tar", last modified: Tue Jun 27 18:54:29 2023, max compression
```

## Comparing `mercury-sync-0.3.7.tar` & `mercury-sync-0.3.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.126904 mercury-sync-0.3.7/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.126904 mercury-sync-0.3.7/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.126904 mercury-sync-0.3.7/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22565 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.126904 mercury-sync-0.3.7/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.126904 mercury-sync-0.3.7/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/models/ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    39747 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/service/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:51:04.126904 mercury-sync-0.3.7/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-27 18:51:04.000000 mercury-sync-0.3.7/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-27 18:51:04.000000 mercury-sync-0.3.7/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:51:04.000000 mercury-sync-0.3.7/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 18:51:04.000000 mercury-sync-0.3.7/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 18:51:04.000000 mercury-sync-0.3.7/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:51:04.130904 mercury-sync-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-27 18:51:01.000000 mercury-sync-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.165677 mercury-sync-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-27 18:54:29.165677 mercury-sync-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.157677 mercury-sync-0.3.8/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22565 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.165677 mercury-sync-0.3.8/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/models/ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.165677 mercury-sync-0.3.8/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39779 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/service/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.165677 mercury-sync-0.3.8/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.165677 mercury-sync-0.3.8/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:54:29.161677 mercury-sync-0.3.8/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-27 18:54:29.000000 mercury-sync-0.3.8/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-27 18:54:29.000000 mercury-sync-0.3.8/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:54:29.000000 mercury-sync-0.3.8/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 18:54:29.000000 mercury-sync-0.3.8/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 18:54:29.000000 mercury-sync-0.3.8/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:54:29.165677 mercury-sync-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-27 18:54:23.000000 mercury-sync-0.3.8/setup.py
```

### Comparing `mercury-sync-0.3.7/LICENSE` & `mercury-sync-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/PKG-INFO` & `mercury-sync-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.7
+Version: 0.3.8
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.7/README.md` & `mercury-sync-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.3.8/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.3.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.3.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.3.8/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.3.8/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.3.8/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/env/env.py` & `mercury-sync-0.3.8/mercury_sync/env/env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/env/load_env.py` & `mercury-sync-0.3.8/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/env/time_parser.py` & `mercury-sync-0.3.8/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.3.8/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.3.8/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/models/healthcheck.py` & `mercury-sync-0.3.8/mercury_sync/models/healthcheck.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/service/controller.py` & `mercury-sync-0.3.8/mercury_sync/service/controller.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/service/monitor.py` & `mercury-sync-0.3.8/mercury_sync/service/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
                 self._local_health_multiplier = max(
                     0, 
                     self._local_health_multiplier - 1
                 )
 
                 return shard_id, healthcheck
 
-            except asyncio.TimeoutError:
+            except (asyncio.TimeoutError, RuntimeError):
                 self._local_health_multiplier = min(
                     self._local_health_multiplier, 
                     self._max_poll_multiplier
                 ) + 1
                 
         check_host = host
         check_port = port
@@ -1075,15 +1075,15 @@
                     asyncio.create_task(
                         self._run_healthcheck(
                             host,
                             port
                         )
                     )
                 )
-
+                
             await asyncio.sleep(
                 self._poll_interval * (self._local_health_multiplier + 1)
             )
 
     async def _run_state_sync(self):
         while self._running:
```

### Comparing `mercury-sync-0.3.7/mercury_sync/service/service.py` & `mercury-sync-0.3.8/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.3.8/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.3.8/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.3.8/mercury_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.7
+Version: 0.3.8
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.7/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.3.8/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.7/setup.py` & `mercury-sync-0.3.8/setup.py`

 * *Files identical despite different names*

