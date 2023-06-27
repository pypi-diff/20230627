# Comparing `tmp/labelprinterkit-0.5.7.tar.gz` & `tmp/labelprinterkit-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelprinterkit-0.5.7.tar", max compression
+gzip compressed data, was "labelprinterkit-0.5.8.tar", max compression
```

## Comparing `labelprinterkit-0.5.7.tar` & `labelprinterkit-0.5.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.7/LICENSE
--rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.7/README.md
--rw-r--r--   0        0        0      152 2023-06-27 15:15:38.729521 labelprinterkit-0.5.7/labelprinterkit/__init__.py
--rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.7/labelprinterkit/backends/__init__.py
--rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.7/labelprinterkit/backends/bluetooth.py
--rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.7/labelprinterkit/backends/network.py
--rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.7/labelprinterkit/backends/usb.py
--rw-r--r--   0        0        0     2452 2023-06-27 15:15:38.730521 labelprinterkit-0.5.7/labelprinterkit/constants.py
--rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.7/labelprinterkit/job.py
--rw-r--r--   0        0        0     7007 2023-06-27 15:51:45.035414 labelprinterkit-0.5.7/labelprinterkit/label.py
--rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.7/labelprinterkit/page.py
--rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.7/labelprinterkit/printers.py
--rw-r--r--   0        0        0      690 2023-06-27 15:51:45.035414 labelprinterkit-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 labelprinterkit-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.8/LICENSE
+-rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.8/README.md
+-rw-r--r--   0        0        0      152 2023-06-27 15:15:38.729521 labelprinterkit-0.5.8/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-27 16:05:21.969699 labelprinterkit-0.5.8/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.8/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.8/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.8/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-27 15:15:38.730521 labelprinterkit-0.5.8/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.8/labelprinterkit/job.py
+-rw-r--r--   0        0        0     7007 2023-06-27 19:07:39.583475 labelprinterkit-0.5.8/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.8/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.8/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      689 2023-06-27 19:07:39.584475 labelprinterkit-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3134 1970-01-01 00:00:00.000000 labelprinterkit-0.5.8/PKG-INFO
```

### Comparing `labelprinterkit-0.5.7/LICENSE` & `labelprinterkit-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/README.md` & `labelprinterkit-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/labelprinterkit/backends/bluetooth.py` & `labelprinterkit-0.5.8/labelprinterkit/backends/bluetooth.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/labelprinterkit/backends/network.py` & `labelprinterkit-0.5.8/labelprinterkit/backends/network.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/labelprinterkit/backends/usb.py` & `labelprinterkit-0.5.8/labelprinterkit/backends/usb.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/labelprinterkit/constants.py` & `labelprinterkit-0.5.8/labelprinterkit/constants.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/labelprinterkit/job.py` & `labelprinterkit-0.5.8/labelprinterkit/job.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/labelprinterkit/label.py` & `labelprinterkit-0.5.8/labelprinterkit/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from typing import TypeVar, NamedTuple, Optional
 
 from PIL import Image, ImageChops, ImageDraw, ImageFont
 try:
     from qrcode import QRCode as _QRCode
     from qrcode.constants import ERROR_CORRECT_L, ERROR_CORRECT_M, ERROR_CORRECT_H, ERROR_CORRECT_Q
 except ImportError:
-    _QRcode = None
+    _QRCode = None
     ERROR_CORRECT_L = 1
     ERROR_CORRECT_M = 0
-    ERROR_CORRECT_H = 2
     ERROR_CORRECT_Q = 3
+    ERROR_CORRECT_H = 2
 
 from .constants import Resolution
 from .page import BasePage, image_to_bitmap
 
 logger = getLogger(__name__)
 
 
@@ -121,15 +121,15 @@
         if self._box_size is None:
             box_size = 2
         else:
             box_size = self._box_size
         probe_box_size = box_size
         qr_image = None
         if self._error_correction is None:
-            error_corrections = [ERROR_CORRECT_Q, ERROR_CORRECT_H, ERROR_CORRECT_M, ERROR_CORRECT_L]
+            error_corrections = [ERROR_CORRECT_H, ERROR_CORRECT_Q, ERROR_CORRECT_M, ERROR_CORRECT_L]
         else:
             error_corrections = [self._error_correction]
         for error_correction in error_corrections:
             while True:
                 logger.debug(f"qrcode: {self._data}, probe_box_size: {probe_box_size}, EC: {error_correction}")
                 qr = _QRCode(error_correction=error_correction, box_size=probe_box_size, border=self._border)
                 qr.add_data(self._data)
```

### Comparing `labelprinterkit-0.5.7/labelprinterkit/page.py` & `labelprinterkit-0.5.8/labelprinterkit/page.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/labelprinterkit/printers.py` & `labelprinterkit-0.5.8/labelprinterkit/printers.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.7/pyproject.toml` & `labelprinterkit-0.5.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "labelprinterkit"
-version = "0.5.7"
+version = "0.5.8"
 description = "A library for creating and printing labels for Brother P-Touch devices"
 authors = ["Adrian Tschira <packages@notafile.com>", "Benedikt Neuffer <benedikt.neuffer@kit.edu>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pillow = "^9.5.0"
 pyusb = "^1.2.1"
 packbits = "^0.6"
 pyserial = {version = "^3.5", optional = true}
 qrcode = {version = "^7.4.2", optional = true, extras = ["pil"]}
-setuptools = "^67.0.0"
+setuptools = "^68.0.0"
 
 [tool.poetry.extras]
 bluetooth = ["pyserial"]
 qrcode = ["qrcode"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `labelprinterkit-0.5.7/PKG-INFO` & `labelprinterkit-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: labelprinterkit
-Version: 0.5.7
+Version: 0.5.8
 Summary: A library for creating and printing labels for Brother P-Touch devices
 License: Apache License, Version 2.0
 Author: Adrian Tschira
 Author-email: packages@notafile.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: bluetooth
 Provides-Extra: qrcode
 Requires-Dist: packbits (>=0.6,<0.7)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0) ; extra == "bluetooth"
 Requires-Dist: pyusb (>=1.2.1,<2.0.0)
 Requires-Dist: qrcode[pil] (>=7.4.2,<8.0.0) ; extra == "qrcode"
-Requires-Dist: setuptools (>=67.0.0,<68.0.0)
+Requires-Dist: setuptools (>=68.0.0,<69.0.0)
 Description-Content-Type: text/markdown
 
 ### Labelprinterkit
 
 Labelprinterkit is a Python3 library for creating and printing labels with
 Brother P-Touch devices. It was developed for the Networking department of
 KIT (Karlsruhe Institute of Technology).
```

