# Comparing `tmp/SNIIMAPP_2-0.2.1.tar.gz` & `tmp/SNIIMAPP_2-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNIIMAPP_2-0.2.1.tar", last modified: Mon Jun 26 18:51:28 2023, max compression
+gzip compressed data, was "SNIIMAPP_2-0.2.2.tar", last modified: Mon Jun 26 22:40:11 2023, max compression
```

## Comparing `SNIIMAPP_2-0.2.1.tar` & `SNIIMAPP_2-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-26 18:51:28.904553 SNIIMAPP_2-0.2.1/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1074 2023-06-26 18:42:46.000000 SNIIMAPP_2-0.2.1/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1166 2023-06-26 18:51:28.904553 SNIIMAPP_2-0.2.1/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      672 2023-06-26 18:02:07.000000 SNIIMAPP_2-0.2.1/README.md
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-26 18:51:28.904553 SNIIMAPP_2-0.2.1/SNIIMAPP_2.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1166 2023-06-26 18:51:28.000000 SNIIMAPP_2-0.2.1/SNIIMAPP_2.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      185 2023-06-26 18:51:28.000000 SNIIMAPP_2-0.2.1/SNIIMAPP_2.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-26 18:51:28.000000 SNIIMAPP_2-0.2.1/SNIIMAPP_2.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       14 2023-06-26 18:51:28.000000 SNIIMAPP_2-0.2.1/SNIIMAPP_2.egg-info/top_level.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1935 2023-06-26 18:35:45.000000 SNIIMAPP_2-0.2.1/precios_sniim.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      480 2023-06-26 18:49:33.000000 SNIIMAPP_2-0.2.1/pyproject.toml
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-06-26 18:51:28.904553 SNIIMAPP_2-0.2.1/setup.cfg
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-26 22:40:11.744668 SNIIMAPP_2-0.2.2/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1074 2023-06-26 19:27:35.000000 SNIIMAPP_2-0.2.2/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      959 2023-06-26 22:40:11.744668 SNIIMAPP_2-0.2.2/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      465 2023-06-26 22:13:05.000000 SNIIMAPP_2-0.2.2/README.md
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-26 22:40:11.744668 SNIIMAPP_2-0.2.2/SNIIMAPP_2.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      959 2023-06-26 22:40:11.000000 SNIIMAPP_2-0.2.2/SNIIMAPP_2.egg-info/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      185 2023-06-26 22:40:11.000000 SNIIMAPP_2-0.2.2/SNIIMAPP_2.egg-info/SOURCES.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-26 22:40:11.000000 SNIIMAPP_2-0.2.2/SNIIMAPP_2.egg-info/dependency_links.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       14 2023-06-26 22:40:11.000000 SNIIMAPP_2-0.2.2/SNIIMAPP_2.egg-info/top_level.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1178 2023-06-26 21:36:02.000000 SNIIMAPP_2-0.2.2/precios_sniim.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      480 2023-06-26 22:39:55.000000 SNIIMAPP_2-0.2.2/pyproject.toml
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-06-26 22:40:11.744668 SNIIMAPP_2-0.2.2/setup.cfg
```

### Comparing `SNIIMAPP_2-0.2.1/LICENSE` & `SNIIMAPP_2-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SNIIMAPP_2-0.2.1/PKG-INFO` & `SNIIMAPP_2-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: SNIIMAPP_2
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Autores:
 
+- MC. Rodolfo Lopez
 - Dr. Oscar de la Torre
 - Dr. Felipe Andoni
-- MC. Rodolfo Lopez
 
 ### Descripcion:
 
 - Extraccion de datos del SNIIM.
 
 ### Requerimientos:
 
+- pip install SNIIM_2
 - pip install mysql-connector-Python
-- git clone https://github.com/rodolfolopezfcca/sniimapp_1
 
 ### Uso:
 
-**usage:** precios_sniim.py [-h] {fyh,granos} start_date end_date 
-
-Libreria para consulta de precios de productos agriculas FCCA UMICH V.1.1 
+La clase devuelve un diccionario con los datos.
 
-**positional arguments:** \
-  **{fyh,granos}**  Producto [fyh: frutas y hortalizas, granos: granos] \
-  **start_date**    Fecha inicio [YYYY-mm-dd] \
-  **end_date**      Fecha fin [YYYY-mm-dd] 
+- from precios_sniim import SNIIM
+- sniim     = SNIIM('fyh', '2023-06-22', '2023-06-22')
+- resultado = sniim.get_data()
 
-**optional arguments:** \
-  -h, --help    show this help message and exit
+**Para formatear la fecha**
+- resultado[0]['fecha'].strftime("%Y-%m-%d")
```

