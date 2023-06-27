# Comparing `tmp/stactools-amazonia-1-0.1.1.tar.gz` & `tmp/stactools-amazonia-1-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-amazonia-1-0.1.1.tar", last modified: Fri Jun 23 20:51:01 2023, max compression
+gzip compressed data, was "stactools-amazonia-1-0.1.2.tar", last modified: Tue Jun 27 18:18:46 2023, max compression
```

## Comparing `stactools-amazonia-1-0.1.1.tar` & `stactools-amazonia-1-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.697386 stactools-amazonia-1-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.697386 stactools-amazonia-1-0.1.1/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/tests/test_stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:18:46.756258 stactools-amazonia-1-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-27 18:18:46.756258 stactools-amazonia-1-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-27 18:18:46.756258 stactools-amazonia-1-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:18:46.752258 stactools-amazonia-1-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:18:46.752258 stactools-amazonia-1-0.1.2/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:18:46.752258 stactools-amazonia-1-0.1.2/src/stactools/amazonia_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/src/stactools/amazonia_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/src/stactools/amazonia_1/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/src/stactools/amazonia_1/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19007 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/src/stactools/amazonia_1/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:18:46.756258 stactools-amazonia-1-0.1.2/src/stactools_amazonia_1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-27 18:18:46.000000 stactools-amazonia-1-0.1.2/src/stactools_amazonia_1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 18:18:46.000000 stactools-amazonia-1-0.1.2/src/stactools_amazonia_1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:18:46.000000 stactools-amazonia-1-0.1.2/src/stactools_amazonia_1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 18:18:46.000000 stactools-amazonia-1-0.1.2/src/stactools_amazonia_1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 18:18:46.000000 stactools-amazonia-1-0.1.2/src/stactools_amazonia_1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:18:46.756258 stactools-amazonia-1-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-27 18:18:30.000000 stactools-amazonia-1-0.1.2/tests/test_stac.py
```

### Comparing `stactools-amazonia-1-0.1.1/LICENSE` & `stactools-amazonia-1-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.1/PKG-INFO` & `stactools-amazonia-1-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-amazonia-1
-Version: 0.1.1
+Version: 0.1.2
 Summary: Amazonia-1 on AWS stactools package
 Home-page: https://github.com/stactools-packages/amazonia-1
 Author: Frederico Liporace
 Author-email: liporace@amskepler.com
 Project-URL: Issues, https://github.com/stactools-packages/amazonia-1/issues
 Keywords: stactools,pystac,catalog,STAC,Amazonia-1
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stactools-amazonia-1-0.1.1/README.md` & `stactools-amazonia-1-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.1/setup.cfg` & `stactools-amazonia-1-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/commands.py` & `stactools-amazonia-1-0.1.2/src/stactools/amazonia_1/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/constants.py` & `stactools-amazonia-1-0.1.2/src/stactools/amazonia_1/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/stac.py` & `stactools-amazonia-1-0.1.2/src/stactools/amazonia_1/stac.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,15 +480,15 @@
             f"{cbers_am['mission'].lower()}:row": int(cbers_am["row"]),
         }
     )
 
     # Metadata bucket
     meta_prefix = "https://s3.amazonaws.com/amazonia-meta-pds/"
     # COG bucket
-    main_prefix = "s3://cbers-pds/"
+    main_prefix = "s3://amazonia-pds/"
 
     # Thumbnail asset
     item.add_asset(
         key="thumbnail",
         asset=Asset.from_dict(
             {
                 "href": meta_prefix
```

### Comparing `stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/PKG-INFO` & `stactools-amazonia-1-0.1.2/src/stactools_amazonia_1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-amazonia-1
-Version: 0.1.1
+Version: 0.1.2
 Summary: Amazonia-1 on AWS stactools package
 Home-page: https://github.com/stactools-packages/amazonia-1
 Author: Frederico Liporace
 Author-email: liporace@amskepler.com
 Project-URL: Issues, https://github.com/stactools-packages/amazonia-1/issues
 Keywords: stactools,pystac,catalog,STAC,Amazonia-1
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stactools-amazonia-1-0.1.1/tests/test_commands.py` & `stactools-amazonia-1-0.1.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.1/tests/test_stac.py` & `stactools-amazonia-1-0.1.2/tests/test_stac.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,20 +113,20 @@
     assert (
         item.assets["thumbnail"].href
         == "https://s3.amazonaws.com/amazonia-meta-pds/AMAZONIA1/WFI/036/018/"
         "AMAZONIA_1_WFI_20220811_036_018_L4/AMAZONIA_1_WFI_20220811_036_018.png"
     )
     assert (
         item.assets["metadata"].href
-        == "s3://cbers-pds/AMAZONIA1/WFI/036/018/AMAZONIA_1_WFI_20220811_036_018_L4/"
+        == "s3://amazonia-pds/AMAZONIA1/WFI/036/018/AMAZONIA_1_WFI_20220811_036_018_L4/"
         "AMAZONIA_1_WFI_20220811_036_018_L4_BAND2.xml"
     )
     assert (
         item.assets["B2"].href
-        == "s3://cbers-pds/AMAZONIA1/WFI/036/018/AMAZONIA_1_WFI_20220811_036_018_L4/"
+        == "s3://amazonia-pds/AMAZONIA1/WFI/036/018/AMAZONIA_1_WFI_20220811_036_018_L4/"
         "AMAZONIA_1_WFI_20220811_036_018_L4_BAND2.tif"
     )
 
     # Create the STAC Item, single optic (LEFT)
     item = stac.create_item(
         "tests/fixtures/AMAZONIA_1_WFI_20220810_033_018_L4_LEFT_BAND2.xml"
     )
@@ -154,18 +154,18 @@
     assert (
         item.assets["thumbnail"].href
         == "https://s3.amazonaws.com/amazonia-meta-pds/AMAZONIA1/WFI/033/018/"
         "AMAZONIA_1_WFI_20220810_033_018_L4/AMAZONIA_1_WFI_20220810_033_018.png"
     )
     assert (
         item.assets["metadata"].href
-        == "s3://cbers-pds/AMAZONIA1/WFI/033/018/AMAZONIA_1_WFI_20220810_033_018_L4/"
+        == "s3://amazonia-pds/AMAZONIA1/WFI/033/018/AMAZONIA_1_WFI_20220810_033_018_L4/"
         "AMAZONIA_1_WFI_20220810_033_018_L4_LEFT_BAND2.xml"
     )
     assert (
         item.assets["B2"].href
-        == "s3://cbers-pds/AMAZONIA1/WFI/033/018/AMAZONIA_1_WFI_20220810_033_018_L4/"
+        == "s3://amazonia-pds/AMAZONIA1/WFI/033/018/AMAZONIA_1_WFI_20220810_033_018_L4/"
         "AMAZONIA_1_WFI_20220810_033_018_L4_LEFT_BAND2.tif"
     )
 
     # Validate
     item.validate()
```

