# Comparing `tmp/oking_oz-3.2.33.tar.gz` & `tmp/oking_oz-3.2.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oking_oz-3.2.33.tar", last modified: Thu Jun  1 17:54:02 2023, max compression
+gzip compressed data, was "oking_oz-3.2.34.tar", last modified: Tue Jun 27 19:49:18 2023, max compression
```

## Comparing `oking_oz-3.2.33.tar` & `oking_oz-3.2.34.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.755423 oking_oz-3.2.33/
--rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/LICENSE
--rw-rw-rw-   0        0        0       29 2023-01-26 18:55:11.000000 oking_oz-3.2.33/MANIFEST.in
--rw-rw-rw-   0        0        0      876 2023-06-01 17:54:02.750436 oking_oz-3.2.33/PKG-INFO
--rw-rw-rw-   0        0        0     1187 2023-01-26 18:55:11.000000 oking_oz-3.2.33/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.301634 oking_oz-3.2.33/oking_oz.egg-info/
--rw-rw-rw-   0        0        0      876 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1551 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-01 17:54:02.000000 oking_oz-3.2.33/oking_oz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-01-26 18:55:11.000000 oking_oz-3.2.33/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 17:54:02.756421 oking_oz-3.2.33/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-06-01 17:49:44.000000 oking_oz-3.2.33/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.317591 oking_oz-3.2.33/src/
--rw-rw-rw-   0        0        0     2979 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/__init__.py
--rw-rw-rw-   0        0        0    25475 2023-04-24 14:39:17.000000 oking_oz-3.2.33/src/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.359479 oking_oz-3.2.33/src/api/
--rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.434281 oking_oz-3.2.33/src/api/entities/
--rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/__init__.py
--rw-rw-rw-   0        0        0     5097 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/cliente.py
--rw-rw-rw-   0        0        0     4496 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/cliente_aprovado.py
--rw-rw-rw-   0        0        0      249 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/cliente_erp_code.py
--rw-rw-rw-   0        0        0      932 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/imposto_produto.py
--rw-rw-rw-   0        0        0     1171 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/lista_preco.py
--rw-rw-rw-   0        0        0      390 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/plano_pagamento_cliente.py
--rw-rw-rw-   0        0        0      934 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/entities/representante.py
--rw-rw-rw-   0        0        0      739 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/oking.py
--rw-rw-rw-   0        0        0    20636 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/api/okvendas.py
--rw-rw-rw-   0        0        0      886 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/api/slack.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.475170 oking_oz-3.2.33/src/database/
--rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/__init__.py
--rw-rw-rw-   0        0        0     2488 2023-01-30 16:28:22.000000 oking_oz-3.2.33/src/database/connection.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.532020 oking_oz-3.2.33/src/database/entities/
--rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/__init__.py
--rw-rw-rw-   0        0        0     1616 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/client.py
--rw-rw-rw-   0        0        0      253 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/client_payment_plan.py
--rw-rw-rw-   0        0        0     1077 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/price_list.py
--rw-rw-rw-   0        0        0      801 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/database/entities/product_tax.py
--rw-rw-rw-   0        0        0      639 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/entities/representative.py
--rw-rw-rw-   0        0        0    50196 2023-06-01 16:36:53.000000 oking_oz-3.2.33/src/database/queries.py
--rw-rw-rw-   0        0        0      327 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/sqlserver_db.py
--rw-rw-rw-   0        0        0     1106 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/database/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.638734 oking_oz-3.2.33/src/entities/
--rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/__init__.py
--rw-rw-rw-   0        0        0      628 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/invoice.py
--rw-rw-rw-   0        0        0      288 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/log.py
--rw-rw-rw-   0        0        0     6846 2023-05-12 18:44:31.000000 oking_oz-3.2.33/src/entities/order.py
--rw-rw-rw-   0        0        0    16869 2023-02-23 22:27:38.000000 oking_oz-3.2.33/src/entities/orderb2b.py
--rw-rw-rw-   0        0        0     6823 2023-05-12 18:23:12.000000 oking_oz-3.2.33/src/entities/orderb2c.py
--rw-rw-rw-   0        0        0     3014 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/pagamento.py
--rw-rw-rw-   0        0        0      351 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/photos_sku.py
--rw-rw-rw-   0        0        0      407 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/price.py
--rw-rw-rw-   0        0        0    10790 2023-02-23 22:27:38.000000 oking_oz-3.2.33/src/entities/product.py
--rw-rw-rw-   0        0        0     1959 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/response.py
--rw-rw-rw-   0        0        0      940 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/entities/tracking.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:54:02.734478 oking_oz-3.2.33/src/jobs/
--rw-rw-rw-   0        0        0        0 2023-01-26 18:55:11.000000 oking_oz-3.2.33/src/jobs/__init__.py
--rw-rw-rw-   0        0        0    18254 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/jobs/client_jobs.py
--rw-rw-rw-   0        0        0     8965 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/jobs/client_payment_plan_jobs.py
--rw-rw-rw-   0        0        0     2937 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/jobs/client_payment_plan_semaphore_jobs.py
--rw-rw-rw-   0        0        0    85575 2023-06-01 16:50:56.000000 oking_oz-3.2.33/src/jobs/order_jobs.py
--rw-rw-rw-   0        0        0    19666 2023-03-20 16:46:08.000000 oking_oz-3.2.33/src/jobs/price_jobs.py
--rw-rw-rw-   0        0        0    25107 2023-04-12 12:17:25.000000 oking_oz-3.2.33/src/jobs/products_jobs.py
--rw-rw-rw-   0        0        0     6841 2023-03-20 16:47:52.000000 oking_oz-3.2.33/src/jobs/representative_jobs.py
--rw-rw-rw-   0        0        0    12784 2023-03-20 16:49:42.000000 oking_oz-3.2.33/src/jobs/stock_jobs.py
--rw-rw-rw-   0        0        0     2003 2023-03-20 16:50:03.000000 oking_oz-3.2.33/src/jobs/system_jobs.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.651420 oking_oz-3.2.34/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.34/LICENSE
+-rw-rw-rw-   0        0        0       29 2022-06-03 11:48:57.000000 oking_oz-3.2.34/MANIFEST.in
+-rw-rw-rw-   0        0        0      935 2023-06-27 19:49:18.651420 oking_oz-3.2.34/PKG-INFO
+-rw-rw-rw-   0        0        0     1187 2022-06-03 12:55:44.000000 oking_oz-3.2.34/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.599281 oking_oz-3.2.34/oking_oz.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-06-27 19:49:18.000000 oking_oz-3.2.34/oking_oz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1551 2023-06-27 19:49:18.000000 oking_oz-3.2.34/oking_oz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 19:49:18.000000 oking_oz-3.2.34/oking_oz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-27 19:49:18.000000 oking_oz-3.2.34/oking_oz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-06-27 19:49:18.000000 oking_oz-3.2.34/oking_oz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-27 19:49:18.000000 oking_oz-3.2.34/oking_oz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-06-03 11:48:57.000000 oking_oz-3.2.34/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 19:49:18.651420 oking_oz-3.2.34/setup.cfg
+-rw-rw-rw-   0        0        0     1833 2023-06-27 19:45:46.000000 oking_oz-3.2.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.601795 oking_oz-3.2.34/src/
+-rw-rw-rw-   0        0        0     2979 2022-08-23 11:22:25.000000 oking_oz-3.2.34/src/__init__.py
+-rw-rw-rw-   0        0        0    25475 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.607323 oking_oz-3.2.34/src/api/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.616840 oking_oz-3.2.34/src/api/entities/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/api/entities/__init__.py
+-rw-rw-rw-   0        0        0     5097 2022-12-16 19:21:16.000000 oking_oz-3.2.34/src/api/entities/cliente.py
+-rw-rw-rw-   0        0        0     4496 2022-12-23 14:47:52.000000 oking_oz-3.2.34/src/api/entities/cliente_aprovado.py
+-rw-rw-rw-   0        0        0      249 2022-12-19 18:06:20.000000 oking_oz-3.2.34/src/api/entities/cliente_erp_code.py
+-rw-rw-rw-   0        0        0      932 2022-10-03 17:41:50.000000 oking_oz-3.2.34/src/api/entities/imposto_produto.py
+-rw-rw-rw-   0        0        0     1171 2022-10-03 17:41:50.000000 oking_oz-3.2.34/src/api/entities/lista_preco.py
+-rw-rw-rw-   0        0        0      390 2022-12-16 19:21:16.000000 oking_oz-3.2.34/src/api/entities/plano_pagamento_cliente.py
+-rw-rw-rw-   0        0        0      934 2022-12-16 19:21:16.000000 oking_oz-3.2.34/src/api/entities/representante.py
+-rw-rw-rw-   0        0        0      739 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/api/oking.py
+-rw-rw-rw-   0        0        0    20636 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/api/okvendas.py
+-rw-rw-rw-   0        0        0      886 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/api/slack.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.621842 oking_oz-3.2.34/src/database/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/database/__init__.py
+-rw-rw-rw-   0        0        0     2488 2022-08-23 11:22:25.000000 oking_oz-3.2.34/src/database/connection.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.628376 oking_oz-3.2.34/src/database/entities/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/database/entities/__init__.py
+-rw-rw-rw-   0        0        0     1616 2022-12-16 19:21:16.000000 oking_oz-3.2.34/src/database/entities/client.py
+-rw-rw-rw-   0        0        0      253 2022-12-16 19:21:16.000000 oking_oz-3.2.34/src/database/entities/client_payment_plan.py
+-rw-rw-rw-   0        0        0     1077 2022-10-03 17:41:50.000000 oking_oz-3.2.34/src/database/entities/price_list.py
+-rw-rw-rw-   0        0        0      801 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/database/entities/product_tax.py
+-rw-rw-rw-   0        0        0      639 2022-12-16 19:21:16.000000 oking_oz-3.2.34/src/database/entities/representative.py
+-rw-rw-rw-   0        0        0    50196 2023-06-27 19:45:46.000000 oking_oz-3.2.34/src/database/queries.py
+-rw-rw-rw-   0        0        0      327 2022-07-04 16:40:47.000000 oking_oz-3.2.34/src/database/sqlserver_db.py
+-rw-rw-rw-   0        0        0     1106 2022-07-04 16:40:47.000000 oking_oz-3.2.34/src/database/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.640896 oking_oz-3.2.34/src/entities/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/entities/__init__.py
+-rw-rw-rw-   0        0        0      628 2022-07-29 17:49:42.000000 oking_oz-3.2.34/src/entities/invoice.py
+-rw-rw-rw-   0        0        0      288 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/entities/log.py
+-rw-rw-rw-   0        0        0     7059 2023-06-27 19:45:46.000000 oking_oz-3.2.34/src/entities/order.py
+-rw-rw-rw-   0        0        0    16869 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/entities/orderb2b.py
+-rw-rw-rw-   0        0        0     6823 2023-05-12 18:30:53.000000 oking_oz-3.2.34/src/entities/orderb2c.py
+-rw-rw-rw-   0        0        0     3014 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/entities/pagamento.py
+-rw-rw-rw-   0        0        0      351 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/entities/photos_sku.py
+-rw-rw-rw-   0        0        0      407 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/entities/price.py
+-rw-rw-rw-   0        0        0    10790 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/entities/product.py
+-rw-rw-rw-   0        0        0     1959 2022-12-16 19:21:16.000000 oking_oz-3.2.34/src/entities/response.py
+-rw-rw-rw-   0        0        0      940 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/entities/tracking.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:49:18.650420 oking_oz-3.2.34/src/jobs/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.34/src/jobs/__init__.py
+-rw-rw-rw-   0        0        0    18254 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/jobs/client_jobs.py
+-rw-rw-rw-   0        0        0     8965 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/jobs/client_payment_plan_jobs.py
+-rw-rw-rw-   0        0        0     2937 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/jobs/client_payment_plan_semaphore_jobs.py
+-rw-rw-rw-   0        0        0    85575 2023-06-27 19:45:46.000000 oking_oz-3.2.34/src/jobs/order_jobs.py
+-rw-rw-rw-   0        0        0    19666 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/jobs/price_jobs.py
+-rw-rw-rw-   0        0        0    25107 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/jobs/products_jobs.py
+-rw-rw-rw-   0        0        0     6841 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/jobs/representative_jobs.py
+-rw-rw-rw-   0        0        0    12784 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/jobs/stock_jobs.py
+-rw-rw-rw-   0        0        0     2003 2023-04-10 18:55:42.000000 oking_oz-3.2.34/src/jobs/system_jobs.py
```

### Comparing `oking_oz-3.2.33/PKG-INFO` & `oking_oz-3.2.34/oking_oz.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
-Name: oking_oz
-Version: 3.2.33
+Name: oking-oz
+Version: 3.2.34
 Summary: Pacote de integração de produtos, preço, estoque e pedidos com o sistema OkVendas da Openk
+Home-page: UNKNOWN
 Author: Openk Tecnologia
 Author-email: <suporte.b2c@openk.com.br>
+License: UNKNOWN
 Keywords: python,oking,openk,okvendas,ok
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -21,7 +24,8 @@
 - Estoque
 - Pedido
 - Produtos
 - Clientes
 
 ## Manual
 <https://doc.clickup.com/d/h/2zgwt-5063/8b4903a4de0ccbd>
+
```

### Comparing `oking_oz-3.2.33/README.md` & `oking_oz-3.2.34/README.md`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/oking_oz.egg-info/PKG-INFO` & `oking_oz-3.2.34/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
-Name: oking-oz
-Version: 3.2.33
+Name: oking_oz
+Version: 3.2.34
 Summary: Pacote de integração de produtos, preço, estoque e pedidos com o sistema OkVendas da Openk
+Home-page: UNKNOWN
 Author: Openk Tecnologia
 Author-email: <suporte.b2c@openk.com.br>
+License: UNKNOWN
 Keywords: python,oking,openk,okvendas,ok
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -21,7 +24,8 @@
 - Estoque
 - Pedido
 - Produtos
 - Clientes
 
 ## Manual
 <https://doc.clickup.com/d/h/2zgwt-5063/8b4903a4de0ccbd>
+
```

### Comparing `oking_oz-3.2.33/oking_oz.egg-info/SOURCES.txt` & `oking_oz-3.2.34/oking_oz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/setup.py` & `oking_oz-3.2.34/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #     f = open('version.txt', 'w')
 #     f.write(f'\tOking {v} - Openk Tecnologia')
 #     f.close()
 
 
 # Utilizar o padrão x.x.x.xxxx para caso precise subir versão de testes para o respositorio test-pypi
 # Utilizar o padrão x.x.x para subir em produção
-version = '3.2.33'
+version = '3.2.34'
 package_name = "oking_oz" if len([c for c in version if c == '.']) < 3 else 'okingtest'
 # save_version(version)
 setup(
     name=package_name,
     version=version,
     author="Openk Tecnologia",
     author_email="<suporte.b2c@openk.com.br>",
```

### Comparing `oking_oz-3.2.33/src/__init__.py` & `oking_oz-3.2.34/src/__init__.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/__main__.py` & `oking_oz-3.2.34/src/__main__.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/api/entities/cliente.py` & `oking_oz-3.2.34/src/api/entities/cliente.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/api/entities/cliente_aprovado.py` & `oking_oz-3.2.34/src/api/entities/cliente_aprovado.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/api/entities/imposto_produto.py` & `oking_oz-3.2.34/src/api/entities/imposto_produto.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/api/entities/lista_preco.py` & `oking_oz-3.2.34/src/api/entities/lista_preco.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/api/entities/representante.py` & `oking_oz-3.2.34/src/api/entities/representante.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/api/oking.py` & `oking_oz-3.2.34/src/api/oking.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/api/okvendas.py` & `oking_oz-3.2.34/src/api/okvendas.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/api/slack.py` & `oking_oz-3.2.34/src/api/slack.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/database/connection.py` & `oking_oz-3.2.34/src/database/connection.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/database/entities/client.py` & `oking_oz-3.2.34/src/database/entities/client.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/database/entities/price_list.py` & `oking_oz-3.2.34/src/database/entities/price_list.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/database/entities/product_tax.py` & `oking_oz-3.2.34/src/database/entities/product_tax.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/database/entities/representative.py` & `oking_oz-3.2.34/src/database/entities/representative.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/database/queries.py` & `oking_oz-3.2.34/src/database/queries.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/database/utils.py` & `oking_oz-3.2.34/src/database/utils.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/entities/invoice.py` & `oking_oz-3.2.34/src/entities/invoice.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/entities/order.py` & `oking_oz-3.2.34/src/entities/orderb2c.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import List
+from typing import List, Dict
 
 class Queue:
     def __init__(self, pedido_id, data_pedido, status, protocolo, data_fila, observacao, valor_total=0.0, numero_pedido_externo='', **kwargs):
         self.order_id = pedido_id
         self.date = data_pedido
         self.status = status
         self.protocol = protocolo
         self.__dict__.update(kwargs)
 
 
-class Order:
+class OrderB2C:
     def __init__(self, id: int, pedido_venda_id: str, data_pedido: str, data_geracao: str,
                  valor_total: float, valor_forma_pagamento: float, valor_desconto: float, valor_frete: float,
                  status: str, quantidade_titulos: int, previsao_entrega: str, codigo_rastreio: str,
                  canal_id: int, transportadora_id: str, transportadora: str, servico_id: int, servico: str,
                  codigo_carga: str, protocolo: str, transacao, usuario: dict, pagamento: list, itens: list,
                  itens_brinde, itens_personalizados, forma_pagamento_parceiro, forma_envio_parceiro: dict,
                  pedido_nota_fiscal, data_entrega: str = str(), data_status: str = str(), cnpj_intermediador='', cnpj_instituicao_pagamento='', canal_site: str = '',
-                 valor_adicional_forma_pagamento: float = 0.0, codigo_pedido_canal_alternativo: str = '', codigo_referencia: str = ''):
+                 valor_adicional_forma_pagamento: float = 0.0, codigo_pedido_canal_alternativo: str = '', codigo_referencia: str = '', **kwargs):
         self.order_id: int = id
         self.order_code: str = pedido_venda_id
         self.date: str = data_pedido
         self.erp_code: str = codigo_referencia
         self.total_amount: float = valor_total
         self.total_discount: float = valor_desconto
         self.freight_amount: float = valor_frete
@@ -31,85 +31,85 @@
         self.carrier: str = transportadora
         self.user: User = User(**usuario)
         self.additional_payment_amount: float = valor_adicional_forma_pagamento
         self.items: List[OrderItem] = [OrderItem(**i) for i in itens]
         self.channel_id = canal_id
         self.mediator_cnpj: str = cnpj_intermediador
         self.payment_institution_cnpj: str = cnpj_instituicao_pagamento
+        self.__dict__.update(kwargs)
 
         payments: List[Payment] = [Payment(**p) for p in pagamento]
         if len(payments) > 0:
             self.paid_date = payments[0].paid_date
             self.flag = payments[0].flag
             self.erp_payment_condition = payments[0].erp_payment_condition
             self.parcels = payments[0].parcels
             self.payment_type = payments[0].type
             self.purchase_code = payments[0].purchase_code
-            self.erp_payment_option = payments[0].erp_payment_option
 
         try:
             partner_shipping_methods: List[PartnerShippingMethod] = [PartnerShippingMethod(**f) for f in forma_envio_parceiro]
         except Exception:
             partner_shipping_methods: List[PartnerShippingMethod] = [PartnerShippingMethod(**forma_envio_parceiro)]
 
         if len(partner_shipping_methods) > 0:
             self.shipping_mode = partner_shipping_methods[0].shipping_mode
 
 
 class PartnerShippingMethod:
     def __init__(self, codigo_rastreio: str, forma_envio: str, tipo_envio: str, status_envio: str, data_previsao_postagem: str, modo_envio: str,
-                 plp: str, rota: str, mega_rota: str):
+                 plp: str, rota: str, mega_rota: str, **kwargs):
         self.shipping_mode: str = modo_envio
+        self.__dict__.update(kwargs)
 
 
 class Payment:
     def __init__(self, opcao_pagamento: str, parcelas: int, bandeira: str, condicao_pagamento_erp: str, tabela_financiamento_rsvarejo: str,
                  tipo_venda_rsvarejo: str, canal_venda_id: str, canal_venda: str, numero_cupom: str, valor_cupom: float, codigo_compra: str,
-                 codigo_pedido_canal: str, data_movimento: str, codigo_mercado: str, titulos, opcao_pagamento_erp: str = None, **kwargs):
+                 codigo_pedido_canal: str, data_movimento: str, codigo_mercado: str, titulos, **kwargs):
         self.type: str = opcao_pagamento
         self.erp_payment_condition: str = condicao_pagamento_erp
         self.parcels: int = parcelas
         self.flag: str = bandeira
         self.paid_date: str = titulos[0]['data_pago']
         self.purchase_code: str = codigo_compra
-        self.erp_payment_option: str = opcao_pagamento_erp
         self.__dict__.update(kwargs)
 
-
 class User:
     def __init__(self, codigo_referencia: str, nome: str, razao_social: str, cpf: str, rg: str, data_nascimento: str,
                  sexo: str, email: str, orgao: str, RegistroEstadual: str, TelefoneResidencial: str, TelefoneCelular: str,
-                 Endereco: dict, EnderecoEntrega: dict, cpnj: str = '', cnpj: str = ''):
+                 Endereco: dict, EnderecoEntrega: dict, cpnj: str = '', cnpj: str = '', **kwargs):
         # adicionado cpnj acima para adaptar a api b2c da Jade
         self.erp_code: str = codigo_referencia
         self.name: str = nome
         self.company_name: str = razao_social
         self.cpf: str = cpf
         self.cnpj: str = cnpj
         self.email: str = email
         self.residential_phone: str = TelefoneResidencial
         self.mobile_phone: str = TelefoneCelular
         self.address: Address = Address(**EnderecoEntrega)
         self.cnpj: str = cnpj
+        self.__dict__.update(kwargs)
 
 
 
 class Address:
     def __init__(self, cep: str, logradouro: str, numero: str, complemento: str, bairro: str, cidade: str,
-                 estado: str, pais: str, referencia: str, descricao: str, tipo_logradouro: str, codigo_ibge: str):
+                 estado: str, pais: str, referencia: str, descricao: str, tipo_logradouro: str, **kwargs):
         self.zipcode: str = cep
         self.address_line: str = logradouro
         self.number: str = numero
         self.complement: str = complemento
         self.neighbourhood: str = bairro or ""
         self.city: str = cidade
         self.state: str = estado
         self.reference: str = referencia
         self.address_type: str = tipo_logradouro or 'Rua'
-        self.ibge_code: str = codigo_ibge
+        self.__dict__.update(kwargs)
 
 
 class OrderItem:
     def __init__(self, sku_principal: str, sku_variacao: str, sku_reference: str, hierarquia_variacao: str, is_restock: bool, codigo_externo_restock: str,
                  ean: str, quantidade: int, value: float, valor_desconto: float, altura: float, comprimento: float, largura: float, peso: float, volume: float,
                  filial_expedicao: str, filial_faturamento: str, cnpj_filial_venda: str, unidade_medida: str = str(), valor_comissao_frete: float = 0.0, valor_frete: float = 0.0,
                  percentual_comissao: float = 0.0, valor_comissao: float = 0.0, tipo_anuncio: str = '', **kwargs):
@@ -121,7 +121,8 @@
         self.value: float = value
         self.discount: float = valor_desconto
         self.freight_value: float = valor_frete
         self.expedition_branch: str = filial_expedicao
         self.invoice_branch: str = filial_faturamento
         self.selling_branch_cnpj: str = cnpj_filial_venda
         self.__dict__.update(kwargs)
+
```

### Comparing `oking_oz-3.2.33/src/entities/orderb2b.py` & `oking_oz-3.2.34/src/entities/orderb2b.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/entities/orderb2c.py` & `oking_oz-3.2.34/src/entities/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import List, Dict
+from typing import List
+
 
 class Queue:
     def __init__(self, pedido_id, data_pedido, status, protocolo, data_fila, observacao, valor_total=0.0, numero_pedido_externo='', **kwargs):
         self.order_id = pedido_id
         self.date = data_pedido
         self.status = status
         self.protocol = protocolo
         self.__dict__.update(kwargs)
 
 
-class OrderB2C:
+class Order:
     def __init__(self, id: int, pedido_venda_id: str, data_pedido: str, data_geracao: str,
                  valor_total: float, valor_forma_pagamento: float, valor_desconto: float, valor_frete: float,
                  status: str, quantidade_titulos: int, previsao_entrega: str, codigo_rastreio: str,
                  canal_id: int, transportadora_id: str, transportadora: str, servico_id: int, servico: str,
                  codigo_carga: str, protocolo: str, transacao, usuario: dict, pagamento: list, itens: list,
                  itens_brinde, itens_personalizados, forma_pagamento_parceiro, forma_envio_parceiro: dict,
                  pedido_nota_fiscal, data_entrega: str = str(), data_status: str = str(), cnpj_intermediador='', cnpj_instituicao_pagamento='', canal_site: str = '',
@@ -31,53 +32,56 @@
         self.carrier: str = transportadora
         self.user: User = User(**usuario)
         self.additional_payment_amount: float = valor_adicional_forma_pagamento
         self.items: List[OrderItem] = [OrderItem(**i) for i in itens]
         self.channel_id = canal_id
         self.mediator_cnpj: str = cnpj_intermediador
         self.payment_institution_cnpj: str = cnpj_instituicao_pagamento
-        self.__dict__.update(kwargs)
 
         payments: List[Payment] = [Payment(**p) for p in pagamento]
         if len(payments) > 0:
             self.paid_date = payments[0].paid_date
             self.flag = payments[0].flag
             self.erp_payment_condition = payments[0].erp_payment_condition
             self.parcels = payments[0].parcels
             self.payment_type = payments[0].type
             self.purchase_code = payments[0].purchase_code
+            self.erp_payment_option = payments[0].erp_payment_option
 
         try:
             partner_shipping_methods: List[PartnerShippingMethod] = [PartnerShippingMethod(**f) for f in forma_envio_parceiro]
         except Exception:
             partner_shipping_methods: List[PartnerShippingMethod] = [PartnerShippingMethod(**forma_envio_parceiro)]
 
         if len(partner_shipping_methods) > 0:
             self.shipping_mode = partner_shipping_methods[0].shipping_mode
+        self.__dict__.update(kwargs)
 
 
 class PartnerShippingMethod:
     def __init__(self, codigo_rastreio: str, forma_envio: str, tipo_envio: str, status_envio: str, data_previsao_postagem: str, modo_envio: str,
                  plp: str, rota: str, mega_rota: str, **kwargs):
         self.shipping_mode: str = modo_envio
         self.__dict__.update(kwargs)
 
 
 class Payment:
     def __init__(self, opcao_pagamento: str, parcelas: int, bandeira: str, condicao_pagamento_erp: str, tabela_financiamento_rsvarejo: str,
                  tipo_venda_rsvarejo: str, canal_venda_id: str, canal_venda: str, numero_cupom: str, valor_cupom: float, codigo_compra: str,
-                 codigo_pedido_canal: str, data_movimento: str, codigo_mercado: str, titulos, **kwargs):
+                 codigo_pedido_canal: str, data_movimento: str, codigo_mercado: str, titulos, opcao_pagamento_erp: str = None, **kwargs):
         self.type: str = opcao_pagamento
         self.erp_payment_condition: str = condicao_pagamento_erp
         self.parcels: int = parcelas
         self.flag: str = bandeira
         self.paid_date: str = titulos[0]['data_pago']
         self.purchase_code: str = codigo_compra
+        self.erp_payment_option: str = opcao_pagamento_erp
         self.__dict__.update(kwargs)
 
+
 class User:
     def __init__(self, codigo_referencia: str, nome: str, razao_social: str, cpf: str, rg: str, data_nascimento: str,
                  sexo: str, email: str, orgao: str, RegistroEstadual: str, TelefoneResidencial: str, TelefoneCelular: str,
                  Endereco: dict, EnderecoEntrega: dict, cpnj: str = '', cnpj: str = '', **kwargs):
         # adicionado cpnj acima para adaptar a api b2c da Jade
         self.erp_code: str = codigo_referencia
         self.name: str = nome
@@ -91,24 +95,26 @@
         self.cnpj: str = cnpj
         self.__dict__.update(kwargs)
 
 
 
 class Address:
     def __init__(self, cep: str, logradouro: str, numero: str, complemento: str, bairro: str, cidade: str,
-                 estado: str, pais: str, referencia: str, descricao: str, tipo_logradouro: str, **kwargs):
+                 estado: str, pais: str, referencia: str, descricao: str, tipo_logradouro: str, codigo_ibge: str
+                 , **kwargs):
         self.zipcode: str = cep
         self.address_line: str = logradouro
         self.number: str = numero
         self.complement: str = complemento
         self.neighbourhood: str = bairro or ""
         self.city: str = cidade
         self.state: str = estado
         self.reference: str = referencia
         self.address_type: str = tipo_logradouro or 'Rua'
+        self.ibge_code: str = codigo_ibge
         self.__dict__.update(kwargs)
 
 
 class OrderItem:
     def __init__(self, sku_principal: str, sku_variacao: str, sku_reference: str, hierarquia_variacao: str, is_restock: bool, codigo_externo_restock: str,
                  ean: str, quantidade: int, value: float, valor_desconto: float, altura: float, comprimento: float, largura: float, peso: float, volume: float,
                  filial_expedicao: str, filial_faturamento: str, cnpj_filial_venda: str, unidade_medida: str = str(), valor_comissao_frete: float = 0.0, valor_frete: float = 0.0,
@@ -121,8 +127,7 @@
         self.value: float = value
         self.discount: float = valor_desconto
         self.freight_value: float = valor_frete
         self.expedition_branch: str = filial_expedicao
         self.invoice_branch: str = filial_faturamento
         self.selling_branch_cnpj: str = cnpj_filial_venda
         self.__dict__.update(kwargs)
-
```

### Comparing `oking_oz-3.2.33/src/entities/pagamento.py` & `oking_oz-3.2.34/src/entities/pagamento.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/entities/product.py` & `oking_oz-3.2.34/src/entities/product.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/entities/response.py` & `oking_oz-3.2.34/src/entities/response.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/entities/tracking.py` & `oking_oz-3.2.34/src/entities/tracking.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/client_jobs.py` & `oking_oz-3.2.34/src/jobs/client_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/client_payment_plan_jobs.py` & `oking_oz-3.2.34/src/jobs/client_payment_plan_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/client_payment_plan_semaphore_jobs.py` & `oking_oz-3.2.34/src/jobs/client_payment_plan_semaphore_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/order_jobs.py` & `oking_oz-3.2.34/src/jobs/order_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/price_jobs.py` & `oking_oz-3.2.34/src/jobs/price_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/products_jobs.py` & `oking_oz-3.2.34/src/jobs/products_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/representative_jobs.py` & `oking_oz-3.2.34/src/jobs/representative_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/stock_jobs.py` & `oking_oz-3.2.34/src/jobs/stock_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.33/src/jobs/system_jobs.py` & `oking_oz-3.2.34/src/jobs/system_jobs.py`

 * *Files identical despite different names*

