# Comparing `tmp/pp_project_pkg-1.0.202306262308-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306270006-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10366 bytes, number of entries: 12
+Zip file size: 10365 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-23 12:39 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-23 12:39 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-26 23:08 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 00:06 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-18 22:21 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306262308.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-26 23:09 pp_project_pkg-1.0.202306262308.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 23:09 pp_project_pkg-1.0.202306262308.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-26 23:09 pp_project_pkg-1.0.202306262308.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-26 23:09 pp_project_pkg-1.0.202306262308.dist-info/RECORD
-12 files, 27436 bytes uncompressed, 8536 bytes compressed:  68.9%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306270006.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 00:06 pp_project_pkg-1.0.202306270006.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 00:06 pp_project_pkg-1.0.202306270006.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-27 00:06 pp_project_pkg-1.0.202306270006.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-27 00:06 pp_project_pkg-1.0.202306270006.dist-info/RECORD
+12 files, 27436 bytes uncompressed, 8535 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306262308.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306270006.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306262308.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306270006.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306262308.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306270006.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306262308.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306270006.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306262308.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306270006.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
-VERSION_DAY = int('26')
-VERSION_HOUR = int('23')
-VERSION_MINUTE = int('08')
+VERSION_DAY = int('27')
+VERSION_HOUR = int('00')
+VERSION_MINUTE = int('06')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306262308
-version_date = '2023/06/26 23:08'
+PATCH_VERSION = 202306270006
+version_date = '2023/06/27 00:06'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306262308.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306270006.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

