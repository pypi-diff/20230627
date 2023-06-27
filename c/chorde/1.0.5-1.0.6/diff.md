# Comparing `tmp/chorde-1.0.5.tar.gz` & `tmp/chorde-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chorde-1.0.5.tar", last modified: Tue Jun 27 15:36:47 2023, max compression
+gzip compressed data, was "chorde-1.0.6.tar", last modified: Tue Jun 27 18:23:07 2023, max compression
```

## Comparing `chorde-1.0.5.tar` & `chorde-1.0.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.402902 chorde-1.0.5/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     8279 2023-06-27 13:47:37.000000 chorde-1.0.5/CHANGELOG
--rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.5/MANIFEST.in
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-27 15:36:47.402902 chorde-1.0.5/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.5/README.rst
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.202901 chorde-1.0.5/lib/
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.258901 chorde-1.0.5/lib/chorde/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-06-27 13:46:52.000000 chorde-1.0.5/lib/chorde/_version.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.394902 chorde-1.0.5/lib/chorde/clients/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   664070 2023-06-27 13:47:53.000000 chorde-1.0.5/lib/chorde/clients/_async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/clients/_async.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    15794 2023-06-27 13:46:52.000000 chorde-1.0.5/lib/chorde/clients/_async.pyx
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.5/lib/chorde/clients/async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2731676 2023-04-17 14:22:41.000000 chorde-1.0.5/lib/chorde/clients/asyncache.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    65380 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/asyncache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.5/lib/chorde/clients/base.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/coherent.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/elasticache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/files.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.5/lib/chorde/clients/inproc.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/inproc.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.5/lib/chorde/clients/memcached.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.5/lib/chorde/clients/tiered.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/tiered.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.5/lib/chorde/decorators.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.5/lib/chorde/decorators.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/decorators.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/dnsutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/external_integration.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.398902 chorde-1.0.5/lib/chorde/mq/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/mq/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/mq/coherence.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/mq/compat.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.402902 chorde-1.0.5/lib/chorde/mq/ipsub/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/mq/ipsub/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/mq/ipsub/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/mq/ipsub/ipsub_zmq.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4570 2023-06-27 13:46:52.000000 chorde-1.0.5/lib/chorde/sPickle.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.5/lib/chorde/serialize.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/shmemutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/threadpool.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/worker.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.262901 chorde-1.0.5/lib/chorde.egg-info/
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/SOURCES.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/dependency_links.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.5/lib/chorde.egg-info/not-zip-safe
--rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/requires.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/top_level.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.5/requirements.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-06-27 15:36:47.402902 chorde-1.0.5/setup.cfg
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-06-27 13:46:52.000000 chorde-1.0.5/setup.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.618338 chorde-1.0.6/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     8379 2023-06-27 18:16:09.000000 chorde-1.0.6/CHANGELOG
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.6/MANIFEST.in
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-27 18:23:07.618338 chorde-1.0.6/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.6/README.rst
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.602338 chorde-1.0.6/lib/
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.606338 chorde-1.0.6/lib/chorde/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-06-27 18:21:58.000000 chorde-1.0.6/lib/chorde/_version.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.618338 chorde-1.0.6/lib/chorde/clients/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   664070 2023-06-27 13:47:53.000000 chorde-1.0.6/lib/chorde/clients/_async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/clients/_async.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    15794 2023-06-27 13:46:52.000000 chorde-1.0.6/lib/chorde/clients/_async.pyx
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.6/lib/chorde/clients/async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2731676 2023-04-17 14:22:41.000000 chorde-1.0.6/lib/chorde/clients/asyncache.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    65380 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/asyncache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.6/lib/chorde/clients/base.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/coherent.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/elasticache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/files.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.6/lib/chorde/clients/inproc.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/inproc.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.6/lib/chorde/clients/memcached.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.6/lib/chorde/clients/tiered.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/tiered.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.6/lib/chorde/decorators.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.6/lib/chorde/decorators.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/decorators.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/dnsutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/external_integration.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.618338 chorde-1.0.6/lib/chorde/mq/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/mq/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/mq/coherence.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/mq/compat.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.618338 chorde-1.0.6/lib/chorde/mq/ipsub/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/mq/ipsub/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/mq/ipsub/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/mq/ipsub/ipsub_zmq.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4668 2023-06-27 18:15:41.000000 chorde-1.0.6/lib/chorde/sPickle.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.6/lib/chorde/serialize.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/shmemutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/threadpool.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/worker.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.606338 chorde-1.0.6/lib/chorde.egg-info/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/SOURCES.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/dependency_links.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.6/lib/chorde.egg-info/not-zip-safe
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/requires.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/top_level.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.6/requirements.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-06-27 18:23:07.618338 chorde-1.0.6/setup.cfg
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-06-27 18:15:18.000000 chorde-1.0.6/setup.py
```

### Comparing `chorde-1.0.5/CHANGELOG` & `chorde-1.0.6/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Change Log
 
 All notable changes to this project will be documented here.
 
+## [1.0.6] - 2023-06-27
+### Bugfixes
+- Allow sPickle unpicklers to accept strings as checksum keys
+
 ## [1.0.5] - 2023-06-27
 ### Bugfixes
 - Allow sPickle to accept strings as checksum keys, automatically
   encode them as UTF8 to get byte keys, as most people would expect
   string keys to work.
 
 ## [1.0.4] - 2023-05-15
```

### Comparing `chorde-1.0.5/PKG-INFO` & `chorde-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.5
+Version: 1.0.6
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.5/README.rst` & `chorde-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/__init__.py` & `chorde-1.0.6/lib/chorde/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/_async.c` & `chorde-1.0.6/lib/chorde/clients/_async.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/_async.pyx` & `chorde-1.0.6/lib/chorde/clients/_async.pyx`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/async.c` & `chorde-1.0.6/lib/chorde/clients/async.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/asyncache.c` & `chorde-1.0.6/lib/chorde/clients/asyncache.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/asyncache.py` & `chorde-1.0.6/lib/chorde/clients/asyncache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/base.c` & `chorde-1.0.6/lib/chorde/clients/base.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/base.py` & `chorde-1.0.6/lib/chorde/clients/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/coherent.py` & `chorde-1.0.6/lib/chorde/clients/coherent.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/elasticache.py` & `chorde-1.0.6/lib/chorde/clients/elasticache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/files.py` & `chorde-1.0.6/lib/chorde/clients/files.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/inproc.c` & `chorde-1.0.6/lib/chorde/clients/inproc.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/inproc.py` & `chorde-1.0.6/lib/chorde/clients/inproc.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/memcached.py` & `chorde-1.0.6/lib/chorde/clients/memcached.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/tiered.c` & `chorde-1.0.6/lib/chorde/clients/tiered.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/clients/tiered.py` & `chorde-1.0.6/lib/chorde/clients/tiered.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/decorators.c` & `chorde-1.0.6/lib/chorde/decorators.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/decorators.pxd` & `chorde-1.0.6/lib/chorde/decorators.pxd`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/decorators.py` & `chorde-1.0.6/lib/chorde/decorators.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/dnsutils.py` & `chorde-1.0.6/lib/chorde/dnsutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/external_integration.py` & `chorde-1.0.6/lib/chorde/external_integration.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/mq/coherence.py` & `chorde-1.0.6/lib/chorde/mq/coherence.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/mq/ipsub/base.py` & `chorde-1.0.6/lib/chorde/mq/ipsub/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/mq/ipsub/ipsub_zmq.py` & `chorde-1.0.6/lib/chorde/mq/ipsub/ipsub_zmq.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/sPickle.py` & `chorde-1.0.6/lib/chorde/sPickle.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,17 @@
         md = hmac.HMAC(checksum_key, rv, checksum_algo).hexdigest().encode("ascii")
         self.file.write(hexlify(struct.pack('<L',len(rv))))
         self.file.write(md)
         self.file.write(rv)
 
 class SecureUnpickler(object):
     def __init__(self, checksum_key, file, *p, **kw):
+        if isinstance(checksum_key, str):
+            checksum_key = checksum_key.encode("utf8")
+
         self.file = file
         self.checksum_key = checksum_key
 
         self.backing_class = kw.pop('backing_class', cPickle.Unpickler)
         self.backing_args = (p, kw)
         self.local = threading.local()
```

### Comparing `chorde-1.0.5/lib/chorde/serialize.py` & `chorde-1.0.6/lib/chorde/serialize.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/shmemutils.py` & `chorde-1.0.6/lib/chorde/shmemutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/threadpool.py` & `chorde-1.0.6/lib/chorde/threadpool.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde/worker.py` & `chorde-1.0.6/lib/chorde/worker.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/lib/chorde.egg-info/PKG-INFO` & `chorde-1.0.6/lib/chorde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.5
+Version: 1.0.6
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.5/lib/chorde.egg-info/SOURCES.txt` & `chorde-1.0.6/lib/chorde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chorde-1.0.5/setup.py` & `chorde-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 no_pyrex = False
 try:
     from Cython.Distutils import build_ext, Extension
     from Cython.Build import cythonize
 except:
     no_pyrex = True
 
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 
 version_path = os.path.join(os.path.dirname(__file__), 'lib', 'chorde', '_version.py')
 if not os.path.exists(version_path):
     with open(version_path, "w") as version_file:
         pass
 with open(version_path, "r+") as version_file:
     version_content = "__version__ = %r" % (VERSION,)
```

