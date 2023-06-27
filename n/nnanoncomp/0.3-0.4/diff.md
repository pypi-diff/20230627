# Comparing `tmp/nnanoncomp-0.3-py3-none-any.whl.zip` & `tmp/nnanoncomp-0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2724 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 14:52 anon_comp_core/__init__.py
--rw-r--r--  2.0 unx     1812 b- defN 23-Jun-27 14:52 anon_comp_core/anonymization.py
--rw-r--r--  2.0 unx     1271 b- defN 23-Jun-27 14:52 anon_comp_core/anonymization_transformations.py
--rw-r--r--  2.0 unx      168 b- defN 23-Jun-27 14:52 nnanoncomp-0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 14:52 nnanoncomp-0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-27 14:52 nnanoncomp-0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      573 b- defN 23-Jun-27 14:52 nnanoncomp-0.3.dist-info/RECORD
-7 files, 3931 bytes uncompressed, 1698 bytes compressed:  56.8%
+Zip file size: 2742 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 16:48 anon_comp_core/__init__.py
+-rw-r--r--  2.0 unx     1812 b- defN 23-Jun-27 16:48 anon_comp_core/anonymization.py
+-rw-r--r--  2.0 unx     1325 b- defN 23-Jun-27 16:48 anon_comp_core/anonymization_transformations.py
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-27 16:48 nnanoncomp-0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 16:48 nnanoncomp-0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-27 16:48 nnanoncomp-0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      573 b- defN 23-Jun-27 16:48 nnanoncomp-0.4.dist-info/RECORD
+7 files, 3985 bytes uncompressed, 1716 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: anon_comp_core/anonymization.py
 Comment: 
 
 Filename: anon_comp_core/anonymization_transformations.py
 Comment: 
 
-Filename: nnanoncomp-0.3.dist-info/METADATA
+Filename: nnanoncomp-0.4.dist-info/METADATA
 Comment: 
 
-Filename: nnanoncomp-0.3.dist-info/WHEEL
+Filename: nnanoncomp-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: nnanoncomp-0.3.dist-info/top_level.txt
+Filename: nnanoncomp-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: nnanoncomp-0.3.dist-info/RECORD
+Filename: nnanoncomp-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anon_comp_core/anonymization_transformations.py

```diff
@@ -1,8 +1,10 @@
 from pyspark.sql.functions import sha2, col, current_timestamp, lit, year, DataFrame
+from pyspark.sql.types import StructType, StringType
+
 
 
 class Transformations():
     @staticmethod
     def _salted_sha2(c: col, salt: str = "asd") -> str:
         return sha2(f"{salt}{c.cast(StringType())}", 256)
```

## Comparing `nnanoncomp-0.3.dist-info/RECORD` & `nnanoncomp-0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 anon_comp_core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 anon_comp_core/anonymization.py,sha256=PfafB17JhMDasA8S44WjwcOJtx9_3gbyrTiOUkejUR4,1812
-anon_comp_core/anonymization_transformations.py,sha256=qlTO0xF9Bt1VlyPNoOfK21fOGX4vaSzWT04ev99BQBw,1271
-nnanoncomp-0.3.dist-info/METADATA,sha256=SAp8gnw1cAOJsKoaEW3MJSXzwei_kdkStzWZKKgdkic,168
-nnanoncomp-0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nnanoncomp-0.3.dist-info/top_level.txt,sha256=iz4micZjzu0AcFM-B4W1_B89SeC4CmXEGlwAVMllto8,15
-nnanoncomp-0.3.dist-info/RECORD,,
+anon_comp_core/anonymization_transformations.py,sha256=SlaTg14ZdAIuvmdJ0F3GuVsCyDzhWY6oZmdIHyUKk-Q,1325
+nnanoncomp-0.4.dist-info/METADATA,sha256=5qm3zha-egVEUst9qBFh1l8pNRPVF7TbrYxFS472ntA,168
+nnanoncomp-0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+nnanoncomp-0.4.dist-info/top_level.txt,sha256=iz4micZjzu0AcFM-B4W1_B89SeC4CmXEGlwAVMllto8,15
+nnanoncomp-0.4.dist-info/RECORD,,
```

