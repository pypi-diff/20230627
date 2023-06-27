# Comparing `tmp/okolab-0.2.0.tar.gz` & `tmp/okolab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okolab-0.2.0.tar", last modified: Thu Mar 23 11:16:46 2023, max compression
+gzip compressed data, was "okolab-0.2.1.tar", last modified: Tue Jun 27 16:04:09 2023, max compression
```

## Comparing `okolab-0.2.0.tar` & `okolab-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-03-23 11:16:46.509062 okolab-0.2.0/
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-03-23 11:16:46.508928 okolab-0.2.0/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-03-23 11:16:46.507917 okolab-0.2.0/okolab/
--rw-r--r--   0 simon      (501) staff       (20)       22 2022-10-20 10:18:45.000000 okolab-0.2.0/okolab/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2357 2023-03-23 11:12:58.000000 okolab-0.2.0/okolab/__main__.py
--rw-r--r--   0 simon      (501) staff       (20)     9740 2023-03-23 11:13:48.000000 okolab-0.2.0/okolab/device.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-03-23 11:16:46.508743 okolab-0.2.0/okolab.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-03-23 11:16:46.000000 okolab-0.2.0/okolab.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      228 2023-03-23 11:16:46.000000 okolab-0.2.0/okolab.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-03-23 11:16:46.000000 okolab-0.2.0/okolab.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       17 2023-03-23 11:16:46.000000 okolab-0.2.0/okolab.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        7 2023-03-23 11:16:46.000000 okolab-0.2.0/okolab.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)      486 2023-03-23 11:14:43.000000 okolab-0.2.0/pyproject.toml
--rw-r--r--   0 simon      (501) staff       (20)     1315 2023-03-22 14:54:19.000000 okolab-0.2.0/readme.md
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-03-23 11:16:46.509097 okolab-0.2.0/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:04:09.251904 okolab-0.2.1/
+-rw-r--r--   0 simon      (501) staff       (20)     1488 2023-06-27 16:04:09.251783 okolab-0.2.1/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:04:09.250751 okolab-0.2.1/okolab/
+-rw-r--r--   0 simon      (501) staff       (20)       22 2022-10-20 10:18:45.000000 okolab-0.2.1/okolab/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2023-05-19 14:46:50.000000 okolab-0.2.1/okolab/__main__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9267 2023-05-21 15:10:21.000000 okolab-0.2.1/okolab/device.py
+-rw-r--r--   0 simon      (501) staff       (20)      538 2023-05-19 15:33:04.000000 okolab-0.2.1/okolab/util.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:04:09.251599 okolab-0.2.1/okolab.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     1488 2023-06-27 16:04:09.000000 okolab-0.2.1/okolab.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      243 2023-06-27 16:04:09.000000 okolab-0.2.1/okolab.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-27 16:04:09.000000 okolab-0.2.1/okolab.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       17 2023-06-27 16:04:09.000000 okolab-0.2.1/okolab.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        7 2023-06-27 16:04:09.000000 okolab-0.2.1/okolab.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)      486 2023-06-27 16:03:13.000000 okolab-0.2.1/pyproject.toml
+-rw-r--r--   0 simon      (501) staff       (20)     1188 2023-05-19 14:46:50.000000 okolab-0.2.1/readme.md
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-27 16:04:09.251943 okolab-0.2.1/setup.cfg
```

### Comparing `okolab-0.2.0/PKG-INFO` & `okolab-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okolab
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package that provides control of the H401-T-CONTROLLER temperature controller from Okolab
 License: EUPL-1.2
 Project-URL: repository, https://github.com/slietar/okolab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Okolab
@@ -28,52 +28,42 @@
 from okolab import OkolabDevice
 
 device = OkolabDevice(address="COM3")
 device = OkolabDevice(address="/dev/tty.usbmodem1101")
 ```
 
 ```py
-def on_close(*, lost):
-  print(f"Connection closed, lost={lost}")
+async with device:
+  # Read temperature
+  temp = await device.get_temperature1()
+  temp = await device.get_temperature2()
 
-device = Device(address="COM3", on_close=on_close)
-```
+  # Write temperature
+  await device.set_temperature_setpoint1(37.0)
+  await device.set_temperature_setpoint2(37.0)
+  ```
 
-```py
-# Read temperature
-temp = await device.get_temperature1()
-temp = await device.get_temperature2()
-
-# Write temperature
-await device.set_temperature_setpoint1(37.0)
-await device.set_temperature_setpoint2(37.0)
+  ```py
+  # Read in parallel
+  await asyncio.gather(
+    device.get_temperature1(),
+    device.get_temperature2()
+  )
 ```
 
 ```py
-# Read in parallel
-await asyncio.gather(
-  device.get_temperature1(),
-  device.get_temperature2()
-)
-```
-
-```py
-from okolab import OkolabDeviceDisconnectedError, OkolabDeviceSystemError
+from okolab import OkolabDeviceConnectionError, OkolabDeviceSystemError
 
 # Catching errors
 try:
   temp = await device.get_temperature1()
-except OkolabDeviceDisconnectedError:
+except OkolabDeviceConnectionError:
   # The device has been disconnected
 except OkolabDeviceSystemError:
   # The device has reported an error
 ```
 
 ```py
-from okolab import OkolabDevice
-
-infos = OkolabDevice.list()
-
-for info in infos:
-  device = info.create()
-  print(await device.get_serial_number())
+for info in OkolabDevice.list():
+  with info.create() as device:
+    print(await device.get_serial_number())
 ```
```

### Comparing `okolab-0.2.0/okolab/__main__.py` & `okolab-0.2.1/okolab/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 async def main():
   root = HierarchyNode(["."])
 
   for device_info in OkolabDevice.list(all=True):
     try:
-      async with (device := device_info.create()):
+      async with device_info.create() as device:
         device_node = HierarchyNode([
           (await device.get_product_name()),
           f"Address: {device.address}",
           f"Serial number: {await device.get_serial_number()}",
           f"Uptime: {await device.get_uptime()}",
           f"Time: {await device.get_time()}"
         ])
```

### Comparing `okolab-0.2.0/okolab/device.py` & `okolab-0.2.1/okolab/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,24 @@
 from enum import IntEnum
 from typing import Optional
 
 import serial
 import serial.tools.list_ports
 from serial import Serial, SerialException
 
+from .util import aexit_handler
+
 
 class OkolabDeviceStatus(IntEnum):
   Ok = 0
   Transient = 1
   Alarm = 2
   Error = 3
   Disabled = 4
 
-class OkolabDeviceConnectionLostError(Exception):
-  """
-  An error raised by `OkolabDevice.closed()` when the connection to the controller is lost.
-  """
-
 class OkolabDeviceConnectionError(Exception):
   """
   An error raised when the connection to the controller fails or is corrupted.
   """
 
 class OkolabDeviceProtocolError(OkolabDeviceConnectionError):
   """
@@ -77,58 +74,26 @@
       self._serial: Optional[Serial] = Serial(
         baudrate=115200,
         port=address
       )
     except (OSError, SerialException) as e:
       raise OkolabDeviceConnectionError from e
 
-  async def close(self):
-    """
-    Closes the connection to the controller.
-    """
-
-    async with self._lock:
-      if self._serial:
-        self._serial.close()
-        self._serial = None
-
-        self._closed.set_result(False)
-
-  async def closed(self):
-    """
-    Returns once the connection to the controller is closed.
-
-    Closes the connection when cancelled.
-
-    Raises
-      OkolabDeviceConnectionLostError: If the connection was lost, as opposed to closed using `close()`.
-      asyncio.CancelledError
-    """
-
-    try:
-      if await asyncio.shield(self._closed):
-        raise OkolabDeviceConnectionLostError
-    except asyncio.CancelledError:
-      await self.close()
-      raise
-
   async def _request(self, command: str):
     def request():
       assert self._serial
       self._serial.write(f"{command}\r".encode("ascii"))
       return self._serial.read_until(b"\r").decode("ascii")
 
     async with self._lock:
       if not self._serial:
         raise OkolabDeviceConnectionError
 
-      loop = asyncio.get_event_loop()
-
       try:
-        res = await asyncio.wait_for(loop.run_in_executor(None, request), timeout=2.0)
+        res = await asyncio.wait_for(asyncio.to_thread(request), timeout=2.0)
       except (SerialException, asyncio.TimeoutError) as e:
         self._serial.close()
         self._serial = None
 
         self._closed.set_result(True)
 
         raise OkolabDeviceConnectionError from e
@@ -327,40 +292,62 @@
 
     if not match:
       raise OkolabDeviceProtocolError
 
     days, hours, minutes, seconds = match.groups()
     return timedelta(days=int(days), hours=int(hours), minutes=int(minutes), seconds=int(seconds))
 
+  async def close(self):
+    """
+    Closes the connection to the controller.
+    """
+
+    async with self._lock:
+      if self._serial:
+        self._serial.close()
+        self._serial = None
+
+        self._closed.set_result(False)
+
+  async def closed(self):
+    """
+    Returns once the connection to the controller is closed.
+    """
+
+    return await asyncio.shield(self._closed)
+
+  async def open(self):
+    pass
+
   async def __aenter__(self):
-    assert self._serial
+    await self.open()
+    return self
 
-  async def __aexit__(self, exc_type, exc, tb):
+  @aexit_handler
+  async def __aexit__(self):
     await self.close()
 
   @staticmethod
   def list(*, all: bool = False):
     """
     Lists visible devices.
 
     Parameters
       all: Whether to include devices that do not have recognized vendor and product ids.
 
     Yields
       Instances of `OkolabDeviceInfo`.
     """
 
-    infos = serial.tools.list_ports.comports()
-
-    for info in infos:
-      if all or (info.vid, info.pid) == (0x03eb, 0x2404):
-        yield OkolabDeviceInfo(address=info.device)
+    for item in serial.tools.list_ports.comports():
+      if all or (item.vid, item.pid) == (0x03eb, 0x2404):
+        yield OkolabDeviceInfo(address=item.device)
 
 
 __all__ = [
-  "OkolabDevice",
-  "OkolabDeviceConnectionError",
-  "OkolabDeviceConnectionLostError",
-  "OkolabDeviceProtocolError",
-  "OkolabDeviceStatus",
-  "OkolabDeviceSystemError"
+  'OkolabDevice',
+  'OkolabDeviceConnectionError',
+  'OkolabDeviceInfo',
+  'OkolabDeviceProtocolError',
+  'OkolabDeviceStatus',
+  'OkolabDeviceSystemError'
 ]
```

### Comparing `okolab-0.2.0/okolab.egg-info/PKG-INFO` & `okolab-0.2.1/okolab.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okolab
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package that provides control of the H401-T-CONTROLLER temperature controller from Okolab
 License: EUPL-1.2
 Project-URL: repository, https://github.com/slietar/okolab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Okolab
@@ -28,52 +28,42 @@
 from okolab import OkolabDevice
 
 device = OkolabDevice(address="COM3")
 device = OkolabDevice(address="/dev/tty.usbmodem1101")
 ```
 
 ```py
-def on_close(*, lost):
-  print(f"Connection closed, lost={lost}")
+async with device:
+  # Read temperature
+  temp = await device.get_temperature1()
+  temp = await device.get_temperature2()
 
-device = Device(address="COM3", on_close=on_close)
-```
+  # Write temperature
+  await device.set_temperature_setpoint1(37.0)
+  await device.set_temperature_setpoint2(37.0)
+  ```
 
-```py
-# Read temperature
-temp = await device.get_temperature1()
-temp = await device.get_temperature2()
-
-# Write temperature
-await device.set_temperature_setpoint1(37.0)
-await device.set_temperature_setpoint2(37.0)
+  ```py
+  # Read in parallel
+  await asyncio.gather(
+    device.get_temperature1(),
+    device.get_temperature2()
+  )
 ```
 
 ```py
-# Read in parallel
-await asyncio.gather(
-  device.get_temperature1(),
-  device.get_temperature2()
-)
-```
-
-```py
-from okolab import OkolabDeviceDisconnectedError, OkolabDeviceSystemError
+from okolab import OkolabDeviceConnectionError, OkolabDeviceSystemError
 
 # Catching errors
 try:
   temp = await device.get_temperature1()
-except OkolabDeviceDisconnectedError:
+except OkolabDeviceConnectionError:
   # The device has been disconnected
 except OkolabDeviceSystemError:
   # The device has reported an error
 ```
 
 ```py
-from okolab import OkolabDevice
-
-infos = OkolabDevice.list()
-
-for info in infos:
-  device = info.create()
-  print(await device.get_serial_number())
+for info in OkolabDevice.list():
+  with info.create() as device:
+    print(await device.get_serial_number())
 ```
```

