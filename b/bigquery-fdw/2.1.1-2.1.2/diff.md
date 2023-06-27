# Comparing `tmp/bigquery-fdw-2.1.1.tar.gz` & `tmp/bigquery-fdw-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigquery-fdw-2.1.1.tar", last modified: Mon Oct 24 02:40:07 2022, max compression
+gzip compressed data, was "bigquery-fdw-2.1.2.tar", last modified: Tue Jun 27 01:43:02 2023, max compression
```

## Comparing `bigquery-fdw-2.1.1.tar` & `bigquery-fdw-2.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gab        (501) staff       (20)        0 2022-10-24 02:40:07.398923 bigquery-fdw-2.1.1/
--rw-r--r--   0 gab        (501) staff       (20)     1073 2017-10-04 01:35:28.000000 bigquery-fdw-2.1.1/LICENSE
--rw-r--r--   0 gab        (501) staff       (20)     7241 2022-10-24 02:40:07.398609 bigquery-fdw-2.1.1/PKG-INFO
--rw-r--r--   0 gab        (501) staff       (20)     4243 2022-06-26 18:40:04.000000 bigquery-fdw-2.1.1/README.md
-drwxr-xr-x   0 gab        (501) staff       (20)        0 2022-10-24 02:40:07.395307 bigquery-fdw-2.1.1/bigquery_fdw.egg-info/
--rw-r--r--   0 gab        (501) staff       (20)     7241 2022-10-24 02:40:06.000000 bigquery-fdw-2.1.1/bigquery_fdw.egg-info/PKG-INFO
--rw-r--r--   0 gab        (501) staff       (20)      308 2022-10-24 02:40:07.000000 bigquery-fdw-2.1.1/bigquery_fdw.egg-info/SOURCES.txt
--rw-r--r--   0 gab        (501) staff       (20)        1 2022-10-24 02:40:06.000000 bigquery-fdw-2.1.1/bigquery_fdw.egg-info/dependency_links.txt
--rw-r--r--   0 gab        (501) staff       (20)       67 2022-10-24 02:40:07.000000 bigquery-fdw-2.1.1/bigquery_fdw.egg-info/entry_points.txt
--rw-r--r--   0 gab        (501) staff       (20)      131 2022-10-24 02:40:07.000000 bigquery-fdw-2.1.1/bigquery_fdw.egg-info/requires.txt
--rw-r--r--   0 gab        (501) staff       (20)       13 2022-10-24 02:40:07.000000 bigquery-fdw-2.1.1/bigquery_fdw.egg-info/top_level.txt
--rw-r--r--   0 gab        (501) staff       (20)       38 2022-10-24 02:40:07.399082 bigquery-fdw-2.1.1/setup.cfg
--rw-r--r--   0 gab        (501) staff       (20)     1722 2022-10-24 02:40:01.000000 bigquery-fdw-2.1.1/setup.py
-drwxr-xr-x   0 gab        (501) staff       (20)        0 2022-10-24 02:40:07.397536 bigquery-fdw-2.1.1/src/
--rw-r--r--   0 gab        (501) staff       (20)        0 2017-09-29 15:03:02.000000 bigquery-fdw-2.1.1/src/__init__.py
--rw-r--r--   0 gab        (501) staff       (20)     3440 2021-01-23 19:36:34.000000 bigquery-fdw-2.1.1/src/bqclient.py
--rw-r--r--   0 gab        (501) staff       (20)     1556 2021-01-23 19:36:34.000000 bigquery-fdw-2.1.1/src/bqclient_test.py
--rw-r--r--   0 gab        (501) staff       (20)    16042 2021-01-23 19:36:34.000000 bigquery-fdw-2.1.1/src/fdw.py
+drwxr-xr-x   0 gab        (501) staff       (20)        0 2023-06-27 01:43:02.499069 bigquery-fdw-2.1.2/
+-rw-r--r--   0 gab        (501) staff       (20)     1073 2017-10-04 01:35:28.000000 bigquery-fdw-2.1.2/LICENSE
+-rw-r--r--   0 gab        (501) staff       (20)     7241 2023-06-27 01:43:02.498944 bigquery-fdw-2.1.2/PKG-INFO
+-rw-r--r--   0 gab        (501) staff       (20)     4243 2022-06-26 18:40:04.000000 bigquery-fdw-2.1.2/README.md
+drwxr-xr-x   0 gab        (501) staff       (20)        0 2023-06-27 01:43:02.498386 bigquery-fdw-2.1.2/bigquery_fdw.egg-info/
+-rw-r--r--   0 gab        (501) staff       (20)     7241 2023-06-27 01:43:02.000000 bigquery-fdw-2.1.2/bigquery_fdw.egg-info/PKG-INFO
+-rw-r--r--   0 gab        (501) staff       (20)      308 2023-06-27 01:43:02.000000 bigquery-fdw-2.1.2/bigquery_fdw.egg-info/SOURCES.txt
+-rw-r--r--   0 gab        (501) staff       (20)        1 2023-06-27 01:43:02.000000 bigquery-fdw-2.1.2/bigquery_fdw.egg-info/dependency_links.txt
+-rw-r--r--   0 gab        (501) staff       (20)       67 2023-06-27 01:43:02.000000 bigquery-fdw-2.1.2/bigquery_fdw.egg-info/entry_points.txt
+-rw-r--r--   0 gab        (501) staff       (20)      132 2023-06-27 01:43:02.000000 bigquery-fdw-2.1.2/bigquery_fdw.egg-info/requires.txt
+-rw-r--r--   0 gab        (501) staff       (20)       13 2023-06-27 01:43:02.000000 bigquery-fdw-2.1.2/bigquery_fdw.egg-info/top_level.txt
+-rw-r--r--   0 gab        (501) staff       (20)       38 2023-06-27 01:43:02.499101 bigquery-fdw-2.1.2/setup.cfg
+-rw-r--r--   0 gab        (501) staff       (20)     1723 2023-06-27 01:37:01.000000 bigquery-fdw-2.1.2/setup.py
+drwxr-xr-x   0 gab        (501) staff       (20)        0 2023-06-27 01:43:02.498784 bigquery-fdw-2.1.2/src/
+-rw-r--r--   0 gab        (501) staff       (20)        0 2017-09-29 15:03:02.000000 bigquery-fdw-2.1.2/src/__init__.py
+-rw-r--r--   0 gab        (501) staff       (20)     3440 2021-01-23 19:36:34.000000 bigquery-fdw-2.1.2/src/bqclient.py
+-rw-r--r--   0 gab        (501) staff       (20)     1556 2021-01-23 19:36:34.000000 bigquery-fdw-2.1.2/src/bqclient_test.py
+-rw-r--r--   0 gab        (501) staff       (20)    16042 2021-01-23 19:36:34.000000 bigquery-fdw-2.1.2/src/fdw.py
```

### Comparing `bigquery-fdw-2.1.1/LICENSE` & `bigquery-fdw-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bigquery-fdw-2.1.1/PKG-INFO` & `bigquery-fdw-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigquery-fdw
-Version: 2.1.1
+Version: 2.1.2
 Summary: BigQuery Foreign Data Wrapper for PostgreSQL
 Home-page: https://github.com/gabfl/bigquery_fdw
 Author: Gabriel Bordeaux
 Author-email: pypi@gab.lc
 License: MIT
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
```

### Comparing `bigquery-fdw-2.1.1/README.md` & `bigquery-fdw-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bigquery-fdw-2.1.1/bigquery_fdw.egg-info/PKG-INFO` & `bigquery-fdw-2.1.2/bigquery_fdw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigquery-fdw
-Version: 2.1.1
+Version: 2.1.2
 Summary: BigQuery Foreign Data Wrapper for PostgreSQL
 Home-page: https://github.com/gabfl/bigquery_fdw
 Author: Gabriel Bordeaux
 Author-email: pypi@gab.lc
 License: MIT
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
```

### Comparing `bigquery-fdw-2.1.1/setup.py` & `bigquery-fdw-2.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,28 @@
     import pypandoc
     long_description = pypandoc.convert_file('README.md', 'rst')
 except (IOError, ImportError):
     long_description = open('README.md').read()
 
 setup(
     name='bigquery-fdw',
-    version='2.1.1',
+    version='2.1.2',
     description='BigQuery Foreign Data Wrapper for PostgreSQL',
     long_description=long_description,
     author='Gabriel Bordeaux',
     author_email='pypi@gab.lc',
     url='https://github.com/gabfl/bigquery_fdw',
     license='MIT',
     packages=['bigquery_fdw'],
     package_dir={'bigquery_fdw': 'src'},
     # external dependencies
     install_requires=[
-        'google-cloud-bigquery==3.3.5',
-        'google-auth==2.13.0',
-        'google-auth-oauthlib==0.5.3',
+        'google-cloud-bigquery==3.11.2',
+        'google-auth==2.21.0',
+        'google-auth-oauthlib==1.0.0',
         'protobuf==4.21.8',  # Forcing version for google-cloud-bigquery
         'grpcio==1.50.0',  # Forcing version for google-cloud-bigquery
         'grpcio-status==1.50.0',  # Forcing version for google-cloud-bigquery
     ],
     entry_points={
         'console_scripts': [
             # 'bigquery_fdw = bigquery_fdw.fdw:main',
```

### Comparing `bigquery-fdw-2.1.1/src/bqclient.py` & `bigquery-fdw-2.1.2/src/bqclient.py`

 * *Files identical despite different names*

### Comparing `bigquery-fdw-2.1.1/src/bqclient_test.py` & `bigquery-fdw-2.1.2/src/bqclient_test.py`

 * *Files identical despite different names*

### Comparing `bigquery-fdw-2.1.1/src/fdw.py` & `bigquery-fdw-2.1.2/src/fdw.py`

 * *Files identical despite different names*

