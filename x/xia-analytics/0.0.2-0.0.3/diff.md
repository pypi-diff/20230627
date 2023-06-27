# Comparing `tmp/xia_analytics-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_analytics-0.0.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 101225 bytes, number of entries: 7
--rw-r--r--  2.0 unx       96 b- defN 23-Jun-26 18:35 xia_analytics/__init__.py
--rw-r--r--  2.0 unx   245760 b- defN 23-Jun-26 18:38 xia_analytics/analyzer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:38 xia_analytics-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      663 b- defN 23-Jun-26 18:38 xia_analytics-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:38 xia_analytics-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-26 18:38 xia_analytics-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      598 b- defN 23-Jun-26 18:38 xia_analytics-0.0.2.dist-info/RECORD
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-27 19:35 xia_analytics/__init__.py
+-rw-r--r--  2.0 unx   245760 b- defN 23-Jun-27 19:38 xia_analytics/analyzer.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      663 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      598 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/RECORD
 7 files, 247381 bytes uncompressed, 100153 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_analytics/__init__.py
 Comment: 
 
 Filename: xia_analytics/analyzer.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_analytics-0.0.2.dist-info/LICENSE.txt
+Filename: xia_analytics-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_analytics-0.0.2.dist-info/METADATA
+Filename: xia_analytics-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_analytics-0.0.2.dist-info/WHEEL
+Filename: xia_analytics-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_analytics-0.0.2.dist-info/top_level.txt
+Filename: xia_analytics-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_analytics-0.0.2.dist-info/RECORD
+Filename: xia_analytics-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_analytics/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_analytics.analyzer import Analyzer
 
 __all__ = [
    "Analyzer"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## Comparing `xia_analytics-0.0.2.dist-info/METADATA` & `xia_analytics-0.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-analytics
-Version: 0.0.2
+Version: 0.0.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-analytics/0.0.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-analytics/0.0.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

