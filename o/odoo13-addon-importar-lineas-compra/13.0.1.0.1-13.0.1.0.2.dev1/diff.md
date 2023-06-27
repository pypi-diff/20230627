# Comparing `tmp/odoo13_addon_importar_lineas_compra-13.0.1.0.1-py3-none-any.whl.zip` & `tmp/odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,11 @@
-Zip file size: 1678 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1175 b- defN 23-May-22 16:47 odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 16:47 odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 16:47 odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      429 b- defN 23-May-22 16:47 odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/RECORD
-4 files, 1701 bytes uncompressed, 832 bytes compressed:  51.1%
+Zip file size: 6550 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-27 09:18 importar_lineas_compra/__init__.py
+-rw-r--r--  2.0 unx     1387 b- defN 23-Jun-27 09:18 importar_lineas_compra/__manifest__.py
+-rw-r--r--  2.0 unx    11273 b- defN 23-Jun-27 09:18 importar_lineas_compra/importar_lineas_compra.py
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-27 09:18 importar_lineas_compra/controllers/__init__.py
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jun-27 09:18 importar_lineas_compra/controllers/download_xls.py
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-27 09:27 odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 09:27 odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-27 09:27 odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      950 b- defN 23-Jun-27 09:27 odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/RECORD
+9 files, 16547 bytes uncompressed, 4852 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -1,13 +1,28 @@
-Filename: odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/METADATA
+Filename: importar_lineas_compra/__init__.py
 Comment: 
 
-Filename: odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/WHEEL
+Filename: importar_lineas_compra/__manifest__.py
 Comment: 
 
-Filename: odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/top_level.txt
+Filename: importar_lineas_compra/importar_lineas_compra.py
 Comment: 
 
-Filename: odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/RECORD
+Filename: importar_lineas_compra/controllers/__init__.py
+Comment: 
+
+Filename: importar_lineas_compra/controllers/download_xls.py
+Comment: 
+
+Filename: odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/METADATA
+Comment: 
+
+Filename: odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/WHEEL
+Comment: 
+
+Filename: odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/top_level.txt
+Comment: 
+
+Filename: odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addon_importar_lineas_compra-13.0.1.0.1.dist-info/METADATA` & `odoo13_addon_importar_lineas_compra-13.0.1.0.2.dev1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo13-addon-importar-lineas-compra
-Version: 13.0.1.0.1
+Version: 13.0.1.0.2.dev1
 Summary: Importar de varias maneras líneas de compra en un pedido.
 Home-page: https://framagit.org/devcontrol
 Author: Colectivo DEVCONTROL
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
```

