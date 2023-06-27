# Comparing `tmp/cht_meteo-0.0.1.tar.gz` & `tmp/cht_meteo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cht_meteo-0.0.1.tar", last modified: Thu May 25 14:21:47 2023, max compression
+gzip compressed data, was "cht_meteo-0.1.0.tar", last modified: Tue Jun 27 09:59:37 2023, max compression
```

## Comparing `cht_meteo-0.0.1.tar` & `cht_meteo-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:21:47.150038 cht_meteo-0.0.1/
--rw-rw-rw-   0        0        0     1081 2023-05-02 11:57:48.000000 cht_meteo-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      540 2023-05-25 14:21:47.148033 cht_meteo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       35 2023-05-04 15:24:55.000000 cht_meteo-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 14:21:47.123074 cht_meteo-0.0.1/cht_meteo/
--rw-rw-rw-   0        0        0      115 2023-05-04 15:32:00.000000 cht_meteo-0.0.1/cht_meteo/__init__.py
--rw-rw-rw-   0        0        0    27760 2023-05-04 16:38:06.000000 cht_meteo-0.0.1/cht_meteo/coamps_tc_forecast.py
--rw-rw-rw-   0        0        0    23527 2023-05-04 16:44:33.000000 cht_meteo-0.0.1/cht_meteo/coamps_tc_hindcast.py
--rw-rw-rw-   0        0        0     4923 2023-05-04 15:53:23.000000 cht_meteo-0.0.1/cht_meteo/coamps_tc_ufl_d01.py
--rw-rw-rw-   0        0        0    12112 2023-05-04 15:56:43.000000 cht_meteo-0.0.1/cht_meteo/gfs_anl_0p50.py
--rw-rw-rw-   0        0        0     8658 2023-05-04 15:54:03.000000 cht_meteo-0.0.1/cht_meteo/gfs_anl_0p50_02.py
--rw-rw-rw-   0        0        0    15244 2023-05-04 16:31:38.000000 cht_meteo-0.0.1/cht_meteo/gfs_anl_0p50_04.py
--rw-rw-rw-   0        0        0     6098 2023-05-04 15:57:30.000000 cht_meteo-0.0.1/cht_meteo/gfs_forecast_0p25.py
--rw-rw-rw-   0        0        0     3780 2023-05-04 15:56:54.000000 cht_meteo-0.0.1/cht_meteo/gfs_forecast_0p25_02.py
--rw-rw-rw-   0        0        0    53873 2023-05-11 09:20:18.000000 cht_meteo-0.0.1/cht_meteo/meteo.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:21:47.142038 cht_meteo-0.0.1/cht_meteo.egg-info/
--rw-rw-rw-   0        0        0      540 2023-05-25 14:21:47.000000 cht_meteo-0.0.1/cht_meteo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-05-25 14:21:47.000000 cht_meteo-0.0.1/cht_meteo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:21:47.000000 cht_meteo-0.0.1/cht_meteo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-25 14:21:47.000000 cht_meteo-0.0.1/cht_meteo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 14:21:47.000000 cht_meteo-0.0.1/cht_meteo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 15:40:27.000000 cht_meteo-0.0.1/cht_meteo.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1209 2023-05-25 14:21:19.000000 cht_meteo-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 14:21:47.150038 cht_meteo-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 14:21:47.146031 cht_meteo-0.0.1/tests/
--rw-rw-rw-   0        0        0     1878 2023-05-12 08:50:44.000000 cht_meteo-0.0.1/tests/test_download_meteo.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:59:37.110238 cht_meteo-0.1.0/
+-rw-rw-rw-   0        0        0     1081 2023-05-02 11:57:48.000000 cht_meteo-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      540 2023-06-27 09:59:37.109065 cht_meteo-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       35 2023-05-04 15:24:55.000000 cht_meteo-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 09:59:37.069059 cht_meteo-0.1.0/cht_meteo/
+-rw-rw-rw-   0        0        0      115 2023-06-27 09:57:56.000000 cht_meteo-0.1.0/cht_meteo/__init__.py
+-rw-rw-rw-   0        0        0    27760 2023-05-04 16:38:06.000000 cht_meteo-0.1.0/cht_meteo/coamps_tc_forecast.py
+-rw-rw-rw-   0        0        0    23527 2023-05-04 16:44:33.000000 cht_meteo-0.1.0/cht_meteo/coamps_tc_hindcast.py
+-rw-rw-rw-   0        0        0     4923 2023-05-04 15:53:23.000000 cht_meteo-0.1.0/cht_meteo/coamps_tc_ufl_d01.py
+-rw-rw-rw-   0        0        0    12112 2023-05-04 15:56:43.000000 cht_meteo-0.1.0/cht_meteo/gfs_anl_0p50.py
+-rw-rw-rw-   0        0        0     8658 2023-05-04 15:54:03.000000 cht_meteo-0.1.0/cht_meteo/gfs_anl_0p50_02.py
+-rw-rw-rw-   0        0        0    15244 2023-05-04 16:31:38.000000 cht_meteo-0.1.0/cht_meteo/gfs_anl_0p50_04.py
+-rw-rw-rw-   0        0        0     6098 2023-05-04 15:57:30.000000 cht_meteo-0.1.0/cht_meteo/gfs_forecast_0p25.py
+-rw-rw-rw-   0        0        0     3780 2023-05-04 15:56:54.000000 cht_meteo-0.1.0/cht_meteo/gfs_forecast_0p25_02.py
+-rw-rw-rw-   0        0        0    53873 2023-05-11 09:20:18.000000 cht_meteo-0.1.0/cht_meteo/meteo.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:59:37.100466 cht_meteo-0.1.0/cht_meteo/misc/
+-rw-rw-rw-   0        0        0      115 2023-06-27 09:58:05.000000 cht_meteo-0.1.0/cht_meteo/misc/__init__.py
+-rw-rw-rw-   0        0        0     2813 2023-05-04 16:21:11.000000 cht_meteo-0.1.0/cht_meteo/misc/fileops.py
+-rw-rw-rw-   0        0        0     2816 2023-05-04 16:38:34.000000 cht_meteo-0.1.0/cht_meteo/misc/misc_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:59:37.086352 cht_meteo-0.1.0/cht_meteo.egg-info/
+-rw-rw-rw-   0        0        0      540 2023-06-27 09:59:36.000000 cht_meteo-0.1.0/cht_meteo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-06-27 09:59:36.000000 cht_meteo-0.1.0/cht_meteo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:59:36.000000 cht_meteo-0.1.0/cht_meteo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-06-27 09:59:36.000000 cht_meteo-0.1.0/cht_meteo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 09:59:36.000000 cht_meteo-0.1.0/cht_meteo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 15:40:27.000000 cht_meteo-0.1.0/cht_meteo.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1657 2023-06-27 09:56:43.000000 cht_meteo-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:59:37.110238 cht_meteo-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 09:59:37.104053 cht_meteo-0.1.0/tests/
+-rw-rw-rw-   0        0        0     1878 2023-05-12 08:50:44.000000 cht_meteo-0.1.0/tests/test_download_meteo.py
```

### Comparing `cht_meteo-0.0.1/LICENSE` & `cht_meteo-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/PKG-INFO` & `cht_meteo-0.1.0/cht_meteo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cht_meteo
-Version: 0.0.1
+Name: cht-meteo
+Version: 0.1.0
 Author-email: Maarten van Ormondt <maarten.vanormondt@deltares.nl>, Julian Hofer <Julian.Hofer@deltares.nl>, Sarwan Peiter <Sarwan.Peiter@deltares.nl>
 License: MIT
 Project-URL: Source, https://github.com/Deltares/cht_meteo
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `cht_meteo-0.0.1/cht_meteo/coamps_tc_forecast.py` & `cht_meteo-0.1.0/cht_meteo/coamps_tc_forecast.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo/coamps_tc_hindcast.py` & `cht_meteo-0.1.0/cht_meteo/coamps_tc_hindcast.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo/coamps_tc_ufl_d01.py` & `cht_meteo-0.1.0/cht_meteo/coamps_tc_ufl_d01.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo/gfs_anl_0p50.py` & `cht_meteo-0.1.0/cht_meteo/gfs_anl_0p50.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo/gfs_anl_0p50_02.py` & `cht_meteo-0.1.0/cht_meteo/gfs_anl_0p50_02.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo/gfs_anl_0p50_04.py` & `cht_meteo-0.1.0/cht_meteo/gfs_anl_0p50_04.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo/gfs_forecast_0p25.py` & `cht_meteo-0.1.0/cht_meteo/gfs_forecast_0p25.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo/gfs_forecast_0p25_02.py` & `cht_meteo-0.1.0/cht_meteo/gfs_forecast_0p25_02.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo/meteo.py` & `cht_meteo-0.1.0/cht_meteo/meteo.py`

 * *Files identical despite different names*

### Comparing `cht_meteo-0.0.1/cht_meteo.egg-info/SOURCES.txt` & `cht_meteo-0.1.0/cht_meteo.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,8 +13,11 @@
 cht_meteo/meteo.py
 cht_meteo.egg-info/PKG-INFO
 cht_meteo.egg-info/SOURCES.txt
 cht_meteo.egg-info/dependency_links.txt
 cht_meteo.egg-info/requires.txt
 cht_meteo.egg-info/top_level.txt
 cht_meteo.egg-info/zip-safe
+cht_meteo/misc/__init__.py
+cht_meteo/misc/fileops.py
+cht_meteo/misc/misc_tools.py
 tests/test_download_meteo.py
```

### Comparing `cht_meteo-0.0.1/tests/test_download_meteo.py` & `cht_meteo-0.1.0/tests/test_download_meteo.py`

 * *Files identical despite different names*

