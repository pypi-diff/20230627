# Comparing `tmp/wafermap-clustering-0.2.8.tar.gz` & `tmp/wafermap-clustering-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.2.8.tar", last modified: Tue Jun 27 11:15:42 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.2.9.tar", last modified: Tue Jun 27 13:05:15 2023, max compression
```

## Comparing `wafermap-clustering-0.2.8.tar` & `wafermap-clustering-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.366420 wafermap-clustering-0.2.8/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-06-27 11:15:42.363921 wafermap-clustering-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 11:15:42.369368 wafermap-clustering-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      990 2023-06-27 11:15:12.000000 wafermap-clustering-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.233943 wafermap-clustering-0.2.8/tests/
--rw-rw-rw-   0        0        0     9104 2023-06-27 09:31:23.000000 wafermap-clustering-0.2.8/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.239249 wafermap-clustering-0.2.8/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.306963 wafermap-clustering-0.2.8/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.2.8/wafermap_clustering/configs/config.py
--rw-rw-rw-   0        0        0      913 2023-06-27 08:34:33.000000 wafermap-clustering-0.2.8/wafermap_clustering/configs/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.316814 wafermap-clustering-0.2.8/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     5708 2023-06-27 09:01:57.000000 wafermap-clustering-0.2.8/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.348134 wafermap-clustering-0.2.8/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.8/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.8/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.2.8/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     5588 2023-06-27 08:44:43.000000 wafermap-clustering-0.2.8/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.285039 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:15.888478 wafermap-clustering-0.2.9/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-06-27 13:05:15.885466 wafermap-clustering-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 13:05:15.889776 wafermap-clustering-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-06-27 13:04:18.000000 wafermap-clustering-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:15.740236 wafermap-clustering-0.2.9/tests/
+-rw-rw-rw-   0        0        0     8837 2023-06-27 12:35:52.000000 wafermap-clustering-0.2.9/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:15.746780 wafermap-clustering-0.2.9/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:15.823356 wafermap-clustering-0.2.9/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.2.9/wafermap_clustering/configs/config.py
+-rw-rw-rw-   0        0        0      913 2023-06-27 08:34:33.000000 wafermap-clustering-0.2.9/wafermap_clustering/configs/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:15.838620 wafermap-clustering-0.2.9/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     5708 2023-06-27 13:02:36.000000 wafermap-clustering-0.2.9/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:15.872420 wafermap-clustering-0.2.9/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.9/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.9/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.2.9/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     5588 2023-06-27 08:44:43.000000 wafermap-clustering-0.2.9/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:15.796336 wafermap-clustering-0.2.9/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-27 13:05:15.000000 wafermap-clustering-0.2.9/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-06-27 13:05:15.000000 wafermap-clustering-0.2.9/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:05:15.000000 wafermap-clustering-0.2.9/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-27 13:05:15.000000 wafermap-clustering-0.2.9/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-27 13:05:15.000000 wafermap-clustering-0.2.9/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.2.8/LICENSE.txt` & `wafermap-clustering-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.8/PKG-INFO` & `wafermap-clustering-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.8
+Version: 0.2.9
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.8.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.8/setup.py` & `wafermap-clustering-0.2.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.8"
+version = "0.2.9"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.2.8/tests/test_clustering.py` & `wafermap-clustering-0.2.9/tests/test_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,14 @@
     KlarfFormat,
 )
 
 ASSETS_PATH: Path = Path(__file__).parent / "assets"
 ASSETS_OUPUT_PATH: Path = ASSETS_PATH / "clustering" / "output"
 
 
-def compare_files(file1_path, file2_path):
-    with open(file1_path, "r") as file1, open(file2_path, "r") as file2:
-        for i, (line1, line2) in enumerate(zip(file1, file2)):
-            if line1 != line2:
-                return False
-
-    return True
-
-
 class TestClustering(unittest.TestCase):
     def setUp(self) -> None:
         self.path_klarf_single_wafer = ASSETS_PATH / "J052SBN_8196_J052SBN-01.000"
         self.path_klarf_multi_wafers = ASSETS_PATH / "J237DTA_3236.000"
         self.path_klarf_single_wafer_large_klarf = ASSETS_PATH / "LARGE_KLARF.000"
 
         self.config = Config(
```

### Comparing `wafermap-clustering-0.2.8/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.2.9/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.8/wafermap_clustering/configs/logging_config.py` & `wafermap-clustering-0.2.9/wafermap_clustering/configs/logging_config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.8/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.2.9/wafermap_clustering/libs/klarf_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         )
         f.write(f"SampleTestPlan {num_sample_test_plan}\n")
         f.write("".join(sample_test_plan_rows))
         for test in single_klarf.wafer.tests:
             f.write(f"InspectionTest {test.id}\n")
             f.write(f"AreaPerTest {test.area:0.10e}\n")
         f.write(
-            f"DefectRecordSpec 14 DEFECTID XREL YREL XINDEX YINDEX XSIZE YSIZE DEFECTAREA DSIZE CLASSNUMBER TEST CLUSTERNUMBER ROUGHBINNUMBER FINEBINNUMBER IMAGECOUNT {attribute} ;\n"
+            f"DefectRecordSpec 16 DEFECTID XREL YREL XINDEX YINDEX XSIZE YSIZE DEFECTAREA DSIZE CLASSNUMBER TEST CLUSTERNUMBER ROUGHBINNUMBER FINEBINNUMBER IMAGECOUNT {attribute} ;\n"
         )
         f.write(f"DefectList\n")
         f.write("".join(defect_rows))
         f.write("EndOfFile;")
 
     return time.time() - tic
```

### Comparing `wafermap-clustering-0.2.8/wafermap_clustering/models/clustering_performance.py` & `wafermap-clustering-0.2.9/wafermap_clustering/models/clustering_performance.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.8/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.2.9/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.8/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.2.9/wafermap_clustering/wafermap_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.8/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.2.9/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.8
+Version: 0.2.9
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.8.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.8/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.2.9/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

