# Comparing `tmp/bettersleepy-0.1.2-py3.11.egg` & `tmp/BetterSleePy-0.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,7 @@
-Zip file size: 1821 bytes, number of entries: 7
--rw-r--r--  2.0 unx      697 b- defN 23-May-13 08:05 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      198 b- defN 23-May-13 08:05 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-13 08:05 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       13 b- defN 23-May-13 08:05 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-13 08:05 EGG-INFO/zip-safe
--rw-r--r--  2.0 unx      132 b- defN 23-May-12 22:03 bettersleepy/__init__.py
--rw-r--r--  2.0 unx      751 b- defN 23-May-13 08:05 bettersleepy/__pycache__/__init__.cpython-311.pyc
-7 files, 1793 bytes uncompressed, 911 bytes compressed:  49.2%
+Zip file size: 1506 bytes, number of entries: 5
+-rwxrwxrwx  2.0 unx      132 b- defN 23-May-29 06:56 bettersleepy/__init__.py
+-rwxrwxrwx  2.0 unx      697 b- defN 23-Jun-27 08:56 BetterSleePy-0.1.3.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      110 b- defN 23-Jun-27 08:56 BetterSleePy-0.1.3.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       13 b- defN 23-Jun-27 08:56 BetterSleePy-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      398 b- defN 23-Jun-27 08:56 BetterSleePy-0.1.3.dist-info/RECORD
+5 files, 1350 bytes uncompressed, 760 bytes compressed:  43.7%
```

## zipnote «TEMP»/diffoscope_qp6d544l_/tmpbz2x72jx_.zip

```diff
@@ -1,22 +1,16 @@
-Filename: EGG-INFO/PKG-INFO
-Comment: 
-
-Filename: EGG-INFO/SOURCES.txt
-Comment: 
-
-Filename: EGG-INFO/dependency_links.txt
+Filename: bettersleepy/__init__.py
 Comment: 
 
-Filename: EGG-INFO/top_level.txt
+Filename: BetterSleePy-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: EGG-INFO/zip-safe
+Filename: BetterSleePy-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: bettersleepy/__init__.py
+Filename: BetterSleePy-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bettersleepy/__pycache__/__init__.cpython-311.pyc
+Filename: BetterSleePy-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `EGG-INFO/PKG-INFO` & `BetterSleePy-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bettersleepy
-Version: 0.1.2
+Name: BetterSleePy
+Version: 0.1.3
 Summary: Makes the Python sleep module easier a bit.
 Home-page: https://github.com/octopus1348/bettersleepy
 Author: Czira Zsombor
 Author-email: czirazsombor313@icloud.com
 
 BetterSleePy
 ============
```

