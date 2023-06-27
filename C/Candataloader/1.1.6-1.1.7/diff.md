# Comparing `tmp/Candataloader-1.1.6.tar.gz` & `tmp/Candataloader-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Candataloader-1.1.6.tar", last modified: Fri Jun 23 09:07:36 2023, max compression
+gzip compressed data, was "dist/Candataloader-1.1.7.tar", last modified: Tue Jun 27 10:17:49 2023, max compression
```

## Comparing `Candataloader-1.1.6.tar` & `Candataloader-1.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-23 09:07:36.000000 Candataloader-1.1.6/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1729 2023-05-25 12:52:06.000000 Candataloader-1.1.6/README.md
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.1.6/Candataloader/__init__.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     2007 2023-06-23 09:02:35.000000 Candataloader-1.1.6/Candataloader/download.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-06-23 09:07:36.000000 Candataloader-1.1.6/setup.cfg
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/dependency_links.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      218 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/SOURCES.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       23 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/top_level.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/PKG-INFO
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      299 2023-06-23 09:07:10.000000 Candataloader-1.1.6/setup.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-06-23 09:07:36.000000 Candataloader-1.1.6/PKG-INFO
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-27 10:17:49.000000 Candataloader-1.1.7/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1729 2023-05-25 12:52:06.000000 Candataloader-1.1.7/README.md
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-27 10:17:49.000000 Candataloader-1.1.7/Candataloader/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.1.7/Candataloader/__init__.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     2007 2023-06-27 10:16:07.000000 Candataloader-1.1.7/Candataloader/download.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-06-27 10:17:49.000000 Candataloader-1.1.7/setup.cfg
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-27 10:17:49.000000 Candataloader-1.1.7/Candataloader.egg-info/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-06-27 10:17:49.000000 Candataloader-1.1.7/Candataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      218 2023-06-27 10:17:49.000000 Candataloader-1.1.7/Candataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       23 2023-06-27 10:17:49.000000 Candataloader-1.1.7/Candataloader.egg-info/top_level.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-06-27 10:17:49.000000 Candataloader-1.1.7/Candataloader.egg-info/PKG-INFO
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      299 2023-06-27 10:16:33.000000 Candataloader-1.1.7/setup.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-06-27 10:17:49.000000 Candataloader-1.1.7/PKG-INFO
```

### Comparing `Candataloader-1.1.6/README.md` & `Candataloader-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `Candataloader-1.1.6/Candataloader/download.py` & `Candataloader-1.1.7/Candataloader/download.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import requests
 
 dataset_mapping = {
-        'Survival': 'https://3e05-203-205-29-5.ngrok-free.app/Survival Analysis Dataset for automobile IDS.csv',
-        'SynCAN': 'https://3e05-203-205-29-5.ngrok-free.app/SynCAN.csv',
-        'ROAD': 'https://3e05-203-205-29-5.ngrok-free.app/ROAD.csv',
-        'Car Hacking': 'https://3e05-203-205-29-5.ngrok-free.app/Car Hacking.csv',
-        'OTIDS': 'https://3e05-203-205-29-5.ngrok-free.app/OTIDS.csv',
-        'Automotive': 'https://3e05-203-205-29-5.ngrok-free.app/autoCAN_Prototype.csv',
+        'Survival': 'https://3670-203-205-29-5.ngrok-free.app/Survival Analysis Dataset for automobile IDS.csv',
+        'SynCAN': 'https://3670-203-205-29-5.ngrok-free.app/SynCAN.csv',
+        'ROAD': 'https://3670-203-205-29-5.ngrok-free.app/ROAD.csv',
+        'Car Hacking': 'https://3670-203-205-29-5.ngrok-free.app/Car Hacking.csv',
+        'OTIDS': 'https://3670-203-205-29-5.ngrok-free.app/OTIDS.csv',
+        'Automotive': 'https://3670-203-205-29-5.ngrok-free.app/autoCAN_Prototype.csv',
     }
 
 def list_datasets():
     datasets = list(dataset_mapping.keys())
     print("Available datasets:")
     for dataset in datasets:
         print(dataset)
```

