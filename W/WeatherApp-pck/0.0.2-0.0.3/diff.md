# Comparing `tmp/WeatherApp_pck-0.0.2.tar.gz` & `tmp/WeatherApp_pck-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WeatherApp_pck-0.0.2.tar", last modified: Sun Jun 25 17:37:52 2023, max compression
+gzip compressed data, was "WeatherApp_pck-0.0.3.tar", last modified: Tue Jun 27 20:30:31 2023, max compression
```

## Comparing `WeatherApp_pck-0.0.2.tar` & `WeatherApp_pck-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:37:52.636372 WeatherApp_pck-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-25 17:37:52.636372 WeatherApp_pck-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-25 17:37:07.000000 WeatherApp_pck-0.0.2/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:37:52.636372 WeatherApp_pck-0.0.2/WeatherApp_pck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-25 17:37:52.000000 WeatherApp_pck-0.0.2/WeatherApp_pck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-25 17:37:52.000000 WeatherApp_pck-0.0.2/WeatherApp_pck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:37:52.000000 WeatherApp_pck-0.0.2/WeatherApp_pck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:37:52.000000 WeatherApp_pck-0.0.2/WeatherApp_pck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:37:52.636372 WeatherApp_pck-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-25 17:37:07.000000 WeatherApp_pck-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:30:31.095598 WeatherApp_pck-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-27 20:30:31.095598 WeatherApp_pck-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-27 20:29:35.000000 WeatherApp_pck-0.0.3/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:30:31.095598 WeatherApp_pck-0.0.3/WeatherApp_pck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-27 20:30:31.000000 WeatherApp_pck-0.0.3/WeatherApp_pck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-27 20:30:31.000000 WeatherApp_pck-0.0.3/WeatherApp_pck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:30:31.000000 WeatherApp_pck-0.0.3/WeatherApp_pck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:30:31.000000 WeatherApp_pck-0.0.3/WeatherApp_pck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:30:31.095598 WeatherApp_pck-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-27 20:29:35.000000 WeatherApp_pck-0.0.3/setup.py
```

### Comparing `WeatherApp_pck-0.0.2/README.txt` & `WeatherApp_pck-0.0.3/README.txt`

 * *Files identical despite different names*

