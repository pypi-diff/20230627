# Comparing `tmp/validador_colab-1.0.0.tar.gz` & `tmp/validador_colab-1.1.0.tar.gz`

## Comparing `validador_colab-1.0.0.tar` & `validador_colab-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,46 @@
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-1.0.0/main.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-1.0.0/requirements.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/__init__.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/colab_counter.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/natural_one.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/sakura.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/smarket_counter.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/entities/validation_detail.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/errors/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/errors/divergent_data.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/errors/no_data_found.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/repositories/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/repositories/colab_counters.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/repositories/smarket_analytics.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/usecases/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/usecases/colab_service.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/core/usecases/smarket_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/configs/__init__.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/configs/configs.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/database/__init__.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/database/postgres.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/database/postgres_controle.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/repositories/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/repositories/colab_counters_repository.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/repositories/smarket_analytics_repository.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/routes/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/routes/daily_conf.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/utils/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/utils/break_no_data_found.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/infra/utils/clean_old_data.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/loop/__init__.py
--rw-r--r--   0        0        0    15078 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/loop/first_block.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 validador_colab-1.0.0/validador_colab/loop/reprocessing_first_block.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-1.0.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.0.0/README.md
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 validador_colab-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 validador_colab-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-1.1.0/main.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-1.1.0/requirements.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/entities/__init__.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/entities/colab_counter.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/entities/datamart_counter.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/entities/natural_one.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/entities/sakura.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/entities/smarket_counter.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/entities/validation_detail.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/errors/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/errors/divergent_data.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/errors/no_data_found.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/repositories/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/repositories/colab_counters.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/repositories/datamart_counters.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/repositories/smarket_analytics.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/usecases/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/usecases/colab_service.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/usecases/datamart_service.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/core/usecases/smarket_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/configs/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/configs/configs.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/database/__init__.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/database/postgres.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/database/postgres_controle.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/repositories/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/repositories/colab_counters_repository.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/repositories/datamart_counters_repository.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/repositories/nova consulta.txt
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/repositories/smarket_analytics_repository.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/routes/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/routes/daily_conf.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/utils/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/utils/break_no_data_found.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/infra/utils/clean_old_data.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/loop/__init__.py
+-rw-r--r--   0        0        0    16045 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/loop/first_block.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/loop/reprocessing_first_block.py
+-rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 validador_colab-1.1.0/validador_colab/loop/second_block.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-1.1.0/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.0/README.md
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 validador_colab-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 validador_colab-1.1.0/PKG-INFO
```

### Comparing `validador_colab-1.0.0/main.py` & `validador_colab-1.1.0/main.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/requirements.txt` & `validador_colab-1.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/core/entities/natural_one.py` & `validador_colab-1.1.0/validador_colab/core/entities/natural_one.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/core/entities/sakura.py` & `validador_colab-1.1.0/validador_colab/core/entities/sakura.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/core/usecases/colab_service.py` & `validador_colab-1.1.0/validador_colab/core/usecases/colab_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/core/usecases/smarket_service.py` & `validador_colab-1.1.0/validador_colab/core/usecases/smarket_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/infra/configs/configs.py` & `validador_colab-1.1.0/validador_colab/infra/configs/configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
         dotenv.load_dotenv()
         self.SMARKET_PROD_HOST = os.getenv('SMARKET_PROD_HOST', 'rds-smarket-next-pg.cf6ldthil3ep.sa-east-1.rds.amazonaws.com')
         self.SMARKET_PROD_PORT = os.getenv('SMARKET_PROD_PORT', '5432')
         self.SMARKET_PROD_NAME = os.getenv('SMARKET_PROD_NAME', 'db_supernosso')
         self.SMARKET_PROD_USERNAME = os.getenv('SMARKET_PROD_USERNAME', 'davi_araujo')
         self.SMARKET_PROD_PASSWORD = os.getenv('SMARKET_PROD_PASSWORD', 'DVAJPG@2021*')
-        self.COLAB_PROD_HOST = os.getenv('COLAB_PROD_HOST')
-        self.COLAB_PROD_PORT = os.getenv('COLAB_PROD_PORT')
-        self.COLAB_PROD_NAME = os.getenv('COLAB_PROD_NAME')
-        self.COLAB_PROD_USERNAME = os.getenv('COLAB_PROD_USERNAME')
-        self.COLAB_PROD_PASSWORD = os.getenv('COLAB_PROD_PASSWORD')
+        self.COLAB_PROD_HOST = os.getenv('COLAB_PROD_HOST', '172.32.0.9')
+        self.COLAB_PROD_PORT = os.getenv('COLAB_PROD_PORT', '5432')
+        self.COLAB_PROD_NAME = os.getenv('COLAB_PROD_NAME', 'dw')
+        self.COLAB_PROD_USERNAME = os.getenv('COLAB_PROD_USERNAME', 'gabriel_borges')
+        self.COLAB_PROD_PASSWORD = os.getenv('COLAB_PROD_PASSWORD', ')_Gabriel!3076!Borges,(')
         self.CLIENT_ID = ''
         self.COLAB_DB = 'dw'
         self.MODE = 'DEV'
 
 
 @lru_cache()
 def get_configs():
```

### Comparing `validador_colab-1.0.0/validador_colab/infra/database/postgres.py` & `validador_colab-1.1.0/validador_colab/infra/database/postgres.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/infra/database/postgres_controle.py` & `validador_colab-1.1.0/validador_colab/infra/database/postgres_controle.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/infra/repositories/colab_counters_repository.py` & `validador_colab-1.1.0/validador_colab/infra/repositories/colab_counters_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/infra/repositories/smarket_analytics_repository.py` & `validador_colab-1.1.0/validador_colab/infra/repositories/smarket_analytics_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/infra/routes/daily_conf.py` & `validador_colab-1.1.0/validador_colab/infra/routes/daily_conf.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/infra/utils/break_no_data_found.py` & `validador_colab-1.1.0/validador_colab/infra/utils/break_no_data_found.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/infra/utils/clean_old_data.py` & `validador_colab-1.1.0/validador_colab/infra/utils/clean_old_data.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/validador_colab/loop/first_block.py` & `validador_colab-1.1.0/validador_colab/loop/first_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,16 @@
 
     # Primeira validação: Se o produto está com os quantitativos iguais na fat_cupom e no Analytics
     for colab_unit in colab_data:
         for smarket_unit in smarket_data:
             if colab_unit.id_cliente == smarket_unit.client_id:
                 if colab_unit.date == smarket_unit.date:
                     if int(colab_unit.seqproduto) == int(smarket_unit.seqproduto):
+                        if colab_unit.seqproduto == 164059:
+                            print("Me gusta lá conchita")
                         if int(colab_unit.qtd_fatcupom) == int(smarket_unit.analytics):
                             if print_corretos:
                                 print('-------------------')
                                 print(f'Cliente {smarket_unit.client_id}')
                                 print(f"Data {smarket_unit.date}")
                                 print(f'Tudo certo no produto: {smarket_unit.seqproduto} - {smarket_unit.description}')
                                 print(f'Quantitativo no analytics: {smarket_unit.analytics}')
@@ -151,18 +153,18 @@
                 if client_id in colab_cliente_data:
                     if date in colab_cliente_data[client_id]:
                         if prod not in colab_cliente_data[client_id][date]:
                             if client_id not in produtos_ausentes_colab:
                                 produtos_ausentes_colab[client_id] = {}
                             if date not in produtos_ausentes_colab[client_id]:
                                 produtos_ausentes_colab[client_id][date] = []
-                            print(f"Produto {prod} não encontrado na base do colab para cliente: {client_id} na data: {date}")
+                            print(f"Produto {prod} não encontrado na base do colab para cliente: {client_id} na data: {date}, para a industria {industry_id}")
                             produtos_ausentes_colab[client_id][date].append(prod)
                     else:
-                        print(f"Data: {date} não encontrada na base do colab para cliente: {client_id}")
+                        print(f"Data: {date} não encontrada na base do colab para cliente: {client_id} para a industria {industry_id}")
                         if client_id not in datas_para_nao_subir:
                             datas_para_nao_subir[client_id] = []
                         if date not in datas_para_nao_subir[client_id]:
                             validation_intel.append(ValidationDetail(
                                 exec_date=datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                                 industry_id=industry_id,
                                 client_id=client_id,
@@ -170,47 +172,47 @@
                                 validation_status=False
                             ))
                             datas_para_nao_subir[client_id].append(date)
 
                         break
 
                 else:
-                    print(f"Cliente não encontrado na base do colab para industria: {industry_id}")
+                    print(f"Cliente {client_id} não encontrado na base do colab para industria: {industry_id}")
 
         # Gerador produtos ausentes analitycs
         for client_id, date_counter in colab_cliente_data.items():
             for date, prod_list in date_counter.items():
                 for prod in prod_list:
                     if client_id in prod_cliente_data:
                         if date in prod_cliente_data[client_id]:
                             if prod not in prod_cliente_data[client_id][date]:
                                 if client_id not in produtos_ausentes_analytics:
                                     produtos_ausentes_analytics[client_id] = {}
                                 if date not in produtos_ausentes_analytics[client_id]:
                                     produtos_ausentes_analytics[client_id][date] = []
                                 produtos_ausentes_analytics[client_id][date].append(prod)
-                                print(f"Produto {prod} não encontrado na base do analytics para cliente: {client_id} na data: {date}")
+                                print(f"Produto {prod} não encontrado na base do analytics para cliente: {client_id} na data: {date} para a industria {industry_id}")
 
                         else:
-                            print(f"Data: {date} não encontrada na base do analytics para cliente: {client_id}")
+                            print(f"Data: {date} não encontrada na base do analytics para cliente: {client_id} para a industria {industry_id}")
                             if client_id not in datas_para_nao_subir:
                                 datas_para_nao_subir[client_id] = []
                             if date not in datas_para_nao_subir[client_id]:
                                 validation_intel.append(ValidationDetail(
                                     exec_date=datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                                     industry_id=industry_id,
                                     client_id=client_id,
                                     sale_date=date,
                                     validation_status=False
                                 ))
                                 datas_para_nao_subir[client_id].append(date)
                             break
 
                     else:
-                        print(f"Cliente não encontrado na base do colab para industria: {industry_id}")
+                        print(f"Cliente {client_id} não encontrado na base do colab para industria: {industry_id}")
 
     # Geração da primeira tabela com base nos valores errados
     if len(count_produtos_errados) > 0:
         for client_id, counter in count_produtos_errados.items():
             for date, count in counter.items():
                 if client_id in datas_para_nao_subir:
                     if date.strftime("%Y-%m-%d") not in [x.strftime("%Y-%m-%d") for x in datas_para_nao_subir[client_id]]:
@@ -230,17 +232,32 @@
                                     exec_date=datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                                     industry_id=industry_id,
                                     client_id=client_id,
                                     sale_date=date,
                                     validation_status=True
                                 )
                             )
+                else:
+                    validation_intel.append(
+                        ValidationDetail(
+                            exec_date=datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                            industry_id=industry_id,
+                            client_id=client_id,
+                            sale_date=date,
+                            validation_status=False
+                        )
+                    )
+                    if client_id not in datas_para_nao_subir:
+                        datas_para_nao_subir[client_id] = []
+                    if date not in datas_para_nao_subir[client_id]:
+                        datas_para_nao_subir[client_id].append(date)
 
 
-    if len(count_produtos_certos) > 0 and len(count_produtos_errados) == 0:
+
+    if len(count_produtos_certos) > 0:
         for client_id, counter in count_produtos_certos.items():
             for date, count in counter.items():
                 if client_id in datas_para_nao_subir:
                     if date.strftime("%Y-%m-%d") not in [x.strftime("%Y-%m-%d") for x in datas_para_nao_subir[client_id]]:
                         if count > 0:
                             validation_intel.append(
                                 ValidationDetail(
@@ -260,22 +277,20 @@
                             sale_date=date,
                             validation_status=True
                         )
                     )
 
     # Inserindo os dados no banco de validation:
     sql_insert = """INSERT INTO
-        PUBLIC.CONTROLE(id_industria, id_cliente, dt_venda, status_validacao)
+        PUBLIC.CONTROLE(id_industria, id_cliente, dt_venda, status_validacao, etapa)
         VALUES
     """
     for validation in validation_intel:
-        sql_insert += f"""({int(validation.industry_id)}, {int(validation.client_id)}, '{validation.sale_date}', {bool(validation.validation_status)}),"""
+        sql_insert += f""" ({int(validation.industry_id)}, {int(validation.client_id)}, '{validation.sale_date}', {bool(validation.validation_status)}, 'fat_cupom'),"""
 
     sql_insert = sql_insert[:-1]
     print(sql_insert)
 
-    DB_CONTROLE.insert(sql_insert)
-
-
+    # DB_CONTROLE.insert(sql_insert)
 
 if __name__ == "__main__":
-    asyncio.run(first_block(11, '2023-06-22', '2023-06-22', False))
+    asyncio.run(first_block(11, '2023-06-23', '2023-06-23', False, True))
```

### Comparing `validador_colab-1.0.0/validador_colab/loop/reprocessing_first_block.py` & `validador_colab-1.1.0/validador_colab/loop/reprocessing_first_block.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/.gitignore` & `validador_colab-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `validador_colab-1.0.0/pyproject.toml` & `validador_colab-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "validador-colab"
 description = 'Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
-version = "1.0.0"
+version = "1.1.0"
 keywords = []
 authors = [
   { name = "Davi Amaral de Araujo", email = "davi@smarketsolutions.com.br" },
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `validador_colab-1.0.0/PKG-INFO` & `validador_colab-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validador-colab
-Version: 1.0.0
+Version: 1.1.0
 Summary: Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics
 Project-URL: Documentation, https://github.com/unknown/validador-colab#readme
 Project-URL: Issues, https://github.com/unknown/validador-colab/issues
 Project-URL: Source, https://github.com/unknown/validador-colab
 Author-email: Davi Amaral de Araujo <davi@smarketsolutions.com.br>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

