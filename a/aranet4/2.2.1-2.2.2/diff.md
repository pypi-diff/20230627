# Comparing `tmp/aranet4-2.2.1.tar.gz` & `tmp/aranet4-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aranet4-2.2.1.tar", last modified: Tue Jun 27 05:09:49 2023, max compression
+gzip compressed data, was "dist/aranet4-2.2.2.tar", last modified: Tue Jun 27 06:23:34 2023, max compression
```

## Comparing `aranet4-2.2.1.tar` & `aranet4-2.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 05:09:49.000000 aranet4-2.2.1/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 05:09:49.000000 aranet4-2.2.1/aranet4.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2023-06-27 05:09:48.000000 aranet4-2.2.1/aranet4.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-27 05:09:48.000000 aranet4-2.2.1/aranet4.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     8239 2023-06-27 05:09:48.000000 aranet4-2.2.1/aranet4.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       61 2023-06-27 05:09:48.000000 aranet4-2.2.1/aranet4.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-06-27 05:09:48.000000 aranet4-2.2.1/aranet4.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      265 2023-06-27 05:09:48.000000 aranet4-2.2.1/aranet4.egg-info/SOURCES.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 05:09:49.000000 aranet4-2.2.1/aranet4/
--rw-r--r--   0 pi        (1000) pi        (1000)      129 2023-06-27 05:03:48.000000 aranet4-2.2.1/aranet4/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    27198 2023-06-27 05:02:15.000000 aranet4-2.2.1/aranet4/client.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9129 2023-06-21 19:45:41.000000 aranet4-2.2.1/aranet4/aranetctl.py
--rw-r--r--   0 pi        (1000) pi        (1000)      759 2023-06-27 05:03:53.000000 aranet4-2.2.1/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)     8239 2023-06-27 05:09:49.000000 aranet4-2.2.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-27 05:09:49.000000 aranet4-2.2.1/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-06-19 17:40:33.000000 aranet4-2.2.1/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 06:23:34.000000 aranet4-2.2.2/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 06:23:34.000000 aranet4-2.2.2/aranet4.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2023-06-27 06:23:33.000000 aranet4-2.2.2/aranet4.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-27 06:23:33.000000 aranet4-2.2.2/aranet4.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     8239 2023-06-27 06:23:33.000000 aranet4-2.2.2/aranet4.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)       61 2023-06-27 06:23:33.000000 aranet4-2.2.2/aranet4.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-06-27 06:23:33.000000 aranet4-2.2.2/aranet4.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      265 2023-06-27 06:23:33.000000 aranet4-2.2.2/aranet4.egg-info/SOURCES.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 06:23:34.000000 aranet4-2.2.2/aranet4/
+-rw-r--r--   0 pi        (1000) pi        (1000)      129 2023-06-27 06:22:51.000000 aranet4-2.2.2/aranet4/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    27525 2023-06-27 06:21:39.000000 aranet4-2.2.2/aranet4/client.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9129 2023-06-21 19:45:41.000000 aranet4-2.2.2/aranet4/aranetctl.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      759 2023-06-27 06:22:40.000000 aranet4-2.2.2/setup.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     8239 2023-06-27 06:23:34.000000 aranet4-2.2.2/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-27 06:23:34.000000 aranet4-2.2.2/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-06-19 17:40:33.000000 aranet4-2.2.2/README.md
```

### Comparing `aranet4-2.2.1/aranet4.egg-info/PKG-INFO` & `aranet4-2.2.2/aranet4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.2.1
+Version: 2.2.2
 Summary: Aranet4 and Aranet2 Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 License: UNKNOWN
 Description: # Aranet4 Python client
         ## Installation
         1. Install aranet4 and its dependencies:
         ```
```

### Comparing `aranet4-2.2.1/aranet4/client.py` & `aranet4-2.2.2/aranet4/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,16 +241,22 @@
             has_manufacurer_data = Aranet4.MANUFACTURER_ID in ad_data.manufacturer_data
 
             if has_manufacurer_data:
                 mf_data = ManufacturerData()
                 raw_bytes = ad_data.manufacturer_data[Aranet4.MANUFACTURER_ID]
 
                 # Basic info
-                value_fmt = "<BBBHB"
-                value = struct.unpack(value_fmt, raw_bytes[0:6])
+                value_fmt = "<BBBB"
+                b0 = 255
+                if device.name.startswith("Aranet2"):
+                    value = struct.unpack(value_fmt, raw_bytes[1:5])
+                    b0 = raw_bytes[1]
+                else:
+                    value = struct.unpack(value_fmt, raw_bytes[0:4])
+                    b0 = raw_bytes[0]
                 mf_data.decode(value)
                 self.manufacturer_data = mf_data
 
                 # Extended info / measurements
                 if len(raw_bytes) >= 24 and device.name.startswith("Aranet2"):
                     value_fmt = "<HHHHBBBHHB"
                     value = struct.unpack(value_fmt, raw_bytes[8:24])
@@ -259,14 +265,16 @@
                     self.readings.name = device.name
                 elif len(raw_bytes) >= 20:
                     value_fmt = "<HHHBBBHH"
                     value = struct.unpack(value_fmt, raw_bytes[8:21])
                     self.readings = CurrentReading()
                     self.readings.decode(value)
                     self.readings.name = device.name
+                else:
+                    mf_data.integrations = False
 
 
 @dataclass
 class RecordItem:
     """dataclass to store historical records"""
 
     date: datetime
@@ -537,30 +545,30 @@
             self.AR4_READ_HISTORY_READINGS_V1, delegate.handle_notification
         )
         while self.reading:
             await asyncio.sleep(0.1)
         await self.device.stop_notify(self.AR4_READ_HISTORY_READINGS_V1)
         return delegate.result
 
-    async def setReadingsInterval(self, interval: int):
+    async def set_readings_interval(self, interval: int):
         """Set reading interval"""
         header = 0x90
         val = struct.pack("<BB", header, interval)
         await self.device.write_gatt_char(self.AR4_WRITE_CMD, val, True)
 
-    async def setHomeIntegrationEnabled(self, enabled: bool):
+    async def set_home_integration_enabled(self, enabled: bool):
         """
         Toggle smart home integrations.
         This is required to receive measurements in advertisements.
         """
         header = 0x91
         val = struct.pack("<BB", header, 1 if enabled else 0)
         await self.device.write_gatt_char(self.AR4_WRITE_CMD, val, True)
 
-    async def setBluetoothRange(self, extended: bool):
+    async def set_bluetooth_range(self, extended: bool):
         """Set bluetooth range"""
         header = 0x91
         val = struct.pack("<BB", header, 1 if extended else 0)
         await self.device.write_gatt_char(self.AR4_WRITE_CMD, val, True)
 
 
 def _log_times(now, total, interval, ago):
```

### Comparing `aranet4-2.2.1/aranet4/aranetctl.py` & `aranet4-2.2.2/aranet4/aranetctl.py`

 * *Files identical despite different names*

### Comparing `aranet4-2.2.1/setup.py` & `aranet4-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aranet4",
-    version="2.2.1",
+    version="2.2.2",
     description="Aranet4 and Aranet2 Python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/Aranet4-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
```

### Comparing `aranet4-2.2.1/PKG-INFO` & `aranet4-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.2.1
+Version: 2.2.2
 Summary: Aranet4 and Aranet2 Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 License: UNKNOWN
 Description: # Aranet4 Python client
         ## Installation
         1. Install aranet4 and its dependencies:
         ```
```

### Comparing `aranet4-2.2.1/README.md` & `aranet4-2.2.2/README.md`

 * *Files identical despite different names*

