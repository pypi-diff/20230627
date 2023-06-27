# Comparing `tmp/labelprinterkit-0.5.5.tar.gz` & `tmp/labelprinterkit-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelprinterkit-0.5.5.tar", max compression
+gzip compressed data, was "labelprinterkit-0.5.6.tar", max compression
```

## Comparing `labelprinterkit-0.5.5.tar` & `labelprinterkit-0.5.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.5/LICENSE
--rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.5/README.md
--rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.5.5/labelprinterkit/__init__.py
--rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.5/labelprinterkit/backends/__init__.py
--rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.5/labelprinterkit/backends/bluetooth.py
--rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.5/labelprinterkit/backends/network.py
--rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.5/labelprinterkit/backends/usb.py
--rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.5.5/labelprinterkit/constants.py
--rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.5/labelprinterkit/job.py
--rw-r--r--   0        0        0     6564 2023-06-27 12:21:54.711106 labelprinterkit-0.5.5/labelprinterkit/label.py
--rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.5/labelprinterkit/page.py
--rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.5/labelprinterkit/printers.py
--rw-r--r--   0        0        0      667 2023-06-27 12:21:54.711106 labelprinterkit-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 labelprinterkit-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.6/LICENSE
+-rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.6/README.md
+-rw-r--r--   0        0        0      152 2023-06-27 15:15:38.729521 labelprinterkit-0.5.6/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.6/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.6/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.6/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.6/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-27 15:15:38.730521 labelprinterkit-0.5.6/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.6/labelprinterkit/job.py
+-rw-r--r--   0        0        0     6564 2023-06-27 12:55:38.912547 labelprinterkit-0.5.6/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.6/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.6/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      690 2023-06-27 15:15:38.730521 labelprinterkit-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 labelprinterkit-0.5.6/PKG-INFO
```

### Comparing `labelprinterkit-0.5.5/LICENSE` & `labelprinterkit-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/README.md` & `labelprinterkit-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/labelprinterkit/backends/bluetooth.py` & `labelprinterkit-0.5.6/labelprinterkit/backends/bluetooth.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/labelprinterkit/backends/network.py` & `labelprinterkit-0.5.6/labelprinterkit/backends/network.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/labelprinterkit/backends/usb.py` & `labelprinterkit-0.5.6/labelprinterkit/backends/usb.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/labelprinterkit/constants.py` & `labelprinterkit-0.5.6/labelprinterkit/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     lmargin: int | None
     printarea: int | None
     rmargin: int | None
 
 
 class MediaSize(Enum):
     NO_MEDIA = TapeInfo(0, 0, None, None, None)
-    W3_5 = TapeInfo(4, 0, 48, 32, 48)
+    W3_5 = TapeInfo(4, 0, 52, 24, 52)
     W6 = TapeInfo(6, 0, 48, 32, 48)
     W9 = TapeInfo(9, 0, 39, 50, 39)
     W12 = TapeInfo(12, 0, 29, 70, 29)
     W18 = TapeInfo(18, 0, 8, 112, 8)
     W24 = TapeInfo(24, 0, 0, 128, 0)
```

### Comparing `labelprinterkit-0.5.5/labelprinterkit/job.py` & `labelprinterkit-0.5.6/labelprinterkit/job.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/labelprinterkit/label.py` & `labelprinterkit-0.5.6/labelprinterkit/label.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/labelprinterkit/page.py` & `labelprinterkit-0.5.6/labelprinterkit/page.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/labelprinterkit/printers.py` & `labelprinterkit-0.5.6/labelprinterkit/printers.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.5/pyproject.toml` & `labelprinterkit-0.5.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "labelprinterkit"
-version = "0.5.5"
+version = "0.5.6"
 description = "A library for creating and printing labels for Brother P-Touch devices"
 authors = ["Adrian Tschira <packages@notafile.com>", "Benedikt Neuffer <benedikt.neuffer@kit.edu>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pillow = "^9.5.0"
 pyusb = "^1.2.1"
 packbits = "^0.6"
 pyserial = {version = "^3.5", optional = true}
 qrcode = {version = "^7.4.2", optional = true, extras = ["pil"]}
+setuptools = "^67.0.0"
 
 [tool.poetry.extras]
 bluetooth = ["pyserial"]
 qrcode = ["qrcode"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `labelprinterkit-0.5.5/PKG-INFO` & `labelprinterkit-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelprinterkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: A library for creating and printing labels for Brother P-Touch devices
 License: Apache License, Version 2.0
 Author: Adrian Tschira
 Author-email: packages@notafile.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Provides-Extra: bluetooth
 Provides-Extra: qrcode
 Requires-Dist: packbits (>=0.6,<0.7)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0) ; extra == "bluetooth"
 Requires-Dist: pyusb (>=1.2.1,<2.0.0)
 Requires-Dist: qrcode[pil] (>=7.4.2,<8.0.0) ; extra == "qrcode"
+Requires-Dist: setuptools (>=67.0.0,<68.0.0)
 Description-Content-Type: text/markdown
 
 ### Labelprinterkit
 
 Labelprinterkit is a Python3 library for creating and printing labels with
 Brother P-Touch devices. It was developed for the Networking department of
 KIT (Karlsruhe Institute of Technology).
```

