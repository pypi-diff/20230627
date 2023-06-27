# Comparing `tmp/wafermap-clustering-0.2.5.tar.gz` & `tmp/wafermap-clustering-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.2.5.tar", last modified: Mon Jun 26 13:29:42 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.2.6.tar", last modified: Mon Jun 26 13:44:34 2023, max compression
```

## Comparing `wafermap-clustering-0.2.5.tar` & `wafermap-clustering-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.371841 wafermap-clustering-0.2.5/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-06-26 13:29:42.368845 wafermap-clustering-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 13:29:42.372712 wafermap-clustering-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-06-26 13:28:21.000000 wafermap-clustering-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.283073 wafermap-clustering-0.2.5/tests/
--rw-rw-rw-   0        0        0     7745 2023-06-26 13:24:39.000000 wafermap-clustering-0.2.5/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.288255 wafermap-clustering-0.2.5/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.335161 wafermap-clustering-0.2.5/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-26 09:19:26.000000 wafermap-clustering-0.2.5/wafermap_clustering/configs/config.py
--rw-rw-rw-   0        0        0      913 2023-06-26 09:21:07.000000 wafermap-clustering-0.2.5/wafermap_clustering/configs/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.342509 wafermap-clustering-0.2.5/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4304 2023-04-06 09:28:27.000000 wafermap-clustering-0.2.5/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.362126 wafermap-clustering-0.2.5/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.5/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.5/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      763 2023-04-06 10:14:19.000000 wafermap-clustering-0.2.5/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     5464 2023-06-26 13:27:41.000000 wafermap-clustering-0.2.5/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.321889 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 13:44:34.659245 wafermap-clustering-0.2.6/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-06-26 13:44:34.656176 wafermap-clustering-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 13:44:34.660605 wafermap-clustering-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-06-26 13:42:59.000000 wafermap-clustering-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:44:34.575576 wafermap-clustering-0.2.6/tests/
+-rw-rw-rw-   0        0        0     7755 2023-06-26 13:40:34.000000 wafermap-clustering-0.2.6/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:44:34.580367 wafermap-clustering-0.2.6/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-06-26 13:44:34.624957 wafermap-clustering-0.2.6/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-26 09:19:26.000000 wafermap-clustering-0.2.6/wafermap_clustering/configs/config.py
+-rw-rw-rw-   0        0        0      913 2023-06-26 09:21:07.000000 wafermap-clustering-0.2.6/wafermap_clustering/configs/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:44:34.629849 wafermap-clustering-0.2.6/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4304 2023-04-06 09:28:27.000000 wafermap-clustering-0.2.6/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:44:34.650006 wafermap-clustering-0.2.6/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.6/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.6/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      763 2023-04-06 10:14:19.000000 wafermap-clustering-0.2.6/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     5482 2023-06-26 13:34:15.000000 wafermap-clustering-0.2.6/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:44:34.611894 wafermap-clustering-0.2.6/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-26 13:44:34.000000 wafermap-clustering-0.2.6/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-06-26 13:44:34.000000 wafermap-clustering-0.2.6/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 13:44:34.000000 wafermap-clustering-0.2.6/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-26 13:44:34.000000 wafermap-clustering-0.2.6/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-26 13:44:34.000000 wafermap-clustering-0.2.6/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.2.5/LICENSE.txt` & `wafermap-clustering-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.5/PKG-INFO` & `wafermap-clustering-0.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.5
+Version: 0.2.6
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.5.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.5/setup.py` & `wafermap-clustering-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.5"
+version = "0.2.6"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.2.5/tests/test_clustering.py` & `wafermap-clustering-0.2.6/tests/test_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         ]
 
         # THEN
         self.assertEqual(summary, expected_summary)
 
     def test_clustering_hdbscan_single_wafer(self):
         # GIVEN
-        output_path = ASSETS_OUPUT_PATH / "J237DTA_3236_hdbscan.000"
+        output_path = ASSETS_OUPUT_PATH
 
         expected_clusters = [615]
 
         # WHEN
         clustering = Clustering(config=self.config, autocreate_logger=True)
         results = clustering.apply(
             klarf_path=self.path_klarf_single_wafer,
@@ -202,28 +202,30 @@
         ]
 
         # THEN
         self.assertEqual(summary, expected_summary)
 
     def test_clustering_dbscan_single_wafer_with_baby_klarf_returned(self):
         # GIVEN
-        output_path = ASSETS_OUPUT_PATH / "J237DTA_3236_clustered.000"
+        output_dir = ASSETS_OUPUT_PATH
+
+        output_klarf = output_dir / "J237DTA_3236_baby_clustered.000"
         saved_klarf_path = ASSETS_PATH / "saved" / "J237DTA_3236_baby_clustered.000"
 
         # WHEN
         clustering = Clustering(config=self.config, autocreate_logger=True)
         clustering.apply(
             klarf_path=self.path_klarf_multi_wafers,
-            output_directory=output_path,
+            output_directory=output_dir,
             klarf_format=KlarfFormat.BABY.value,
         )
 
         # THEN
         self.assertEqual(
-            compare_files(saved_klarf_path, output_path),
+            compare_files(saved_klarf_path, output_dir),
             True,
         )
 
     def test_clustering_dbscan_single_wafer_with_full_klarf_returned(self):
         # GIVEN
         output_path = ASSETS_OUPUT_PATH / "J237DTA_3236_clustered.000"
         saved_klarf_path = ASSETS_PATH / "saved" / "J237DTA_3236_full_clustered.000"
```

### Comparing `wafermap-clustering-0.2.5/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.2.6/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.5/wafermap_clustering/configs/logging_config.py` & `wafermap-clustering-0.2.6/wafermap_clustering/configs/logging_config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.5/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.2.6/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.5/wafermap_clustering/models/clustering_performance.py` & `wafermap-clustering-0.2.6/wafermap_clustering/models/clustering_performance.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.5/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.2.6/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.5/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.2.6/wafermap_clustering/wafermap_clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 clustered_defects=clustered_defects,
             )
 
             output_timestamp = None
             output_filename = (
                 (
                     output_directory
-                    / f"{single_klarf.lot_id}_{single_klarf.step_id}_{single_klarf.wafer.id}.000"
+                    / f"{single_klarf.lot_id}_{single_klarf.step_id}_{single_klarf.wafer.id}_{clustering_mode}.000"
                 )
                 if output_directory is not None
                 else None
             )
             match klarf_format:
                 case KlarfFormat.BABY.value if output_directory is not None:
                     output_timestamp = klarf_lib.write_baby_klarf(
```

### Comparing `wafermap-clustering-0.2.5/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.2.6/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.5
+Version: 0.2.6
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.5.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.5/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.2.6/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

