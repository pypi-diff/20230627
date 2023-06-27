# Comparing `tmp/cygnsslib-1.3.2.tar.gz` & `tmp/cygnsslib-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cygnsslib-1.3.2.tar", last modified: Thu May  4 00:07:45 2023, max compression
+gzip compressed data, was "cygnsslib-1.3.3.tar", last modified: Tue Jun 27 17:54:11 2023, max compression
```

## Comparing `cygnsslib-1.3.2.tar` & `cygnsslib-1.3.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/
--rw-rw-rw-   0 root         (0) root         (0)    15905 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13015 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib/
--rw-rw-rw-   0 root         (0) root         (0)    14486 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/CygDdmId.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    63464 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/cyg.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib/cygnss_download/
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/cygnss_download/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib/data_downloader/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/cyg_ant_ptrn.py
--rw-rw-rw-   0 root         (0) root         (0)     5663 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cyg_rawif.py
--rw-rw-rw-   0 root         (0) root         (0)    19700 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cygnss.py
--rw-rw-rw-   0 root         (0) root         (0)     6530 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cygnss_sftp.py
--rw-rw-rw-   0 root         (0) root         (0)    13187 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_srtm.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/istarmap.py
--rw-rw-rw-   0 root         (0) root         (0)     4905 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/plotting.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib/srtm_download/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/srtm_download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9205 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    15905 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/list_loc2kml.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_download_cyg_data.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_download_srtm.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_find_land_prod_from_cvs.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_search_within_circle.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_write_sp_within_radius.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)    15905 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13015 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/src/cygnsslib/
+-rw-rw-rw-   0 root         (0) root         (0)    14486 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/CygDdmId.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    63577 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/cyg.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/src/cygnsslib/cygnss_download/
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/cygnss_download/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/src/cygnsslib/data_downloader/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/data_downloader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/data_downloader/cyg_ant_ptrn.py
+-rw-rw-rw-   0 root         (0) root         (0)     5663 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/data_downloader/download_cyg_rawif.py
+-rw-rw-rw-   0 root         (0) root         (0)    19700 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/data_downloader/download_cygnss.py
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/data_downloader/download_cygnss_sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)    13178 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/data_downloader/download_srtm.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/istarmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     4905 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/plotting.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/src/cygnsslib/srtm_download/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/srtm_download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9205 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/cygnsslib/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/src/cygnsslib.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    15905 2023-06-27 17:54:11.000000 cygnsslib-1.3.3/src/cygnsslib.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-27 17:54:11.000000 cygnsslib-1.3.3/src/cygnsslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 17:54:11.000000 cygnsslib-1.3.3/src/cygnsslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-27 17:54:11.000000 cygnsslib-1.3.3/src/cygnsslib.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-06-27 17:54:11.000000 cygnsslib-1.3.3/src/cygnsslib.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:54:11.867342 cygnsslib-1.3.3/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/tests/list_loc2kml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/tests/test_download_cyg_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/tests/test_download_srtm.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/tests/test_find_land_prod_from_cvs.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/tests/test_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/tests/test_search_within_circle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-06-27 17:54:00.000000 cygnsslib-1.3.3/src/tests/test_write_sp_within_radius.py
```

### Comparing `cygnsslib-1.3.2/PKG-INFO` & `cygnsslib-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cygnsslib
-Version: 1.3.2
+Version: 1.3.3
 Summary: Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC
 Home-page: https://bitbucket.org/usc_mixil/cygnsslib
 Author: Amer Melebari and James D. Campbell
 Author-email: amelebar@usc.edu
 License: UNKNOWN
 Description: # CYGNSS Library
```

### Comparing `cygnsslib-1.3.2/README.md` & `cygnsslib-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/setup.py` & `cygnsslib-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as fh:
     req = fh.read()
 
 setup(
     name='cygnsslib',
-    version='1.3.2',
+    version='1.3.3',
     author='Amer Melebari and James D. Campbell',
     author_email='amelebar@usc.edu',
     description='Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC',
     long_description=long_description,
     install_requires=req.split(),
     long_description_content_type="text/markdown",
     url='https://bitbucket.org/usc_mixil/cygnsslib',
```

### Comparing `cygnsslib-1.3.2/src/cygnsslib/CygDdmId.py` & `cygnsslib-1.3.3/src/cygnsslib/CygDdmId.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib/__init__.py` & `cygnsslib-1.3.3/src/cygnsslib/__init__.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib/cyg.py` & `cygnsslib-1.3.3/src/cygnsslib/cyg.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,14 +456,16 @@
 
     # create in-situ kml file
     st_ref = ogr.StyleTable()
     st_ref.AddStyle("ref_normal", 'SYMBOL(c:#FFFF00,s:1.0,id:"http://maps.google.com/mapfiles/kml/shapes/flag.png")')
     st_ref.AddStyle("ref_highlight", 'SYMBOL(c:#FFFF00,s:1.3,id:"http://maps.google.com/mapfiles/kml/shapes/flag.png")')
     dvr = ogr.GetDriverByName("KML")
     out_ref = out_root + "_search_area.kml"
+    if not os.path.isdir(os.path.dirname(out_ref)):
+        os.makedirs(os.path.dirname(out_ref), exist_ok=True)
     ds_out_ref = dvr.CreateDataSource(out_ref)
     ds_out_ref.SetStyleTable(st_ref)
     lyr_name = "search_area"
     lyr = ds_out_ref.CreateLayer(lyr_name, geom_type=ogr.wkbLinearRing)
     lyr.CreateField(ogr.FieldDefn("Name", ogr.OFTString))
     feat = ogr.Feature(lyr.GetLayerDefn())
     feat.SetGeometry(poly)
```

### Comparing `cygnsslib-1.3.2/src/cygnsslib/data_downloader/cyg_ant_ptrn.py` & `cygnsslib-1.3.3/src/cygnsslib/data_downloader/cyg_ant_ptrn.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cyg_rawif.py` & `cygnsslib-1.3.3/src/cygnsslib/data_downloader/download_cyg_rawif.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cygnss.py` & `cygnsslib-1.3.3/src/cygnsslib/data_downloader/download_cygnss.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cygnss_sftp.py` & `cygnsslib-1.3.3/src/cygnsslib/data_downloader/download_cygnss_sftp.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_srtm.py` & `cygnsslib-1.3.3/src/cygnsslib/data_downloader/download_srtm.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,17 +272,17 @@
         os.makedirs(out_folder, exist_ok=True)
     if earthdata_usr_pass is None:
         earthdata_usr_pass = get_earthdata_cred()
 
     d_file_paths = list()
     for lat in list_lat:
         for lon in list_lon:
-            d_file_paths.append(download_srtm_ght_single_file(lat, lon, out_folder=out_folder, earthdata_usr_pass=earthdata_usr_pass,
-                                                              save_pass=save_pass, unzipfile=unzipfile, remove_zipedfile=remove_zippedfile,
-                                                              silent_run=silent_run))
+            file_name = download_srtm_ght_single_file(lat, lon, out_folder, earthdata_usr_pass, save_pass, unzipfile, remove_zippedfile, silent_run)
+            if file_name is not None:  # only add when we download files
+                d_file_paths.append(file_name)
 
     return d_file_paths
 
 
 def download_srtm_ght_single_file(lat, lon, out_folder=None, earthdata_usr_pass=None, save_pass=True, unzipfile=False, remove_zipedfile=True,
                                   silent_run=False):
     """
@@ -327,14 +327,16 @@
             print(f'{file_path:s} file exist')
         return file_path
 
     if earthdata_usr_pass is None:
         earthdata_usr_pass = get_earthdata_cred()
     file_url = f'{SRTM_USGS_URL:s}{file_name:s}'
     saved_zip_file = _download_file_earthdata(file_url, out_folder, auth=earthdata_usr_pass)
+    if saved_zip_file is None:  # If no file, i.e. over ocean
+        return None
     if not unzipfile:
         return saved_zip_file
 
     extract_srtm_zipfile(saved_zip_file, out_folder)
     unzipped_file = os.path.join(out_folder, get_srtm_unzipped_file_name(file_name))
     if remove_zipedfile:
         os.remove(saved_zip_file)
```

### Comparing `cygnsslib-1.3.2/src/cygnsslib/istarmap.py` & `cygnsslib-1.3.3/src/cygnsslib/istarmap.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib/plotting.py` & `cygnsslib-1.3.3/src/cygnsslib/plotting.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib/util.py` & `cygnsslib-1.3.3/src/cygnsslib/util.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/cygnsslib.egg-info/PKG-INFO` & `cygnsslib-1.3.3/src/cygnsslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cygnsslib
-Version: 1.3.2
+Version: 1.3.3
 Summary: Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC
 Home-page: https://bitbucket.org/usc_mixil/cygnsslib
 Author: Amer Melebari and James D. Campbell
 Author-email: amelebar@usc.edu
 License: UNKNOWN
 Description: # CYGNSS Library
```

### Comparing `cygnsslib-1.3.2/src/cygnsslib.egg-info/SOURCES.txt` & `cygnsslib-1.3.3/src/cygnsslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/tests/list_loc2kml.py` & `cygnsslib-1.3.3/src/tests/list_loc2kml.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/tests/test_download_cyg_data.py` & `cygnsslib-1.3.3/src/tests/test_download_cyg_data.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/tests/test_functions.py` & `cygnsslib-1.3.3/src/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/tests/test_search_within_circle.py` & `cygnsslib-1.3.3/src/tests/test_search_within_circle.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.2/src/tests/test_write_sp_within_radius.py` & `cygnsslib-1.3.3/src/tests/test_write_sp_within_radius.py`

 * *Files identical despite different names*

