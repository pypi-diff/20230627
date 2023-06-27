# Comparing `tmp/pp_project_pkg-1.0.202306271231-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306271358-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 12541 bytes, number of entries: 20
+Zip file size: 12708 bytes, number of entries: 20
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
--rw-rw-r--  2.0 unx     9193 b- defN 23-Jun-27 12:30 pp_project_pkg/pp_tables.py
+-rw-rw-r--  2.0 unx     9275 b- defN 23-Jun-27 13:57 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-20 14:19 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 12:31 pp_project_pkg/version.py
--rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-20 09:33 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271231.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 12:31 pp_project_pkg-1.0.202306271231.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 12:31 pp_project_pkg-1.0.202306271231.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 12:31 pp_project_pkg-1.0.202306271231.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1799 b- defN 23-Jun-27 12:31 pp_project_pkg-1.0.202306271231.dist-info/RECORD
-20 files, 31526 bytes uncompressed, 9513 bytes compressed:  69.8%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 13:58 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     5156 b- defN 23-Jun-27 13:57 pp_project_pkg/wrangling.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271358.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 13:58 pp_project_pkg-1.0.202306271358.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 13:58 pp_project_pkg-1.0.202306271358.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 13:58 pp_project_pkg-1.0.202306271358.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1799 b- defN 23-Jun-27 13:58 pp_project_pkg-1.0.202306271358.dist-info/RECORD
+20 files, 32162 bytes uncompressed, 9680 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271231.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306271358.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271231.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306271358.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271231.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306271358.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271231.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306271358.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271231.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306271358.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/pp_tables.py

```diff
@@ -96,56 +96,56 @@
        
   from pp_configuration_service.site s
 		inner join pp_configuration_service.site_configuration sc on s.id = sc.site_id
 		inner join pp_configuration_service.meal_period_configuration mpc on sc.id = mpc.site_configuration_entity_id
 	 where s.site_id = {}""".format(self.site_id)
         return wv.read_sql(q1,self.engine)
 
-    @time_wrapper
-    def pp_production_rework(self):
-        q1 = """select 
-    curr_state.site_id,
-    service.id as service_id,
-    service.start_date as meal_service_start_date,
-    meal_period_config.meal_period,
-    food_group.id as food_group_id, 
-    food_item.id as food_item_id, 
-    food_item."name",  
-    food_item_figures.taxonomy_code,
-    food_item_figures.unit, 
-    food_item_figures.figure_type, 
-    food_item_figures.quantity_kg as quantity_kg,
-                (select vfir.quantity_kg  from pp_meal_service.view_food_item_rework vfir 
-                where vfir.view_food_item_id = food_item.id
-                and vfir.id = (select max(vfir.id)
-                          from pp_meal_service.view_food_item_rework vfir, pp_meal_service.view_food_item fi
-                          where vfir.view_food_item_id = fi.id
-                          and vfir.view_food_item_id = food_item.id)) as rework, 
-       food_item_figures.created as food_item_figure_created
-    from
-        pp_meal_service.view_current_state curr_state, 
-        pp_meal_service.view_service service,
-        pp_meal_service.view_meal_period_configuration meal_period_config,
-        pp_meal_service.view_food_group food_group,
-        pp_meal_service.view_food_item food_item,
-        pp_meal_service.view_food_item_figures food_item_figures
+    # @time_wrapper
+    # def pp_production_rework(self):
+    #     q1 = """select 
+    # curr_state.site_id,
+    # service.id as service_id,
+    # service.start_date as meal_service_start_date,
+    # meal_period_config.meal_period,
+    # food_group.id as food_group_id, 
+    # food_item.id as food_item_id, 
+    # food_item."name",  
+    # food_item_figures.taxonomy_code,
+    # food_item_figures.unit, 
+    # food_item_figures.figure_type, 
+    # food_item_figures.quantity_kg as quantity_kg,
+    #             (select vfir.quantity_kg  from pp_meal_service.view_food_item_rework vfir 
+    #             where vfir.view_food_item_id = food_item.id
+    #             and vfir.id = (select max(vfir.id)
+    #                       from pp_meal_service.view_food_item_rework vfir, pp_meal_service.view_food_item fi
+    #                       where vfir.view_food_item_id = fi.id
+    #                       and vfir.view_food_item_id = food_item.id)) as rework, 
+    #    food_item_figures.created as food_item_figure_created
+    # from
+    #     pp_meal_service.view_current_state curr_state, 
+    #     pp_meal_service.view_service service,
+    #     pp_meal_service.view_meal_period_configuration meal_period_config,
+    #     pp_meal_service.view_food_group food_group,
+    #     pp_meal_service.view_food_item food_item,
+    #     pp_meal_service.view_food_item_figures food_item_figures
 
-        where curr_state.id = service.view_current_state_id
-        and service.id = food_group.view_service_id
-        and meal_period_config.view_service_id = service.id
-        and food_group.id = food_item.view_food_group_id
-        and food_item.id = food_item_figures.view_food_item_id
-        and food_item_figures.figure_type = 'PRODUCTION_ADJUSTMENT'
-        and food_item_figures.id = (select max(vfif2.id) from pp_meal_service.view_food_item_figures vfif2 
-                where food_item_figures.view_food_item_id  = vfif2.view_food_item_id)
-        and curr_state.site_id = {}
-        and service.start_date between '{}' and '{}'
-        order by service.id desc
-        """.format(self.site_id,self.date_start_time,self.date_end_time)
-        return wv.read_sql(q1,self.engine)
+    #     where curr_state.id = service.view_current_state_id
+    #     and service.id = food_group.view_service_id
+    #     and meal_period_config.view_service_id = service.id
+    #     and food_group.id = food_item.view_food_group_id
+    #     and food_item.id = food_item_figures.view_food_item_id
+    #     and food_item_figures.figure_type = 'PRODUCTION_ADJUSTMENT'
+    #     and food_item_figures.id = (select max(vfif2.id) from pp_meal_service.view_food_item_figures vfif2 
+    #             where food_item_figures.view_food_item_id  = vfif2.view_food_item_id)
+    #     and curr_state.site_id = {}
+    #     and service.start_date between '{}' and '{}'
+    #     order by service.id desc
+    #     """.format(self.site_id,self.date_start_time,self.date_end_time)
+    #     return wv.read_sql(q1,self.engine)
 
     @time_wrapper
     def pp_production(self):
         q1 = """select 
         meal_service_id,
         taxonomy_code,
         actual_production_unit,
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('27')
-VERSION_HOUR = int('12')
-VERSION_MINUTE = int('31')
+VERSION_HOUR = int('13')
+VERSION_MINUTE = int('58')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306271231
-version_date = '2023/06/27 12:31'
+PATCH_VERSION = 202306271358
+version_date = '2023/06/27 13:58'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## pp_project_pkg/wrangling.py

```diff
@@ -13,16 +13,18 @@
     """
     
     hub_custom_breakdown = queries_res[0]
     site_info = queries_res[1]
     pp_driver_input = queries_res[2]
     food_items = queries_res[3]
     meal_period_configuration = queries_res[4]
-    pp_production_rework = queries_res[5]
-    waste_data_for_site = queries_res[6]
+    #pp_production_rework = queries_res[5]
+    pp_production = queries_res[5]
+    pp_rework = queries_res[6]
+    waste_data_for_site = queries_res[7]
     
     meal_period_start = meal_period_configuration['waste_disposal_start_time'].values[0]
     meal_period_end = meal_period_configuration['waste_disposal_end_time'].values[0]
     
     meal_period_end_dt =parser.parse(meal_period_end)   
     meal_period_start_dt =parser.parse(meal_period_start)
     
@@ -31,14 +33,20 @@
 
     cover_count = None
     if len(actual_covers.values) > 0:
         cover_count = actual_covers.values[0]
     else:
         cover_count = covers.values[0]
     
+    pp_rework = pp_rework.drop(columns=['meal_service_id']).reset_index(drop=True)
+    pp_production_rework = pd.merge(pp_production, pp_rework, on=['taxonomy_code'])
+    name_pd = pd.read_csv('./taxcode_name_mapping.csv')
+    name_pd = name_pd.drop(columns=['Unnamed: 0']).reset_index(drop=True)
+    name_pd = name_pd.rename(columns={name_pd.columns[0]:'taxonomy_code',name_pd.columns[1]:'name'})
+    pp_production_rework = pd.merge(pp_production_rework, name_pd, on=['taxonomy_code'])
 
     actual_production_and_rework = pp_production_rework.copy()
     actual_production_and_rework['quantity_g'] = actual_production_and_rework['quantity_kg']*1000
     actual_production_and_rework['rework_g'] = actual_production_and_rework['rework']*1000
     
     joined_df = waste_data_for_site.join(hub_custom_breakdown.set_index('id'), on='reason_guid', how='inner')
```

## Comparing `pp_project_pkg-1.0.202306271231.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306271358.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306271231.dist-info/RECORD` & `pp_project_pkg-1.0.202306271358.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 mlflow_pipelines/train_model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/train_model/model_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=xW9v6KON3cAC3-4yP50rC6VCwv0tCeJ6h25oILWyGRw,5335
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
-pp_project_pkg/pp_tables.py,sha256=PdrOD0_6NzsFK5ADzDiopxQY9yc33TToLkI9w_h7Ug8,9193
+pp_project_pkg/pp_tables.py,sha256=UuU_ILMxc91vnMf8NbOomzzQfEyAdB2MQV_SvKQtIIU,9275
 pp_project_pkg/utils.py,sha256=qWUhyGz6Vz_0SOF_SvQbRlr2qxEIl2kqjvE32pZSipw,6657
-pp_project_pkg/version.py,sha256=jog7vDhcVN2Z43gq_AY5vjmopgShNdeJy4d0euNTGOw,396
-pp_project_pkg/wrangling.py,sha256=5B-LkqLulZm9RGNvN9BsU6T7vqra7pMGRwr0cj9ovdY,4602
-pp_project_pkg-1.0.202306271231.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306271231.dist-info/METADATA,sha256=UwxGcUQTgqu_tu8tsosEgv4Hlzr7K53z1bYnA1q9sBk,191
-pp_project_pkg-1.0.202306271231.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202306271231.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202306271231.dist-info/RECORD,,
+pp_project_pkg/version.py,sha256=n9zcW3AdRSeiMk54zx_Fikd4guLu7gqtaOBSgEvZVqA,396
+pp_project_pkg/wrangling.py,sha256=eMvIxt5SRXciI5Msb-n_I6Ekhs8tKORz3-Wsldattuw,5156
+pp_project_pkg-1.0.202306271358.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306271358.dist-info/METADATA,sha256=GTx0jmoh3JXrgh5UduzE5AjveMt0j4uEjRYvlB5diSU,191
+pp_project_pkg-1.0.202306271358.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202306271358.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202306271358.dist-info/RECORD,,
```

