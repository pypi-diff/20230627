# Comparing `tmp/newtools-2.2.475.tar.gz` & `tmp/newtools-2.2.489.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newtools-2.2.475.tar", last modified: Mon May 22 09:59:48 2023, max compression
+gzip compressed data, was "dist/newtools-2.2.489.tar", last modified: Tue Jun 27 17:09:31 2023, max compression
```

## Comparing `newtools-2.2.475.tar` & `newtools-2.2.489.tar`

### file list

```diff
@@ -1,41 +1,62 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-22 09:57:42.000000 newtools-2.2.475/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-22 09:59:48.000000 newtools-2.2.475/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-22 09:57:42.000000 newtools-2.2.475/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/aws/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/aws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9641 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/aws/load_partitions.py
--rw-rw-rw-   0 root         (0) root         (0)     6435 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/aws/s3_location.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/db/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6912 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/db/athena.py
--rw-rw-rw-   0 root         (0) root         (0)    40091 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/db/cached_query.py
--rw-rw-rw-   0 root         (0) root         (0)    12954 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/db/sql_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/doggo/
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5576 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    13423 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/doggo.py
--rw-rw-rw-   0 root         (0) root         (0)    19227 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/fs.py
--rw-rw-rw-   0 root         (0) root         (0)     9277 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/lock.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/log/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/log/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9531 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/log/json_persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/log/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/log/persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3452 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/optional_imports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/queue/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/queue/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5151 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/queue/task_queue.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-22 09:57:42.000000 newtools-2.2.475/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-22 09:59:48.000000 newtools-2.2.475/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2296 2023-05-22 09:57:42.000000 newtools-2.2.475/setup.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-22 09:59:44.000000 newtools-2.2.475/version.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-27 17:06:48.000000 newtools-2.2.489/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-27 17:09:31.000000 newtools-2.2.489/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-27 17:06:48.000000 newtools-2.2.489/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/aws/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/aws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9641 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/aws/load_partitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6435 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/aws/s3_location.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/db/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14643 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/db/athena.py
+-rw-rw-rw-   0 root         (0) root         (0)    40091 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/db/cached_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     1470 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/db/data_types.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/db/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/db/sql/create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)    12954 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/db/sql_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/doggo/
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/doggo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5576 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/doggo/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    13423 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/doggo/doggo.py
+-rw-rw-rw-   0 root         (0) root         (0)    19227 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/doggo/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9277 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/doggo/lock.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/log/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/log/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9531 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/log/json_persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/log/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/log/persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/optional_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/queue/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/queue/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5151 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/queue/task_queue.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/tests/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/tests/test_data/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/tests/test_data/create_tables_athena/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/create_tables_athena/no_partitions.sql
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/create_tables_athena/partitions_no_projection.sql
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/create_tables_athena/partitions_with_projection.sql
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/athena_test.sql
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/ctas_test.sql
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/ctas_test_2.sql
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/ctas_test_no_data.sql
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/test_select.sql
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/test_select_bad.sql
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/test_select_in.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/query_tests/test_select_s3_path.sql
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools/tests/test_data/sqlclient/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/sqlclient/create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-27 17:06:48.000000 newtools-2.2.489/newtools/tests/test_data/sqlclient/query_file.sql
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-27 17:09:31.000000 newtools-2.2.489/newtools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-27 17:06:48.000000 newtools-2.2.489/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-27 17:09:31.000000 newtools-2.2.489/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2023-06-27 17:06:48.000000 newtools-2.2.489/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-27 17:09:28.000000 newtools-2.2.489/version.txt
```

### Comparing `newtools-2.2.475/PKG-INFO` & `newtools-2.2.489/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.475
+Version: 2.2.489
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.475/README.md` & `newtools-2.2.489/README.md`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/__init__.py` & `newtools-2.2.489/newtools/__init__.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/aws/load_partitions.py` & `newtools-2.2.489/newtools/aws/load_partitions.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/aws/s3_location.py` & `newtools-2.2.489/newtools/aws/s3_location.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/db/cached_query.py` & `newtools-2.2.489/newtools/db/cached_query.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/db/sql_client.py` & `newtools-2.2.489/newtools/db/sql_client.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/doggo/csv.py` & `newtools-2.2.489/newtools/doggo/csv.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/doggo/doggo.py` & `newtools-2.2.489/newtools/doggo/doggo.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/doggo/fs.py` & `newtools-2.2.489/newtools/doggo/fs.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/doggo/lock.py` & `newtools-2.2.489/newtools/doggo/lock.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/log/json_persistent_field_logger.py` & `newtools-2.2.489/newtools/log/json_persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/log/log.py` & `newtools-2.2.489/newtools/log/log.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/log/persistent_field_logger.py` & `newtools-2.2.489/newtools/log/persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/optional_imports.py` & `newtools-2.2.489/newtools/optional_imports.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools/queue/task_queue.py` & `newtools-2.2.489/newtools/queue/task_queue.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.475/newtools.egg-info/PKG-INFO` & `newtools-2.2.489/newtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.475
+Version: 2.2.489
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.475/setup.py` & `newtools-2.2.489/setup.py`

 * *Files identical despite different names*

