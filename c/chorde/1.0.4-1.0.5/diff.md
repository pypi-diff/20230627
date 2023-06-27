# Comparing `tmp/chorde-1.0.4.tar.gz` & `tmp/chorde-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chorde-1.0.4.tar", last modified: Mon May 15 17:04:26 2023, max compression
+gzip compressed data, was "chorde-1.0.5.tar", last modified: Tue Jun 27 15:36:47 2023, max compression
```

## Comparing `chorde-1.0.4.tar` & `chorde-1.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.548640 chorde-1.0.4/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     8084 2023-05-15 17:02:17.000000 chorde-1.0.4/CHANGELOG
--rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.4/MANIFEST.in
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-05-15 17:04:26.548640 chorde-1.0.4/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.4/README.rst
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.532639 chorde-1.0.4/lib/
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.536640 chorde-1.0.4/lib/chorde/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-05-15 17:04:06.000000 chorde-1.0.4/lib/chorde/_version.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.548640 chorde-1.0.4/lib/chorde/clients/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   663617 2023-05-15 17:02:59.000000 chorde-1.0.4/lib/chorde/clients/_async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/clients/_async.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    15767 2023-05-15 17:00:02.000000 chorde-1.0.4/lib/chorde/clients/_async.pyx
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.4/lib/chorde/clients/async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2731676 2023-04-17 14:22:41.000000 chorde-1.0.4/lib/chorde/clients/asyncache.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    65380 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/asyncache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.4/lib/chorde/clients/base.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/coherent.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/elasticache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/files.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.4/lib/chorde/clients/inproc.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/inproc.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.4/lib/chorde/clients/memcached.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.4/lib/chorde/clients/tiered.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/tiered.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.4/lib/chorde/decorators.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.4/lib/chorde/decorators.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/decorators.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/dnsutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/external_integration.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.548640 chorde-1.0.4/lib/chorde/mq/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/mq/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/mq/coherence.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/mq/compat.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.548640 chorde-1.0.4/lib/chorde/mq/ipsub/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/mq/ipsub/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/mq/ipsub/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/mq/ipsub/ipsub_zmq.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4920 2023-04-21 13:34:45.000000 chorde-1.0.4/lib/chorde/sPickle.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.4/lib/chorde/serialize.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/shmemutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/threadpool.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/worker.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.540639 chorde-1.0.4/lib/chorde.egg-info/
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/SOURCES.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/dependency_links.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.4/lib/chorde.egg-info/not-zip-safe
--rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/requires.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/top_level.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.4/requirements.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-05-15 17:04:26.548640 chorde-1.0.4/setup.cfg
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-05-15 17:03:37.000000 chorde-1.0.4/setup.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.402902 chorde-1.0.5/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     8279 2023-06-27 13:47:37.000000 chorde-1.0.5/CHANGELOG
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.5/MANIFEST.in
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-27 15:36:47.402902 chorde-1.0.5/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.5/README.rst
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.202901 chorde-1.0.5/lib/
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.258901 chorde-1.0.5/lib/chorde/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-06-27 13:46:52.000000 chorde-1.0.5/lib/chorde/_version.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.394902 chorde-1.0.5/lib/chorde/clients/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   664070 2023-06-27 13:47:53.000000 chorde-1.0.5/lib/chorde/clients/_async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/clients/_async.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    15794 2023-06-27 13:46:52.000000 chorde-1.0.5/lib/chorde/clients/_async.pyx
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.5/lib/chorde/clients/async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2731676 2023-04-17 14:22:41.000000 chorde-1.0.5/lib/chorde/clients/asyncache.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    65380 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/asyncache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.5/lib/chorde/clients/base.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/coherent.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/elasticache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/files.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.5/lib/chorde/clients/inproc.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/inproc.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.5/lib/chorde/clients/memcached.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.5/lib/chorde/clients/tiered.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/clients/tiered.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.5/lib/chorde/decorators.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.5/lib/chorde/decorators.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/decorators.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/dnsutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/external_integration.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.398902 chorde-1.0.5/lib/chorde/mq/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/mq/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/mq/coherence.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/mq/compat.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.402902 chorde-1.0.5/lib/chorde/mq/ipsub/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.5/lib/chorde/mq/ipsub/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/mq/ipsub/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/mq/ipsub/ipsub_zmq.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4570 2023-06-27 13:46:52.000000 chorde-1.0.5/lib/chorde/sPickle.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.5/lib/chorde/serialize.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/shmemutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/threadpool.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.5/lib/chorde/worker.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 15:36:47.262901 chorde-1.0.5/lib/chorde.egg-info/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/SOURCES.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/dependency_links.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.5/lib/chorde.egg-info/not-zip-safe
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/requires.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-06-27 15:36:47.000000 chorde-1.0.5/lib/chorde.egg-info/top_level.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.5/requirements.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-06-27 15:36:47.402902 chorde-1.0.5/setup.cfg
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-06-27 13:46:52.000000 chorde-1.0.5/setup.py
```

### Comparing `chorde-1.0.4/CHANGELOG` & `chorde-1.0.5/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Change Log
 
 All notable changes to this project will be documented here.
 
+## [1.0.5] - 2023-06-27
+### Bugfixes
+- Allow sPickle to accept strings as checksum keys, automatically
+  encode them as UTF8 to get byte keys, as most people would expect
+  string keys to work.
+
 ## [1.0.4] - 2023-05-15
 ### Bugfixes
 - Fix empty reason field when re-raising tornado.web.HTTPError
 
 ## [1.0.3] - 2023-04-21
 ### Bugfixes
 - Various string encoding fixes
```

### Comparing `chorde-1.0.4/PKG-INFO` & `chorde-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.4
+Version: 1.0.5
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.4/README.rst` & `chorde-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/__init__.py` & `chorde-1.0.5/lib/chorde/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/_async.c` & `chorde-1.0.5/lib/chorde/clients/_async.c`

 * *Files 0% similar despite different names*

```diff
@@ -2119,15 +2119,16 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   int __pyx_t_17;
-  char const *__pyx_t_18;
+  int __pyx_t_18;
+  char const *__pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reraise", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_strip = __pyx_optional_args->strip;
@@ -2361,44 +2362,53 @@
   /*try:*/ {
 
     /* "chorde/clients/_async.pyx":60
  *             del exc
  *         try:
  *             if not strip:             # <<<<<<<<<<<<<<
  *                 kwargs = {}
- *                 if isinstance(exc_obj, _HTTPError):
+ *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):
  */
     __pyx_t_6 = ((!(__pyx_v_strip != 0)) != 0);
     if (__pyx_t_6) {
 
       /* "chorde/clients/_async.pyx":61
  *         try:
  *             if not strip:
  *                 kwargs = {}             # <<<<<<<<<<<<<<
- *                 if isinstance(exc_obj, _HTTPError):
+ *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):
  *                     # Workaround for tornado's HTTPError which does not function
  */
       __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_v_kwargs = ((PyObject*)__pyx_t_4);
       __pyx_t_4 = 0;
 
       /* "chorde/clients/_async.pyx":62
  *             if not strip:
  *                 kwargs = {}
- *                 if isinstance(exc_obj, _HTTPError):             # <<<<<<<<<<<<<<
+ *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):             # <<<<<<<<<<<<<<
  *                     # Workaround for tornado's HTTPError which does not function
  *                     # correctly without a reason, and reason is given only as kwarg
  */
+      __pyx_t_17 = (__pyx_v_6chorde_7clients_6_async__HTTPError != Py_None);
+      __pyx_t_18 = (__pyx_t_17 != 0);
+      if (__pyx_t_18) {
+      } else {
+        __pyx_t_6 = __pyx_t_18;
+        goto __pyx_L16_bool_binop_done;
+      }
       __pyx_t_4 = __pyx_v_6chorde_7clients_6_async__HTTPError;
       __Pyx_INCREF(__pyx_t_4);
-      __pyx_t_6 = PyObject_IsInstance(__pyx_v_exc_obj, __pyx_t_4); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 62, __pyx_L12_error)
+      __pyx_t_18 = PyObject_IsInstance(__pyx_v_exc_obj, __pyx_t_4); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 62, __pyx_L12_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_17 = (__pyx_t_6 != 0);
-      if (__pyx_t_17) {
+      __pyx_t_17 = (__pyx_t_18 != 0);
+      __pyx_t_6 = __pyx_t_17;
+      __pyx_L16_bool_binop_done:;
+      if (__pyx_t_6) {
 
         /* "chorde/clients/_async.pyx":65
  *                     # Workaround for tornado's HTTPError which does not function
  *                     # correctly without a reason, and reason is given only as kwarg
  *                     kwargs["reason"] = exc_obj.reason             # <<<<<<<<<<<<<<
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:
@@ -2407,15 +2417,15 @@
         __Pyx_GOTREF(__pyx_t_4);
         if (unlikely(PyDict_SetItem(__pyx_v_kwargs, __pyx_n_s_reason, __pyx_t_4) < 0)) __PYX_ERR(0, 65, __pyx_L12_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
         /* "chorde/clients/_async.pyx":62
  *             if not strip:
  *                 kwargs = {}
- *                 if isinstance(exc_obj, _HTTPError):             # <<<<<<<<<<<<<<
+ *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):             # <<<<<<<<<<<<<<
  *                     # Workaround for tornado's HTTPError which does not function
  *                     # correctly without a reason, and reason is given only as kwarg
  */
       }
 
       /* "chorde/clients/_async.pyx":66
  *                     # correctly without a reason, and reason is given only as kwarg
@@ -2440,53 +2450,53 @@
       __PYX_ERR(0, 66, __pyx_L12_error)
 
       /* "chorde/clients/_async.pyx":60
  *             del exc
  *         try:
  *             if not strip:             # <<<<<<<<<<<<<<
  *                 kwargs = {}
- *                 if isinstance(exc_obj, _HTTPError):
+ *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):
  */
     }
 
     /* "chorde/clients/_async.pyx":67
  *                     kwargs["reason"] = exc_obj.reason
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:             # <<<<<<<<<<<<<<
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  */
-    __pyx_t_17 = (__pyx_v_exc_tb != Py_None);
-    __pyx_t_6 = (__pyx_t_17 != 0);
-    if (__pyx_t_6) {
+    __pyx_t_6 = (__pyx_v_exc_tb != Py_None);
+    __pyx_t_17 = (__pyx_t_6 != 0);
+    if (__pyx_t_17) {
 
       /* "chorde/clients/_async.pyx":68
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:
  *                 if exc_obj is not None:             # <<<<<<<<<<<<<<
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  */
-      __pyx_t_6 = (__pyx_v_exc_obj != Py_None);
-      __pyx_t_17 = (__pyx_t_6 != 0);
-      if (likely(__pyx_t_17)) {
+      __pyx_t_17 = (__pyx_v_exc_obj != Py_None);
+      __pyx_t_6 = (__pyx_t_17 != 0);
+      if (likely(__pyx_t_6)) {
 
         /* "chorde/clients/_async.pyx":69
  *             elif exc_tb is not None:
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:             # <<<<<<<<<<<<<<
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj
  */
         __pyx_t_1 = __Pyx_GetAttr(__pyx_v_exc_obj, __pyx_n_s_traceback); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_17 = (__pyx_t_1 != __pyx_v_exc_tb);
+        __pyx_t_6 = (__pyx_t_1 != __pyx_v_exc_tb);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_6 = (__pyx_t_17 != 0);
-        if (__pyx_t_6) {
+        __pyx_t_17 = (__pyx_t_6 != 0);
+        if (__pyx_t_17) {
 
           /* "chorde/clients/_async.pyx":70
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)             # <<<<<<<<<<<<<<
  *                     raise exc_obj
  *                 else:
@@ -2598,17 +2608,17 @@
     /* "chorde/clients/_async.pyx":74
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:             # <<<<<<<<<<<<<<
  *                 raise exc_obj
  *             else:
  */
-    __pyx_t_6 = (__pyx_v_exc_obj != Py_None);
-    __pyx_t_17 = (__pyx_t_6 != 0);
-    if (unlikely(__pyx_t_17)) {
+    __pyx_t_17 = (__pyx_v_exc_obj != Py_None);
+    __pyx_t_6 = (__pyx_t_17 != 0);
+    if (unlikely(__pyx_t_6)) {
 
       /* "chorde/clients/_async.pyx":75
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:
  *                 raise exc_obj             # <<<<<<<<<<<<<<
  *             else:
  *                 raise exc_typ()
@@ -2677,15 +2687,15 @@
       if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14) < 0)) __Pyx_ErrFetch(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14);
       __Pyx_XGOTREF(__pyx_t_16);
       __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_XGOTREF(__pyx_t_14);
       __Pyx_XGOTREF(__pyx_t_13);
       __Pyx_XGOTREF(__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_11);
-      __pyx_t_9 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_18 = __pyx_filename;
+      __pyx_t_9 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_19 = __pyx_filename;
       {
         __Pyx_DECREF(__pyx_v_exc_typ);
         __pyx_v_exc_typ = NULL;
         __Pyx_DECREF(__pyx_v_exc_obj);
         __pyx_v_exc_obj = NULL;
         __Pyx_DECREF(__pyx_v_exc_tb);
         __pyx_v_exc_tb = NULL;
@@ -2697,15 +2707,15 @@
         __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_12, __pyx_t_11);
       }
       __Pyx_XGIVEREF(__pyx_t_16);
       __Pyx_XGIVEREF(__pyx_t_15);
       __Pyx_XGIVEREF(__pyx_t_14);
       __Pyx_ErrRestore(__pyx_t_16, __pyx_t_15, __pyx_t_14);
       __pyx_t_16 = 0; __pyx_t_15 = 0; __pyx_t_14 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0; __pyx_t_11 = 0;
-      __pyx_lineno = __pyx_t_9; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_18;
+      __pyx_lineno = __pyx_t_9; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_19;
       goto __pyx_L1_error;
     }
   }
 
   /* "chorde/clients/_async.pyx":50
  * 
  *     @cython.ccall
```

### Comparing `chorde-1.0.4/lib/chorde/clients/_async.pyx` & `chorde-1.0.5/lib/chorde/clients/_async.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             exc_typ, exc_obj, exc_tb = exc
         finally:
             # Don't leave references to the exc/tb in the frame
             del exc
         try:
             if not strip:
                 kwargs = {}
-                if isinstance(exc_obj, _HTTPError):
+                if _HTTPError is not None and isinstance(exc_obj, _HTTPError):
                     # Workaround for tornado's HTTPError which does not function
                     # correctly without a reason, and reason is given only as kwarg
                     kwargs["reason"] = exc_obj.reason
                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
             elif exc_tb is not None:
                 if exc_obj is not None:
                     if getattr(exc_obj, '__traceback__') is not exc_tb:
```

### Comparing `chorde-1.0.4/lib/chorde/clients/async.c` & `chorde-1.0.5/lib/chorde/clients/async.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/asyncache.c` & `chorde-1.0.5/lib/chorde/clients/asyncache.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/asyncache.py` & `chorde-1.0.5/lib/chorde/clients/asyncache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/base.c` & `chorde-1.0.5/lib/chorde/clients/base.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/base.py` & `chorde-1.0.5/lib/chorde/clients/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/coherent.py` & `chorde-1.0.5/lib/chorde/clients/coherent.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/elasticache.py` & `chorde-1.0.5/lib/chorde/clients/elasticache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/files.py` & `chorde-1.0.5/lib/chorde/clients/files.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/inproc.c` & `chorde-1.0.5/lib/chorde/clients/inproc.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/inproc.py` & `chorde-1.0.5/lib/chorde/clients/inproc.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/memcached.py` & `chorde-1.0.5/lib/chorde/clients/memcached.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/tiered.c` & `chorde-1.0.5/lib/chorde/clients/tiered.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/clients/tiered.py` & `chorde-1.0.5/lib/chorde/clients/tiered.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/decorators.c` & `chorde-1.0.5/lib/chorde/decorators.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/decorators.pxd` & `chorde-1.0.5/lib/chorde/decorators.pxd`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/decorators.py` & `chorde-1.0.5/lib/chorde/decorators.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/dnsutils.py` & `chorde-1.0.5/lib/chorde/dnsutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/external_integration.py` & `chorde-1.0.5/lib/chorde/external_integration.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/mq/coherence.py` & `chorde-1.0.5/lib/chorde/mq/coherence.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/mq/ipsub/base.py` & `chorde-1.0.5/lib/chorde/mq/ipsub/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/mq/ipsub/ipsub_zmq.py` & `chorde-1.0.5/lib/chorde/mq/ipsub/ipsub_zmq.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/sPickle.py` & `chorde-1.0.5/lib/chorde/sPickle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 # -*- coding: utf-8 -*-
-# This monster makes it all compatible with up to py2.0 :-o
 
 __all__ = [
     "SecurePickler",
     "SecureUnpickler",
 ]
 
-#lint:disable
-try:
-    from hashlib import sha256 as checksum_algo
-except ImportError:
-    try:
-        from hashlib import sha1 as checksum_algo
-    except ImportError:
-        try:
-            from hashlib import md5 as checksum_algo
-        except ImportError:
-            try:
-                from sha import sha as checksum_algo
-            except ImportError:
-                from md5 import md5 as checksum_algo
-#lint:enable
+from hashlib import sha256 as checksum_algo
 checksum_algo_name = checksum_algo.__name__.replace('openssl_','')
 
 import hmac
 import struct
 import threading
 from binascii import hexlify, unhexlify
 
 import pickle as cPickle  # lint:ok
 from io import BytesIO  # lint:ok
 
 class SecurePickler(object):
     def __init__(self, checksum_key, file, *p, **kw):
+        if isinstance(checksum_key, str):
+            checksum_key = checksum_key.encode("utf8")
+
         self.file = file
         self.checksum_key = checksum_key
 
         self.backing_class = kw.pop('backing_class', cPickle.Pickler)
         self.backing_args = (p, kw)
         self.local = threading.local()
```

### Comparing `chorde-1.0.4/lib/chorde/serialize.py` & `chorde-1.0.5/lib/chorde/serialize.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/shmemutils.py` & `chorde-1.0.5/lib/chorde/shmemutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/threadpool.py` & `chorde-1.0.5/lib/chorde/threadpool.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde/worker.py` & `chorde-1.0.5/lib/chorde/worker.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/lib/chorde.egg-info/PKG-INFO` & `chorde-1.0.5/lib/chorde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.4
+Version: 1.0.5
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.4/lib/chorde.egg-info/SOURCES.txt` & `chorde-1.0.5/lib/chorde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chorde-1.0.4/setup.py` & `chorde-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 no_pyrex = False
 try:
     from Cython.Distutils import build_ext, Extension
     from Cython.Build import cythonize
 except:
     no_pyrex = True
 
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 
 version_path = os.path.join(os.path.dirname(__file__), 'lib', 'chorde', '_version.py')
 if not os.path.exists(version_path):
     with open(version_path, "w") as version_file:
         pass
 with open(version_path, "r+") as version_file:
     version_content = "__version__ = %r" % (VERSION,)
```

