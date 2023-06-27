# Comparing `tmp/pp_project_pkg-1.0.202306271602-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306271606-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 12416 bytes, number of entries: 19
+Zip file size: 12414 bytes, number of entries: 19
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
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 16:02 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 16:06 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5164 b- defN 23-Jun-27 14:08 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271602.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 16:02 pp_project_pkg-1.0.202306271602.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 16:02 pp_project_pkg-1.0.202306271602.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 16:02 pp_project_pkg-1.0.202306271602.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1721 b- defN 23-Jun-27 16:02 pp_project_pkg-1.0.202306271602.dist-info/RECORD
-19 files, 31691 bytes uncompressed, 9510 bytes compressed:  70.0%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271606.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 16:06 pp_project_pkg-1.0.202306271606.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 16:06 pp_project_pkg-1.0.202306271606.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 16:06 pp_project_pkg-1.0.202306271606.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1721 b- defN 23-Jun-27 16:06 pp_project_pkg-1.0.202306271606.dist-info/RECORD
+19 files, 31691 bytes uncompressed, 9508 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271602.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306271606.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271602.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306271606.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271602.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306271606.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271602.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306271606.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271602.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306271606.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('27')
 VERSION_HOUR = int('16')
-VERSION_MINUTE = int('02')
+VERSION_MINUTE = int('06')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306271602
-version_date = '2023/06/27 16:02'
+PATCH_VERSION = 202306271606
+version_date = '2023/06/27 16:06'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306271602.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306271606.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306271602.dist-info/RECORD` & `pp_project_pkg-1.0.202306271606.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=xW9v6KON3cAC3-4yP50rC6VCwv0tCeJ6h25oILWyGRw,5335
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/utils.py,sha256=qWUhyGz6Vz_0SOF_SvQbRlr2qxEIl2kqjvE32pZSipw,6657
-pp_project_pkg/version.py,sha256=157l05dDzrYIQtmcFv4MQroA8-xB41iizddSX2a6kYY,396
+pp_project_pkg/version.py,sha256=QtqAxNK2VHuoZt0ELZ0Xsde9ztDzYrb2IkXQHBvqfrw,396
 pp_project_pkg/wrangling.py,sha256=yhSUk82kjfgbEDRpHj-eqf2IfXuvTYRu_l2jWKKtw5U,5164
-pp_project_pkg-1.0.202306271602.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306271602.dist-info/METADATA,sha256=uT6C-XtWHcLATfSdeJ-EDYQ2x5LFve_KBm-1UbNp8wo,191
-pp_project_pkg-1.0.202306271602.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202306271602.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202306271602.dist-info/RECORD,,
+pp_project_pkg-1.0.202306271606.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306271606.dist-info/METADATA,sha256=QrmNwETgPNwYjeawzgvUCIPJqYTX-AVYPzGuRnUi2zI,191
+pp_project_pkg-1.0.202306271606.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202306271606.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202306271606.dist-info/RECORD,,
```

