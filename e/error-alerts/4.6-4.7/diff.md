# Comparing `tmp/error-alerts-4.6.tar.gz` & `tmp/error-alerts-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-4.6.tar", last modified: Tue Jun 27 11:16:18 2023, max compression
+gzip compressed data, was "error-alerts-4.7.tar", last modified: Tue Jun 27 11:57:58 2023, max compression
```

## Comparing `error-alerts-4.6.tar` & `error-alerts-4.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:16:18.536996 error-alerts-4.6/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.6/.gitignore
--rw-rw-rw-   0        0        0     1305 2023-06-27 11:16:18.537994 error-alerts-4.6/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 11:16:18.532998 error-alerts-4.6/error_alerts/
--rw-rw-rw-   0        0        0     3116 2023-06-27 11:16:13.000000 error-alerts-4.6/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:16:18.536996 error-alerts-4.6/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1305 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 11:16:18.000000 error-alerts-4.6/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 11:16:18.537994 error-alerts-4.6/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-06-27 11:16:10.000000 error-alerts-4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:57:58.021526 error-alerts-4.7/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.7/.gitignore
+-rw-rw-rw-   0        0        0     1305 2023-06-27 11:57:58.022525 error-alerts-4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 11:57:58.017530 error-alerts-4.7/error_alerts/
+-rw-rw-rw-   0        0        0     3116 2023-06-27 11:16:13.000000 error-alerts-4.7/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:57:58.021526 error-alerts-4.7/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1305 2023-06-27 11:57:57.000000 error-alerts-4.7/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-27 11:57:57.000000 error-alerts-4.7/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:57:57.000000 error-alerts-4.7/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 11:57:57.000000 error-alerts-4.7/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 11:57:57.000000 error-alerts-4.7/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 11:57:58.022525 error-alerts-4.7/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-27 11:57:52.000000 error-alerts-4.7/setup.py
```

### Comparing `error-alerts-4.6/PKG-INFO` & `error-alerts-4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.6
+Version: 4.7
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-4.6/README.md` & `error-alerts-4.7/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-4.6/error_alerts/__init__.py` & `error-alerts-4.7/error_alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `error-alerts-4.6/error_alerts.egg-info/PKG-INFO` & `error-alerts-4.7/error_alerts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.6
+Version: 4.7
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

