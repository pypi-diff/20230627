# Comparing `tmp/lightcon-1.4.1.tar.gz` & `tmp/lightcon-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcon-1.4.1.tar", last modified: Fri Jun 23 12:49:59 2023, max compression
+gzip compressed data, was "lightcon-1.4.2.tar", last modified: Tue Jun 27 11:40:38 2023, max compression
```

## Comparing `lightcon-1.4.1.tar` & `lightcon-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/
--rw-rw-rw-   0        0        0     1082 2023-06-23 12:47:15.000000 lightcon-1.4.1/LICENCE
--rw-rw-rw-   0        0        0      249 2023-06-23 12:47:15.000000 lightcon-1.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6252 2023-06-23 12:49:59.820604 lightcon-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5605 2023-06-23 12:47:15.000000 lightcon-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/lightcon/
--rw-rw-rw-   0        0        0        0 2023-06-23 12:47:15.000000 lightcon-1.4.1/lightcon/__config__.py
--rw-rw-rw-   0        0        0      715 2023-06-23 12:47:15.000000 lightcon-1.4.1/lightcon/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-23 12:47:15.000000 lightcon-1.4.1/lightcon/_globals.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/lightcon/datasets/
-drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/lightcon/datasets/data/
--rw-rw-rw-   0        0        0    11967 2023-06-23 12:49:16.000000 lightcon-1.4.1/lightcon/datasets/data/motor_parameters.json
--rw-rw-rw-   0        0        0     3335 2023-06-23 12:49:16.000000 lightcon-1.4.1/lightcon/datasets/data/stage_parameters.json
-drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/lightcon.egg-info/
--rw-rw-rw-   0        0        0     6252 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 12:49:59.820604 lightcon-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1744 2023-06-23 12:47:15.000000 lightcon-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-27 11:38:49.000000 lightcon-1.4.2/LICENCE
+-rw-rw-rw-   0        0        0      249 2023-06-27 11:38:49.000000 lightcon-1.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6252 2023-06-27 11:40:38.856850 lightcon-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5605 2023-06-27 11:38:49.000000 lightcon-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/lightcon/
+-rw-rw-rw-   0        0        0        0 2023-06-27 11:38:49.000000 lightcon-1.4.2/lightcon/__config__.py
+-rw-rw-rw-   0        0        0      715 2023-06-27 11:38:49.000000 lightcon-1.4.2/lightcon/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 11:38:49.000000 lightcon-1.4.2/lightcon/_globals.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/lightcon/datasets/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/lightcon/datasets/data/
+-rw-rw-rw-   0        0        0    11968 2023-06-27 11:39:53.000000 lightcon-1.4.2/lightcon/datasets/data/motor_parameters.json
+-rw-rw-rw-   0        0        0     4990 2023-06-27 11:39:53.000000 lightcon-1.4.2/lightcon/datasets/data/stage_parameters.json
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/lightcon.egg-info/
+-rw-rw-rw-   0        0        0     6252 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 11:40:38.856850 lightcon-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1744 2023-06-27 11:38:49.000000 lightcon-1.4.2/setup.py
```

### Comparing `lightcon-1.4.1/LICENCE` & `lightcon-1.4.2/LICENCE`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.1/PKG-INFO` & `lightcon-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.4.1
+Version: 1.4.2
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.4.1/README.md` & `lightcon-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.1/lightcon/__init__.py` & `lightcon-1.4.2/lightcon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 from . import wintopas
 from . import timing_controller
 from . import style
 from . import laser_clients
 from . import harpia
 from . import harpia_daq
```

### Comparing `lightcon-1.4.1/lightcon/datasets/data/motor_parameters.json` & `lightcon-1.4.2/lightcon/datasets/data/motor_parameters.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'Info'": "{'Date': '2023-06-26T11:42:22.3986928+00:00'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "Info": {
-        "Date": "2023-06-23T08:06:48.911324+00:00",
+        "Date": "2023-06-26T11:42:22.3986928+00:00",
         "MD5": "AA95745FAC085A5DD18092740CAF4427"
     },
     "Values": {
         "8HS11-0204S": {
             "Acc": 170,
             "AlarmEn": 255,
             "Config": 11909,
```

### Comparing `lightcon-1.4.1/lightcon/datasets/data/stage_parameters.json` & `lightcon-1.4.2/lightcon/datasets/data/stage_parameters.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {"'Info'": "{'Date': '2023-06-26T11:42:22.6223486+00:00', 'MD5': "*

 * *           "'78B9F3DD1D86D3A8C954E7488784CDB9'}",*

 * * "'Values'": "{'Light Conversion TA-HA-H1-H2': OrderedDict([('AlarmEn', 255), ('Config', 11909), "*

 * *             "('FnSlpAcc', 26), ('FnSlpDec', 26), ('FsSpeed', 1023), ('IntSpeed', 16383), "*

 * *             "('KTherm', 0), ('KvalAcc', 20), ('KvalDec', 20), ('KvalHold', 5), ('KvalRun', 20), "*

 * *             "('MinSpeed', 4305), ('OcdTh', 8), ('StSlp', 17), ('StallTh', 25), ('StageName', "*

 * *          […]*

```diff
@@ -1,11 +1,11 @@
 {
     "Info": {
-        "Date": "2023-06-23T08:06:49.4903741+00:00",
-        "MD5": "EF3B2C995CF9AEF5D11F7A2A93D61FA6"
+        "Date": "2023-06-26T11:42:22.6223486+00:00",
+        "MD5": "78B9F3DD1D86D3A8C954E7488784CDB9"
     },
     "Values": {
         "Light Conversion 987-70A": {
             "Acc": 171,
             "AlarmEn": 255,
             "Config": 11909,
             "Dec": 171,
@@ -29,14 +29,72 @@
             "ReductionCoefficient": 1.0,
             "StSlp": 4,
             "StageName": "Light Conversion 987-70A",
             "StallTh": 28,
             "StepMode": 6,
             "TravelLength": 5800
         },
+        "Light Conversion TA-HA-H1-H2": {
+            "Acc": 137,
+            "AlarmEn": 255,
+            "Config": 11909,
+            "Dec": 103,
+            "Description": "SHG unit for HARPIA-TA",
+            "FnSlpAcc": 26,
+            "FnSlpDec": 26,
+            "FsSpeed": 1023,
+            "IntSpeed": 16383,
+            "KTherm": 0,
+            "KvalAcc": 20,
+            "KvalDec": 20,
+            "KvalHold": 5,
+            "KvalRun": 20,
+            "LsEnable": 0,
+            "LsInvert": 0,
+            "LsSwap": 0,
+            "MaxSpeed": 65,
+            "MinSpeed": 4305,
+            "MotorName": "Sanyo Denki SH2281-5671",
+            "OcdTh": 8,
+            "ReductionCoefficient": 90.0,
+            "StSlp": 17,
+            "StageName": "Light Conversion TA-HA-H1-H2",
+            "StallTh": 25,
+            "StepMode": 6,
+            "TravelLength": 0
+        },
+        "Light Conversion TA-HA-STIRRER": {
+            "Acc": 343,
+            "AlarmEn": 255,
+            "Config": 11909,
+            "Dec": 343,
+            "Description": "Magnetic sample stirrer",
+            "FnSlpAcc": 10,
+            "FnSlpDec": 10,
+            "FsSpeed": 1023,
+            "IntSpeed": 16383,
+            "KTherm": 0,
+            "KvalAcc": 97,
+            "KvalDec": 97,
+            "KvalHold": 30,
+            "KvalRun": 97,
+            "LsEnable": 0,
+            "LsInvert": 0,
+            "LsSwap": 0,
+            "MaxSpeed": 163,
+            "MinSpeed": 4305,
+            "MotorName": "Sanyo Denki SH2141-5541",
+            "OcdTh": 8,
+            "ReductionCoefficient": 1.0,
+            "StSlp": 2,
+            "StageName": "Light Conversion TA-HA-STIRRER",
+            "StallTh": 19,
+            "StepMode": 6,
+            "TravelLength": 0
+        },
         "Light Conversion TA-RS-0370": {
             "Acc": 343,
             "AlarmEn": 255,
             "Config": 11909,
             "Dec": 343,
             "Description": "Glan-Taylor rotator for HARPIA-TF-KERR",
             "FnSlpAcc": 29,
```

### Comparing `lightcon-1.4.1/lightcon.egg-info/PKG-INFO` & `lightcon-1.4.2/lightcon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.4.1
+Version: 1.4.2
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.4.1/setup.py` & `lightcon-1.4.2/setup.py`

 * *Files identical despite different names*

