# Comparing `tmp/labelprinterkit-0.5.6.tar.gz` & `tmp/labelprinterkit-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelprinterkit-0.5.6.tar", max compression
+gzip compressed data, was "labelprinterkit-0.5.7.tar", max compression
```

## Comparing `labelprinterkit-0.5.6.tar` & `labelprinterkit-0.5.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.6/LICENSE
--rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.6/README.md
--rw-r--r--   0        0        0      152 2023-06-27 15:15:38.729521 labelprinterkit-0.5.6/labelprinterkit/__init__.py
--rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.6/labelprinterkit/backends/__init__.py
--rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.6/labelprinterkit/backends/bluetooth.py
--rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.6/labelprinterkit/backends/network.py
--rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.6/labelprinterkit/backends/usb.py
--rw-r--r--   0        0        0     2452 2023-06-27 15:15:38.730521 labelprinterkit-0.5.6/labelprinterkit/constants.py
--rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.6/labelprinterkit/job.py
--rw-r--r--   0        0        0     6564 2023-06-27 12:55:38.912547 labelprinterkit-0.5.6/labelprinterkit/label.py
--rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.6/labelprinterkit/page.py
--rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.6/labelprinterkit/printers.py
--rw-r--r--   0        0        0      690 2023-06-27 15:15:38.730521 labelprinterkit-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 labelprinterkit-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.7/LICENSE
+-rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.7/README.md
+-rw-r--r--   0        0        0      152 2023-06-27 15:15:38.729521 labelprinterkit-0.5.7/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.7/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.7/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.7/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.7/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-27 15:15:38.730521 labelprinterkit-0.5.7/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.7/labelprinterkit/job.py
+-rw-r--r--   0        0        0     7007 2023-06-27 15:51:45.035414 labelprinterkit-0.5.7/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.7/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.7/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      690 2023-06-27 15:51:45.035414 labelprinterkit-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 labelprinterkit-0.5.7/PKG-INFO
```

### Comparing `labelprinterkit-0.5.6/LICENSE` & `labelprinterkit-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/README.md` & `labelprinterkit-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/labelprinterkit/backends/bluetooth.py` & `labelprinterkit-0.5.7/labelprinterkit/backends/bluetooth.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/labelprinterkit/backends/network.py` & `labelprinterkit-0.5.7/labelprinterkit/backends/network.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/labelprinterkit/backends/usb.py` & `labelprinterkit-0.5.7/labelprinterkit/backends/usb.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/labelprinterkit/constants.py` & `labelprinterkit-0.5.7/labelprinterkit/constants.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/labelprinterkit/job.py` & `labelprinterkit-0.5.7/labelprinterkit/job.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/labelprinterkit/label.py` & `labelprinterkit-0.5.7/labelprinterkit/label.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,45 +105,54 @@
                 lower = test
             else:
                 return test
 
 
 class QrCode(Item):
     def __init__(self, width: int, data: str,
-                 error_correction: Optional[ERROR_CORRECT_M | ERROR_CORRECT_H | ERROR_CORRECT_Q] = ERROR_CORRECT_M,
+                 error_correction: Optional[ERROR_CORRECT_M | ERROR_CORRECT_H | ERROR_CORRECT_Q] = None,
                  box_size: int | None = None, border: int = 0):
         self._width = width
         self._data = data
         self._error_correction = error_correction
         self._box_size = box_size
         self._border = border
 
     def render(self) -> Image:
         if self._box_size is None:
             box_size = 2
         else:
             box_size = self._box_size
         probe_box_size = box_size
         qr_image = None
-        while True:
-            logger.debug(f"qrcode: {self._data}, probe_box_size: {probe_box_size}")
-            qr = _QRCode(error_correction=self._error_correction, box_size=probe_box_size, border=self._border)
-            qr.add_data(self._data)
-            new_image = qr.make_image()
-            if new_image.size[0] <= self._width:
-                qr_image = new_image
-                probe_box_size += 1
-            elif qr_image is None:
-                raise RuntimeError("Data does not fit in qrcode")
-            else:
-                break
-            if self._box_size is not None:
+        if self._error_correction is None:
+            error_corrections = [ERROR_CORRECT_Q, ERROR_CORRECT_H, ERROR_CORRECT_M, ERROR_CORRECT_L]
+        else:
+            error_corrections = [self._error_correction]
+        for error_correction in error_corrections:
+            while True:
+                logger.debug(f"qrcode: {self._data}, probe_box_size: {probe_box_size}, EC: {error_correction}")
+                qr = _QRCode(error_correction=error_correction, box_size=probe_box_size, border=self._border)
+                qr.add_data(self._data)
+                new_image = qr.make_image()
+                if new_image.size[0] <= self._width:
+                    qr_image = new_image
+                    probe_box_size += 1
+                elif qr_image is None:
+                    break
+                else:
+                    break
+                if self._box_size is not None:
+                    break
+            if qr_image:
                 break
+        if not qr_image:
+            raise RuntimeError("Data does not fit in qrcode")
 
-        logger.debug(f"qrcode: {self._data}, final box_size: {probe_box_size - 1}")
+        logger.debug(f"qrcode: {self._data}, final box_size: {probe_box_size - 1}, EC: {error_correction}")
 
         rest = self._width - qr_image.size[1]
         image = Image.new("1", (qr_image.size[0], self._width), "white")
         image.paste(qr_image, (0, rest // 2))
 
         return image
```

### Comparing `labelprinterkit-0.5.6/labelprinterkit/page.py` & `labelprinterkit-0.5.7/labelprinterkit/page.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/labelprinterkit/printers.py` & `labelprinterkit-0.5.7/labelprinterkit/printers.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.6/pyproject.toml` & `labelprinterkit-0.5.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labelprinterkit"
-version = "0.5.6"
+version = "0.5.7"
 description = "A library for creating and printing labels for Brother P-Touch devices"
 authors = ["Adrian Tschira <packages@notafile.com>", "Benedikt Neuffer <benedikt.neuffer@kit.edu>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `labelprinterkit-0.5.6/PKG-INFO` & `labelprinterkit-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelprinterkit
-Version: 0.5.6
+Version: 0.5.7
 Summary: A library for creating and printing labels for Brother P-Touch devices
 License: Apache License, Version 2.0
 Author: Adrian Tschira
 Author-email: packages@notafile.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

