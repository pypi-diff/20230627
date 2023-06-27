# Comparing `tmp/pp_project_pkg-1.0.202306271359-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306271402-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 12708 bytes, number of entries: 20
+Zip file size: 12715 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:05 mlflow_pipelines/run.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-27 12:31 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-27 10:05 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-20 14:19 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 13:59 pp_project_pkg/version.py
--rw-rw-r--  2.0 unx     5156 b- defN 23-Jun-27 13:57 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271359.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 13:59 pp_project_pkg-1.0.202306271359.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 13:59 pp_project_pkg-1.0.202306271359.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 13:59 pp_project_pkg-1.0.202306271359.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1799 b- defN 23-Jun-27 13:59 pp_project_pkg-1.0.202306271359.dist-info/RECORD
-20 files, 32139 bytes uncompressed, 9680 bytes compressed:  69.9%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 14:02 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     5168 b- defN 23-Jun-27 14:02 pp_project_pkg/wrangling.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271402.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 14:02 pp_project_pkg-1.0.202306271402.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 14:02 pp_project_pkg-1.0.202306271402.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 14:02 pp_project_pkg-1.0.202306271402.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1799 b- defN 23-Jun-27 14:02 pp_project_pkg-1.0.202306271402.dist-info/RECORD
+20 files, 32151 bytes uncompressed, 9687 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271359.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306271402.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271359.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306271402.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271359.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306271402.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271359.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306271402.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271359.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306271402.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('27')
-VERSION_HOUR = int('13')
-VERSION_MINUTE = int('59')
+VERSION_HOUR = int('14')
+VERSION_MINUTE = int('02')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306271359
-version_date = '2023/06/27 13:59'
+PATCH_VERSION = 202306271402
+version_date = '2023/06/27 14:02'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## pp_project_pkg/wrangling.py

```diff
@@ -41,16 +41,16 @@
     pp_production_rework = pd.merge(pp_production, pp_rework, on=['taxonomy_code'])
     name_pd = pd.read_csv('./taxcode_name_mapping.csv')
     name_pd = name_pd.drop(columns=['Unnamed: 0']).reset_index(drop=True)
     name_pd = name_pd.rename(columns={name_pd.columns[0]:'taxonomy_code',name_pd.columns[1]:'name'})
     pp_production_rework = pd.merge(pp_production_rework, name_pd, on=['taxonomy_code'])
 
     actual_production_and_rework = pp_production_rework.copy()
-    actual_production_and_rework['quantity_g'] = actual_production_and_rework['quantity_kg']*1000
-    actual_production_and_rework['rework_g'] = actual_production_and_rework['rework']*1000
+    actual_production_and_rework['quantity_g'] = actual_production_and_rework['actual_production_kg']*1000
+    actual_production_and_rework['rework_g'] = actual_production_and_rework['rework_kg']*1000
     
     joined_df = waste_data_for_site.join(hub_custom_breakdown.set_index('id'), on='reason_guid', how='inner')
 
     # Filter the joined dataframe based on the 'name' column
     filtered_df = joined_df.loc[joined_df['name'] == 'Overproduction']
      
     if logger and site_data:
```

## Comparing `pp_project_pkg-1.0.202306271359.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306271402.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306271359.dist-info/RECORD` & `pp_project_pkg-1.0.202306271402.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=xW9v6KON3cAC3-4yP50rC6VCwv0tCeJ6h25oILWyGRw,5335
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/utils.py,sha256=qWUhyGz6Vz_0SOF_SvQbRlr2qxEIl2kqjvE32pZSipw,6657
-pp_project_pkg/version.py,sha256=8zENpEqEaO6mLhUzI59dkmdWUfv2q3zCGcUgbripib0,396
-pp_project_pkg/wrangling.py,sha256=eMvIxt5SRXciI5Msb-n_I6Ekhs8tKORz3-Wsldattuw,5156
-pp_project_pkg-1.0.202306271359.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306271359.dist-info/METADATA,sha256=8Jdrm8sa-myCLMlvx3JtCok599DMmrzkt2wgKdSivZU,191
-pp_project_pkg-1.0.202306271359.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202306271359.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202306271359.dist-info/RECORD,,
+pp_project_pkg/version.py,sha256=G6M5MbnlC5Ig4kg7NZhaI_QHPSItz6yEdI45-fqCnmg,396
+pp_project_pkg/wrangling.py,sha256=JF4umFB6ITIvxCBguw6c9Wg_8wl4JXmRZErzFYtwFb8,5168
+pp_project_pkg-1.0.202306271402.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306271402.dist-info/METADATA,sha256=sB7dRYdfV8AoMBWA-h1hiASHx4ROHSBc7aU9iARmRRI,191
+pp_project_pkg-1.0.202306271402.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202306271402.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202306271402.dist-info/RECORD,,
```

