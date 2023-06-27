# Comparing `tmp/remotemanager-0.7.1.tar.gz` & `tmp/remotemanager-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.7.1.tar", last modified: Fri Jun 23 06:58:09 2023, max compression
+gzip compressed data, was "remotemanager-0.8.0.tar", last modified: Tue Jun 27 13:28:04 2023, max compression
```

## Comparing `remotemanager-0.7.1.tar` & `remotemanager-0.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.806987 remotemanager-0.7.1/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-23 06:58:09.806987 remotemanager-0.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.7.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-22 15:30:59.000000 remotemanager-0.7.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-22 15:30:59.000000 remotemanager-0.7.1/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.7.1/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12730 2023-06-13 13:42:38.000000 remotemanager-0.7.1/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.7.1/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.7.1/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.7.1/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.7.1/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    25087 2023-06-16 10:42:35.000000 remotemanager-0.7.1/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50410 2023-06-22 14:49:18.000000 remotemanager-0.7.1/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    22383 2023-06-14 09:06:03.000000 remotemanager-0.7.1/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.7.1/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4920 2023-06-22 14:49:18.000000 remotemanager-0.7.1/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.7.1/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.7.1/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.7.1/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.7.1/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.7.1/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.7.1/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.7.1/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.7.1/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.7.1/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.7.1/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.7.1/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9283 2023-06-14 07:47:50.000000 remotemanager-0.7.1/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.806987 remotemanager-0.7.1/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 06:58:09.806987 remotemanager-0.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.534990 remotemanager-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-27 13:28:04.534990 remotemanager-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-27 06:55:16.000000 remotemanager-0.8.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.526990 remotemanager-0.8.0/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-27 06:55:16.000000 remotemanager-0.8.0/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.526990 remotemanager-0.8.0/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.0/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12847 2023-06-26 12:50:24.000000 remotemanager-0.8.0/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.0/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.0/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.0/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.0/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    25581 2023-06-26 08:49:48.000000 remotemanager-0.8.0/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47377 2023-06-27 06:55:16.000000 remotemanager-0.8.0/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2023-06-26 08:49:48.000000 remotemanager-0.8.0/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    23856 2023-06-27 12:51:29.000000 remotemanager-0.8.0/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.0/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4920 2023-06-26 12:50:24.000000 remotemanager-0.8.0/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.0/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.0/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.0/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.0/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.0/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.0/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.0/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.534990 remotemanager-0.8.0/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.0/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.0/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.534990 remotemanager-0.8.0/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.0/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.0/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9435 2023-06-26 08:49:48.000000 remotemanager-0.8.0/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.534990 remotemanager-0.8.0/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.526990 remotemanager-0.8.0/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 13:28:04.534990 remotemanager-0.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.0/setup.py
```

### Comparing `remotemanager-0.7.1/LICENSE` & `remotemanager-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/PKG-INFO` & `remotemanager-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.7.1
+Version: 0.8.0
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.7.1/README.md` & `remotemanager-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/pyproject.toml` & `remotemanager-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.7.1"
+current_version = "0.8.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.7.1/remotemanager/connection/cmd.py` & `remotemanager-0.8.0/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/connection/computers/base.py` & `remotemanager-0.8.0/remotemanager/connection/computers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     Extend this class for connecting to your machine
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.shebang = "#!/bin/bash"
-        self._parser = NotImplemented
+        self._parser = None
 
         self.choice_groupings = []
 
         self._extra = ""
         self._internal_extra = ""
 
     def __setattr__(self, key, value):
@@ -55,15 +55,15 @@
             if isinstance(getattr(self, key), (optional, required)):
                 getattr(self, key).value = value
                 return
 
         object.__setattr__(self, key, value)
 
     def pack(self, *args, **kwargs):
-        if not isinstance(self._parser, Function):
+        if not isinstance(self._parser, (Function, type(None))):
             self._parser = Function(self._parser)
 
         return super().pack(*args, **kwargs)
 
     @classmethod
     def from_dict(cls, spec: dict, **url_args):
         """
@@ -320,14 +320,16 @@
 
         download_file(url, filename)
 
         return cls.from_yaml(filename, **url_args)
 
     @property
     def parser(self):
+        if self._parser is None:
+            return None
         if not isinstance(self._parser, Function):
             self._parser = Function(self._parser)
         return self._parser.object
 
     @parser.setter
     def parser(self, parser):
         if not isinstance(parser, Function):
@@ -397,14 +399,17 @@
                 kwargs["jobname"] = kwargs.pop("name")
 
         self.update_resources(**kwargs)
 
         if not self.valid:
             raise RuntimeError(f"missing required arguments: {self.missing}")
 
+        if self._parser is None:
+            return []
+
         return self.parser(self.argument_dict)
 
     @property
     def extra(self):
         return self._internal_extra + self._extra
 
     @extra.setter
```

### Comparing `remotemanager-0.7.1/remotemanager/connection/computers/example.py` & `remotemanager-0.8.0/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/connection/computers/options.py` & `remotemanager-0.8.0/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/connection/computers/parsers.py` & `remotemanager-0.8.0/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/connection/testing_object.py` & `remotemanager-0.8.0/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/connection/url.py` & `remotemanager-0.8.0/remotemanager/connection/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,39 +579,42 @@
         self._parent = parent
 
     def file_mtime(
         self,
         files: list,
         local: bool = None,
         python: bool = False,
+        ignore_empty: bool = False,
         dry_run: bool = False,
     ) -> dict:
         """
         Check file modification times of [files]
 
         Args:
             files (list):
                 list of paths to files
             local (bool):
                 force a local search
             python (bool):
                 ensure python style search is used
+            ignore_empty (bool):
+                also check the filesize, ignoring empty files
             dry_run (bool):
                 print command only
 
         Returns (dict):
             {file: mtime (unix)} dictionary
         """
 
         self._logger.info(f"performing stat on files: {files}")
         if local is None:
             local = self._parent.is_local
 
         files = ensure_list(files)
-        times, error = self._file_mtime(files, local, python, dry_run)
+        times, error = self._file_mtime(files, local, python, ignore_empty, dry_run)
 
         if dry_run:
             # in this instance "times" is simply the command
             return times
 
         self._logger.info("received:")
         self._logger.info(times)
@@ -622,37 +625,41 @@
                 output[file] = times[file]
 
             else:
                 output[file] = None
 
         return output
 
-    def _file_mtime(self, files: list, local: bool, python: bool, dry_run: bool):
+    def _file_mtime(
+        self, files: list, local: bool, python: bool, ignore_empty: bool, dry_run: bool
+    ):
         """
         Perform the "stat -c %Y" command on a list of files,
         returning the result. Uses a python command backup if this fails
 
         Args:
             files (list):
                 list of files to check
             local (bool):
                 force a local search
             python (bool):
                 force the python override
+            ignore_empty (bool):
+                also check the filesize, ignoring empty files
             dry_run (bool):
                 print command only
 
         Returns:
             (list): list of file unix times
         """
         sep = ","
 
         def stat():
             self._logger.debug("attempting raw stat command on files")
-            basecmd = f"stat -c %n{sep}%Y"
+            basecmd = f"stat -c %n{sep}%Y{sep}%s"
             if len(files) == 1:
                 cmd = f"{basecmd} {files[0]}"
             else:
                 cmd = f"{basecmd} {{" + ",".join(files) + "}"
 
             ret = self._parent.cmd(
                 cmd, local=local, raise_errors=False, dry_run=dry_run
@@ -660,15 +667,21 @@
 
             if dry_run:
                 return ret, "", "", ""
 
             times = {}
             for line in ret.stdout.split("\n"):
                 try:
-                    times[line.split(sep)[0]] = int(float(line.split(sep)[1]))
+                    fname = line.split(sep)[0]
+                    mtime = int(float(line.split(sep)[1]))
+                    fsize = int(float(line.split(sep)[2]))
+
+                    if ignore_empty and fsize == 0:
+                        continue
+                    times[fname] = mtime
                 except IndexError:
                     pass
 
             return times, ret.stderr.split("\n"), ret.returncode, ret.stderr
 
         def pystat():
             self._logger.debug("attempting python stat on files")
```

### Comparing `remotemanager-0.7.1/remotemanager/dataset/dataset.py` & `remotemanager-0.8.0/remotemanager/dataset/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import gc
 import os
 import typing
 import time
 import shutil
 import warnings
 
-from remotemanager.connection.detect_locale_error import detect_locale_error
 from remotemanager.storage.remotefunction import cached_functions
 from remotemanager.connection.url import URL
 from remotemanager.storage.database import Database
 from remotemanager.storage.function import Function
 from remotemanager.dataset.runner import Runner, localwinerror
 import remotemanager.transport as tp
 import remotemanager.serialisation as sr
@@ -324,18 +323,14 @@
         return self.global_run_args.get("local_dir", Runner._default_local_dir)
 
     @property
     def repofile(self) -> str:
         return f"{self.name}-{self.short_uuid}-repo"
 
     @property
-    def stderr_dump(self) -> str:
-        return f"stderr-{self.short_uuid}.out"
-
-    @property
     def master_script(self) -> str:
         return f"{self.name}-{self.short_uuid}-master.sh"
 
     @property
     def argfile(self) -> str:
         return f"args-{self.name}-{self.short_uuid}"
 
@@ -1134,15 +1129,15 @@
             else:
                 submitter = self.url.submitter
             runline = f"{submitter} {runner.jobscript.name}"
 
             asynchronous = runner.run_option("asynchronous", True)
             if asynchronous and self.url.submitter == "bash":
                 self._logger.debug('appending "&" for async run')
-                runline += f" 2>> {self.stderr_dump} &"
+                runline += f" 2>> {runner.errorfile.name} &"
 
             if runner.remote_dir not in master_scripts:
                 master_scripts[runner.remote_dir] = []
             master_scripts[runner.remote_dir].append(runline)
 
             for file in runner.extra_files["send"]:
                 self.transport.queue_for_push(
@@ -1153,41 +1148,31 @@
 
         if not any_file_written:
             return self._run_finalise()
 
         cmds = []
         i = 0
         for remote, lines in master_scripts.items():
-            scriptname = f"{i}-{self.master_script}"
-            i += 1
-            _scriptfile = TrackedFile(self.local_dir, remote, scriptname)
-            self._master_scripts.append(_scriptfile)
-            # newline='\n' is required to stop windows clients adding the \r\n
-            self._logger.info(f"writing to master script at {_scriptfile.local}")
-
-            if asynchronous and self.url.submitter == "bash":
-                # adds the content of the stderr file back into stderr
-                lines.append(
-                    f"if [ -e {self.stderr_dump} ]; "
-                    f"then >&2 cat {self.stderr_dump}; fi"
-                )
-
-            with open(_scriptfile.local, "w+", newline="\n") as o:
-                content = "\n".join(lines)
-                if self.add_newline:
-                    content += "\n"
-                o.write(content)
-            self.transport.queue_for_push(scriptname, self.local_dir, remote)
-            cmd = (
-                f"cd {remote} && "
-                f"if [ -e {self.stderr_dump} ]; "
-                f"then rm {self.stderr_dump}; fi "
-                f"&& {self.url.shell} {scriptname}"
-            )
-            cmds.append(cmd)
+            if not self.is_child:
+                scriptname = f"{i}-{self.master_script}"
+                i += 1
+                _scriptfile = TrackedFile(self.local_dir, remote, scriptname)
+                self._master_scripts.append(_scriptfile)
+                # newline='\n' is required to stop windows clients adding the \r\n
+                self._logger.info(f"writing to master script at {_scriptfile.local}")
+
+                with open(_scriptfile.local, "w+", newline="\n") as o:
+                    o.write(f"rm -f *{self.short_uuid}*error.out\n")
+                    content = "\n".join(lines)
+                    if self.add_newline:
+                        content += "\n"
+                    o.write(content)
+                self.transport.queue_for_push(scriptname, self.local_dir, remote)
+                cmd = f"cd {remote} && {self.url.shell} {scriptname}"
+                cmds.append(cmd)
 
             # send a repo for each new remote dir
             # TODO this should ideally be reduced to just _one_
             self._write_to_repo(self.local_dir, remote)
 
         if not dry_run:
             self.transport.transfer()
@@ -1232,19 +1217,19 @@
                 o.write("\n")
 
             if self.is_parent:
                 o.write("### dependency functions ###\n")
 
                 o.write(
                     """
-def submit_child(file):
+def submit_child(file, stderr):
     import subprocess
     subprocess.Popen(f"bash '{file}'",
                      stdout=subprocess.PIPE,
-                     stderr=subprocess.PIPE,
+                     stderr=open(stderr, "w+"),
                      shell=True,
                      universal_newlines=True)
 \n"""
                 )
 
                 o.write("\n")
 
@@ -1285,196 +1270,123 @@
             files_to_check.append(runner.resultfile.remote)
 
             if runner.errorfile is not None:
                 self._logger.info(f"looking for error file {runner.errorfile.remote}")
                 _error_files.append(runner.errorfile.remote)
 
         # check all at once for both result and error files in a single call
-        result = self.url.utils.file_mtime(files_to_check + _error_files)
+        result = self.url.utils.file_mtime(
+            files_to_check + _error_files, ignore_empty=True
+        )
 
         # separate out the error files into their own dict
         errors = {}
         for file in _error_files:
             try:
                 errors[file] = result.pop(file)
             except KeyError:
                 pass
 
         return result, errors
 
     def fetch_results(
         self,
         raise_if_not_finished: bool = False,
-        ignore_errors: bool = False,
         quiet: bool = False,
     ) -> None:
         """
         Collect any scripted run resultfiles and insert them into their runners
 
         Args:
             raise_if_not_finished (bool):
                 raise an error if all calculations not finished
-            ignore_errors (bool):
-                will ignore any raised errors if True
 
         Returns:
             None
         """
         Quiet.state = quiet
-        if not ignore_errors:
-            self._check_run_errors()
 
         result_mtimes, error_mtimes = self._check_for_runner_outputs()
 
-        if not any(result_mtimes.values()):
-            self._logger.info("no valid results found, exiting early")
+        # no reason to continue if we don't have any files, find out if that's the case
+        valid_results = [t for t in result_mtimes.values() if t is not None]
+        valid_errors = [t for t in error_mtimes.values() if t is not None]
+        if len(valid_results) + len(valid_errors) == 0:
+            self._logger.info("no valid results or errors found, exiting early")
             Quiet.state = False
             return
 
         self._logger.info("present result files:")
         self._logger.info(format_iterable(result_mtimes))
         for runner in self.runners:
             if result_mtimes[runner.resultfile.remote]:
                 self.transport.queue_for_pull(
                     os.path.split(runner.resultfile.remote)[1],
                     runner.local_dir,
                     os.path.split(runner.resultfile.remote)[0],
                 )
+            if error_mtimes[runner.errorfile.remote]:
+                self.transport.queue_for_pull(
+                    os.path.split(runner.errorfile.remote)[1],
+                    runner.local_dir,
+                    os.path.split(runner.errorfile.remote)[0],
+                )
 
-                for file in runner.extra_files["recv"]:
-                    rmt = (
-                        runner.run_dir
-                        if runner.run_dir is not None
-                        else runner.remote_dir
-                    )
-                    remote = os.path.join(rmt, os.path.split(file)[0])
-                    self.transport.queue_for_pull(
-                        os.path.split(file)[1], runner.local_dir, remote
-                    )
+            for file in runner.extra_files["recv"]:
+                rmt = (
+                    runner.run_dir if runner.run_dir is not None else runner.remote_dir
+                )
+                remote = os.path.join(rmt, os.path.split(file)[0])
+                self.transport.queue_for_pull(
+                    os.path.split(file)[1], runner.local_dir, remote
+                )
 
-        self._logger.info("pulling completed result files")
+        self._logger.info("pulling completed result and error files")
         self.transport.transfer()
         for runner in self.runners:
-            if result_mtimes[runner.resultfile.remote]:
-                runner.read_resultfile()
+            runner.read_local_files()
 
         self.database.update(self.pack())
 
-        if not all(self._is_finished(result_mtimes)) and raise_if_not_finished:
+        if raise_if_not_finished and not all(self._is_finished()):
             raise RuntimeError("Calculations not yet completed!")
         Quiet.state = False
 
-    def _check_run_errors(self) -> None:
-        self._logger.info("checking for run errors")
-
-        cmd_list = []
-        stderr_list = [self.stderr_dump]
-        if self.dependency:
-            for ds in self.dependency.get_parents(self)[::-1]:
-                cmd_list += ds.run_cmds
-                stderr_list.append(ds.stderr_dump)
-
-        self._logger.info(f"list of stderr files: {stderr_list}")
-
-        cmd_list += self._run_cmds
-
-        errs = [c.stderr for c in cmd_list if c.stderr is not None and c.stderr != ""]
-
-        if len(errs) == 0:
-            self._logger.info("no errors found at run, checking for stderr.out files")
-
-            remotes = []
-            for cmd in cmd_list:
-                remote = cmd.sent.split(" &&")[0][4:]
-                if remote not in remotes:
-                    remotes.append(remote)
-
-            self._logger.info(f"looking in remotes {remotes}")
-
-            errfiles = []
-            for remote in remotes:
-                for stderr_file in stderr_list:
-                    errfiles.append(f"{remote}/{stderr_file}")
-
-            errfiles = self.url.utils.file_presence(errfiles)
-
-            self._logger.info(f"error presence: {errfiles}")
-
-            if not any(list(errfiles.values())):
-                return
-
-            time.sleep(0.5)
-            errs = []
-            for file, presence in errfiles.items():
-                if presence:
-                    errs.append(self.url.cmd(f"cat {file}").stdout)
-
-            if len([e for e in errs if e != ""]) == 0:
-                self._logger.info(f"all errors are empty files")
-                return
-
-        print(f"There are {len(errs)} errors, printing (most recent call last):")
-
-        error_summaries = []
-        locale_errors = []
-        for error in errs:
-            locale_errors.append(detect_locale_error(error))
-            self._logger.error(error)
-            error_summaries.append(error.split("\n")[-1])
-
-        if all(locale_errors):
-            return
-
-        from remotemanager import Logger
-
-        msg = (
-            "There was an issue during running. "
-            f"See printed info or logfile at {Logger.path}\n"
-            f"Summary:\n{error_summaries}"
-        )
-        if self.url.raise_errors:
-            raise RuntimeError(msg)
-        print(msg)
-
     @property
     def is_finished(self) -> list:
         return self._is_finished()
 
-    def _is_finished(self, files: dict = None, verbose: bool = True) -> list:
+    def _is_finished(self, verbose: bool = True) -> list:
         """
         Check if the runners have finished
 
         Args:
-            files (dict):
-                will use this dict of files instead of rechecking if passed
             verbose (bool):
                 disables printing if False
 
         Returns (list):
             boolean list corresponding to the Runner order
         """
         if not verbose:
             Quiet.state = True
         # initialise an empty return dict
         ret = {r.uuid: None for r in self.runners}
         # if we're skipping, check in with the runners
-        # since the runner.is_finished will be valid...
+        # since runner.is_finished = True will be valid...
         for runner in self.runners:
             if not runner.run_args.get("skip") or runner.run_args.get("force", False):
                 continue
             self._logger.info(f"checking in with runner {runner}")
 
             if runner.is_finished:
                 ret[runner.uuid] = True
 
-        errs = {}
-        if files is None:
-            self._logger.runtime("checking for files")
-            # look for the resultfiles
-            files, errs = self._check_for_runner_outputs()
+        self._logger.runtime("checking for files")
+        # look for the resultfiles
+        files, errs = self._check_for_runner_outputs()
 
         # create a list of the resultfiles that are available
         def check_file_mtime(mtime: int, last_sub: int) -> bool:
             """
             Checks mtime against last_sub, returning True if mtime is after the sub.
             Uses unix epoch time.
 
@@ -1496,59 +1408,49 @@
         for runner in self.runners:
             # if we've already decided this runner, ignore it
             if ret[runner.uuid] is not None:
                 continue
             # get last submission time and the mtimes of the relevant files
             last_submitted = runner.last_submitted
             mtime_result = files[runner.resultfile.remote]
-            mtime_error = errs.get(runner.errorfile.remote, None)
-            # check the resultfile mtime. A missing file will have a time of None
-            ret[runner.uuid] = check_file_mtime(mtime_result, last_submitted)
+            mtime_error = errs[runner.errorfile.remote]
+            # check the mtimes. A missing file will have a time of None
+            finished_result = check_file_mtime(mtime_result, last_submitted)
+            finished_error = check_file_mtime(mtime_error, last_submitted)
+
+            ret[runner.uuid] = finished_result or finished_error
 
             self._logger.debug(
                 f"checking file {runner.resultfile.remote}. "
                 f"mtime {mtime_result} vs runner submit time "
                 f"{last_submitted} -> {ret[runner.uuid]}"
             )
-            # if we have an error file, check it also
-            # TODO we could move the raise_errors before the print section, as this is
-            #   currently completely blocking the search
-            if check_file_mtime(mtime_error, last_submitted) and self.url.raise_errors:
-                self._logger.debug("Found an error file, checking contents")
-                errmsg = self.url.cmd(f"cat {runner.errorfile.remote}").stdout
-                if errmsg != "":
-                    self._logger.warning("Stderr file is valid, raising")
-                    raise RuntimeError(errmsg)
 
         Quiet.state = False
         return list(ret.values())
 
     @property
     def all_finished(self) -> bool:
         """
         Check if `all` runners have finished
 
         Returns (bool):
             True if all runners have completed their runs
         """
         return all(self.is_finished)
 
-    def wait(
-        self, interval: int = 10, timeout: int = None, verbose: bool = False
-    ) -> None:
+    def wait(self, interval: int = 10, timeout: int = None) -> None:
         """
         Block run until completion, checking every `interval` seconds
 
         Args:
             interval (int):
                 check interval time in seconds
             timeout (int):
                 maximum time to wait (s)
-            verbose (bool):
-                Silent if False
         """
         t0 = time.time()
         while not all(self._is_finished(verbose=False)):
             time.sleep(interval)
 
             if timeout is not None and time.time() - t0 > timeout:
                 raise RuntimeError("wait timed out")
@@ -1558,7 +1460,17 @@
         """
         Access the results of the runners
 
         Returns (list):
             runner.result for each runner
         """
         return [r.result for r in self.runners]
+
+    @property
+    def errors(self) -> list:
+        """
+        Access the errors of the runners
+
+        Returns (list):
+            runner.result for each runner
+        """
+        return [r.error for r in self.runners]
```

### Comparing `remotemanager-0.7.1/remotemanager/dataset/dependency.py` & `remotemanager-0.8.0/remotemanager/dataset/dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,17 @@
                 ds.runners[-1]._dependency_info["parent_import"] = lstr
 
             tmp = []
             for child in self.get_children(ds):
                 tmp.append(f"import time")
                 tmp.append(f"time.sleep(1)")
                 tmp.append(
-                    f'repo.submit_child("' f'{child.runners[-1].jobscript.name}")\n'
+                    f'repo.submit_child("'
+                    f'{child.runners[-1].jobscript.name}", '
+                    f'"{child.runners[-1].errorfile.name}")\n'
                 )
             ds.runners[-1]._dependency_info["child_submit"] = tmp
 
             ds.database.update(ds.pack())
 
     def run(self, *args, **kwargs):
         self._logger.info("dependency internal run call")
```

### Comparing `remotemanager-0.7.1/remotemanager/dataset/runner.py` & `remotemanager-0.8.0/remotemanager/dataset/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,15 +207,14 @@
                 file type. Jobscript, result file, etc.
             ext (str):
                 file extension
 
         Returns:
             str: formatted filename
         """
-        self._logger.info(f"creating filename for {ftype} and extension {ext}")
         return f"{self.identifier}-{ftype}{ext}"
 
     @property
     def runfile(self) -> TrackedFile:
         """
         Filename of the python runfile
         """
@@ -247,15 +246,17 @@
         return TrackedFile(self.local_dir, joined, base_name)
 
     @property
     def errorfile(self) -> TrackedFile:
         """
         File tracker for error dumpfile
         """
-        return TrackedFile(self.local_dir, self.remote_dir, self.parent.stderr_dump)
+        base_name = self._format_filename("error", ".out")
+
+        return TrackedFile(self.local_dir, self.remote_dir, base_name)
 
     def _relative_remote_dir(self, file: str) -> str:
         """
         remote dir path relative to run dir
         """
         self._logger.info(
             f"getting relative path to remote dir for file "
@@ -353,38 +354,50 @@
     @property
     def extra_files(self) -> dict:
         """
         Returns the extra files set for this runner
         """
         return self._extra_files
 
-    def read_resultfile(self):
-        rfile = self.resultfile.local
-        self._logger.info("reading locally discovered runfile")
-        result = self.parent.serialiser.load(rfile)
-
-        timestamp = int(os.path.getmtime(rfile))
-        if timestamp < self.last_submitted and not self.is_finished:
-            self._logger.warning(f"{self}: calculation not completed yet")
-            return False
+    def read_local_files(self):
+        self._logger.runtime("reading local runner files")
+        result = False
+        if os.path.isfile(self.resultfile.local):
+            self._logger.info("reading locally discovered runfile")
+            result = self.parent.serialiser.load(self.resultfile.local)
 
-        mtime = datetime.fromtimestamp(timestamp)
-        self.insert_history(mtime, "resultfile created remotely")
+            timestamp = int(os.path.getmtime(self.resultfile.local))
+            if timestamp < self.last_submitted and not self.is_finished:
+                self._logger.warning(f"{self}: calculation not completed yet")
 
-        self.result = result
-        return True
+            mtime = datetime.fromtimestamp(timestamp)
+            self.insert_history(mtime, "resultfile created remotely")
+
+            self.result = result
+            result = True
+
+        try:
+            with open(self.errorfile.local, "r") as o:
+                error = o.read().strip()
+
+                if error != "":
+                    self._logger.runtime("valid error found, storing")
+                    self.error = error.split("\n")[-1]
+        except FileNotFoundError:
+            self._logger.runtime("no error file found")
+
+        return result
 
     @property
     def result(self):
         """
         Result (If available)
         """
-
         if os.path.isfile(self.resultfile.local):
-            success = self.read_resultfile()
+            success = self.read_local_files()
 
             if success:
                 return self._result
 
         if hasattr(self, "_result"):
             try:
                 if SERIALISED_STORAGE_KEY in self._result:
@@ -403,21 +416,55 @@
         Args:
             result:
                 run result
         """
         self._result = result
         self.state = "completed"
 
+    @property
+    def error(self):
+        """
+        Error (If one exists)
+        """
+        if hasattr(self, "_error"):
+            return self._error
+        return None
+
+    @error.setter
+    def error(self, error) -> None:
+        """
+        Creates and sets the error property
+
+        Args:
+            error:
+                run error string
+        """
+        self._error = error
+        self.state = "completed"
+
     def clear_result(self) -> None:
         """
         Removes any results, and sets the state to "result wiped"
         """
-        try:
+        if hasattr(self, "_result"):
             del self._result
-        except AttributeError:
+            self._logger.info("deleted _result property")
+        if hasattr(self, "_error"):
+            del self._error
+            self._logger.info("deleted _error property")
+
+        try:
+            os.remove(self.resultfile.local)
+            self._logger.info("removed result file")
+        except FileNotFoundError:
+            pass
+        try:
+            os.remove(self.errorfile.local)
+            self._logger.info("removed error file")
+        except FileNotFoundError:
             pass
 
         def remove_file(path):
             self._logger.info(f"attempting to clear result file {path}")
             try:
                 os.remove(path)
                 self._logger.info("Done")
@@ -678,18 +725,18 @@
 
         if self.run_dir and self.run_dir != self.remote_dir:
             self._logger.debug("run dir is separate to remote dir, appending extras")
             cmd = (
                 f"pydir=$PWD\n"
                 f"mkdir -p {self.run_dir} && "
                 f"cd {self.run_dir} && "
-                f"{python} ${{pydir}}/{self.runfile.name}"
+                f"{python} ${{pydir}}/{self.runfile.name} 2>> {self.errorfile.name}"
             )
         else:
-            runline = f"{python} {self.runfile.name}"
+            runline = f"{python} {self.runfile.name} 2>> {self.errorfile.name}"
             self._logger.debug(f"directly appending line {runline}")
             cmd = runline  # run file
 
         tmp.append(cmd)
 
         path = self.jobscript.local
         output = "\n".join(tmp)
@@ -709,15 +756,15 @@
     def is_finished(self) -> bool:
         """
         Attempts to determine if this runner has completed its run
 
         Returns (bool):
             completion status
         """
-        fin = hasattr(self, "_result")
+        fin = hasattr(self, "_result") or hasattr(self, "_error")
         self._logger.info(
             f"checking finished state of runner {self.short_uuid} -> {fin}"
         )
         return fin
 
     def update_run_options(self, run_args: dict) -> None:
         """
```

### Comparing `remotemanager-0.7.1/remotemanager/jupyter/magic.py` & `remotemanager-0.8.0/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/logging/__init__.py` & `remotemanager-0.8.0/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/logging/log.py` & `remotemanager-0.8.0/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/logging/utils.py` & `remotemanager-0.8.0/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/logging/verbosity.py` & `remotemanager-0.8.0/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/serialisation/__init__.py` & `remotemanager-0.8.0/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/serialisation/serial.py` & `remotemanager-0.8.0/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.8.0/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.8.0/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/storage/database.py` & `remotemanager-0.8.0/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/storage/function.py` & `remotemanager-0.8.0/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/storage/remotefunction.py` & `remotemanager-0.8.0/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/storage/sendablemixin.py` & `remotemanager-0.8.0/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/storage/trackedfile.py` & `remotemanager-0.8.0/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/transport/cp.py` & `remotemanager-0.8.0/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/transport/rsync.py` & `remotemanager-0.8.0/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/transport/scp.py` & `remotemanager-0.8.0/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/transport/transport.py` & `remotemanager-0.8.0/remotemanager/transport/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -269,24 +269,28 @@
         methods for ideas on how to do this.
 
         Returns (str):
             formatted command for issuing a transfer
         """
         raise NotImplementedError
 
-    def transfer(self, dry_run: bool = False, prepend: bool = True):
+    def transfer(
+        self, dry_run: bool = False, prepend: bool = True, raise_errors: bool = True
+    ):
         """
         Perform the actual transfer
 
         Args:
             dry_run (bool):
                 do not perform command, just return the command(s) to be
                 executed
             prepend (bool):
                 enable forced cmd prepending
+            raise_errors (bool):
+                will not raise any stderr if False
 
         Returns (str, None):
             the dry run string, or None
         """
 
         self._logger.info(f"executing a transfer")
 
@@ -304,15 +308,15 @@
         if dry_run:
             return [
                 self.url.cmd(cmd, dry_run=True, local=True, prepend=prepend)
                 for cmd in commands
             ]
 
         for cmd in commands:
-            self.url.cmd(cmd, local=True, prepend=prepend)
+            self.url.cmd(cmd, local=True, prepend=prepend, raise_errors=raise_errors)
             # wipe the transfer queue
             self.wipe_transfers()
 
     def wipe_transfers(self):
         self._logger.info("wiping transfers")
         self._transfers = {}
```

### Comparing `remotemanager-0.7.1/remotemanager/utils/__init__.py` & `remotemanager-0.8.0/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/utils/flags.py` & `remotemanager-0.8.0/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager/utils/version.py` & `remotemanager-0.8.0/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.1/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.8.0/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.7.1
+Version: 0.8.0
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.7.1/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.8.0/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

