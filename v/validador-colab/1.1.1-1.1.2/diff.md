# Comparing `tmp/validador_colab-1.1.1.tar.gz` & `tmp/validador_colab-1.1.2.tar.gz`

## Comparing `validador_colab-1.1.1.tar` & `validador_colab-1.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-1.1.1/main.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-1.1.1/requirements.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/entities/__init__.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/entities/colab_counter.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/entities/datamart_counter.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/entities/natural_one.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/entities/sakura.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/entities/smarket_counter.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/entities/validation_detail.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/errors/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/errors/divergent_data.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/errors/no_data_found.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/repositories/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/repositories/colab_counters.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/repositories/datamart_counters.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/repositories/smarket_analytics.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/usecases/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/usecases/colab_service.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/usecases/datamart_service.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/core/usecases/smarket_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/configs/__init__.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/configs/configs.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/database/__init__.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/database/postgres.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/database/postgres_controle.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/repositories/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/repositories/colab_counters_repository.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/repositories/datamart_counters_repository.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/repositories/nova consulta.txt
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/repositories/smarket_analytics_repository.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/routes/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/routes/daily_conf.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/utils/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/utils/break_no_data_found.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/infra/utils/clean_old_data.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/loop/__init__.py
--rw-r--r--   0        0        0    16043 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/loop/first_block.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/loop/reprocessing_first_block.py
--rw-r--r--   0        0        0    16093 2020-02-02 00:00:00.000000 validador_colab-1.1.1/validador_colab/loop/second_block.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-1.1.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.1/README.md
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 validador_colab-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 validador_colab-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-1.1.2/main.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-1.1.2/requirements.txt
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/entities/__init__.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/entities/colab_counter.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/entities/datamart_counter.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/entities/natural_one.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/entities/sakura.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/entities/smarket_counter.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/entities/validation_detail.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/errors/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/errors/divergent_data.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/errors/no_data_found.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/repositories/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/repositories/colab_counters.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/repositories/datamart_counters.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/repositories/smarket_analytics.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/usecases/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/usecases/colab_service.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/usecases/datamart_service.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/core/usecases/smarket_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/configs/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/configs/configs.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/database/__init__.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/database/postgres.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/database/postgres_controle.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/repositories/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/repositories/colab_counters_repository.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/repositories/datamart_counters_repository.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/repositories/nova consulta.txt
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/repositories/smarket_analytics_repository.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/routes/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/routes/daily_conf.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/utils/__init__.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/utils/break_no_data_found.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/infra/utils/clean_old_data.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/loop/__init__.py
+-rw-r--r--   0        0        0    16056 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/loop/first_block.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/loop/reprocessing_first_block.py
+-rw-r--r--   0        0        0    16109 2020-02-02 00:00:00.000000 validador_colab-1.1.2/validador_colab/loop/second_block.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-1.1.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-1.1.2/README.md
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 validador_colab-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 validador_colab-1.1.2/PKG-INFO
```

### Comparing `validador_colab-1.1.1/main.py` & `validador_colab-1.1.2/main.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/requirements.txt` & `validador_colab-1.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/core/entities/natural_one.py` & `validador_colab-1.1.2/validador_colab/core/entities/natural_one.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/core/entities/sakura.py` & `validador_colab-1.1.2/validador_colab/core/entities/sakura.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/core/usecases/colab_service.py` & `validador_colab-1.1.2/validador_colab/core/usecases/colab_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/core/usecases/datamart_service.py` & `validador_colab-1.1.2/validador_colab/core/usecases/datamart_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/core/usecases/smarket_service.py` & `validador_colab-1.1.2/validador_colab/core/usecases/smarket_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/configs/configs.py` & `validador_colab-1.1.2/validador_colab/infra/configs/configs.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/database/postgres.py` & `validador_colab-1.1.2/validador_colab/infra/database/postgres.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/database/postgres_controle.py` & `validador_colab-1.1.2/validador_colab/infra/database/postgres_controle.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/repositories/colab_counters_repository.py` & `validador_colab-1.1.2/validador_colab/infra/repositories/colab_counters_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/repositories/datamart_counters_repository.py` & `validador_colab-1.1.2/validador_colab/infra/repositories/datamart_counters_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/repositories/nova consulta.txt` & `validador_colab-1.1.2/validador_colab/infra/repositories/nova consulta.txt`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/repositories/smarket_analytics_repository.py` & `validador_colab-1.1.2/validador_colab/infra/repositories/smarket_analytics_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/routes/daily_conf.py` & `validador_colab-1.1.2/validador_colab/infra/routes/daily_conf.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/infra/utils/break_no_data_found.py` & `validador_colab-1.1.2/validador_colab/infra/utils/break_no_data_found.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import datetime
 
-def break_no_data_found(industry, date_start, date_end):
 
-    sql_base = "INSERT INTO PUBLIC.CONTROLE(id_industria, id_cliente, dt_venda, status_validacao) VALUES "
+def break_no_data_found(industry, date_start, date_end, etapa):
+
+    if not etapa:
+        raise ValueError('Missing parameter etapa')
+
+    sql_base = "INSERT INTO PUBLIC.CONTROLE(id_industria, id_cliente, dt_venda, status_validacao, etapa) VALUES "
 
     date_start = datetime.datetime.strptime(date_start, "%Y-%m-%d")
     date_finish = datetime.datetime.strptime(date_end, "%Y-%m-%d")
     numdays = date_finish - date_start
 
     date_list = [date_finish - datetime.timedelta(days=x) for x in range(numdays.days + 1)]
 
     for date in date_list:
         for client in industry.clients:
-            sql_base += f"""({industry.id},{client},'{date.strftime("%Y-%m-%d")}', false),"""
+            sql_base += f"""({industry.id},{client},'{date.strftime("%Y-%m-%d")}', false, '{etapa}'),"""
 
     sql_base = sql_base[:-1]
     return sql_base
 
 if __name__ == "__main__":
     from validador_colab.core.entities import Sakura
     break_no_data_found(Sakura(), '2023-06-20', '2023-06-21')
```

### Comparing `validador_colab-1.1.1/validador_colab/infra/utils/clean_old_data.py` & `validador_colab-1.1.2/validador_colab/infra/utils/clean_old_data.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/loop/first_block.py` & `validador_colab-1.1.2/validador_colab/loop/first_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if len(smarket_data) == 0 or len(colab_data) == 0:
         print("Erro na execução:")
         print(f"Data de consulta: {date_start} - {date_end}")
         print(f"len(smarket_data) = {len(smarket_data)}")
         print(f"len(colab_data) = {len(colab_data)}")
         print("Classificando dias como não aptos a atualização")
 
-        DB_CONTROLE.insert(break_no_data_found(industry, date_start, date_end))
+        DB_CONTROLE.insert(break_no_data_found(industry, date_start, date_end, 'fat_cupom'))
         print("Finalizando processo")
         return 0
 
     #esta merda aqui vai ficar troncha, loop dentro de loop, mas é o que tem pra hoje
     print('Iniciando processamento')
     count_produtos_certos = {}
     count_produtos_errados = {}
```

### Comparing `validador_colab-1.1.1/validador_colab/loop/reprocessing_first_block.py` & `validador_colab-1.1.2/validador_colab/loop/reprocessing_first_block.py`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/validador_colab/loop/second_block.py` & `validador_colab-1.1.2/validador_colab/loop/second_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if len(smarket_data) == 0 or len(datamart_data) == 0:
         print("Erro na execução:")
         print(f"Data de consulta: {date_start} - {date_end}")
         print(f"len(smarket_data) = {len(smarket_data)}")
         print(f"len(colab_data) = {len(datamart_data)}")
         print("Classificando dias como não aptos a atualização")
 
-        # DB_CONTROLE.insert(break_no_data_found(industry, date_start, date_end))
+        DB_CONTROLE.insert(break_no_data_found(industry, date_start, date_end, 'datamart'))
         print("Finalizando processo")
         return 0
 
     #esta merda aqui vai ficar troncha, loop dentro de loop, mas é o que tem pra hoje
     print('Iniciando processamento')
     count_produtos_certos = {}
     count_produtos_errados = {}
@@ -286,8 +286,8 @@
 
     sql_insert = sql_insert[:-1]
     print(sql_insert)
 
     DB_CONTROLE.insert(sql_insert)
 
 if __name__ == "__main__":
-    asyncio.run(second_block(13, '2023-06-18', '2023-06-18', False))
+    asyncio.run(second_block(13, '2023-06-18', '2023-06-18', False, True))
```

### Comparing `validador_colab-1.1.1/.gitignore` & `validador_colab-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `validador_colab-1.1.1/pyproject.toml` & `validador_colab-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "validador-colab"
 description = 'Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
-version = "1.1.1"
+version = "1.1.2"
 keywords = []
 authors = [
   { name = "Davi Amaral de Araujo", email = "davi@smarketsolutions.com.br" },
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `validador_colab-1.1.1/PKG-INFO` & `validador_colab-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validador-colab
-Version: 1.1.1
+Version: 1.1.2
 Summary: Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics
 Project-URL: Documentation, https://github.com/unknown/validador-colab#readme
 Project-URL: Issues, https://github.com/unknown/validador-colab/issues
 Project-URL: Source, https://github.com/unknown/validador-colab
 Author-email: Davi Amaral de Araujo <davi@smarketsolutions.com.br>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

