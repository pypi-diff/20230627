# Comparing `tmp/dissect.sql-3.6.dev1.tar.gz` & `tmp/dissect.sql-3.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.sql-3.6.dev1.tar", last modified: Fri Jun 16 12:50:50 2023, max compression
+gzip compressed data, was "dissect.sql-3.6.dev2.tar", last modified: Tue Jun 27 07:49:28 2023, max compression
```

## Comparing `dissect.sql-3.6.dev1.tar` & `dissect.sql-3.6.dev2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:50.493886 dissect.sql-3.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-16 12:50:50.493886 dissect.sql-3.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:50.477885 dissect.sql-3.6.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:50.485886 dissect.sql-3.6.dev1/dissect/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/dissect/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/dissect/sql/c_sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/dissect/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/dissect/sql/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/dissect/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:50.485886 dissect.sql-3.6.dev1/dissect.sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-16 12:50:50.000000 dissect.sql-3.6.dev1/dissect.sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-16 12:50:50.000000 dissect.sql-3.6.dev1/dissect.sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:50:50.000000 dissect.sql-3.6.dev1/dissect.sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:50:50.000000 dissect.sql-3.6.dev1/dissect.sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:50:50.000000 dissect.sql-3.6.dev1/dissect.sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-16 12:50:37.000000 dissect.sql-3.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:50:50.493886 dissect.sql-3.6.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:50.489886 dissect.sql-3.6.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:50.489886 dissect.sql-3.6.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/data/test.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:50.489886 dissect.sql-3.6.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/test_default_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/test_parse_table_columns_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:50:32.000000 dissect.sql-3.6.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:28.965871 dissect.sql-3.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-27 07:49:28.965871 dissect.sql-3.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:28.961871 dissect.sql-3.6.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:28.965871 dissect.sql-3.6.dev2/dissect/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/dissect/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/dissect/sql/c_sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/dissect/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/dissect/sql/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/dissect/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:28.965871 dissect.sql-3.6.dev2/dissect.sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-27 07:49:28.000000 dissect.sql-3.6.dev2/dissect.sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-27 07:49:28.000000 dissect.sql-3.6.dev2/dissect.sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:28.000000 dissect.sql-3.6.dev2/dissect.sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:49:28.000000 dissect.sql-3.6.dev2/dissect.sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:28.000000 dissect.sql-3.6.dev2/dissect.sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-27 07:49:17.000000 dissect.sql-3.6.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:28.965871 dissect.sql-3.6.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:28.965871 dissect.sql-3.6.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:28.965871 dissect.sql-3.6.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/data/test.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:28.965871 dissect.sql-3.6.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/test_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/test_parse_table_columns_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:49:12.000000 dissect.sql-3.6.dev2/tox.ini
```

### Comparing `dissect.sql-3.6.dev1/LICENSE` & `dissect.sql-3.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/PKG-INFO` & `dissect.sql-3.6.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.sql
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parsers for the SQLite database file format, commonly used by applications to store configuration data
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.sql
 Project-URL: repository, https://github.com/fox-it/dissect.sql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.sql-3.6.dev1/README.md` & `dissect.sql-3.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/dissect/sql/c_sqlite3.py` & `dissect.sql-3.6.dev2/dissect/sql/c_sqlite3.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/dissect/sql/sqlite3.py` & `dissect.sql-3.6.dev2/dissect/sql/sqlite3.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/dissect/sql/utils.py` & `dissect.sql-3.6.dev2/dissect/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/dissect.sql.egg-info/PKG-INFO` & `dissect.sql-3.6.dev2/dissect.sql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.sql
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parsers for the SQLite database file format, commonly used by applications to store configuration data
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.sql
 Project-URL: repository, https://github.com/fox-it/dissect.sql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.sql-3.6.dev1/dissect.sql.egg-info/SOURCES.txt` & `dissect.sql-3.6.dev2/dissect.sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/pyproject.toml` & `dissect.sql-3.6.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/tests/data/test.sqlite` & `dissect.sql-3.6.dev2/tests/data/test.sqlite`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/tests/docs/Makefile` & `dissect.sql-3.6.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/tests/docs/conf.py` & `dissect.sql-3.6.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/tests/test_default_values.py` & `dissect.sql-3.6.dev2/tests/test_default_values.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/tests/test_parse_table_columns_constraints.py` & `dissect.sql-3.6.dev2/tests/test_parse_table_columns_constraints.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/tests/test_row.py` & `dissect.sql-3.6.dev2/tests/test_row.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/tests/test_sqlite.py` & `dissect.sql-3.6.dev2/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.6.dev1/tox.ini` & `dissect.sql-3.6.dev2/tox.ini`

 * *Files identical despite different names*

