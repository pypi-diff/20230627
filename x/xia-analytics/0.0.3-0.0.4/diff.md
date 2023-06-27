# Comparing `tmp/xia_analytics-0.0.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_analytics-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 101225 bytes, number of entries: 7
--rw-r--r--  2.0 unx       96 b- defN 23-Jun-27 19:35 xia_analytics/__init__.py
--rw-r--r--  2.0 unx   245760 b- defN 23-Jun-27 19:38 xia_analytics/analyzer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      663 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      598 b- defN 23-Jun-27 19:38 xia_analytics-0.0.3.dist-info/RECORD
-7 files, 247381 bytes uncompressed, 100153 bytes compressed:  59.5%
+Zip file size: 101226 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-27 19:40 xia_analytics/__init__.py
+-rw-r--r--  2.0 unx   245760 b- defN 23-Jun-27 19:42 xia_analytics/analyzer.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      663 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      598 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/RECORD
+7 files, 247381 bytes uncompressed, 100154 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_analytics/__init__.py
 Comment: 
 
 Filename: xia_analytics/analyzer.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_analytics-0.0.3.dist-info/LICENSE.txt
+Filename: xia_analytics-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_analytics-0.0.3.dist-info/METADATA
+Filename: xia_analytics-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_analytics-0.0.3.dist-info/WHEEL
+Filename: xia_analytics-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_analytics-0.0.3.dist-info/top_level.txt
+Filename: xia_analytics-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_analytics-0.0.3.dist-info/RECORD
+Filename: xia_analytics-0.0.4.dist-info/RECORD
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
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `xia_analytics-0.0.3.dist-info/METADATA` & `xia_analytics-0.0.4.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-analytics
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-analytics/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-analytics/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_analytics-0.0.3.dist-info/RECORD` & `xia_analytics-0.0.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_analytics/__init__.py,sha256=di6DCYNa7hFB5MNKwTZSef-WFCDfHV7yAn1zcOTCOYI,96
-xia_analytics/analyzer.cp39-win_amd64.pyd,sha256=kNYrAhFnLzVk57UB00sQSe_SrEH8zfQ7L52Qs5lY-Ko,245760
-xia_analytics-0.0.3.dist-info/LICENSE.txt,sha256=f8ikpEGaPKtKuwQX2o_OTwnZkwjdWOOTdtZ8VFx-4vM,151
-xia_analytics-0.0.3.dist-info/METADATA,sha256=zbAUgTwayEWJPM9jqm5fd_3_ukndr0xFgrY_Lf2F820,663
-xia_analytics-0.0.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_analytics-0.0.3.dist-info/top_level.txt,sha256=kr8j9N82NjYdNE_q3fPy-jKGYWo0TV2VxqlEfITztMs,14
-xia_analytics-0.0.3.dist-info/RECORD,,
+xia_analytics/__init__.py,sha256=kRUlLg8wiCuIG04jh6dbhLRqKRikTWL5nrhXk-g-wUk,96
+xia_analytics/analyzer.cp39-win_amd64.pyd,sha256=Xm2cV-ARn_WgOfgCMk-ueXEzdo_fjihN1fdJgL1m8TU,245760
+xia_analytics-0.0.4.dist-info/LICENSE.txt,sha256=f8ikpEGaPKtKuwQX2o_OTwnZkwjdWOOTdtZ8VFx-4vM,151
+xia_analytics-0.0.4.dist-info/METADATA,sha256=5qwCqyjX8palMLpu8-CNLH0Qn-OfQEBR1WgISEOlj5I,663
+xia_analytics-0.0.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_analytics-0.0.4.dist-info/top_level.txt,sha256=kr8j9N82NjYdNE_q3fPy-jKGYWo0TV2VxqlEfITztMs,14
+xia_analytics-0.0.4.dist-info/RECORD,,
```

