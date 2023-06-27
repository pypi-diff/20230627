# Comparing `tmp/wafermap-clustering-0.2.7.tar.gz` & `tmp/wafermap-clustering-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.2.7.tar", last modified: Tue Jun 27 09:36:12 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.2.8.tar", last modified: Tue Jun 27 11:15:42 2023, max compression
```

## Comparing `wafermap-clustering-0.2.7.tar` & `wafermap-clustering-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:36:12.387679 wafermap-clustering-0.2.7/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-06-27 09:36:12.383474 wafermap-clustering-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 09:36:12.388865 wafermap-clustering-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-06-27 09:33:10.000000 wafermap-clustering-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:36:12.235974 wafermap-clustering-0.2.7/tests/
--rw-rw-rw-   0        0        0     9104 2023-06-27 09:31:23.000000 wafermap-clustering-0.2.7/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:36:12.245055 wafermap-clustering-0.2.7/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-06-27 09:36:12.322288 wafermap-clustering-0.2.7/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.2.7/wafermap_clustering/configs/config.py
--rw-rw-rw-   0        0        0      913 2023-06-27 08:34:33.000000 wafermap-clustering-0.2.7/wafermap_clustering/configs/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:36:12.331953 wafermap-clustering-0.2.7/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     5708 2023-06-27 09:01:57.000000 wafermap-clustering-0.2.7/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:36:12.374127 wafermap-clustering-0.2.7/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.7/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.7/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.2.7/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     5588 2023-06-27 08:44:43.000000 wafermap-clustering-0.2.7/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:36:12.296607 wafermap-clustering-0.2.7/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-27 09:36:12.000000 wafermap-clustering-0.2.7/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-06-27 09:36:12.000000 wafermap-clustering-0.2.7/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:36:12.000000 wafermap-clustering-0.2.7/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-27 09:36:12.000000 wafermap-clustering-0.2.7/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-27 09:36:12.000000 wafermap-clustering-0.2.7/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.366420 wafermap-clustering-0.2.8/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-06-27 11:15:42.363921 wafermap-clustering-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 11:15:42.369368 wafermap-clustering-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-06-27 11:15:12.000000 wafermap-clustering-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.233943 wafermap-clustering-0.2.8/tests/
+-rw-rw-rw-   0        0        0     9104 2023-06-27 09:31:23.000000 wafermap-clustering-0.2.8/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.239249 wafermap-clustering-0.2.8/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.306963 wafermap-clustering-0.2.8/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.2.8/wafermap_clustering/configs/config.py
+-rw-rw-rw-   0        0        0      913 2023-06-27 08:34:33.000000 wafermap-clustering-0.2.8/wafermap_clustering/configs/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.316814 wafermap-clustering-0.2.8/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     5708 2023-06-27 09:01:57.000000 wafermap-clustering-0.2.8/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.348134 wafermap-clustering-0.2.8/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.8/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.8/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.2.8/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     5588 2023-06-27 08:44:43.000000 wafermap-clustering-0.2.8/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:15:42.285039 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-27 11:15:42.000000 wafermap-clustering-0.2.8/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.2.7/LICENSE.txt` & `wafermap-clustering-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.7/PKG-INFO` & `wafermap-clustering-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.7
+Version: 0.2.8
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.7.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.8.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.7/setup.py` & `wafermap-clustering-0.2.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
-version = "0.2.7"
+version = "0.2.8"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
         "wafermap_clustering.libs",
         "wafermap_clustering.models",
     ],
     install_requires=[
-        "klarf-reader",
-        "scikit-learn",
-        "setuptools",
-        "hdbscan",
+        "klarf-reader==0.3.3",
+        "scikit-learn==1.2.1",
+        "setuptools==65.6.3",
+        "hdbscan==0.8.29",
     ],
     license="MIT",
     author="Maxime MARTIN",
     author_email="maxime.martin02@hotmail.fr",
     description="A project to apply clustering on wafermaps",
     url="https://github.com/Impro02/wafermap-clustering",
     download_url="https://github.com/Impro02/wafermap-clustering/archive/refs/tags/%s.tar.gz"
```

### Comparing `wafermap-clustering-0.2.7/tests/test_clustering.py` & `wafermap-clustering-0.2.8/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.7/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.2.8/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.7/wafermap_clustering/configs/logging_config.py` & `wafermap-clustering-0.2.8/wafermap_clustering/configs/logging_config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.7/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.2.8/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.7/wafermap_clustering/models/clustering_performance.py` & `wafermap-clustering-0.2.8/wafermap_clustering/models/clustering_performance.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.7/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.2.8/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.7/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.2.8/wafermap_clustering/wafermap_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.7/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.2.8/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.7
+Version: 0.2.8
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.7.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.8.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.7/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.2.8/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

