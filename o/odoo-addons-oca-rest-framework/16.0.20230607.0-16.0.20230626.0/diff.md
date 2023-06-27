# Comparing `tmp/odoo_addons_oca_rest_framework-16.0.20230607.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_rest_framework-16.0.20230626.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1468 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1050 b- defN 23-Jun-08 05:04 odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 05:04 odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-08 05:04 odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      429 b- defN 23-Jun-08 05:04 odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/RECORD
-4 files, 1572 bytes uncompressed, 622 bytes compressed:  60.4%
+Zip file size: 1479 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1183 b- defN 23-Jun-27 05:01 odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 05:01 odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-27 05:01 odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      429 b- defN 23-Jun-27 05:01 odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/RECORD
+4 files, 1705 bytes uncompressed, 633 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/METADATA
+Filename: odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/WHEEL
+Filename: odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/RECORD
+Filename: odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_rest_framework-16.0.20230607.0.dist-info/METADATA` & `odoo_addons_oca_rest_framework-16.0.20230626.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-rest-framework
-Version: 16.0.20230607.0
+Version: 16.0.20230626.0
 Summary: Meta package for oca-rest-framework Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -13,13 +13,15 @@
 Requires-Dist: odoo-addon-base-rest-datamodel (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-rest-demo (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-rest-pydantic (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-datamodel (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-extendable (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-extendable-fastapi (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-fastapi (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-fastapi-auth-jwt (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-fastapi-auth-jwt-demo (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-graphql-base (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-graphql-demo (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pydantic (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

