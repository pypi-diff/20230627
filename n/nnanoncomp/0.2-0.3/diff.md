# Comparing `tmp/nnanoncomp-0.2-py3-none-any.whl.zip` & `tmp/nnanoncomp-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,9 @@
-Zip file size: 1016 bytes, number of entries: 4
--rw-r--r--  2.0 unx      168 b- defN 23-Jun-27 14:43 nnanoncomp-0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 14:43 nnanoncomp-0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-27 14:43 nnanoncomp-0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      300 b- defN 23-Jun-27 14:43 nnanoncomp-0.2.dist-info/RECORD
-4 files, 561 bytes uncompressed, 426 bytes compressed:  24.1%
+Zip file size: 2724 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 14:52 anon_comp_core/__init__.py
+-rw-r--r--  2.0 unx     1812 b- defN 23-Jun-27 14:52 anon_comp_core/anonymization.py
+-rw-r--r--  2.0 unx     1271 b- defN 23-Jun-27 14:52 anon_comp_core/anonymization_transformations.py
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-27 14:52 nnanoncomp-0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 14:52 nnanoncomp-0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-27 14:52 nnanoncomp-0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      573 b- defN 23-Jun-27 14:52 nnanoncomp-0.3.dist-info/RECORD
+7 files, 3931 bytes uncompressed, 1698 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -1,13 +1,22 @@
-Filename: nnanoncomp-0.2.dist-info/METADATA
+Filename: anon_comp_core/__init__.py
 Comment: 
 
-Filename: nnanoncomp-0.2.dist-info/WHEEL
+Filename: anon_comp_core/anonymization.py
 Comment: 
 
-Filename: nnanoncomp-0.2.dist-info/top_level.txt
+Filename: anon_comp_core/anonymization_transformations.py
 Comment: 
 
-Filename: nnanoncomp-0.2.dist-info/RECORD
+Filename: nnanoncomp-0.3.dist-info/METADATA
+Comment: 
+
+Filename: nnanoncomp-0.3.dist-info/WHEEL
+Comment: 
+
+Filename: nnanoncomp-0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: nnanoncomp-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

