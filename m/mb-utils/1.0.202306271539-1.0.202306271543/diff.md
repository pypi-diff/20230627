# Comparing `tmp/mb_utils-1.0.202306271539-py3-none-any.whl.zip` & `tmp/mb_utils-1.0.202306271543-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 7935 bytes, number of entries: 14
+Zip file size: 7948 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx      311 b- defN 23-Jun-06 15:13 mb_utils/src/__init__.py
 -rw-rw-r--  2.0 unx     3330 b- defN 23-May-30 16:38 mb_utils/src/deprecated.py
 -rw-rw-r--  2.0 unx     1318 b- defN 23-May-30 16:38 mb_utils/src/extra.py
 -rw-rw-r--  2.0 unx     1813 b- defN 23-May-30 16:38 mb_utils/src/logging.py
 -rw-rw-r--  2.0 unx      664 b- defN 23-May-30 16:38 mb_utils/src/path_checker.py
 -rw-rw-r--  2.0 unx     1306 b- defN 23-May-30 16:38 mb_utils/src/retry_decorator.py
--rw-rw-r--  2.0 unx     3764 b- defN 23-Jun-27 15:39 mb_utils/src/s3.py
+-rw-rw-r--  2.0 unx     3819 b- defN 23-Jun-27 15:43 mb_utils/src/s3.py
 -rw-rw-r--  2.0 unx      777 b- defN 23-May-30 16:38 mb_utils/src/terminal.py
 -rw-rw-r--  2.0 unx     1821 b- defN 23-May-30 16:38 mb_utils/src/verify_image.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 15:39 mb_utils/src/version.py
--rw-rw-r--  2.0 unx      251 b- defN 23-Jun-27 15:39 mb_utils-1.0.202306271539.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 15:39 mb_utils-1.0.202306271539.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-27 15:39 mb_utils-1.0.202306271539.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1156 b- defN 23-Jun-27 15:39 mb_utils-1.0.202306271539.dist-info/RECORD
-14 files, 17008 bytes uncompressed, 6005 bytes compressed:  64.7%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-27 15:43 mb_utils/src/version.py
+-rw-rw-r--  2.0 unx      251 b- defN 23-Jun-27 15:43 mb_utils-1.0.202306271543.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 15:43 mb_utils-1.0.202306271543.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-27 15:43 mb_utils-1.0.202306271543.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1156 b- defN 23-Jun-27 15:43 mb_utils-1.0.202306271543.dist-info/RECORD
+14 files, 17063 bytes uncompressed, 6018 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: mb_utils/src/verify_image.py
 Comment: 
 
 Filename: mb_utils/src/version.py
 Comment: 
 
-Filename: mb_utils-1.0.202306271539.dist-info/METADATA
+Filename: mb_utils-1.0.202306271543.dist-info/METADATA
 Comment: 
 
-Filename: mb_utils-1.0.202306271539.dist-info/WHEEL
+Filename: mb_utils-1.0.202306271543.dist-info/WHEEL
 Comment: 
 
-Filename: mb_utils-1.0.202306271539.dist-info/top_level.txt
+Filename: mb_utils-1.0.202306271543.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_utils-1.0.202306271539.dist-info/RECORD
+Filename: mb_utils-1.0.202306271543.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_utils/src/s3.py

```diff
@@ -113,12 +113,14 @@
 
     if 'Contents' in objects:
         for obj in objects['Contents']:
             if logger:
                 logger.info(obj['Key'])
             else:
                 print(obj['Key'])
+        return objects['Contents']
     else:
         if logger:
             logger.info(f"No objects found in {bucket_name}")
         else:
-            print(f"No objects found in {bucket_name}")
+            print(f"No objects found in {bucket_name}")
+        return None
```

## mb_utils/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('27')
 VERSION_HOUR = int('15')
-VERSION_MINUTE = int('39')
+VERSION_MINUTE = int('43')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306271539
-version_date = '2023/06/27 15:39'
+PATCH_VERSION = 202306271543
+version_date = '2023/06/27 15:43'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_utils-1.0.202306271539.dist-info/RECORD` & `mb_utils-1.0.202306271543.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 mb_utils/src/__init__.py,sha256=DkLZ1-4phWsDQ8DArT12K-4JIuXT2AogzJ5p9xVcLbw,311
 mb_utils/src/deprecated.py,sha256=yHz0JrDjGJDVT71gILr2JIYu6x1wWyENcUf4-lkuv10,3330
 mb_utils/src/extra.py,sha256=NP5JlU0oktw7j2cn_-W3rAMzjMYDKwzBeiSjpg-Evh4,1318
 mb_utils/src/logging.py,sha256=bwkKDej4pI1WzNKrQs9rTRx73z-EyZkB7UCPsYHnbs0,1813
 mb_utils/src/path_checker.py,sha256=MrE3P2hkDjOIWyZJ-Lh1X3wODKRnJk_nfVgKW0nQEMU,664
 mb_utils/src/retry_decorator.py,sha256=1lotNMXwALWFgb0ikrK9B-flOOMj9tTlOQgYCb-ejwY,1306
-mb_utils/src/s3.py,sha256=j36X8eNtETiYKGQoeUbV9v0XiOVhWL-Dkh8KH6Fpt9s,3764
+mb_utils/src/s3.py,sha256=xiN5COFi8ryvFEwHeTjYwc-FMtrK5HPdRdfkbJiYSFY,3819
 mb_utils/src/terminal.py,sha256=_1l8K9CwAFYx4UgfkwOWfgeZ2bZu4s-71gnyxWJc2xA,777
 mb_utils/src/verify_image.py,sha256=L_XAlYBsdAhTkMSVcMpgwS0Ea8I9r-ZjoChjL0GHT38,1821
-mb_utils/src/version.py,sha256=6Md1Yd5YQ-5TNhAUvqbmeO2uAfNA81rDOOb3ZLxpam0,396
-mb_utils-1.0.202306271539.dist-info/METADATA,sha256=vUWA3kWb7fLchqeXlyKnZHUkwKngtiJY7I4XbumlJdA,251
-mb_utils-1.0.202306271539.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mb_utils-1.0.202306271539.dist-info/top_level.txt,sha256=xeK1qEZ7uoXfZyNlYlurb_F_T8trKUaTU_Fm_UpKhyg,9
-mb_utils-1.0.202306271539.dist-info/RECORD,,
+mb_utils/src/version.py,sha256=K2PTVPJK56pdp51cqiQ7XAsWommS1CQZdMsbHArotQc,396
+mb_utils-1.0.202306271543.dist-info/METADATA,sha256=omve6ViLwG9magA5ck5qIYCaNA4SXsBEitkVYGQld8U,251
+mb_utils-1.0.202306271543.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mb_utils-1.0.202306271543.dist-info/top_level.txt,sha256=xeK1qEZ7uoXfZyNlYlurb_F_T8trKUaTU_Fm_UpKhyg,9
+mb_utils-1.0.202306271543.dist-info/RECORD,,
```

