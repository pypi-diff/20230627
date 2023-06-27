# Comparing `tmp/pp_project_pkg-1.0.202306271547-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306271552-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 12419 bytes, number of entries: 19
+Zip file size: 12418 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx      887 b- defN 23-Jun-27 14:49 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-27 10:05 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-20 14:19 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 15:47 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 15:52 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5164 b- defN 23-Jun-27 14:08 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271547.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 15:48 pp_project_pkg-1.0.202306271547.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 15:48 pp_project_pkg-1.0.202306271547.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 15:48 pp_project_pkg-1.0.202306271547.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1721 b- defN 23-Jun-27 15:48 pp_project_pkg-1.0.202306271547.dist-info/RECORD
-19 files, 31691 bytes uncompressed, 9513 bytes compressed:  70.0%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271552.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 15:52 pp_project_pkg-1.0.202306271552.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 15:52 pp_project_pkg-1.0.202306271552.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 15:52 pp_project_pkg-1.0.202306271552.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1721 b- defN 23-Jun-27 15:52 pp_project_pkg-1.0.202306271552.dist-info/RECORD
+19 files, 31691 bytes uncompressed, 9512 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271547.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306271552.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271547.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306271552.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271547.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306271552.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271547.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306271552.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271547.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306271552.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('27')
 VERSION_HOUR = int('15')
-VERSION_MINUTE = int('47')
+VERSION_MINUTE = int('52')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306271547
-version_date = '2023/06/27 15:47'
+PATCH_VERSION = 202306271552
+version_date = '2023/06/27 15:52'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306271547.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306271552.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

