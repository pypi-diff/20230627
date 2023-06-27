# Comparing `tmp/web_list_info_spider-0.6-py3-none-any.whl.zip` & `tmp/web_list_info_spider-0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5078 bytes, number of entries: 8
+Zip file size: 5069 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 09:05 web_list_info_spider/__init__.py
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-27 09:05 web_list_info_spider/__main__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-27 09:08 web_list_info_spider/__main__.py
 -rw-r--r--  2.0 unx    11569 b- defN 23-Jun-27 08:52 web_list_info_spider/main.py
--rw-r--r--  2.0 unx      212 b- defN 23-Jun-27 09:06 web_list_info_spider-0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 09:06 web_list_info_spider-0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 23-Jun-27 09:06 web_list_info_spider-0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-27 09:06 web_list_info_spider-0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      706 b- defN 23-Jun-27 09:06 web_list_info_spider-0.6.dist-info/RECORD
-8 files, 12706 bytes uncompressed, 3818 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx      212 b- defN 23-Jun-27 09:08 web_list_info_spider-0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 09:08 web_list_info_spider-0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-27 09:08 web_list_info_spider-0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-27 09:08 web_list_info_spider-0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      706 b- defN 23-Jun-27 09:08 web_list_info_spider-0.8.dist-info/RECORD
+8 files, 12685 bytes uncompressed, 3809 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: web_list_info_spider/__main__.py
 Comment: 
 
 Filename: web_list_info_spider/main.py
 Comment: 
 
-Filename: web_list_info_spider-0.6.dist-info/METADATA
+Filename: web_list_info_spider-0.8.dist-info/METADATA
 Comment: 
 
-Filename: web_list_info_spider-0.6.dist-info/WHEEL
+Filename: web_list_info_spider-0.8.dist-info/WHEEL
 Comment: 
 
-Filename: web_list_info_spider-0.6.dist-info/entry_points.txt
+Filename: web_list_info_spider-0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: web_list_info_spider-0.6.dist-info/top_level.txt
+Filename: web_list_info_spider-0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: web_list_info_spider-0.6.dist-info/RECORD
+Filename: web_list_info_spider-0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## web_list_info_spider/__main__.py

```diff
@@ -1,3 +1,3 @@
-from web_list_data_spider.web_list_info_spider.main import cli
+from web_list_info_spider.main import cli
 
 cli()
```

