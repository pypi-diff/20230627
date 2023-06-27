# Comparing `tmp/drb-driver-zip-1.2.0.tar.gz` & `tmp/drb-driver-zip-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-zip-1.2.0.tar", last modified: Fri Apr  7 13:44:35 2023, max compression
+gzip compressed data, was "drb-driver-zip-1.2.1.tar", last modified: Tue Jun 27 16:05:10 2023, max compression
```

## Comparing `drb-driver-zip-1.2.0.tar` & `drb-driver-zip-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.123805 drb-driver-zip-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:43:02.000000 drb-driver-zip-1.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-19 10:42:26.000000 drb-driver-zip-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1781 2023-04-07 13:44:35.123805 drb-driver-zip-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1181 2022-12-19 10:07:56.000000 drb-driver-zip-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.111805 drb-driver-zip-1.2.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2022-12-19 10:07:56.000000 drb-driver-zip-1.2.0/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.103805 drb-driver-zip-1.2.0/docs/dev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.111805 drb-driver-zip-1.2.0/docs/dev/example/
--rw-rw-rw-   0 root         (0) root         (0)      789 2022-12-19 10:07:56.000000 drb-driver-zip-1.2.0/docs/dev/example/open.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.107805 drb-driver-zip-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.107805 drb-driver-zip-1.2.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.127805 drb-driver-zip-1.2.0/drb/drivers/zip/
--rw-rw-rw-   0 root         (0) root         (0)      232 2022-12-19 10:07:56.000000 drb-driver-zip-1.2.0/drb/drivers/zip/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-07 13:44:35.127805 drb-driver-zip-1.2.0/drb/drivers/zip/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8999 2023-04-06 08:41:32.000000 drb-driver-zip-1.2.0/drb/drivers/zip/zip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.115805 drb-driver-zip-1.2.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       97 2022-12-19 13:19:25.000000 drb-driver-zip-1.2.0/drb/exceptions/zip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.107805 drb-driver-zip-1.2.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.115805 drb-driver-zip-1.2.0/drb/topics/zip/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 10:07:56.000000 drb-driver-zip-1.2.0/drb/topics/zip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-07 13:43:53.000000 drb-driver-zip-1.2.0/drb/topics/zip/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.119805 drb-driver-zip-1.2.0/drb_driver_zip.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-04-07 13:44:35.000000 drb-driver-zip-1.2.0/drb_driver_zip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      636 2023-04-07 13:44:35.000000 drb-driver-zip-1.2.0/drb_driver_zip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 13:44:35.000000 drb-driver-zip-1.2.0/drb_driver_zip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-07 13:44:35.000000 drb-driver-zip-1.2.0/drb_driver_zip.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 13:44:34.000000 drb-driver-zip-1.2.0/drb_driver_zip.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-07 13:44:35.000000 drb-driver-zip-1.2.0/drb_driver_zip.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-07 13:44:35.000000 drb-driver-zip-1.2.0/drb_driver_zip.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-24 13:31:07.000000 drb-driver-zip-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-03-24 13:31:07.000000 drb-driver-zip-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-04-07 13:44:35.123805 drb-driver-zip-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-03-24 13:31:07.000000 drb-driver-zip-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 13:44:35.123805 drb-driver-zip-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 13:31:07.000000 drb-driver-zip-1.2.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2022-12-19 10:07:56.000000 drb-driver-zip-1.2.0/tests/test_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-03-24 13:31:07.000000 drb-driver-zip-1.2.0/tests/test_signature.py
--rw-rw-rw-   0 root         (0) root         (0)    12735 2023-03-24 13:31:07.000000 drb-driver-zip-1.2.0/tests/test_zip.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-19 10:07:56.000000 drb-driver-zip-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:10.000754 drb-driver-zip-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-06-27 16:05:10.000754 drb-driver-zip-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.996754 drb-driver-zip-1.2.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.992754 drb-driver-zip-1.2.1/docs/dev/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.996754 drb-driver-zip-1.2.1/docs/dev/example/
+-rw-rw-rw-   0 root         (0) root         (0)      789 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/docs/dev/example/open.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.992754 drb-driver-zip-1.2.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.992754 drb-driver-zip-1.2.1/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:10.000754 drb-driver-zip-1.2.1/drb/drivers/zip/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/drb/drivers/zip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-27 16:05:10.000754 drb-driver-zip-1.2.1/drb/drivers/zip/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8999 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/drb/drivers/zip/zip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.996754 drb-driver-zip-1.2.1/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/drb/exceptions/zip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.992754 drb-driver-zip-1.2.1/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.996754 drb-driver-zip-1.2.1/drb/topics/zip/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:04:51.000000 drb-driver-zip-1.2.1/drb/topics/zip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-27 16:04:51.000000 drb-driver-zip-1.2.1/drb/topics/zip/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:09.996754 drb-driver-zip-1.2.1/drb_driver_zip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-06-27 16:05:09.000000 drb-driver-zip-1.2.1/drb_driver_zip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-27 16:05:09.000000 drb-driver-zip-1.2.1/drb_driver_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 16:05:09.000000 drb-driver-zip-1.2.1/drb_driver_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-27 16:05:09.000000 drb-driver-zip-1.2.1/drb_driver_zip.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 16:05:09.000000 drb-driver-zip-1.2.1/drb_driver_zip.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-27 16:05:09.000000 drb-driver-zip-1.2.1/drb_driver_zip.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-27 16:05:09.000000 drb-driver-zip-1.2.1/drb_driver_zip.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-06-27 16:05:10.000754 drb-driver-zip-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:10.000754 drb-driver-zip-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:04:51.000000 drb-driver-zip-1.2.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/tests/test_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    12735 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/tests/test_zip.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-06-27 15:38:49.000000 drb-driver-zip-1.2.1/versioneer.py
```

### Comparing `drb-driver-zip-1.2.0/LICENCE.txt` & `drb-driver-zip-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/PKG-INFO` & `drb-driver-zip-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-zip
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB driver Zip
 Home-page: https://gitlab.com/drb-python/impl/zip
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, https://drb-python.gitlab.io/impl/zip
 Project-URL: Source, https://gitlab.com/drb-python/impl/zip
```

### Comparing `drb-driver-zip-1.2.0/README.md` & `drb-driver-zip-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/docs/conf.py` & `drb-driver-zip-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/docs/dev/example/open.py` & `drb-driver-zip-1.2.1/docs/dev/example/open.py`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/drb/drivers/zip/zip.py` & `drb-driver-zip-1.2.1/drb/drivers/zip/zip.py`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/drb_driver_zip.egg-info/PKG-INFO` & `drb-driver-zip-1.2.1/drb_driver_zip.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-zip
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB driver Zip
 Home-page: https://gitlab.com/drb-python/impl/zip
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, https://drb-python.gitlab.io/impl/zip
 Project-URL: Source, https://gitlab.com/drb-python/impl/zip
```

### Comparing `drb-driver-zip-1.2.0/drb_driver_zip.egg-info/SOURCES.txt` & `drb-driver-zip-1.2.1/drb_driver_zip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/setup.cfg` & `drb-driver-zip-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/tests/test_impl.py` & `drb-driver-zip-1.2.1/tests/test_impl.py`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/tests/test_signature.py` & `drb-driver-zip-1.2.1/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/tests/test_zip.py` & `drb-driver-zip-1.2.1/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `drb-driver-zip-1.2.0/versioneer.py` & `drb-driver-zip-1.2.1/versioneer.py`

 * *Files identical despite different names*

