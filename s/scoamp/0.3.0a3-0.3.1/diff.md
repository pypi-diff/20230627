# Comparing `tmp/scoamp-0.3.0a3-py3-none-any.whl.zip` & `tmp/scoamp-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 23630 bytes, number of entries: 20
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-19 04:00 scoamp/__init__.py
--rw-r--r--  2.0 unx     6668 b- defN 23-Jun-19 04:00 scoamp/api.py
--rw-r--r--  2.0 unx     9566 b- defN 23-Jun-19 04:00 scoamp/toolkit.py
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-19 04:00 scoamp/commands/__init__.py
--rw-r--r--  2.0 unx     4668 b- defN 23-Jun-19 04:00 scoamp/commands/api.py
--rw-r--r--  2.0 unx     7581 b- defN 23-Jun-19 04:00 scoamp/commands/lfs.py
--rw-rw-rw-  2.0 unx     2135 b- defN 23-Jun-19 04:00 scoamp/schema/public-model-meta.json
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-19 04:00 scoamp/utils/__init__.py
--rw-r--r--  2.0 unx     5080 b- defN 23-Jun-19 04:00 scoamp/utils/api_utils.py
--rw-r--r--  2.0 unx     1692 b- defN 23-Jun-19 04:00 scoamp/utils/error.py
--rw-r--r--  2.0 unx     5150 b- defN 23-Jun-19 04:00 scoamp/utils/helper.py
--rw-r--r--  2.0 unx      405 b- defN 23-Jun-19 04:00 scoamp/utils/logger.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-19 04:00 tests/__init__.py
--rw-r--r--  2.0 unx     9110 b- defN 23-Jun-19 04:00 tests/test_utils_helper.py
--rw-rw-rw-  2.0 unx    11334 b- defN 23-Jun-19 04:00 scoamp-0.3.0a3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1236 b- defN 23-Jun-19 04:00 scoamp-0.3.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 04:00 scoamp-0.3.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jun-19 04:00 scoamp-0.3.0a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-19 04:00 scoamp-0.3.0a3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1588 b- defN 23-Jun-19 04:00 scoamp-0.3.0a3.dist-info/RECORD
-20 files, 66875 bytes uncompressed, 21054 bytes compressed:  68.5%
+Zip file size: 23599 bytes, number of entries: 20
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-27 05:28 scoamp/__init__.py
+-rw-r--r--  2.0 unx     6668 b- defN 23-Jun-27 05:28 scoamp/api.py
+-rw-r--r--  2.0 unx     9566 b- defN 23-Jun-27 05:28 scoamp/toolkit.py
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-27 05:28 scoamp/commands/__init__.py
+-rw-r--r--  2.0 unx     4668 b- defN 23-Jun-27 05:28 scoamp/commands/api.py
+-rw-r--r--  2.0 unx     7581 b- defN 23-Jun-27 05:28 scoamp/commands/lfs.py
+-rw-rw-rw-  2.0 unx     2135 b- defN 23-Jun-27 05:28 scoamp/schema/public-model-meta.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 05:28 scoamp/utils/__init__.py
+-rw-r--r--  2.0 unx     5080 b- defN 23-Jun-27 05:28 scoamp/utils/api_utils.py
+-rw-r--r--  2.0 unx     1692 b- defN 23-Jun-27 05:28 scoamp/utils/error.py
+-rw-r--r--  2.0 unx     5150 b- defN 23-Jun-27 05:28 scoamp/utils/helper.py
+-rw-r--r--  2.0 unx      405 b- defN 23-Jun-27 05:28 scoamp/utils/logger.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 05:28 tests/__init__.py
+-rw-r--r--  2.0 unx     9110 b- defN 23-Jun-27 05:28 tests/test_utils_helper.py
+-rw-rw-rw-  2.0 unx    11334 b- defN 23-Jun-27 05:28 scoamp-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1234 b- defN 23-Jun-27 05:28 scoamp-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 05:28 scoamp-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-27 05:28 scoamp-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-27 05:28 scoamp-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1576 b- defN 23-Jun-27 05:28 scoamp-0.3.1.dist-info/RECORD
+20 files, 66860 bytes uncompressed, 21047 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_utils_helper.py
 Comment: 
 
-Filename: scoamp-0.3.0a3.dist-info/LICENSE
+Filename: scoamp-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: scoamp-0.3.0a3.dist-info/METADATA
+Filename: scoamp-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: scoamp-0.3.0a3.dist-info/WHEEL
+Filename: scoamp-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: scoamp-0.3.0a3.dist-info/entry_points.txt
+Filename: scoamp-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: scoamp-0.3.0a3.dist-info/top_level.txt
+Filename: scoamp-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: scoamp-0.3.0a3.dist-info/RECORD
+Filename: scoamp-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scoamp/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.3.0a3'
+__version__ = '0.3.1'
```

## Comparing `scoamp-0.3.0a3.dist-info/LICENSE` & `scoamp-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scoamp-0.3.0a3.dist-info/METADATA` & `scoamp-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoamp
-Version: 0.3.0a3
+Version: 0.3.1
 Summary: SenseCore AI Model Platform Command Line Tool
 Home-page: UNKNOWN
 Author: SenseTime, Inc.
 Author-email: hpan@sensetime.com
 License: Apache 2.0
 Keywords: machine-learning deep-learning models
 Platform: UNKNOWN
```

## Comparing `scoamp-0.3.0a3.dist-info/RECORD` & `scoamp-0.3.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-scoamp/__init__.py,sha256=UhltNHjvoNzusF_7ZZozBRB4tHF_v12MTvCGwpoR99I,23
+scoamp/__init__.py,sha256=TZkGuMIRSRmUY3XCIs5owt2o60vXyqYMHWIkhx65uYE,22
 scoamp/api.py,sha256=RmmZNMrVXJ7W3XFZBcfyBVyWJ1VjiyN2u_KyMTD4BEc,6668
 scoamp/toolkit.py,sha256=76ptHxR3yh2kQxjzP0Ei4ajXUZslD2eMkPLD1N3Qgdo,9566
 scoamp/commands/__init__.py,sha256=y1F-rP1F_zPOEYhMd_wRmC9a6ZZyr9QcE4GWkIbT0og,486
 scoamp/commands/api.py,sha256=o8sDH5ZczxnqeqH0AlUgC1IDkyeQomyz0VoU5i8DJ5k,4668
 scoamp/commands/lfs.py,sha256=YA4Zj7W7lzoYQF-ulcG1bRgnJ0TXyi_D0JE4aLNNJzU,7581
 scoamp/schema/public-model-meta.json,sha256=EIQMSVftVNCt6GS6-x9XbKirK-SS75mJRKMsFQWCsEg,2135
 scoamp/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scoamp/utils/api_utils.py,sha256=P9JHJl2KHOqspJrHMOsLvJl-FY3CpjBWDjglNncGQHU,5080
 scoamp/utils/error.py,sha256=g9LWBJd89hSzq2adqHfhBq0TIUz-K2pv-XyU8wg_zoM,1692
 scoamp/utils/helper.py,sha256=KLH089HaSyENxYb0c0o9b1aUJgvnGWL6GYInAfEdEF0,5150
 scoamp/utils/logger.py,sha256=PQcpywlU1IHbv1dvdKOI2s3hNqR3KlRIRurqFKfeDag,405
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_utils_helper.py,sha256=gFx9h7jjiCao2hbZoT_ES08xtrFRizfPLIvp17uronQ,9110
-scoamp-0.3.0a3.dist-info/LICENSE,sha256=R-z_qud7owqMORJyRv9VAVEhRkcRWJOyCJnyCG4Ds5E,11334
-scoamp-0.3.0a3.dist-info/METADATA,sha256=f4wPsdc5yYsRwacr8mq3eHQfAx5Zjgg54JeH5OGYUJY,1236
-scoamp-0.3.0a3.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-scoamp-0.3.0a3.dist-info/entry_points.txt,sha256=oXMR4tQerRPB0zht7ok37JQCiiq-XL0B1hFDgAkI90M,48
-scoamp-0.3.0a3.dist-info/top_level.txt,sha256=R-1KO00uSz-w1PWLRS6mRHjNP5yFJIKSrafHwVzvYBU,13
-scoamp-0.3.0a3.dist-info/RECORD,,
+scoamp-0.3.1.dist-info/LICENSE,sha256=R-z_qud7owqMORJyRv9VAVEhRkcRWJOyCJnyCG4Ds5E,11334
+scoamp-0.3.1.dist-info/METADATA,sha256=P6SqEt61hUSASyV3shhcaDHuzaYLuMA-oTygQqBCgRo,1234
+scoamp-0.3.1.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+scoamp-0.3.1.dist-info/entry_points.txt,sha256=oXMR4tQerRPB0zht7ok37JQCiiq-XL0B1hFDgAkI90M,48
+scoamp-0.3.1.dist-info/top_level.txt,sha256=R-1KO00uSz-w1PWLRS6mRHjNP5yFJIKSrafHwVzvYBU,13
+scoamp-0.3.1.dist-info/RECORD,,
```

