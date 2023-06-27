# Comparing `tmp/lns-icloudpy-0.0.2.tar.gz` & `tmp/lns-icloudpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lns-icloudpy-0.0.2.tar", last modified: Sun Feb 12 02:23:44 2023, max compression
+gzip compressed data, was "lns-icloudpy-0.0.3.tar", last modified: Tue Jun 27 06:55:15 2023, max compression
```

## Comparing `lns-icloudpy-0.0.2.tar` & `lns-icloudpy-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 02:23:44.712600 lns-icloudpy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-02-12 02:23:44.712600 lns-icloudpy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 02:23:44.708600 lns-icloudpy-0.0.2/icloudpy/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 02:23:44.708600 lns-icloudpy-0.0.2/icloudpy/services/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/findmyiphone.py
--rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/reminders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/services/ubiquity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/icloudpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 02:23:44.712600 lns-icloudpy-0.0.2/lns_icloudpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-02-12 02:23:44.000000 lns-icloudpy-0.0.2/lns_icloudpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-12 02:23:44.000000 lns-icloudpy-0.0.2/lns_icloudpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 02:23:44.000000 lns-icloudpy-0.0.2/lns_icloudpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-12 02:23:44.000000 lns-icloudpy-0.0.2/lns_icloudpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-12 02:23:44.000000 lns-icloudpy-0.0.2/lns_icloudpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-12 02:23:44.000000 lns-icloudpy-0.0.2/lns_icloudpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 02:23:44.712600 lns-icloudpy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-02-12 02:23:33.000000 lns-icloudpy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:55:15.447467 lns-icloudpy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-06-27 06:55:15.447467 lns-icloudpy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:55:15.443467 lns-icloudpy-0.0.3/icloudpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:55:15.447467 lns-icloudpy-0.0.3/icloudpy/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/findmyiphone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/reminders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/services/ubiquity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/icloudpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:55:15.447467 lns-icloudpy-0.0.3/lns_icloudpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-06-27 06:55:15.000000 lns-icloudpy-0.0.3/lns_icloudpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-27 06:55:15.000000 lns-icloudpy-0.0.3/lns_icloudpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:55:15.000000 lns-icloudpy-0.0.3/lns_icloudpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 06:55:15.000000 lns-icloudpy-0.0.3/lns_icloudpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 06:55:15.000000 lns-icloudpy-0.0.3/lns_icloudpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 06:55:15.000000 lns-icloudpy-0.0.3/lns_icloudpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 06:55:15.447467 lns-icloudpy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-27 06:55:04.000000 lns-icloudpy-0.0.3/setup.py
```

### Comparing `lns-icloudpy-0.0.2/LICENSE` & `lns-icloudpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/PKG-INFO` & `lns-icloudpy-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lns-icloudpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library to interact with iCloud web service
 Home-page: https://github.com/leafnsand/icloudpy
 Author: leafnsand
 Author-email: xavier.jiang@leafnsand.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lns-icloudpy Version: 0.0.2 Summary: Python library
+Metadata-Version: 2.1 Name: lns-icloudpy Version: 0.0.3 Summary: Python library
 to interact with iCloud web service Home-page: https://github.com/leafnsand/
 icloudpy Author: leafnsand Author-email: xavier.jiang@leafnsand.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE # iCloudPy [![CI - Main](https://github.com/mandarons/
 icloudpy/actions/workflows/ci-main-test-coverage.yml/badge.svg)](https://
 github.com/mandarons/icloudpy/actions/workflows/ci-main-test-coverage.yml) [!
```

### Comparing `lns-icloudpy-0.0.2/README.md` & `lns-icloudpy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/base.py` & `lns-icloudpy-0.0.3/icloudpy/base.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/cmdline.py` & `lns-icloudpy-0.0.3/icloudpy/cmdline.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/exceptions.py` & `lns-icloudpy-0.0.3/icloudpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/__init__.py` & `lns-icloudpy-0.0.3/icloudpy/services/__init__.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/account.py` & `lns-icloudpy-0.0.3/icloudpy/services/account.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/calendar.py` & `lns-icloudpy-0.0.3/icloudpy/services/calendar.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/contacts.py` & `lns-icloudpy-0.0.3/icloudpy/services/contacts.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/drive.py` & `lns-icloudpy-0.0.3/icloudpy/services/drive.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/findmyiphone.py` & `lns-icloudpy-0.0.3/icloudpy/services/findmyiphone.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/photos.py` & `lns-icloudpy-0.0.3/icloudpy/services/photos.py`

 * *Files 2% similar despite different names*

```diff
@@ -574,23 +574,29 @@
         self._service = service
         self._master_record = master_record
         self._asset_record = asset_record
 
         self._versions = None
 
     PHOTO_VERSION_LOOKUP = {
-        "original": "resOriginal",
+        "full": "resJPEGFull",
+        "large": "resJPEGLarge",
         "medium": "resJPEGMed",
         "thumb": "resJPEGThumb",
+        "sidecar": "resSidecar",
+        "original": "resOriginal",
+        "original_alt": "resOriginalAlt",
     }
 
     VIDEO_VERSION_LOOKUP = {
-        "original": "resOriginal",
+        "full": "resVidFull",
         "medium": "resVidMed",
         "thumb": "resVidSmall",
+        "original": "resOriginal",
+        "original_compl": "resOriginalVidCompl",
     }
 
     @property
     def id(self):
         """Gets the photo id."""
         return self._master_record["recordName"]
```

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/reminders.py` & `lns-icloudpy-0.0.3/icloudpy/services/reminders.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/services/ubiquity.py` & `lns-icloudpy-0.0.3/icloudpy/services/ubiquity.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/icloudpy/utils.py` & `lns-icloudpy-0.0.3/icloudpy/utils.py`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/lns_icloudpy.egg-info/PKG-INFO` & `lns-icloudpy-0.0.3/lns_icloudpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lns-icloudpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library to interact with iCloud web service
 Home-page: https://github.com/leafnsand/icloudpy
 Author: leafnsand
 Author-email: xavier.jiang@leafnsand.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lns-icloudpy Version: 0.0.2 Summary: Python library
+Metadata-Version: 2.1 Name: lns-icloudpy Version: 0.0.3 Summary: Python library
 to interact with iCloud web service Home-page: https://github.com/leafnsand/
 icloudpy Author: leafnsand Author-email: xavier.jiang@leafnsand.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE # iCloudPy [![CI - Main](https://github.com/mandarons/
 icloudpy/actions/workflows/ci-main-test-coverage.yml/badge.svg)](https://
 github.com/mandarons/icloudpy/actions/workflows/ci-main-test-coverage.yml) [!
```

### Comparing `lns-icloudpy-0.0.2/lns_icloudpy.egg-info/SOURCES.txt` & `lns-icloudpy-0.0.3/lns_icloudpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lns-icloudpy-0.0.2/setup.py` & `lns-icloudpy-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 
 from setuptools import find_packages, setup
 
 REPO_URL = "https://github.com/leafnsand/icloudpy"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 with open("README.md") as fh:
     long_description = fh.read()
 with open("requirements.txt") as fh:
     required = fh.read().splitlines()
 
 setup(
```

