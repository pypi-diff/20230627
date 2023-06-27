# Comparing `tmp/animage-data_sorter-1.1.2.tar.gz` & `tmp/animage-data_sorter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\animage-data_sorter-1.1.2.tar", last modified: Mon Jun 19 08:42:44 2023, max compression
+gzip compressed data, was "dist\animage-data_sorter-1.1.3.tar", last modified: Tue Jun 27 07:13:32 2023, max compression
```

## Comparing `animage-data_sorter-1.1.2.tar` & `animage-data_sorter-1.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/
--rw-rw-rw-   0        0        0     1363 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/
--rw-rw-rw-   0        0        0     1363 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/data_sorter/
--rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.2/data_sorter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/data_sorter/old/
--rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageASLUtility.py
--rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDCMUtility.py
--rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorter.py
--rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterGEeASL7.py
--rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterGEpCASL13.py
--rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterMISC.py
--rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterPhilips13.py
--rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens4.py
--rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens5.py
--rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemensPASL.py
--rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
--rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterUtility.py
--rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.2/data_sorter/old/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/data_sorter/restructure/
--rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.1.2/data_sorter/restructure/__init__.py
--rw-rw-rw-   0        0        0    36867 2023-06-07 06:32:18.000000 animage-data_sorter-1.1.2/data_sorter/restructure/_dicom.py
--rw-rw-rw-   0        0        0     9885 2023-05-16 02:58:30.000000 animage-data_sorter-1.1.2/data_sorter/restructure/_dicom_util.py
--rw-rw-rw-   0        0        0     3833 2023-05-16 01:45:10.000000 animage-data_sorter-1.1.2/data_sorter/restructure/_type.py
--rw-rw-rw-   0        0        0     4279 2023-05-29 05:21:20.000000 animage-data_sorter-1.1.2/data_sorter/restructure/data_sorter_base.py
--rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.2/data_sorter/restructure/dcm2nifti.py
--rw-rw-rw-   0        0        0     3515 2023-05-17 05:44:59.000000 animage-data_sorter-1.1.2/data_sorter/restructure/errors.py
--rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.2/data_sorter/restructure/ge_3d_pcasl.py
--rw-rw-rw-   0        0        0     8516 2023-05-29 05:23:17.000000 animage-data_sorter-1.1.2/data_sorter/restructure/ge_easl.py
--rw-rw-rw-   0        0        0    10444 2023-06-19 06:06:18.000000 animage-data_sorter-1.1.2/data_sorter/restructure/noASL_MRI.py
--rw-rw-rw-   0        0        0     4431 2023-06-07 08:39:25.000000 animage-data_sorter-1.1.2/data_sorter/restructure/philips_3d_pcasl.py
--rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pasl.py
--rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pcasl.py
--rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pcasl_old.py
--rw-rw-rw-   0        0        0     4421 2023-05-16 01:48:06.000000 animage-data_sorter-1.1.2/data_sorter/restructure/uih_3d_pasl.py
--rw-rw-rw-   0        0        0       42 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-06-19 08:40:59.000000 animage-data_sorter-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/
+-rw-rw-rw-   0        0        0     1363 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/
+-rw-rw-rw-   0        0        0     1363 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/data_sorter/
+-rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.3/data_sorter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/data_sorter/old/
+-rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageASLUtility.py
+-rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDCMUtility.py
+-rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorter.py
+-rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterGEeASL7.py
+-rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterGEpCASL13.py
+-rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterMISC.py
+-rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterPhilips13.py
+-rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens4.py
+-rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens5.py
+-rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemensPASL.py
+-rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
+-rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterUtility.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.3/data_sorter/old/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/data_sorter/restructure/
+-rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.1.3/data_sorter/restructure/__init__.py
+-rw-rw-rw-   0        0        0    37031 2023-06-26 03:46:08.000000 animage-data_sorter-1.1.3/data_sorter/restructure/_dicom.py
+-rw-rw-rw-   0        0        0    12556 2023-06-26 04:37:14.000000 animage-data_sorter-1.1.3/data_sorter/restructure/_dicom_util.py
+-rw-rw-rw-   0        0        0     4330 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.3/data_sorter/restructure/_type.py
+-rw-rw-rw-   0        0        0     4279 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.3/data_sorter/restructure/data_sorter_base.py
+-rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.3/data_sorter/restructure/dcm2nifti.py
+-rw-rw-rw-   0        0        0     3515 2023-05-17 05:44:59.000000 animage-data_sorter-1.1.3/data_sorter/restructure/errors.py
+-rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.3/data_sorter/restructure/ge_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8516 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.3/data_sorter/restructure/ge_easl.py
+-rw-rw-rw-   0        0        0    12139 2023-06-27 06:57:43.000000 animage-data_sorter-1.1.3/data_sorter/restructure/noASL_MRI.py
+-rw-rw-rw-   0        0        0     4431 2023-06-07 08:39:25.000000 animage-data_sorter-1.1.3/data_sorter/restructure/philips_3d_pcasl.py
+-rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pasl.py
+-rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pcasl_old.py
+-rw-rw-rw-   0        0        0     4513 2023-06-26 05:05:08.000000 animage-data_sorter-1.1.3/data_sorter/restructure/uih_3d_pasl.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-06-27 07:13:04.000000 animage-data_sorter-1.1.3/setup.py
```

### Comparing `animage-data_sorter-1.1.2/PKG-INFO` & `animage-data_sorter-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data_sorter
-Version: 1.1.2
+Version: 1.1.3
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.1.2/README.md` & `animage-data_sorter-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/animage_data_sorter.egg-info/PKG-INFO` & `animage-data_sorter-1.1.3/animage_data_sorter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data-sorter
-Version: 1.1.2
+Version: 1.1.3
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.1.2/animage_data_sorter.egg-info/SOURCES.txt` & `animage-data_sorter-1.1.3/animage_data_sorter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/__init__.py` & `animage-data_sorter-1.1.3/data_sorter/__init__.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageASLUtility.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageASLUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDCMUtility.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDCMUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorter.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorter.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterGEeASL7.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterGEeASL7.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterGEpCASL13.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterGEpCASL13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterMISC.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterMISC.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterPhilips13.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterPhilips13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens4.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens4.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens5.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens5.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemensPASL.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemensPASL.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens_UCLA.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens_UCLA.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterUtility.py` & `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/__init__.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/__init__.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/_dicom.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/_dicom.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,15 +455,15 @@
                 if data_type != MRI_Type.MRI_TYPE_UnKnown:
                     pass
                 else:
                     if (series_description.startswith('tgse_pcasl_pld') and
                         not series_description.startswith('tgse_pcasl_pld5')) or \
                             series_description.startswith('tgse_pcasl_m0'):
                         ASL_type, data_type = ASL_Type.ASL_PCASL, MRI_Type.MRI_TYPE_1Delay_3D_PCASL_SIEMENS
-                    elif series_description.startswith('tgse_pcasl'):
+                    elif series_description.startswith('tgse_pcasl') or series_description.startswith('pcasl_5delay'):
                         ASL_type, data_type = ASL_Type.ASL_PCASL, MRI_Type.MRI_TYPE_5Delay_3D_PCASL_SIEMENS
                     elif series_description.find('te00_ti') > -1:
                         ASL_type, data_type = ASL_Type.ASL_PCASL, MRI_Type.MRI_TYPE_4Delay_3D_PCASL_SIEMENS_Old
                     elif series_description.startswith('asl_3d') or series_description.find('m0') > -1:
                         ASL_type, data_type = ASL_type.ASL_PASL, MRI_Type.MRI_TYPE_3D_PASL_SIEMENS
                     elif series_description.find('t1') > -1:
                         data_type = MRI_Type.MRI_TYPE_T1
@@ -511,23 +511,26 @@
                     data_type = MRI_Type.MRI_TYPE_T2
                 elif series_description.find('dwi') > -1 or series_description.find('adc') > -1 or \
                         series_description.find('apparent diffusion coefficient') > -1:
                     data_type = MRI_Type.MRI_TYPE_DWI
 
         elif manufacturer == MANUFACTURER.kMANUFACTURER_UIH:
             if series_description is not None and series_description != '':
-                if series_description.startswith('asl_3d'):
+                if series_description.find('asl_3d') > -1:
                     ASL_type, data_type = ASL_type, MRI_Type.MRI_TYPE_3D_PASL_UIH
                 elif series_description.find('t1') > -1:
                     data_type = MRI_Type.MRI_TYPE_T1
                     # t1 放在t2 flair前面；避免t1 flair被认为是 t2 flair
                 elif series_description.find('flair') > -1 or series_description.find('fluid') > -1:
                     data_type = MRI_Type.MRI_TYPE_T2_FLAIR
                 elif series_description.find('t2') > -1:
                     data_type = MRI_Type.MRI_TYPE_T2
+                elif series_description.find('dwi') > -1:
+                    data_type = MRI_Type.MRI_TYPE_DWI
+
 
         return ASL_type, data_type
 
     def validate_series(self):
         '''
         验证数据的完整性以及正确性；计算出层厚、层数量、以及重复次数是否符合要求
         :return:
```

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/_type.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -82,14 +82,27 @@
 
     MRI_TYPE_T1 = 'T1'
     MRI_TYPE_T2 = 'T2'
     MRI_TYPE_T2_FLAIR = 'T2_FLAIR'
     MRI_TYPE_DWI = 'DWI'
 
     # MRI_TYPE_ADC = 'ADC'
+    def SimpleName(self) -> str:
+        if self in [
+            MRI_Type.MRI_TYPE_5Delay_3D_PCASL_SIEMENS,
+            MRI_Type.MRI_TYPE_1Delay_3D_PCASL_SIEMENS,
+            MRI_Type.MRI_TYPE_4Delay_3D_PCASL_SIEMENS_Old,
+            MRI_Type.MRI_TYPE_3D_PASL_SIEMENS,
+            MRI_Type.MRI_TYPE_3D_PCASL_GE,
+            MRI_Type.MRI_TYPE_3D_PCASL_PHILIPS,
+            MRI_Type.MRI_TYPE_3D_PASL_UIH,
+        ]:
+            return 'ASL'
+        else:
+            return self.value
 
 class SliceDirection(Enum):
     Axial = 'XY' # 轴状面
     Coronal = 'XZ'  # 冠状面
     Sagittal = 'YZ' # 矢状面
 
     def iSL(self):
```

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/data_sorter_base.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/data_sorter_base.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/dcm2nifti.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/errors.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/errors.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/ge_3d_pcasl.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/ge_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/ge_easl.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/ge_easl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/noASL_MRI.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/noASL_MRI.py`

 * *Files 15% similar despite different names*

```diff
@@ -114,85 +114,120 @@
         self.series_list = self.DWI_list + self.ADC_list
 
     def validate_series(self):
         if len(self.DWI_list) < 1:
             raise MissingSequenceError('DWI')
         elif len(self.DWI_list) > 1:
             logger.warning(f'发现{len(self.DWI_list)}组DWI数据')
-        self.DWI = self.DWI_list[0]
 
+        # 判断DWI序列的多B值是否同属于一个序列
+        self.is_find_multi_volume = False
+        for dwi in self.DWI_list:
+            if dwi.Repetition > 1:
+                self.DWI = dwi
+                self.is_find_multi_volume = True
+                break
+
+        # 多B值不在同一个序列，必须要求DWI_list大于1
+        if (not self.is_find_multi_volume):
+            if len(self.DWI_list) < 2:
+                raise Exception('需要给出2个不同B值的DWI序列') # todo 定义一个错误
+            else:
+                first_dwi = self.DWI_list[0]
+                second_dwi = self.DWI_list[1]
+                self.DWI = first_dwi
+                if first_dwi.SliceNumber != second_dwi.SliceNumber:
+                    raise Exception('DWI序列空间不一致')  # todo 定义一个错误
+
+
+        # ADC序列验证，允许不存在。
         if len(self.ADC_list) < 1:
-            logger.warning(f'未发现ADC序列')
-            self.ADC: SeriesModel = None
-            # raise MissingSequenceError('ADC')
+            logger.info(f'未发现ADC序列')
+            self.ADC = None
         else:
-            logger.warning(f'发现{len(self.DWI_list)}组ADC数据')
+            logger.debug(f'发现{len(self.DWI_list)}组ADC数据')
             self.ADC = self.ADC_list[0]
 
         if self.ADC is not None and self.DWI.SliceNumber != self.ADC.SliceNumber:
             raise SpaceIsDifferentError('DWI', 'ADC')
-        if self.ADC is not None and (self.DWI.Repetition != 2 or self.ADC.Repetition != 1):
-            raise SliceLessError(self.ADC.SliceNumber)
 
-    def Sorter(self):
-        super(DataSorterDWI, self).Sorter()
-        self.validate_series()
 
-        # DWI需要包含B0与B1000
-        # 标准dicom中的B值(弥散系数)标签信息
-        second_slice_number = 1 if self.DWI.is_second_arrangement_mode else self.DWI.SliceNumber
+    @staticmethod
+    def get_tag(dcm_obj: Union[DicomRequiredTags, pydicom.Dataset], key, default=None):
+        if isinstance(dcm_obj, DicomRequiredTags):
+            return dcm_obj.get_tag(key, default=default)
+        else:
+            return DicomRequiredTags.get_key(key, dcm_obj, default)
 
-        def get_tag(dcm_obj: Union[DicomRequiredTags, pydicom.Dataset], key, default=None):
-            if isinstance(dcm_obj, DicomRequiredTags):
-                return dcm_obj.get_tag(key, default=default)
+    def find_two_instance(self):
+        # 多B值不在同一个序列, 找到第二个Volume的位置
+        if self.is_find_multi_volume:
+            second_slice_number = 1 if self.DWI.is_second_arrangement_mode else self.DWI.SliceNumber
+            # 3D dicom的B值在PerFrameFunctionalGroupsSequence中
+            if self.DWI.dicom_image_type == DICOM_IMAGE_TYPE.DICOM_IMAGE_TYPE_3D:
+                first_instance = self.get_tag(self.DWI.PerFrameFunctionalGroupsSequence[0], (0x0018, 0x9117))[0]
+                second_instance = \
+                    self.get_tag(self.DWI.PerFrameFunctionalGroupsSequence[second_slice_number], (0x0018, 0x9117))[0]
             else:
-                return DicomRequiredTags.get_key(key, dcm_obj, default)
+                first_instance = self.DWI[0]
+                second_instance = self.DWI[second_slice_number]
 
-        # 3D dicom的B值在PerFrameFunctionalGroupsSequence中
-        if self.DWI.dicom_image_type == DICOM_IMAGE_TYPE.DICOM_IMAGE_TYPE_3D:
-            first_instance = get_tag(self.DWI.PerFrameFunctionalGroupsSequence[0], (0x0018, 0x9117))[0]
-            second_instance = get_tag(self.DWI.PerFrameFunctionalGroupsSequence[second_slice_number], (0x0018, 0x9117))[0]
+            DWI_image = self.DWI.load()
+            return (first_instance, DWI_image[...,0]), (second_instance, DWI_image[...,1])
         else:
-            first_instance = self.DWI[0]
-            second_instance = self.DWI[second_slice_number]
+            first_dwi = self.DWI_list[0]
+            second_dwi = self.DWI_list[1]
+            if first_dwi.dicom_image_type == DICOM_IMAGE_TYPE.DICOM_IMAGE_TYPE_3D:
+                first_instance = self.get_tag(first_dwi.PerFrameFunctionalGroupsSequence[0], (0x0018, 0x9117))[0]
+                second_instance = \
+                    self.get_tag(second_dwi.PerFrameFunctionalGroupsSequence[0], (0x0018, 0x9117))[0]
+            else:
+                first_instance = first_dwi[0]
+                second_instance = second_dwi[0]
+            return (first_instance, first_dwi.load()), (second_instance, second_dwi.load())
+
+    def Sorter(self):
+        super(DataSorterDWI, self).Sorter()
+        self.validate_series()
+        (first_instance, first_volume), (second_instance, second_volume) = self.find_two_instance()
 
-        first_b_value = get_tag(first_instance, (0x0018, 0x9087), 0)
-        second_b_value = get_tag(second_instance, (0x0018, 0x9087), 0)
+        # DWI需要包含B0与B1000
+        # 标准dicom中的B值(弥散系数)标签信息
+        first_b_value = self.get_tag(first_instance, (0x0018, 0x9087), 0)
+        second_b_value = self.get_tag(second_instance, (0x0018, 0x9087), 0)
         if self.DWI.Manufacturer == MANUFACTURER.kMANUFACTURER_GE:
             first_b_value = first_b_value if first_b_value != 0 else \
-                get_tag(first_instance, (0x0043, 0x1039), [0])[0]
+                self.get_tag(first_instance, (0x0043, 0x1039), [0])[0]
             second_b_value = second_b_value if second_b_value != 0 else \
-                get_tag(second_instance, (0x0043, 0x1039), [0])[0]
+                self.get_tag(second_instance, (0x0043, 0x1039), [0])[0]
 
         elif self.DWI.Manufacturer == MANUFACTURER.kMANUFACTURER_SIEMENS:
             first_b_value = first_b_value if first_b_value != 0 else \
-                get_tag(first_instance, (0x0019, 0x100C), 0)
+                self.get_tag(first_instance, (0x0019, 0x100C), 0)
             second_b_value = second_b_value if second_b_value != 0 else \
-                get_tag(second_instance, (0x0019, 0x100C), 0)
+                self.get_tag(second_instance, (0x0019, 0x100C), 0)
 
-        elif self.DWI.Manufacturer == MANUFACTURER.kMANUFACTURER_PHILIPS:
+        elif self.DWI.Manufacturer in [MANUFACTURER.kMANUFACTURER_PHILIPS, MANUFACTURER.kMANUFACTURER_UIH]:
             pass
-            # first_b_value = self.DWI[0].get_tag((0x0018, 0x9087), 0)
-            # second_b_value = self.DWI[self.DWI.SliceNumber].get_tag((0x0018, 0x9087), 0)
 
         else:
             raise UnSupportDataTypeError(self.DWI.Manufacturer)
 
         first_b_value = int(first_b_value)
         second_b_value = int(second_b_value)
+        logger.info(f'DWI使用的两个B值：{first_b_value}, {second_b_value}')
         if first_b_value == 0 and second_b_value == 0:
             raise DiffusionBValueMissingError()
 
-        DWI_img = self.DWI.load()
         cur_series_number = SeriesNumberStartWith.DWI
 
-        write_dicom_series(DWI_img[...,0], self.DWI, f'dwi-b{first_b_value}', cur_series_number,
+        write_dicom_series(first_volume, self.DWI, f'dwi-b{first_b_value}', cur_series_number,
                            os.path.join(self.output_root, 'dwi', f'b{first_b_value}'))
         cur_series_number += 1
-        write_dicom_series(DWI_img[...,1], self.DWI, f'dwi-b{second_b_value}', cur_series_number,
+        write_dicom_series(second_volume, self.DWI, f'dwi-b{second_b_value}', cur_series_number,
                                os.path.join(self.output_root, 'dwi', f'b{second_b_value}'))
 
         cur_series_number += 1
         rescale_type = '10^-6 mm^2/s'
         if self.ADC is not None:
             # ADC， 确定单位
             rescale_type_1 = self.ADC.get_tag((0x0028, 0x1054), '')
@@ -206,18 +241,18 @@
             ADC_img = self.ADC.load(rescale)[...,0]
             write_dicom_series(ADC_img, self.DWI, 'dwi-adc', cur_series_number,
                                os.path.join(self.output_root, 'dwi', 'adc'))
 
         else:
             logger.debug(f'开始计算ADC')
             # 使second_b_value等于较大B值的那个图像
-            first_b0_idx, second_b1_idx = 0, 1
             if first_b_value > second_b_value:
                 first_b_value, second_b_value = second_b_value, first_b_value
-                first_b0_idx, second_b1_idx = second_b1_idx, first_b0_idx
-            ADC_img = np.log(DWI_img[...,first_b0_idx] / DWI_img[...,second_b1_idx]) / (second_b_value - first_b_value)
+                first_volume, second_volume = second_volume, first_volume
+            ADC_img = np.log(first_volume / second_volume) / (second_b_value - first_b_value)
+            # ADC_img = -1000 * np.log(np.divide(second_volume, first_volume))
             ADC_img[np.isinf(ADC_img) | np.isnan(ADC_img)] = 0
             ADC_img *= 10**6
             ADC_img[ADC_img < 0] = -256
 
             write_dicom_series(ADC_img, self.DWI, 'dwi-adc', cur_series_number,
                                os.path.join(self.output_root, 'dwi', 'adc'))
```

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/philips_3d_pcasl.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/philips_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pasl.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pcasl.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pcasl_old.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pcasl_old.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.2/data_sorter/restructure/uih_3d_pasl.py` & `animage-data_sorter-1.1.3/data_sorter/restructure/uih_3d_pasl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 from ._dicom import *
-from ._dicom_util import write_dicom_series
+from ._dicom_util import write_dicom_series, convert
 from .data_sorter_base import DataSorterASLBase
 
 
 class DataSorterUIHPASL(DataSorterASLBase):
     def __init__(self, data_type, output_root, delay_time, delay_rep, label_dur, series_list, extra_factor, calc_c_cbf):
         DataSorterASLBase.__init__(self, data_type, output_root, delay_time, delay_rep, label_dur, series_list, calc_c_cbf)
         if extra_factor is None or extra_factor == 0:
             logger.debug('extra_factor 未设置')
             # raise Exception('extra_factor 未设置')
         else:
             self.extra_factor = 32 / extra_factor
-        self.M0 = None
-        self.CBF = None # CBF参数图
-        self.Control = None
-        self.Label = None
+        self.M0 = []
+        self.CBF = [] # CBF参数图
+        self.Control = []
+        self.Label = []
 
         self.M0_count = 0
         self.CBF_count = 0
         # 区别M0与灌注图
         for series in self.series_list:
             if not isinstance(series, SeriesModel):
                 continue
             seriesDescription = series.SeriesDescription.lower().replace('-', ' ')
             if seriesDescription.find('m0') > -1:
                 self.M0_count += 1
-                self.M0 = series
+                self.M0.append(series)
             elif seriesDescription.find('cbf') > -1:
                 self.CBF_count += 1
-                self.CBF = series
+                self.CBF.append(series)
             elif seriesDescription.find('ctrl') > -1:
-                self.Control = series
+                self.Control.append(series)
             elif seriesDescription.find('tag') > -1:
-                self.Label = series
+                self.Label.append(series)
 
     def validate_series(self):
-        if self.M0 is None:
+        if len(self.M0) == 0:
             raise MissingSequenceError('M0')
-        if self.CBF is None:
+        if len(self.CBF) == 0:
             raise MissingSequenceError('CBF')
 
-        if self.M0_count > 1:
-            raise SeriesTooMany(f'发现{self.M0_count}组M0图像，请保留一组再进行处理')
-        if self.CBF_count > 1:
-            raise SeriesTooMany(f'发现{self.CBF_count}组CBF图像，请保留一组再进行处理')
+        # if self.M0_count > 1:
+        #     raise SeriesTooMany(f'发现{self.M0_count}组M0图像，请保留一组再进行处理')
+        # if self.CBF_count > 1:
+        #     raise SeriesTooMany(f'发现{self.CBF_count}组CBF图像，请保留一组再进行处理')
 
     def Sorter(self):
         super(DataSorterUIHPASL, self).Sorter()
 
         self.validate_series()
 
         # self.generate_calc_cbf_3d_pasl()
         self.generate_cbf_3d_pasl()
 
     def generate_cbf_3d_pasl(self):
-        self.M0: SeriesModel
+        self.M0: SeriesModel = self.M0[0]
         m0_image = self.M0.load()
         # 多张M0只有第一张有效
         m0_image = m0_image[...,0]
-        write_dicom_series(m0_image, self.M0, 'asl-m0', 1001, os.path.join(self.output_root, 'asl', 'm0'))
+        m0_nii = write_dicom_series(m0_image, self.M0, 'asl-m0', 1001, os.path.join(self.output_root, 'asl', 'm0'))
+
+        for i, cbf in enumerate(self.CBF):
+            cbf_image = cbf.load()[...,0]
+            cbf_nii = write_dicom_series(cbf_image * 10, cbf, f'asl-cbf{i+1}', 1002 + i,
+                               os.path.join(self.output_root, 'asl', f'cbf{i+1}'), slope=0.1)
+
+            convert(cbf_nii, cbf_nii, m0_nii)
+
+        super().calc_correct_CBF(np.concatenate([i.load() for i in self.CBF], axis=3), self.CBF[0], 1002+len(self.CBF))
+
 
-        self.CBF: SeriesModel
-        cbf_image = self.CBF.load()
-        cbf_image = cbf_image[...,0]
-        # todo M0与CBF分辨率不一致时
-        # if cbf_image.shape != m0_image.shape:
-        #     raise SpaceIsDifferentError('CBF', 'M0')
-        write_dicom_series(cbf_image * 10, self.CBF, 'asl-cbf1', 1002, os.path.join(self.output_root, 'asl', 'cbf1'),
-                           slope=0.1)
 
     def generate_calc_cbf_3d_pasl(self):
         self.M0: SeriesModel
         m0_image = self.M0.load()
         # 多张M0只有第一张有效
         m0_image = m0_image[:,:,:,0]
         write_dicom_series(m0_image, self.M0, 'asl-m0', 1001, os.path.join(self.output_root, 'asl', 'm0'))
```

### Comparing `animage-data_sorter-1.1.2/setup.py` & `animage-data_sorter-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="animage-data_sorter",
-  version="1.1.2",
+  version="1.1.3",
   author="zhaomy",
   author_email="zhaomy@an-image.cn",
   description="dicom sort",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://gitee.com/AnImage-Beijing/data_sorter",
   packages=setuptools.find_packages(),
```

