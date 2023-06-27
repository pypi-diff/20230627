# Comparing `tmp/pits-0.1.0-py3-none-any.whl.zip` & `tmp/pits-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 2486 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-27 05:53 pits-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1801 b- defN 23-Jun-27 05:53 pits-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 05:53 pits-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-27 05:53 pits-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      370 b- defN 23-Jun-27 05:53 pits-0.1.0.dist-info/RECORD
-5 files, 3336 bytes uncompressed, 1796 bytes compressed:  46.2%
+Zip file size: 3775 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     3245 b- defN 23-Jun-27 05:49 pits/__init__.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1801 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      443 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/RECORD
+6 files, 6654 bytes uncompressed, 2977 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
-Filename: pits-0.1.0.dist-info/LICENSE
+Filename: pits/__init__.py
 Comment: 
 
-Filename: pits-0.1.0.dist-info/METADATA
+Filename: pits-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pits-0.1.0.dist-info/WHEEL
+Filename: pits-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pits-0.1.0.dist-info/top_level.txt
+Filename: pits-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pits-0.1.0.dist-info/RECORD
+Filename: pits-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: pits-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pits-0.1.0.dist-info/LICENSE` & `pits-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pits-0.1.0.dist-info/METADATA` & `pits-0.1.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pits
-Version: 0.1.0
+Version: 0.1.1
 Summary: Point-in-time Storage.
 Author-email: Sun Yijiang <sunyijiang@gmail.com>
 Project-URL: Homepage, https://github.com/sunyj/pits
 Project-URL: Bug Tracker, https://github.com/sunyj/pits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

