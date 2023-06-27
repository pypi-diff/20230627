# Comparing `tmp/dopplrSDK-2.4.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-2.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 4898 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat    10779 b- defN 23-Jun-26 12:17 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      621 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 23-Jun-26 12:33 dopplrSDK-2.4.0.dist-info/RECORD
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-27 07:50 dopplrSDK-2.5.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      621 b- defN 23-Jun-27 07:50 dopplrSDK-2.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-27 07:50 dopplrSDK-2.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-27 07:50 dopplrSDK-2.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 23-Jun-27 07:50 dopplrSDK-2.5.0.dist-info/RECORD
 6 files, 13057 bytes uncompressed, 4032 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-2.4.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-2.5.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-2.4.0.dist-info/METADATA
+Filename: dopplrSDK-2.5.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-2.4.0.dist-info/WHEEL
+Filename: dopplrSDK-2.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-2.4.0.dist-info/top_level.txt
+Filename: dopplrSDK-2.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-2.4.0.dist-info/RECORD
+Filename: dopplrSDK-2.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dopplrSDK-2.4.0.dist-info/LICENSE.txt` & `dopplrSDK-2.5.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-2.4.0.dist-info/METADATA` & `dopplrSDK-2.5.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 2.4.0
+Version: 2.5.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: psycopg2-binary (==2.9.6)
 Requires-Dist: pandas (==2.0.2)
 Requires-Dist: boto3 (==1.26.153)
 Requires-Dist: pycryptodome (==3.18.0)
-Requires-Dist: cryptography (==41.0.6)
+Requires-Dist: cryptography (==41.0.1)
 Requires-Dist: azure-storage-blob (==12.15.0)
 Requires-Dist: botocore (==1.29.79)
 
 UNKNOWN
```

