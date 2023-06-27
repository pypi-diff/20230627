# Comparing `tmp/pymilldb-0.0.7.tar.gz` & `tmp/pymilldb-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilldb-0.0.7.tar", last modified: Thu Jun 22 20:11:07 2023, max compression
+gzip compressed data, was "pymilldb-0.0.8.tar", last modified: Tue Jun 27 13:27:32 2023, max compression
```

## Comparing `pymilldb-0.0.7.tar` & `pymilldb-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.402823 pymilldb-0.0.7/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1095 2023-06-01 18:38:01.000000 pymilldb-0.0.7/LICENSE
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-22 20:11:07.402823 pymilldb-0.0.7/PKG-INFO
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      523 2023-06-01 18:38:01.000000 pymilldb-0.0.7/README.md
--rw-rw-r--   0 zeus      (1000) zeus      (1000)       89 2023-06-01 18:38:01.000000 pymilldb-0.0.7/pyproject.toml
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      633 2023-06-22 20:11:07.402823 pymilldb-0.0.7/setup.cfg
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.250806 pymilldb-0.0.7/src/
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.338816 pymilldb-0.0.7/src/pymilldb/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      167 2023-06-01 18:38:01.000000 pymilldb-0.0.7/src/pymilldb/__init__.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     2802 2023-06-07 16:03:26.000000 pymilldb-0.0.7/src/pymilldb/mdb_client.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1518 2023-06-07 16:03:26.000000 pymilldb-0.0.7/src/pymilldb/protocol.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1430 2023-06-07 16:03:26.000000 pymilldb-0.0.7/src/pymilldb/sampler.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)    10748 2023-06-22 20:09:52.000000 pymilldb-0.0.7/src/pymilldb/tensor_store.py
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.402823 pymilldb-0.0.7/src/pymilldb/utils/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:38:01.000000 pymilldb-0.0.7/src/pymilldb/utils/__init__.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      353 2023-06-01 18:38:01.000000 pymilldb-0.0.7/src/pymilldb/utils/decorators.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      630 2023-06-01 18:38:01.000000 pymilldb-0.0.7/src/pymilldb/utils/graph.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     2173 2023-06-07 16:03:26.000000 pymilldb-0.0.7/src/pymilldb/utils/packer.py
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.342816 pymilldb-0.0.7/src/pymilldb.egg-info/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-22 20:11:07.000000 pymilldb-0.0.7/src/pymilldb.egg-info/PKG-INFO
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      437 2023-06-22 20:11:07.000000 pymilldb-0.0.7/src/pymilldb.egg-info/SOURCES.txt
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        1 2023-06-22 20:11:07.000000 pymilldb-0.0.7/src/pymilldb.egg-info/dependency_links.txt
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        9 2023-06-22 20:11:07.000000 pymilldb-0.0.7/src/pymilldb.egg-info/top_level.txt
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.343078 pymilldb-0.0.8/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1095 2023-05-30 21:05:16.000000 pymilldb-0.0.8/LICENSE
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-27 13:27:32.343078 pymilldb-0.0.8/PKG-INFO
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      523 2023-05-30 21:18:35.000000 pymilldb-0.0.8/README.md
+-rw-r--r--   0 zeus      (1000) zeus      (1000)       89 2023-05-30 21:05:16.000000 pymilldb-0.0.8/pyproject.toml
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      633 2023-06-27 13:27:32.343078 pymilldb-0.0.8/setup.cfg
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.333078 pymilldb-0.0.8/src/
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.343078 pymilldb-0.0.8/src/pymilldb/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      226 2023-06-27 13:06:16.000000 pymilldb-0.0.8/src/pymilldb/__init__.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     2802 2023-06-06 21:04:43.000000 pymilldb-0.0.8/src/pymilldb/mdb_client.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1600 2023-06-27 13:20:48.000000 pymilldb-0.0.8/src/pymilldb/node_iterator.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1655 2023-06-27 13:03:43.000000 pymilldb-0.0.8/src/pymilldb/protocol.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1430 2023-06-06 21:04:43.000000 pymilldb-0.0.8/src/pymilldb/sampler.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)    10748 2023-06-23 13:54:50.000000 pymilldb-0.0.8/src/pymilldb/tensor_store.py
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.343078 pymilldb-0.0.8/src/pymilldb/utils/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:05:16.000000 pymilldb-0.0.8/src/pymilldb/utils/__init__.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      353 2023-05-30 21:05:16.000000 pymilldb-0.0.8/src/pymilldb/utils/decorators.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      630 2023-05-30 21:05:16.000000 pymilldb-0.0.8/src/pymilldb/utils/graph.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     2173 2023-06-06 21:04:43.000000 pymilldb-0.0.8/src/pymilldb/utils/packer.py
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.343078 pymilldb-0.0.8/src/pymilldb.egg-info/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-27 13:27:32.000000 pymilldb-0.0.8/src/pymilldb.egg-info/PKG-INFO
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      467 2023-06-27 13:27:32.000000 pymilldb-0.0.8/src/pymilldb.egg-info/SOURCES.txt
+-rw-r--r--   0 zeus      (1000) zeus      (1000)        1 2023-06-27 13:27:32.000000 pymilldb-0.0.8/src/pymilldb.egg-info/dependency_links.txt
+-rw-r--r--   0 zeus      (1000) zeus      (1000)        9 2023-06-27 13:27:32.000000 pymilldb-0.0.8/src/pymilldb.egg-info/top_level.txt
```

### Comparing `pymilldb-0.0.7/LICENSE` & `pymilldb-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.7/PKG-INFO` & `pymilldb-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymilldb-0.0.7/README.md` & `pymilldb-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.7/setup.cfg` & `pymilldb-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymilldb
-version = 0.0.7
+version = 0.0.8
 author = Vicente Calisto
 author_email = vecalisto@uc.cl
 description = A python library for MillenniumDB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MillenniumDB/PyMillDB
 project_urls =
```

### Comparing `pymilldb-0.0.7/src/pymilldb/mdb_client.py` & `pymilldb-0.0.8/src/pymilldb/mdb_client.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.7/src/pymilldb/sampler.py` & `pymilldb-0.0.8/src/pymilldb/sampler.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.7/src/pymilldb/tensor_store.py` & `pymilldb-0.0.8/src/pymilldb/tensor_store.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.7/src/pymilldb/utils/graph.py` & `pymilldb-0.0.8/src/pymilldb/utils/graph.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.7/src/pymilldb/utils/packer.py` & `pymilldb-0.0.8/src/pymilldb/utils/packer.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.7/src/pymilldb.egg-info/PKG-INFO` & `pymilldb-0.0.8/src/pymilldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

