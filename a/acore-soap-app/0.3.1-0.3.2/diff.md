# Comparing `tmp/acore_soap_app-0.3.1.tar.gz` & `tmp/acore_soap_app-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_soap_app-0.3.1.tar", last modified: Mon Jun 26 06:12:06 2023, max compression
+gzip compressed data, was "acore_soap_app-0.3.2.tar", last modified: Tue Jun 27 13:53:57 2023, max compression
```

## Comparing `acore_soap_app-0.3.1.tar` & `acore_soap_app-0.3.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.293966 acore_soap_app-0.3.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5568 2023-06-26 06:12:06.293819 acore_soap_app-0.3.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4429 2023-06-26 04:04:32.000000 acore_soap_app-0.3.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.289971 acore_soap_app-0.3.1/acore_soap_app/
--rw-r--r--   0 sanhehu    (501) staff       (20)      413 2023-06-21 15:44:20.000000 acore_soap_app-0.3.1/acore_soap_app/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 06:00:45.000000 acore_soap_app-0.3.1/acore_soap_app/_version.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.291107 acore_soap_app-0.3.1/acore_soap_app/agent/
--rw-r--r--   0 sanhehu    (501) staff       (20)      795 2023-06-21 01:55:28.000000 acore_soap_app-0.3.1/acore_soap_app/agent/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      731 2023-06-21 15:11:48.000000 acore_soap_app-0.3.1/acore_soap_app/agent/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      425 2023-05-10 15:07:05.000000 acore_soap_app-0.3.1/acore_soap_app/agent/execute-command.xml
--rw-r--r--   0 sanhehu    (501) staff       (20)    12691 2023-06-21 15:30:39.000000 acore_soap_app-0.3.1/acore_soap_app/agent/impl.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      314 2023-06-21 15:29:07.000000 acore_soap_app-0.3.1/acore_soap_app/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.291470 acore_soap_app-0.3.1/acore_soap_app/cli/
--rw-r--r--   0 sanhehu    (501) staff       (20)       67 2023-06-21 15:12:04.000000 acore_soap_app-0.3.1/acore_soap_app/cli/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5155 2023-06-26 05:56:16.000000 acore_soap_app-0.3.1/acore_soap_app/cli/impl.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2461 2023-06-26 05:51:01.000000 acore_soap_app-0.3.1/acore_soap_app/cli/main.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.291598 acore_soap_app-0.3.1/acore_soap_app/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/acore_soap_app/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      982 2023-06-21 01:09:10.000000 acore_soap_app-0.3.1/acore_soap_app/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      660 2023-06-20 12:56:41.000000 acore_soap_app-0.3.1/acore_soap_app/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.292111 acore_soap_app-0.3.1/acore_soap_app/sdk/
--rw-r--r--   0 sanhehu    (501) staff       (20)      175 2023-06-21 01:56:33.000000 acore_soap_app-0.3.1/acore_soap_app/sdk/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      271 2023-06-26 03:14:10.000000 acore_soap_app-0.3.1/acore_soap_app/sdk/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.292539 acore_soap_app-0.3.1/acore_soap_app/sdk/canned/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-26 03:12:13.000000 acore_soap_app-0.3.1/acore_soap_app/sdk/canned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      292 2023-06-26 03:14:58.000000 acore_soap_app-0.3.1/acore_soap_app/sdk/canned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4886 2023-06-26 03:14:28.000000 acore_soap_app-0.3.1/acore_soap_app/sdk/canned/impl.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6272 2023-06-21 15:33:19.000000 acore_soap_app-0.3.1/acore_soap_app/sdk/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.293027 acore_soap_app-0.3.1/acore_soap_app/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/acore_soap_app/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/acore_soap_app/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-21 13:24:48.000000 acore_soap_app-0.3.1/acore_soap_app/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      646 2023-06-21 12:16:28.000000 acore_soap_app-0.3.1/acore_soap_app/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.293441 acore_soap_app-0.3.1/acore_soap_app/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/acore_soap_app/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/acore_soap_app/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.290645 acore_soap_app-0.3.1/acore_soap_app.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5568 2023-06-26 06:12:06.000000 acore_soap_app-0.3.1/acore_soap_app.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1189 2023-06-26 06:12:06.000000 acore_soap_app-0.3.1/acore_soap_app.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 06:12:06.000000 acore_soap_app-0.3.1/acore_soap_app.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       55 2023-06-26 06:12:06.000000 acore_soap_app-0.3.1/acore_soap_app.egg-info/entry_points.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      383 2023-06-26 06:12:06.000000 acore_soap_app-0.3.1/acore_soap_app.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-26 06:12:06.000000 acore_soap_app-0.3.1/acore_soap_app.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      971 2023-06-26 06:00:33.000000 acore_soap_app-0.3.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-06-21 13:24:55.000000 acore_soap_app-0.3.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-26 05:45:55.000000 acore_soap_app-0.3.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 06:12:06.294014 acore_soap_app-0.3.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-06-20 13:22:31.000000 acore_soap_app-0.3.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 06:12:06.293599 acore_soap_app-0.3.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      226 2023-06-20 05:17:17.000000 acore_soap_app-0.3.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.585047 acore_soap_app-0.3.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5568 2023-06-27 13:53:57.584884 acore_soap_app-0.3.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4429 2023-06-26 04:04:32.000000 acore_soap_app-0.3.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.578909 acore_soap_app-0.3.2/acore_soap_app/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      413 2023-06-21 15:44:20.000000 acore_soap_app-0.3.2/acore_soap_app/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-27 13:53:17.000000 acore_soap_app-0.3.2/acore_soap_app/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.580751 acore_soap_app-0.3.2/acore_soap_app/agent/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      795 2023-06-21 01:55:28.000000 acore_soap_app-0.3.2/acore_soap_app/agent/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      731 2023-06-21 15:11:48.000000 acore_soap_app-0.3.2/acore_soap_app/agent/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      425 2023-05-10 15:07:05.000000 acore_soap_app-0.3.2/acore_soap_app/agent/execute-command.xml
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12691 2023-06-21 15:30:39.000000 acore_soap_app-0.3.2/acore_soap_app/agent/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      314 2023-06-21 15:29:07.000000 acore_soap_app-0.3.2/acore_soap_app/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.581544 acore_soap_app-0.3.2/acore_soap_app/cli/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       67 2023-06-21 15:12:04.000000 acore_soap_app-0.3.2/acore_soap_app/cli/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5155 2023-06-26 05:56:16.000000 acore_soap_app-0.3.2/acore_soap_app/cli/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2461 2023-06-26 05:51:01.000000 acore_soap_app-0.3.2/acore_soap_app/cli/main.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.581885 acore_soap_app-0.3.2/acore_soap_app/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/acore_soap_app/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      982 2023-06-21 01:09:10.000000 acore_soap_app-0.3.2/acore_soap_app/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      660 2023-06-20 12:56:41.000000 acore_soap_app-0.3.2/acore_soap_app/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.582785 acore_soap_app-0.3.2/acore_soap_app/sdk/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      175 2023-06-21 01:56:33.000000 acore_soap_app-0.3.2/acore_soap_app/sdk/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      271 2023-06-26 03:14:10.000000 acore_soap_app-0.3.2/acore_soap_app/sdk/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.583559 acore_soap_app-0.3.2/acore_soap_app/sdk/canned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-26 03:12:13.000000 acore_soap_app-0.3.2/acore_soap_app/sdk/canned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      292 2023-06-26 03:14:58.000000 acore_soap_app-0.3.2/acore_soap_app/sdk/canned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4886 2023-06-26 03:14:28.000000 acore_soap_app-0.3.2/acore_soap_app/sdk/canned/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6272 2023-06-21 15:33:19.000000 acore_soap_app-0.3.2/acore_soap_app/sdk/core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.584124 acore_soap_app-0.3.2/acore_soap_app/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/acore_soap_app/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/acore_soap_app/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-21 13:24:48.000000 acore_soap_app-0.3.2/acore_soap_app/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      646 2023-06-21 12:16:28.000000 acore_soap_app-0.3.2/acore_soap_app/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.584518 acore_soap_app-0.3.2/acore_soap_app/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/acore_soap_app/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/acore_soap_app/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.579878 acore_soap_app-0.3.2/acore_soap_app.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5568 2023-06-27 13:53:57.000000 acore_soap_app-0.3.2/acore_soap_app.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1189 2023-06-27 13:53:57.000000 acore_soap_app-0.3.2/acore_soap_app.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-27 13:53:57.000000 acore_soap_app-0.3.2/acore_soap_app.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       55 2023-06-27 13:53:57.000000 acore_soap_app-0.3.2/acore_soap_app.egg-info/entry_points.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      383 2023-06-27 13:53:57.000000 acore_soap_app-0.3.2/acore_soap_app.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-27 13:53:57.000000 acore_soap_app-0.3.2/acore_soap_app.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1113 2023-06-27 13:53:36.000000 acore_soap_app-0.3.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-06-21 13:24:55.000000 acore_soap_app-0.3.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-27 13:52:01.000000 acore_soap_app-0.3.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-27 13:53:57.585090 acore_soap_app-0.3.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-06-20 13:22:31.000000 acore_soap_app-0.3.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 13:53:57.584660 acore_soap_app-0.3.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      226 2023-06-20 05:17:17.000000 acore_soap_app-0.3.2/tests/test_api.py
```

### Comparing `acore_soap_app-0.3.1/AUTHORS.rst` & `acore_soap_app-0.3.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/LICENSE.txt` & `acore_soap_app-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/PKG-INFO` & `acore_soap_app-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_soap_app
-Version: 0.3.1
+Version: 0.3.2
 Summary: Azerothcore World of Warcraft Soap Remote Access Python Library.
 Home-page: https://github.com/MacHu-GWU/acore_soap_app-project
-Download-URL: https://pypi.python.org/pypi/acore_soap_app/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_soap_app/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_soap_app-0.3.1/README.rst` & `acore_soap_app-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/agent/__init__.py` & `acore_soap_app-0.3.2/acore_soap_app/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/agent/api.py` & `acore_soap_app-0.3.2/acore_soap_app/agent/api.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/agent/impl.py` & `acore_soap_app-0.3.2/acore_soap_app/agent/impl.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/cli/impl.py` & `acore_soap_app-0.3.2/acore_soap_app/cli/impl.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/cli/main.py` & `acore_soap_app-0.3.2/acore_soap_app/cli/main.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/exc.py` & `acore_soap_app-0.3.2/acore_soap_app/exc.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/paths.py` & `acore_soap_app-0.3.2/acore_soap_app/paths.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/sdk/canned/impl.py` & `acore_soap_app-0.3.2/acore_soap_app/sdk/canned/impl.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/sdk/core.py` & `acore_soap_app-0.3.2/acore_soap_app/sdk/core.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/tests/mock_aws.py` & `acore_soap_app-0.3.2/acore_soap_app/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/utils.py` & `acore_soap_app-0.3.2/acore_soap_app/utils.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app/vendor/pytest_cov_helper.py` & `acore_soap_app-0.3.2/acore_soap_app/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/acore_soap_app.egg-info/PKG-INFO` & `acore_soap_app-0.3.2/acore_soap_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-soap-app
-Version: 0.3.1
+Version: 0.3.2
 Summary: Azerothcore World of Warcraft Soap Remote Access Python Library.
 Home-page: https://github.com/MacHu-GWU/acore_soap_app-project
-Download-URL: https://pypi.python.org/pypi/acore_soap_app/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_soap_app/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_soap_app-0.3.1/acore_soap_app.egg-info/SOURCES.txt` & `acore_soap_app-0.3.2/acore_soap_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/release-history.rst` & `acore_soap_app-0.3.2/release-history.rst`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.2 (2023-06-27)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Miscellaneous**
+
+- upgrade dependencies
+
+
 0.3.1 (2023-06-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``acsoap canned measure-server-status`` command
```

### Comparing `acore_soap_app-0.3.1/requirements-doc.txt` & `acore_soap_app-0.3.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.3.1/setup.py` & `acore_soap_app-0.3.2/setup.py`

 * *Files identical despite different names*

