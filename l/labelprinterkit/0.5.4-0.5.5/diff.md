# Comparing `tmp/labelprinterkit-0.5.4.tar.gz` & `tmp/labelprinterkit-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelprinterkit-0.5.4.tar", max compression
+gzip compressed data, was "labelprinterkit-0.5.5.tar", max compression
```

## Comparing `labelprinterkit-0.5.4.tar` & `labelprinterkit-0.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.4/LICENSE
--rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.4/README.md
--rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.5.4/labelprinterkit/__init__.py
--rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.4/labelprinterkit/backends/__init__.py
--rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.4/labelprinterkit/backends/bluetooth.py
--rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.4/labelprinterkit/backends/network.py
--rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.4/labelprinterkit/backends/usb.py
--rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.5.4/labelprinterkit/constants.py
--rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.4/labelprinterkit/job.py
--rw-r--r--   0        0        0     6450 2023-06-24 11:50:05.192647 labelprinterkit-0.5.4/labelprinterkit/label.py
--rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.4/labelprinterkit/page.py
--rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.4/labelprinterkit/printers.py
--rw-r--r--   0        0        0      667 2023-06-24 12:43:54.859120 labelprinterkit-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 labelprinterkit-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.5/README.md
+-rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.5.5/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.5/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.5/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.5/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.5/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.5.5/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.5/labelprinterkit/job.py
+-rw-r--r--   0        0        0     6564 2023-06-27 12:21:54.711106 labelprinterkit-0.5.5/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.5/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.5/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      667 2023-06-27 12:21:54.711106 labelprinterkit-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 labelprinterkit-0.5.5/PKG-INFO
```

### Comparing `labelprinterkit-0.5.4/LICENSE` & `labelprinterkit-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/README.md` & `labelprinterkit-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/labelprinterkit/backends/bluetooth.py` & `labelprinterkit-0.5.5/labelprinterkit/backends/bluetooth.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/labelprinterkit/backends/network.py` & `labelprinterkit-0.5.5/labelprinterkit/backends/network.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/labelprinterkit/backends/usb.py` & `labelprinterkit-0.5.5/labelprinterkit/backends/usb.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/labelprinterkit/constants.py` & `labelprinterkit-0.5.5/labelprinterkit/constants.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/labelprinterkit/job.py` & `labelprinterkit-0.5.5/labelprinterkit/job.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/labelprinterkit/label.py` & `labelprinterkit-0.5.5/labelprinterkit/label.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from abc import ABC, abstractmethod
 from logging import getLogger
 from math import ceil
-from typing import TypeVar, NamedTuple
+from typing import TypeVar, NamedTuple, Optional
 
 from PIL import Image, ImageChops, ImageDraw, ImageFont
 try:
-    import qrcode
+    from qrcode import QRCode as _QRCode
+    from qrcode.constants import ERROR_CORRECT_L, ERROR_CORRECT_M, ERROR_CORRECT_H, ERROR_CORRECT_Q
 except ImportError:
-    qrcode = None
+    _QRcode = None
+    ERROR_CORRECT_L = 1
+    ERROR_CORRECT_M = 0
+    ERROR_CORRECT_H = 2
+    ERROR_CORRECT_Q = 3
 
 from .constants import Resolution
 from .page import BasePage, image_to_bitmap
 
 logger = getLogger(__name__)
 
 
@@ -100,16 +105,15 @@
                 lower = test
             else:
                 return test
 
 
 class QrCode(Item):
     def __init__(self, width: int, data: str,
-                 error_correction: qrcode.constants.ERROR_CORRECT_L | qrcode.constants.ERROR_CORRECT_M |
-                 qrcode.constants.ERROR_CORRECT_H | qrcode.constants.ERROR_CORRECT_Q = qrcode.constants.ERROR_CORRECT_M,
+                 error_correction: Optional[ERROR_CORRECT_M | ERROR_CORRECT_H | ERROR_CORRECT_Q] = ERROR_CORRECT_M,
                  box_size: int | None = None, border: int = 0):
         self._width = width
         self._data = data
         self._error_correction = error_correction
         self._box_size = box_size
         self._border = border
 
@@ -118,15 +122,15 @@
             box_size = 2
         else:
             box_size = self._box_size
         probe_box_size = box_size
         qr_image = None
         while True:
             logger.debug(f"qrcode: {self._data}, probe_box_size: {probe_box_size}")
-            qr = qrcode.QRCode(error_correction=self._error_correction, box_size=probe_box_size, border=self._border)
+            qr = _QRCode(error_correction=self._error_correction, box_size=probe_box_size, border=self._border)
             qr.add_data(self._data)
             new_image = qr.make_image()
             if new_image.size[0] <= self._width:
                 qr_image = new_image
                 probe_box_size += 1
             elif qr_image is None:
                 raise RuntimeError("Data does not fit in qrcode")
```

### Comparing `labelprinterkit-0.5.4/labelprinterkit/page.py` & `labelprinterkit-0.5.5/labelprinterkit/page.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/labelprinterkit/printers.py` & `labelprinterkit-0.5.5/labelprinterkit/printers.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.4/pyproject.toml` & `labelprinterkit-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labelprinterkit"
-version = "0.5.4"
+version = "0.5.5"
 description = "A library for creating and printing labels for Brother P-Touch devices"
 authors = ["Adrian Tschira <packages@notafile.com>", "Benedikt Neuffer <benedikt.neuffer@kit.edu>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `labelprinterkit-0.5.4/PKG-INFO` & `labelprinterkit-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelprinterkit
-Version: 0.5.4
+Version: 0.5.5
 Summary: A library for creating and printing labels for Brother P-Touch devices
 License: Apache License, Version 2.0
 Author: Adrian Tschira
 Author-email: packages@notafile.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

