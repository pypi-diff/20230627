# Comparing `tmp/odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1-py3-none-any.whl.zip` & `tmp/odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,13 @@
-Zip file size: 1562 bytes, number of entries: 4
--rw-r--r--  2.0 unx      573 b- defN 23-Jun-26 09:02 odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 09:02 odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-26 09:02 odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      444 b- defN 23-Jun-26 09:02 odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/RECORD
-4 files, 1114 bytes uncompressed, 684 bytes compressed:  38.6%
+Zip file size: 9890 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      960 b- defN 23-Jun-27 09:18 exportar_deposito_xls/__init__.py
+-rw-r--r--  2.0 unx     1930 b- defN 23-Jun-27 09:18 exportar_deposito_xls/__manifest__.py
+-rw-r--r--  2.0 unx      931 b- defN 23-Jun-27 09:18 exportar_deposito_xls/controllers/__init__.py
+-rw-r--r--  2.0 unx     2411 b- defN 23-Jun-27 09:18 exportar_deposito_xls/controllers/main.py
+-rw-r--r--  2.0 unx      960 b- defN 23-Jun-27 09:18 exportar_deposito_xls/models/__init__.py
+-rw-r--r--  2.0 unx     1387 b- defN 23-Jun-27 09:18 exportar_deposito_xls/models/res_partner.py
+-rw-r--r--  2.0 unx    12253 b- defN 23-Jun-27 09:18 exportar_deposito_xls/models/wizard.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Jun-27 09:25 odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 09:25 odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 23-Jun-27 09:25 odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1119 b- defN 23-Jun-27 09:25 odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/RECORD
+11 files, 22643 bytes uncompressed, 7926 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,13 +1,34 @@
-Filename: odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/METADATA
+Filename: exportar_deposito_xls/__init__.py
 Comment: 
 
-Filename: odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/WHEEL
+Filename: exportar_deposito_xls/__manifest__.py
 Comment: 
 
-Filename: odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/top_level.txt
+Filename: exportar_deposito_xls/controllers/__init__.py
 Comment: 
 
-Filename: odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/RECORD
+Filename: exportar_deposito_xls/controllers/main.py
+Comment: 
+
+Filename: exportar_deposito_xls/models/__init__.py
+Comment: 
+
+Filename: exportar_deposito_xls/models/res_partner.py
+Comment: 
+
+Filename: exportar_deposito_xls/models/wizard.py
+Comment: 
+
+Filename: odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/METADATA
+Comment: 
+
+Filename: odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/WHEEL
+Comment: 
+
+Filename: odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/top_level.txt
+Comment: 
+
+Filename: odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev1.dist-info/METADATA` & `odoo13_addon_exportar_deposito_xls-13.0.1.0.4.dev2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo13-addon-exportar-deposito-xls
-Version: 13.0.1.0.4.dev1
+Version: 13.0.1.0.4.dev2
 Summary: Muestra el stock actual por deposito.
 Home-page: https://framagit.org/devcontrol
 Author: Colectivo DEVCONTROL
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
```

