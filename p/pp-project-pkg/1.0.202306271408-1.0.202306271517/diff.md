# Comparing `tmp/pp_project_pkg-1.0.202306271408-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306271517-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 12719 bytes, number of entries: 20
+Zip file size: 12550 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:05 mlflow_pipelines/run.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/fetch_data/__init__.py
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-27 12:31 mlflow_pipelines/fetch_data/get_data.py
+-rw-rw-r--  2.0 unx      887 b- defN 23-Jun-27 14:49 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-27 10:05 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-20 14:19 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 14:08 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 15:17 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5164 b- defN 23-Jun-27 14:08 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271408.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 14:09 pp_project_pkg-1.0.202306271408.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 14:09 pp_project_pkg-1.0.202306271408.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 14:09 pp_project_pkg-1.0.202306271408.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1799 b- defN 23-Jun-27 14:09 pp_project_pkg-1.0.202306271408.dist-info/RECORD
-20 files, 32147 bytes uncompressed, 9691 bytes compressed:  69.9%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271517.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 15:18 pp_project_pkg-1.0.202306271517.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 15:18 pp_project_pkg-1.0.202306271517.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 15:18 pp_project_pkg-1.0.202306271517.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1798 b- defN 23-Jun-27 15:18 pp_project_pkg-1.0.202306271517.dist-info/RECORD
+20 files, 31768 bytes uncompressed, 9522 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271408.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306271517.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271408.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306271517.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271408.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306271517.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271408.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306271517.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271408.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306271517.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_pipelines/fetch_data/get_data.py

```diff
@@ -1,33 +1,31 @@
 from mb_utils.src import logging
 import mb.pandas as pd
 from pp_project_pkg.utils import site_date_res,check_report_close_date,download_upload_dates_report
-import argparse
 import hydra
+from omegaconf import DictConfig
+
 
 @hydra.main(config_name='./config.yml')
-def fetch_data_run(args,logger=None):
-    site_number = args.site_id
-    site_start_date = args.date
+def fetch_data_run(config: DictConfig):
+    # site_number = args.site_id
+    # site_start_date = args.date
+    
+    if config['data']['logger']:
+        logger = logging.logger
+    else:
+        logger = None
 
-    site_res =  site_date_res(site_number,logger=logger)
-    report_res = check_report_close_date(site_res,start_date=site_start_date)
+    site_res =  site_date_res(config['data']['site_res'],logger=logger)
+    report_res = check_report_close_date(site_res,start_date=config['data']['site_res'])
     if logger:
         logger.info(report_res.head())
 
     report_dates_res  = download_upload_dates_report(report_res,logger=logger)
     if logger:
         logger.info(report_dates_res.head())
 
     return report_dates_res
 
 
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(
-        description="Pp_project training Script")
-    parser.add_argument("-d","--date", type=str, default='2023-06-20' , help="Date for getting the waste/production plan for. Default : 2023-06-06")
-    parser.add_argument("-s","--site_id", type=int,default=30607, help="Site id. Default: 30607")
-    parser.add_argument("-l","--logger", type=str,default=None, help="Logger. Default: None")
-    args = parser.parse_args()
-    if args.logger:
-        logger = logging.logger
-    fetch_data_run(args,logger=logger)
+    fetch_data_run()
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('27')
-VERSION_HOUR = int('14')
-VERSION_MINUTE = int('08')
+VERSION_HOUR = int('15')
+VERSION_MINUTE = int('17')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306271408
-version_date = '2023/06/27 14:08'
+PATCH_VERSION = 202306271517
+version_date = '2023/06/27 15:17'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306271408.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306271517.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306271408.dist-info/RECORD` & `pp_project_pkg-1.0.202306271517.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 mlflow_pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/run.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/fetch_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mlflow_pipelines/fetch_data/get_data.py,sha256=nwWzNCKRJzDnWAFmauea7ux6VjCL8TpezEs63oL6JBQ,1265
+mlflow_pipelines/fetch_data/get_data.py,sha256=OCoL8C6L0H-tKN5p5eSxo6l6elnrXU21EPB5Tk-IgY8,887
 mlflow_pipelines/train_model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/train_model/model_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=xW9v6KON3cAC3-4yP50rC6VCwv0tCeJ6h25oILWyGRw,5335
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/utils.py,sha256=qWUhyGz6Vz_0SOF_SvQbRlr2qxEIl2kqjvE32pZSipw,6657
-pp_project_pkg/version.py,sha256=lFRXT1gmFrIgSyvRJ-gh5octgBaNzCrkHYNvQC9YKQw,396
+pp_project_pkg/version.py,sha256=UmYG6OBdJxkF_vWfkfYNnw-5qKfK3cRsPcdYkNAo-ww,396
 pp_project_pkg/wrangling.py,sha256=yhSUk82kjfgbEDRpHj-eqf2IfXuvTYRu_l2jWKKtw5U,5164
-pp_project_pkg-1.0.202306271408.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306271408.dist-info/METADATA,sha256=n8kRstFaVDZRTjH-C_YWkFi3nProFavDJejww5UZOAc,191
-pp_project_pkg-1.0.202306271408.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202306271408.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202306271408.dist-info/RECORD,,
+pp_project_pkg-1.0.202306271517.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306271517.dist-info/METADATA,sha256=8cHVyEG1ajMF80-mzk5QApaYq4XIYWon4698vIinFJ4,191
+pp_project_pkg-1.0.202306271517.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202306271517.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202306271517.dist-info/RECORD,,
```

