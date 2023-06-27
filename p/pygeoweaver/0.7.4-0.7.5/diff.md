# Comparing `tmp/pygeoweaver-0.7.4.tar.gz` & `tmp/pygeoweaver-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.7.4.tar", last modified: Wed Jun 21 07:22:41 2023, max compression
+gzip compressed data, was "pygeoweaver-0.7.5.tar", last modified: Tue Jun 27 13:04:08 2023, max compression
```

## Comparing `pygeoweaver-0.7.4.tar` & `pygeoweaver-0.7.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:22:41.663782 pygeoweaver-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 07:22:41.663782 pygeoweaver-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:22:41.659782 pygeoweaver-0.7.4/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/download_gw.bat
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/download_gw.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/java_bin.bat
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/java_bin.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/jdk_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_find.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_resetpassword.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/sc_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/start.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/start.sh
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/stop.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:22:41.659782 pygeoweaver-0.7.4/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 07:22:41.000000 pygeoweaver-0.7.4/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-21 07:22:41.000000 pygeoweaver-0.7.4/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:22:41.000000 pygeoweaver-0.7.4/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 07:22:41.000000 pygeoweaver-0.7.4/pygeoweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 07:22:41.000000 pygeoweaver-0.7.4/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 07:22:41.663782 pygeoweaver-0.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:22:41.659782 pygeoweaver-0.7.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/test/test_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-21 07:22:31.000000 pygeoweaver-0.7.4/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:08.838161 pygeoweaver-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-27 13:04:08.838161 pygeoweaver-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:08.838161 pygeoweaver-0.7.5/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/download_gw.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/download_gw.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/java_bin.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/java_bin.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/jdk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/sc_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/start.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/stop.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:08.838161 pygeoweaver-0.7.5/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-27 13:04:08.000000 pygeoweaver-0.7.5/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-27 13:04:08.000000 pygeoweaver-0.7.5/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:04:08.000000 pygeoweaver-0.7.5/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 13:04:08.000000 pygeoweaver-0.7.5/pygeoweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 13:04:08.000000 pygeoweaver-0.7.5/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-27 13:04:08.838161 pygeoweaver-0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:04:08.838161 pygeoweaver-0.7.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/test/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-27 13:03:56.000000 pygeoweaver-0.7.5/test/test_server.py
```

### Comparing `pygeoweaver-0.7.4/LICENSE` & `pygeoweaver-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/PKG-INFO` & `pygeoweaver-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.7.4
+Version: 0.7.5
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <4,>=3.7
```

### Comparing `pygeoweaver-0.7.4/README.md` & `pygeoweaver-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/__main__.py` & `pygeoweaver-0.7.5/pygeoweaver/__main__.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/jdk_utils.py` & `pygeoweaver-0.7.5/pygeoweaver/jdk_utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_create.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_create.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_detail.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_export.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_find.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_find.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_help.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_help.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_history.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_history.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_import.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_list.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_resetpassword.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_resetpassword.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_run.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_run.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/sc_sync.py` & `pygeoweaver-0.7.5/pygeoweaver/sc_sync.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/server.py` & `pygeoweaver-0.7.5/pygeoweaver/server.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/start.bat` & `pygeoweaver-0.7.5/pygeoweaver/start.bat`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/start.sh` & `pygeoweaver-0.7.5/pygeoweaver/start.sh`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver/utils.py` & `pygeoweaver-0.7.5/pygeoweaver/utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.7.5/pygeoweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.7.4
+Version: 0.7.5
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <4,>=3.7
```

### Comparing `pygeoweaver-0.7.4/pygeoweaver.egg-info/SOURCES.txt` & `pygeoweaver-0.7.5/pygeoweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/pyproject.toml` & `pygeoweaver-0.7.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "pytest-cov"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.7.4"
+version = "0.7.5"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7,<4"
 classifiers = [
@@ -18,24 +18,26 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.7.4"
+version = "0.7.5"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
 setuptools = ">=61.0"
 requests = "2.28.2"
 pydantic = "1.10.9"
+ipython = "8.14.0"
+pandas = "2.0.2"
 
 [tool.poetry.scripts]
 
 [tool.pytest.ini_options]
 addopts = "-p no:warnings --cov=pygeoweaver --cov-report=html"
```

### Comparing `pygeoweaver-0.7.4/test/test_detail.py` & `pygeoweaver-0.7.5/test/test_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.4/test/test_server.py` & `pygeoweaver-0.7.5/test/test_server.py`

 * *Files identical despite different names*

