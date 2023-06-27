# Comparing `tmp/pp_project_pkg-1.0.202306271035-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306271231-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 11714 bytes, number of entries: 20
+Zip file size: 12541 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:05 mlflow_pipelines/run.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/fetch_data/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:33 mlflow_pipelines/fetch_data/get_data.py
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-27 12:31 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-27 10:05 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
--rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-06 15:26 pp_project_pkg/pp_tables.py
+-rw-rw-r--  2.0 unx     9193 b- defN 23-Jun-27 12:30 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-20 14:19 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 10:35 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 12:31 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-20 09:33 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271035.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 10:35 pp_project_pkg-1.0.202306271035.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 10:35 pp_project_pkg-1.0.202306271035.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 10:35 pp_project_pkg-1.0.202306271035.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1796 b- defN 23-Jun-27 10:35 pp_project_pkg-1.0.202306271035.dist-info/RECORD
-20 files, 28180 bytes uncompressed, 8686 bytes compressed:  69.2%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306271231.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-27 12:31 pp_project_pkg-1.0.202306271231.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 12:31 pp_project_pkg-1.0.202306271231.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jun-27 12:31 pp_project_pkg-1.0.202306271231.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1799 b- defN 23-Jun-27 12:31 pp_project_pkg-1.0.202306271231.dist-info/RECORD
+20 files, 31526 bytes uncompressed, 9513 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271035.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306271231.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271035.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306271231.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271035.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306271231.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271035.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306271231.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306271035.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306271231.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_pipelines/fetch_data/get_data.py

```diff
@@ -0,0 +1,80 @@
+00000000: 6672 6f6d 206d 625f 7574 696c 732e 7372  from mb_utils.sr
+00000010: 6320 696d 706f 7274 206c 6f67 6769 6e67  c import logging
+00000020: 0a69 6d70 6f72 7420 6d62 2e70 616e 6461  .import mb.panda
+00000030: 7320 6173 2070 640a 6672 6f6d 2070 705f  s as pd.from pp_
+00000040: 7072 6f6a 6563 745f 706b 672e 7574 696c  project_pkg.util
+00000050: 7320 696d 706f 7274 2073 6974 655f 6461  s import site_da
+00000060: 7465 5f72 6573 2c63 6865 636b 5f72 6570  te_res,check_rep
+00000070: 6f72 745f 636c 6f73 655f 6461 7465 2c64  ort_close_date,d
+00000080: 6f77 6e6c 6f61 645f 7570 6c6f 6164 5f64  ownload_upload_d
+00000090: 6174 6573 5f72 6570 6f72 740a 696d 706f  ates_report.impo
+000000a0: 7274 2061 7267 7061 7273 650a 696d 706f  rt argparse.impo
+000000b0: 7274 2068 7964 7261 0a0a 4068 7964 7261  rt hydra..@hydra
+000000c0: 2e6d 6169 6e28 636f 6e66 6967 5f6e 616d  .main(config_nam
+000000d0: 653d 272e 2f63 6f6e 6669 672e 796d 6c27  e='./config.yml'
+000000e0: 290a 6465 6620 6665 7463 685f 6461 7461  ).def fetch_data
+000000f0: 5f72 756e 2861 7267 732c 6c6f 6767 6572  _run(args,logger
+00000100: 3d4e 6f6e 6529 3a0a 2020 2020 7369 7465  =None):.    site
+00000110: 5f6e 756d 6265 7220 3d20 6172 6773 2e73  _number = args.s
+00000120: 6974 655f 6964 0a20 2020 2073 6974 655f  ite_id.    site_
+00000130: 7374 6172 745f 6461 7465 203d 2061 7267  start_date = arg
+00000140: 732e 6461 7465 0a0a 2020 2020 7369 7465  s.date..    site
+00000150: 5f72 6573 203d 2020 7369 7465 5f64 6174  _res =  site_dat
+00000160: 655f 7265 7328 7369 7465 5f6e 756d 6265  e_res(site_numbe
+00000170: 722c 6c6f 6767 6572 3d6c 6f67 6765 7229  r,logger=logger)
+00000180: 0a20 2020 2072 6570 6f72 745f 7265 7320  .    report_res 
+00000190: 3d20 6368 6563 6b5f 7265 706f 7274 5f63  = check_report_c
+000001a0: 6c6f 7365 5f64 6174 6528 7369 7465 5f72  lose_date(site_r
+000001b0: 6573 2c73 7461 7274 5f64 6174 653d 7369  es,start_date=si
+000001c0: 7465 5f73 7461 7274 5f64 6174 6529 0a20  te_start_date). 
+000001d0: 2020 2069 6620 6c6f 6767 6572 3a0a 2020     if logger:.  
+000001e0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+000001f0: 6f28 7265 706f 7274 5f72 6573 2e68 6561  o(report_res.hea
+00000200: 6428 2929 0a0a 2020 2020 7265 706f 7274  d())..    report
+00000210: 5f64 6174 6573 5f72 6573 2020 3d20 646f  _dates_res  = do
+00000220: 776e 6c6f 6164 5f75 706c 6f61 645f 6461  wnload_upload_da
+00000230: 7465 735f 7265 706f 7274 2872 6570 6f72  tes_report(repor
+00000240: 745f 7265 732c 6c6f 6767 6572 3d6c 6f67  t_res,logger=log
+00000250: 6765 7229 0a20 2020 2069 6620 6c6f 6767  ger).    if logg
+00000260: 6572 3a0a 2020 2020 2020 2020 6c6f 6767  er:.        logg
+00000270: 6572 2e69 6e66 6f28 7265 706f 7274 5f64  er.info(report_d
+00000280: 6174 6573 5f72 6573 2e68 6561 6428 2929  ates_res.head())
+00000290: 0a0a 2020 2020 7265 7475 726e 2072 6570  ..    return rep
+000002a0: 6f72 745f 6461 7465 735f 7265 730a 0a0a  ort_dates_res...
+000002b0: 6966 205f 5f6e 616d 655f 5f20 3d3d 2027  if __name__ == '
+000002c0: 5f5f 6d61 696e 5f5f 273a 0a20 2020 2070  __main__':.    p
+000002d0: 6172 7365 7220 3d20 6172 6770 6172 7365  arser = argparse
+000002e0: 2e41 7267 756d 656e 7450 6172 7365 7228  .ArgumentParser(
+000002f0: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
+00000300: 7469 6f6e 3d22 5070 5f70 726f 6a65 6374  tion="Pp_project
+00000310: 2074 7261 696e 696e 6720 5363 7269 7074   training Script
+00000320: 2229 0a20 2020 2070 6172 7365 722e 6164  ").    parser.ad
+00000330: 645f 6172 6775 6d65 6e74 2822 2d64 222c  d_argument("-d",
+00000340: 222d 2d64 6174 6522 2c20 7479 7065 3d73  "--date", type=s
+00000350: 7472 2c20 6465 6661 756c 743d 2732 3032  tr, default='202
+00000360: 332d 3036 2d32 3027 202c 2068 656c 703d  3-06-20' , help=
+00000370: 2244 6174 6520 666f 7220 6765 7474 696e  "Date for gettin
+00000380: 6720 7468 6520 7761 7374 652f 7072 6f64  g the waste/prod
+00000390: 7563 7469 6f6e 2070 6c61 6e20 666f 722e  uction plan for.
+000003a0: 2044 6566 6175 6c74 203a 2032 3032 332d   Default : 2023-
+000003b0: 3036 2d30 3622 290a 2020 2020 7061 7273  06-06").    pars
+000003c0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+000003d0: 222d 7322 2c22 2d2d 7369 7465 5f69 6422  "-s","--site_id"
+000003e0: 2c20 7479 7065 3d69 6e74 2c64 6566 6175  , type=int,defau
+000003f0: 6c74 3d33 3036 3037 2c20 6865 6c70 3d22  lt=30607, help="
+00000400: 5369 7465 2069 642e 2044 6566 6175 6c74  Site id. Default
+00000410: 3a20 3330 3630 3722 290a 2020 2020 7061  : 30607").    pa
+00000420: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+00000430: 7428 222d 6c22 2c22 2d2d 6c6f 6767 6572  t("-l","--logger
+00000440: 222c 2074 7970 653d 7374 722c 6465 6661  ", type=str,defa
+00000450: 756c 743d 4e6f 6e65 2c20 6865 6c70 3d22  ult=None, help="
+00000460: 4c6f 6767 6572 2e20 4465 6661 756c 743a  Logger. Default:
+00000470: 204e 6f6e 6522 290a 2020 2020 6172 6773   None").    args
+00000480: 203d 2070 6172 7365 722e 7061 7273 655f   = parser.parse_
+00000490: 6172 6773 2829 0a20 2020 2069 6620 6172  args().    if ar
+000004a0: 6773 2e6c 6f67 6765 723a 0a20 2020 2020  gs.logger:.     
+000004b0: 2020 206c 6f67 6765 7220 3d20 6c6f 6767     logger = logg
+000004c0: 696e 672e 6c6f 6767 6572 0a20 2020 2066  ing.logger.    f
+000004d0: 6574 6368 5f64 6174 615f 7275 6e28 6172  etch_data_run(ar
+000004e0: 6773 2c6c 6f67 6765 723d 6c6f 6767 6572  gs,logger=logger
+000004f0: 29                                       )
```

## pp_project_pkg/pp_tables.py

```diff
@@ -14,15 +14,15 @@
         return result
     return wrapper
 
 
 class queries():
     def __init__(self,date = '2023-05-29',site_id= 30607 ,logger=None) :
           self.logger = logger
-          self.query_list = ['hub_custom_breakdown','site_info','pp_driver_input','food_items','meal_period_configuration','pp_production_rework','waste_data_for_site']
+          self.query_list = ['hub_custom_breakdown','site_info','pp_driver_input','food_items','meal_period_configuration','pp_production_rework','pp_production','pp_rework','waste_data_for_site']
           self.date = date
           self.engine = wv.ml_engine
           self.date_start_time = date + ' 00:00:00'
           self.date_end_time = date + ' 23:59:59'
           self.site_id = site_id
 
     @time_wrapper
@@ -109,21 +109,21 @@
     meal_period_config.meal_period,
     food_group.id as food_group_id, 
     food_item.id as food_item_id, 
     food_item."name",  
     food_item_figures.taxonomy_code,
     food_item_figures.unit, 
     food_item_figures.figure_type, 
-    food_item_figures.quantity_kg / 10 as quantity_kg,
+    food_item_figures.quantity_kg as quantity_kg,
                 (select vfir.quantity_kg  from pp_meal_service.view_food_item_rework vfir 
                 where vfir.view_food_item_id = food_item.id
                 and vfir.id = (select max(vfir.id)
                           from pp_meal_service.view_food_item_rework vfir, pp_meal_service.view_food_item fi
                           where vfir.view_food_item_id = fi.id
-                          and vfir.view_food_item_id = food_item.id)) / 1 as rework, 
+                          and vfir.view_food_item_id = food_item.id)) as rework, 
        food_item_figures.created as food_item_figure_created
     from
         pp_meal_service.view_current_state curr_state, 
         pp_meal_service.view_service service,
         pp_meal_service.view_meal_period_configuration meal_period_config,
         pp_meal_service.view_food_group food_group,
         pp_meal_service.view_food_item food_item,
@@ -140,14 +140,62 @@
         and curr_state.site_id = {}
         and service.start_date between '{}' and '{}'
         order by service.id desc
         """.format(self.site_id,self.date_start_time,self.date_end_time)
         return wv.read_sql(q1,self.engine)
 
     @time_wrapper
+    def pp_production(self):
+        q1 = """select 
+        meal_service_id,
+        taxonomy_code,
+        actual_production_unit,
+        actual_production_kg
+        from (
+            select 
+            svc.id as meal_service_id,
+            fi.taxonomy_code as taxonomy_code,
+            fif.quantity_unit as actual_production_unit,
+            fif.quantity_kg as actual_production_kg,
+            rank() over (partition by svc.id, fif.taxonomy_code order by fif.created desc) as rnk
+        from pp_meal_service.view_food_group as fg
+        inner join pp_meal_service.view_food_item as fi on fi.view_food_group_id = fg.id
+        inner join pp_meal_service.view_food_item_figures as fif on fif.view_food_item_id = fi.id
+        inner join pp_meal_service.view_service as svc on svc.id = fg.view_service_id
+        where svc.start_date between'{}' and '{}' 
+        and figure_type = 'PRODUCTION_ADJUSTMENT'
+        ) as ordered_figures
+        where rnk = 1""".format(self.date_start_time,self.date_end_time)
+        return wv.read_sql(q1,self.engine)
+
+    @time_wrapper
+    def pp_rework(self):
+        q1="""SELECT
+        meal_service_id,
+        taxonomy_code,
+        rework_unit,
+        rework_kg
+        from (
+            select 
+            svc.id as meal_service_id,
+            fi.taxonomy_code as taxonomy_code,
+            fir.quantity as rework_unit,
+            fir.quantity_kg as rework_kg,
+            rank() over (partition by svc.id, fir.view_food_item_id order by fir.created desc) as rnk
+        from pp_meal_service.view_food_group as fg
+        inner join pp_meal_service.view_food_item as fi on fi.view_food_group_id = fg.id
+        inner join pp_meal_service.view_food_item_rework as fir on fir.view_food_item_id = fi.id
+        inner join pp_meal_service.view_service as svc on svc.id = fg.view_service_id
+        where svc.start_date between '{}' and '{}' 
+        ) as ordered_figures
+        where rnk = 1""".format(self.date_start_time,self.date_end_time)
+        return wv.read_sql(q1,self.engine)
+
+
+    @time_wrapper
     def waste_data_for_site(self):
         q1 = """select e.id,
        site_guid, 
        item_id, 
        reason_guid, 
        m.value as weight_g,
        local_time,
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('27')
-VERSION_HOUR = int('10')
-VERSION_MINUTE = int('35')
+VERSION_HOUR = int('12')
+VERSION_MINUTE = int('31')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306271035
-version_date = '2023/06/27 10:35'
+PATCH_VERSION = 202306271231
+version_date = '2023/06/27 12:31'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306271035.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306271231.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306271035.dist-info/RECORD` & `pp_project_pkg-1.0.202306271231.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 mlflow_pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/run.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/fetch_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mlflow_pipelines/fetch_data/get_data.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mlflow_pipelines/fetch_data/get_data.py,sha256=nwWzNCKRJzDnWAFmauea7ux6VjCL8TpezEs63oL6JBQ,1265
 mlflow_pipelines/train_model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/train_model/model_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=xW9v6KON3cAC3-4yP50rC6VCwv0tCeJ6h25oILWyGRw,5335
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
-pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
+pp_project_pkg/pp_tables.py,sha256=PdrOD0_6NzsFK5ADzDiopxQY9yc33TToLkI9w_h7Ug8,9193
 pp_project_pkg/utils.py,sha256=qWUhyGz6Vz_0SOF_SvQbRlr2qxEIl2kqjvE32pZSipw,6657
-pp_project_pkg/version.py,sha256=zR3wElMDSfqeU7RXxPsdfLHCOSBZbIH5UzMwk2MrDBM,396
+pp_project_pkg/version.py,sha256=jog7vDhcVN2Z43gq_AY5vjmopgShNdeJy4d0euNTGOw,396
 pp_project_pkg/wrangling.py,sha256=5B-LkqLulZm9RGNvN9BsU6T7vqra7pMGRwr0cj9ovdY,4602
-pp_project_pkg-1.0.202306271035.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306271035.dist-info/METADATA,sha256=-UNh_n7PPdqgaGrVZHurZQST7RW3LZfhjUNfL42Ev5Q,191
-pp_project_pkg-1.0.202306271035.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202306271035.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202306271035.dist-info/RECORD,,
+pp_project_pkg-1.0.202306271231.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306271231.dist-info/METADATA,sha256=UwxGcUQTgqu_tu8tsosEgv4Hlzr7K53z1bYnA1q9sBk,191
+pp_project_pkg-1.0.202306271231.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202306271231.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202306271231.dist-info/RECORD,,
```

