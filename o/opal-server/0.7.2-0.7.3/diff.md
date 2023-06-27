# Comparing `tmp/opal-server-0.7.2.tar.gz` & `tmp/opal-server-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-server-0.7.2.tar", last modified: Tue Jun 20 15:19:32 2023, max compression
+gzip compressed data, was "opal-server-0.7.3.tar", last modified: Tue Jun 27 11:25:37 2023, max compression
```

## Comparing `opal-server-0.7.2.tar` & `opal-server-0.7.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.128324 opal-server-0.7.2/
--rw-r--r--   0 roekatz    (501) staff       (20)     9134 2023-06-20 15:19:32.127933 opal-server-0.7.2/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.118151 opal-server-0.7.2/opal_server/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11023 2023-06-03 11:34:06.000000 opal-server-0.7.2/opal_server/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.121381 opal-server-0.7.2/opal_server/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5303 2023-06-18 09:48:03.000000 opal-server-0.7.2/opal_server/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6169 2023-06-20 13:37:00.000000 opal-server-0.7.2/opal_server/data/data_update_publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)    13130 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/git_fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/loadlimiting.py
--rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.121711 opal-server-0.7.2/opal_server/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/policy/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.122801 opal-server-0.7.2/opal_server/policy/bundles/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/policy/bundles/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4447 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/policy/bundles/api.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.124384 opal-server-0.7.2/opal_server/policy/watcher/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/policy/watcher/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4529 2023-06-18 09:48:03.000000 opal-server-0.7.2/opal_server/policy/watcher/callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6422 2023-06-03 11:34:06.000000 opal-server-0.7.2/opal_server/policy/watcher/factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4568 2023-06-18 09:48:03.000000 opal-server-0.7.2/opal_server/policy/watcher/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.125321 opal-server-0.7.2/opal_server/policy/webhook/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/policy/webhook/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5691 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/policy/webhook/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/policy/webhook/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/policy/webhook/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3659 2023-06-18 09:46:46.000000 opal-server-0.7.2/opal_server/pubsub.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1390 2023-05-09 07:59:18.000000 opal-server-0.7.2/opal_server/redis.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.126455 opal-server-0.7.2/opal_server/scopes/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/scopes/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12555 2023-06-18 09:48:03.000000 opal-server-0.7.2/opal_server/scopes/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/scopes/loader.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1325 2023-05-09 07:59:18.000000 opal-server-0.7.2/opal_server/scopes/scope_repository.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7256 2023-06-20 13:37:00.000000 opal-server-0.7.2/opal_server/scopes/service.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2811 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/scopes/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.126860 opal-server-0.7.2/opal_server/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1423 2023-05-09 07:59:18.000000 opal-server-0.7.2/opal_server/security/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal-server-0.7.2/opal_server/security/jwks.py
--rw-r--r--   0 roekatz    (501) staff       (20)    17522 2023-05-29 10:10:14.000000 opal-server-0.7.2/opal_server/server.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-06-18 09:47:49.000000 opal-server-0.7.2/opal_server/statistics.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:32.121008 opal-server-0.7.2/opal_server.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     9134 2023-06-20 15:19:32.000000 opal-server-0.7.2/opal_server.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1246 2023-06-20 15:19:32.000000 opal-server-0.7.2/opal_server.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 15:19:32.000000 opal-server-0.7.2/opal_server.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-06-20 15:19:32.000000 opal-server-0.7.2/opal_server.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      565 2023-06-20 15:19:32.000000 opal-server-0.7.2/opal_server.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-20 15:19:32.000000 opal-server-0.7.2/opal_server.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-20 15:19:32.128399 opal-server-0.7.2/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2979 2022-12-08 13:40:17.000000 opal-server-0.7.2/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:37.010969 opal-server-0.7.3/
+-rw-r--r--   0 roekatz    (501) staff       (20)     9134 2023-06-27 11:25:37.010337 opal-server-0.7.3/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:36.993014 opal-server-0.7.3/opal_server/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11023 2023-06-20 17:01:29.000000 opal-server-0.7.3/opal_server/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:36.998137 opal-server-0.7.3/opal_server/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5303 2023-06-20 17:01:29.000000 opal-server-0.7.3/opal_server/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6169 2023-06-27 10:36:06.000000 opal-server-0.7.3/opal_server/data/data_update_publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13130 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/git_fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/loadlimiting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:36.998763 opal-server-0.7.3/opal_server/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/policy/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:36.999487 opal-server-0.7.3/opal_server/policy/bundles/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/policy/bundles/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4447 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/policy/bundles/api.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:37.002253 opal-server-0.7.3/opal_server/policy/watcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/policy/watcher/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4529 2023-06-20 17:01:29.000000 opal-server-0.7.3/opal_server/policy/watcher/callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6422 2023-06-20 17:01:29.000000 opal-server-0.7.3/opal_server/policy/watcher/factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4767 2023-06-27 11:24:48.000000 opal-server-0.7.3/opal_server/policy/watcher/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:37.004865 opal-server-0.7.3/opal_server/policy/webhook/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/policy/webhook/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5691 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/policy/webhook/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/policy/webhook/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/policy/webhook/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3659 2023-06-18 09:46:46.000000 opal-server-0.7.3/opal_server/pubsub.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1390 2023-05-09 07:59:18.000000 opal-server-0.7.3/opal_server/redis.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:37.008215 opal-server-0.7.3/opal_server/scopes/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/scopes/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12555 2023-06-20 17:01:29.000000 opal-server-0.7.3/opal_server/scopes/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/scopes/loader.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1325 2023-05-09 07:59:18.000000 opal-server-0.7.3/opal_server/scopes/scope_repository.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7256 2023-06-27 10:36:06.000000 opal-server-0.7.3/opal_server/scopes/service.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2811 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/scopes/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:37.009563 opal-server-0.7.3/opal_server/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1423 2023-05-09 07:59:18.000000 opal-server-0.7.3/opal_server/security/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal-server-0.7.3/opal_server/security/jwks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    17522 2023-05-29 10:10:14.000000 opal-server-0.7.3/opal_server/server.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-06-18 09:47:49.000000 opal-server-0.7.3/opal_server/statistics.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:36.996789 opal-server-0.7.3/opal_server.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     9134 2023-06-27 11:25:36.000000 opal-server-0.7.3/opal_server.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1246 2023-06-27 11:25:36.000000 opal-server-0.7.3/opal_server.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-27 11:25:36.000000 opal-server-0.7.3/opal_server.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-06-27 11:25:36.000000 opal-server-0.7.3/opal_server.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      565 2023-06-27 11:25:36.000000 opal-server-0.7.3/opal_server.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-27 11:25:36.000000 opal-server-0.7.3/opal_server.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-27 11:25:37.011093 opal-server-0.7.3/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2979 2022-12-08 13:40:17.000000 opal-server-0.7.3/setup.py
```

### Comparing `opal-server-0.7.2/PKG-INFO` & `opal-server-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.7.2
+Version: 0.7.3
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.7.2 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.3 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
```

### Comparing `opal-server-0.7.2/opal_server/cli.py` & `opal-server-0.7.3/opal_server/cli.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/config.py` & `opal-server-0.7.3/opal_server/config.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/data/api.py` & `opal-server-0.7.3/opal_server/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/data/data_update_publisher.py` & `opal-server-0.7.3/opal_server/data/data_update_publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/git_fetcher.py` & `opal-server-0.7.3/opal_server/git_fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/loadlimiting.py` & `opal-server-0.7.3/opal_server/loadlimiting.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/policy/bundles/api.py` & `opal-server-0.7.3/opal_server/policy/bundles/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/policy/watcher/callbacks.py` & `opal-server-0.7.3/opal_server/policy/watcher/callbacks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/policy/watcher/factory.py` & `opal-server-0.7.3/opal_server/policy/watcher/factory.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/policy/watcher/task.py` & `opal-server-0.7.3/opal_server/policy/watcher/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,29 +34,35 @@
                 self._webhook_tasks.remove(task)
 
         self._webhook_tasks.append(asyncio.create_task(self.trigger(topic, data)))
 
     async def _listen_to_webhook_notifications(self):
         # Webhook api route can be hit randomly in all workers, so it publishes a message to the webhook topic.
         # This listener, running in the leader's context, would actually trigger the repo pull
+
+        async def _subscribe_internal():
+            logger.info(
+                "listening on webhook topic: '{topic}'",
+                topic=opal_server_config.POLICY_REPO_WEBHOOK_TOPIC,
+            )
+            await self._pubsub_endpoint.subscribe(
+                [opal_server_config.POLICY_REPO_WEBHOOK_TOPIC],
+                self._on_webhook,
+            )
+
         if self._pubsub_endpoint.broadcaster is not None:
             async with self._pubsub_endpoint.broadcaster.get_listening_context():
-                logger.info(
-                    "listening on webhook topic: '{topic}'",
-                    topic=opal_server_config.POLICY_REPO_WEBHOOK_TOPIC,
-                )
-
-                await self._pubsub_endpoint.subscribe(
-                    [opal_server_config.POLICY_REPO_WEBHOOK_TOPIC],
-                    self._on_webhook,
-                )
+                await _subscribe_internal()
                 await self._pubsub_endpoint.broadcaster.get_reader_task()
 
                 # Stop the watcher if broadcaster disconnects
                 self.signal_stop()
+        else:
+            # If no broadcaster is configured, just subscribe, no need to wait on anything
+            await _subscribe_internal()
 
     async def start(self):
         """starts the policy watcher and registers a failure callback to
         terminate gracefully."""
         logger.info("Launching policy watcher")
         self._tasks.append(asyncio.create_task(self._listen_to_webhook_notifications()))
         self._init_should_stop()
```

### Comparing `opal-server-0.7.2/opal_server/policy/webhook/api.py` & `opal-server-0.7.3/opal_server/policy/webhook/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/policy/webhook/deps.py` & `opal-server-0.7.3/opal_server/policy/webhook/deps.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/policy/webhook/listener.py` & `opal-server-0.7.3/opal_server/policy/webhook/listener.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/publisher.py` & `opal-server-0.7.3/opal_server/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/pubsub.py` & `opal-server-0.7.3/opal_server/pubsub.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/redis.py` & `opal-server-0.7.3/opal_server/redis.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/scopes/api.py` & `opal-server-0.7.3/opal_server/scopes/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/scopes/loader.py` & `opal-server-0.7.3/opal_server/scopes/loader.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/scopes/scope_repository.py` & `opal-server-0.7.3/opal_server/scopes/scope_repository.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/scopes/service.py` & `opal-server-0.7.3/opal_server/scopes/service.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/scopes/task.py` & `opal-server-0.7.3/opal_server/scopes/task.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/security/api.py` & `opal-server-0.7.3/opal_server/security/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/security/jwks.py` & `opal-server-0.7.3/opal_server/security/jwks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/server.py` & `opal-server-0.7.3/opal_server/server.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server/statistics.py` & `opal-server-0.7.3/opal_server/statistics.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server.egg-info/PKG-INFO` & `opal-server-0.7.3/opal_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.7.2
+Version: 0.7.3
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.7.2 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.3 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
```

### Comparing `opal-server-0.7.2/opal_server.egg-info/SOURCES.txt` & `opal-server-0.7.3/opal_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.2/opal_server.egg-info/requires.txt` & `opal-server-0.7.3/opal_server.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 websockets<11,>=10.3
 ddtrace<2,>=1.1.4
 slowapi<1,>=0.1.5
 aioredis<3,>=2.0.1
 pygit2<2,>=1.9.2
 asgiref<4,>=3.5.2
 redis<5,>=4.3.4
-opal-common==0.7.2
+opal-common==0.7.3
 charset-normalizer<3,>=2.0.12
 idna<4,>=3.3
 typer<1,>=0.4.1
 fastapi<1,>=0.78.0
 fastapi_websocket_pubsub==0.3.4
 fastapi_websocket_rpc<1,>=0.1.21
 gunicorn<21,>=20.1.0
```

### Comparing `opal-server-0.7.2/setup.py` & `opal-server-0.7.3/setup.py`

 * *Files identical despite different names*

