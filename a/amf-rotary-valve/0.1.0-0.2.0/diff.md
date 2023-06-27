# Comparing `tmp/amf-rotary-valve-0.1.0.tar.gz` & `tmp/amf-rotary-valve-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amf-rotary-valve-0.1.0.tar", last modified: Fri Mar 24 18:27:48 2023, max compression
+gzip compressed data, was "amf-rotary-valve-0.2.0.tar", last modified: Tue Jun 27 17:19:39 2023, max compression
```

## Comparing `amf-rotary-valve-0.1.0.tar` & `amf-rotary-valve-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 adaptyvbio   (501) staff       (20)        0 2023-03-24 18:27:48.425796 amf-rotary-valve-0.1.0/
--rw-r--r--   0 adaptyvbio   (501) staff       (20)     1025 2023-03-24 18:27:48.425689 amf-rotary-valve-0.1.0/PKG-INFO
-drwxr-xr-x   0 adaptyvbio   (501) staff       (20)        0 2023-03-24 18:27:48.424909 amf-rotary-valve-0.1.0/amf_rotary_valve/
--rw-r--r--   0 adaptyvbio   (501) staff       (20)       22 2023-03-24 10:50:45.000000 amf-rotary-valve-0.1.0/amf_rotary_valve/__init__.py
--rw-r--r--   0 adaptyvbio   (501) staff       (20)     1267 2023-03-24 17:29:51.000000 amf-rotary-valve-0.1.0/amf_rotary_valve/__main__.py
--rw-r--r--   0 adaptyvbio   (501) staff       (20)     7503 2023-03-24 17:35:48.000000 amf-rotary-valve-0.1.0/amf_rotary_valve/device.py
-drwxr-xr-x   0 adaptyvbio   (501) staff       (20)        0 2023-03-24 18:27:48.425558 amf-rotary-valve-0.1.0/amf_rotary_valve.egg-info/
--rw-r--r--   0 adaptyvbio   (501) staff       (20)     1025 2023-03-24 18:27:48.000000 amf-rotary-valve-0.1.0/amf_rotary_valve.egg-info/PKG-INFO
--rw-r--r--   0 adaptyvbio   (501) staff       (20)      308 2023-03-24 18:27:48.000000 amf-rotary-valve-0.1.0/amf_rotary_valve.egg-info/SOURCES.txt
--rw-r--r--   0 adaptyvbio   (501) staff       (20)        1 2023-03-24 18:27:48.000000 amf-rotary-valve-0.1.0/amf_rotary_valve.egg-info/dependency_links.txt
--rw-r--r--   0 adaptyvbio   (501) staff       (20)       17 2023-03-24 18:27:48.000000 amf-rotary-valve-0.1.0/amf_rotary_valve.egg-info/requires.txt
--rw-r--r--   0 adaptyvbio   (501) staff       (20)       17 2023-03-24 18:27:48.000000 amf-rotary-valve-0.1.0/amf_rotary_valve.egg-info/top_level.txt
--rw-r--r--   0 adaptyvbio   (501) staff       (20)      477 2023-03-24 18:26:49.000000 amf-rotary-valve-0.1.0/pyproject.toml
--rw-r--r--   0 adaptyvbio   (501) staff       (20)      744 2023-03-24 11:37:27.000000 amf-rotary-valve-0.1.0/readme.md
--rw-r--r--   0 adaptyvbio   (501) staff       (20)       38 2023-03-24 18:27:48.425826 amf-rotary-valve-0.1.0/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 17:19:39.009192 amf-rotary-valve-0.2.0/
+-rw-r--r--   0 simon      (501) staff       (20)     1015 2023-06-27 17:19:39.009059 amf-rotary-valve-0.2.0/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 17:19:39.007953 amf-rotary-valve-0.2.0/amf_rotary_valve/
+-rw-r--r--   0 simon      (501) staff       (20)       22 2023-05-19 14:47:19.000000 amf-rotary-valve-0.2.0/amf_rotary_valve/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1258 2023-06-27 17:14:42.000000 amf-rotary-valve-0.2.0/amf_rotary_valve/__main__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6839 2023-06-27 17:15:05.000000 amf-rotary-valve-0.2.0/amf_rotary_valve/device.py
+-rw-r--r--   0 simon      (501) staff       (20)      568 2023-06-27 17:14:42.000000 amf-rotary-valve-0.2.0/amf_rotary_valve/util.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 17:19:39.008879 amf-rotary-valve-0.2.0/amf_rotary_valve.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     1015 2023-06-27 17:19:39.000000 amf-rotary-valve-0.2.0/amf_rotary_valve.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      333 2023-06-27 17:19:39.000000 amf-rotary-valve-0.2.0/amf_rotary_valve.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-27 17:19:39.000000 amf-rotary-valve-0.2.0/amf_rotary_valve.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       17 2023-06-27 17:19:39.000000 amf-rotary-valve-0.2.0/amf_rotary_valve.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)       17 2023-06-27 17:19:39.000000 amf-rotary-valve-0.2.0/amf_rotary_valve.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)      477 2023-06-27 17:18:55.000000 amf-rotary-valve-0.2.0/pyproject.toml
+-rw-r--r--   0 simon      (501) staff       (20)      734 2023-05-19 14:47:19.000000 amf-rotary-valve-0.2.0/readme.md
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-27 17:19:39.009229 amf-rotary-valve-0.2.0/setup.cfg
```

### Comparing `amf-rotary-valve-0.1.0/PKG-INFO` & `amf-rotary-valve-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amf-rotary-valve
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package that provides control of AMF rotary valves
 License: EUPL-1.2
 Project-URL: repository, https://github.com/slietar/amf-rotary-valve
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # amf-rotary-valve
@@ -23,27 +23,27 @@
 
 
 ## Usage
 
 ```py
 from amf_rotary_valve import AMFDevice
 
-device = OkolabDevice(address="COM3")
-device = OkolabDevice(address="/dev/tty.usbmodem1101")
+device = AMFDevice(address="COM3")
+device = AMFDevice(address="/dev/tty.usbmodem1101")
 ```
 
 ```py
 async with device:
   await device.home()
 
   valve_count = await device.get_valve_count()
   current_valve = await device.get_valve()
 
   # Rotate to the next valve
   await device.rotate(current_valve % valve_count + 1)
 ```
 
 ```py
-for info in OkolabDevice.list():
-  async with (device := info.create())
+for info in AMFDevice.list():
+  async with info.create() as device:
     print(await device.get_unique_id())
 ```
```

### Comparing `amf-rotary-valve-0.1.0/amf_rotary_valve/__main__.py` & `amf-rotary-valve-0.2.0/amf_rotary_valve/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,27 +18,27 @@
         for index, child in enumerate(self.children)
     ])
 
 
 async def main():
   root = HierarchyNode(["."])
 
-  for device_info in AMFDevice.list(all=True):
+  for device_info in AMFDevice.list():
     try:
-      async with (device := device_info.create()):
+      async with device_info.create() as device:
         valve = await device.get_valve()
 
         root.children.append(HierarchyNode([
           "Rotary valve",
           f"Address: {device.address}",
           f"Unique id: {await device.get_unique_id()}",
           f"Current valve: {valve if valve is not None else '<uninitialized>'}",
           f"Valve count: {await device.get_valve_count()}"
         ]))
-    except AMFDeviceConnectionError:
+    except* AMFDeviceConnectionError:
       pass
 
   if root.children:
     print(root.format())
   else:
     print("No device found.")
```

### Comparing `amf-rotary-valve-0.1.0/amf_rotary_valve/device.py` & `amf-rotary-valve-0.2.0/amf_rotary_valve/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,214 +1,142 @@
 import asyncio
-from asyncio import Future
 import builtins
+from asyncio import Event, Future, Lock, Task
 from dataclasses import dataclass
-from typing import Optional, overload
-from serial import Serial
+from typing import Any, Optional, overload
 
 import serial.tools.list_ports
+from serial import Serial
 from serial.serialutil import SerialException
 
+from .util import aexit_handler
+
 
 Datatype = type[bool] | type[int]
 
 class AMFDeviceConnectionError(Exception):
   pass
 
-class AMFDeviceConnectionLostError(AMFDeviceConnectionError):
-  pass
-
 
 @dataclass(frozen=True, kw_only=True)
 class AMFDeviceInfo:
   address: str
 
   def create(self):
     return AMFDevice(self.address)
 
 
 class AMFDevice:
   def __init__(self, address: str):
-    self.address = address
+    """
+    Constructs an `AMFDevice` instance and opens the connection to the device.
+
+    Parameters
+      address: The address of the device, such as `COM3` or `/dev/tty.usbmodem1101`.
+
+    Raises
+      AMFDeviceConnectionError: If the device is unreachable.
+    """
 
-    self._closed = Future[bool]()
+    self.address = address
 
     try:
-      self._serial: Optional[Serial] = Serial(
+      self._serial = Serial(
         baudrate=9600,
         port=address
       )
     except (OSError, SerialException) as e:
       raise AMFDeviceConnectionError from e
 
     self._busy = False
-    self._busy_future: Optional[Future] = None
-    self._closed_exc = Future[None]()
     self._closing = False
-    self._query_futures = list[Future]()
-    self._main_task = asyncio.create_task(self._main_func())
-
-  async def _main_func(self):
-    read_task = asyncio.create_task(self._read_loop())
-
-    try:
-      await asyncio.shield(asyncio.wait([
-        self._closed_exc,
-        read_task
-      ], return_when=asyncio.FIRST_COMPLETED))
-    except asyncio.CancelledError: # Called .close()
-      pass
-
-    if self._busy_future:
-      self._busy_future.set_exception(AMFDeviceConnectionError())
-
-    for future in self._query_futures:
-      future.set_exception(AMFDeviceConnectionError())
-
-    assert self._serial
-    self._serial.close()
-    self._serial = None
-
-    if not self._closing:
-      read_task.cancel()
-      self._closing = True
-
-    try:
-      await read_task
-    except asyncio.CancelledError:
-      pass
-    except SerialException as e:
-      raise AMFDeviceConnectionLostError from e
-
-    if self._closed_exc.done() and (exc := self._closed_exc.exception()):
-      raise AMFDeviceConnectionLostError from exc
+    self._error_event = Event()
+    self._query_future = Future[Any]()
+    self._query_lock = Lock()
+    self._read_task: Optional[Task[None]] = None
+    self._run_future: Optional[Future[Any]] = None
+    self._run_lock = Lock()
 
   async def _read_loop(self):
-    loop = asyncio.get_event_loop()
-
     try:
       while True:
-        assert self._serial
-        serial = self._serial
-
-        self._receive((await loop.run_in_executor(None, lambda: serial.read_until(b"\n")))[0:-2])
+        # Call _receive() to process the received data
+        self._receive((await asyncio.to_thread(lambda: self._serial.read_until(b"\n")))[0:-2])
+    except SerialException as e:
+      raise AMFDeviceConnectionError from e
     finally:
-      self._read_task = None
-
-  async def close(self):
-    """
-    Closes the device.
-    """
-
-    if not self._closing:
-      self._closing = True
-      futures = self._query_futures + ([self._busy_future] if self._busy_future else list())
-
-      if futures:
-        await asyncio.wait(futures)
-
-      self._main_task.cancel()
-
-    try:
-      await self._main_task
-    except AMFDeviceConnectionLostError:
-      pass
-    except asyncio.CancelledError: # If the the main task didn't have time to start.
-      pass
-
-  async def closed(self):
-    """
-    Waits for the device to close.
+      if not self._closing:
+        self._error_event.set()
 
-    When cancelled, closes the device and waits for it to close.
+      # Raise exceptions in all the current futures
 
-    Raises
-      asyncio.CancelledError
-      AMFDeviceConnectionLostError: If the connection was lost rather than closed explicitly.
-    """
-
-    try:
-      await asyncio.shield(self._main_task)
-    except asyncio.CancelledError:
-      await self.close()
-      raise
+      if self._query_future and not self._query_future.done():
+        self._query_future.set_exception(AMFDeviceConnectionError())
+      if self._run_future and not self._run_future.done():
+        self._run_future.set_exception(AMFDeviceConnectionError())
 
   @overload
   async def _query(self, command: str, dtype: type[bool]) -> bool:
     pass
 
   @overload
   async def _query(self, command: str, dtype: type[int]) -> int:
     pass
 
   @overload
   async def _query(self, command: str, dtype = None) -> str:
     pass
 
-  async def _query(self, command: str, dtype: Optional[type[bool] | type[int]] = None):
-    if self._closing:
-      raise AMFDeviceConnectionError
-
-    future = Future()
-    self._query_futures.append(future)
+  async def _query(self, command: str, dtype: Optional[Datatype] = None):
+    async with self._query_lock:
+      if self._closing or self._error_event.is_set():
+        raise AMFDeviceConnectionError
 
-    loop = asyncio.get_event_loop()
+      self._query_future = Future[Any]()
 
-    try:
       try:
-        assert (serial := self._serial)
-        await loop.run_in_executor(None, lambda: serial.write(f"/_{command}\r".encode("utf-8")))
-        return self._parse(await asyncio.wait_for(future, timeout=2.0), dtype=dtype)
-      except:
-        self._query_futures.remove(future)
-        raise
-    except (SerialException, asyncio.TimeoutError) as e:
-      self._closed_exc.set_exception(e)
-      await self.closed()
-
-      # This statement won't is unreachable as self.closed() will raise an AMFDeviceConnectionLostError.
-      raise
+        await asyncio.to_thread(lambda: self._serial.write(f"/_{command}\r".encode()))
+        return self._parse(await asyncio.wait_for(asyncio.shield(self._query_future), timeout=2.0), dtype=dtype)
+      except (SerialException, asyncio.TimeoutError) as e:
+        self._error_event.set()
+        raise AMFDeviceConnectionError from e
+      finally:
+        self._query_future = None
 
   def _parse(self, data: bytes, dtype: Optional[Datatype] = None):
-    response = data[3:-1].decode("utf-8")
+    response = data[3:-1].decode()
 
     match dtype:
       case builtins.bool:
         return (response == "1")
       case builtins.int:
         return int(response)
       case _:
         return response
 
   def _receive(self, data: bytes):
     was_busy = self._busy
     self._busy = (data[2] & (1 << 5)) < 1
 
-    if self._busy_future and was_busy and (not self._busy):
-      self._busy_future.set_result(data)
-      self._busy_future = None
+    if self._run_future and was_busy and (not self._busy):
+      self._run_future.set_result(data)
+    elif self._query_future:
+      self._query_future.set_result(data)
     else:
-      query_future, *self._query_futures = self._query_futures
-      query_future.set_result(data)
+      raise Exception("Dropping data")
 
   async def _run(self, command: str):
-    if self._closing:
-      raise AMFDeviceConnectionError
-
-    while self._busy_future:
-      await self._busy_future
+    async with self._run_lock:
+      self._run_future = Future[Any]()
 
-    future = Future()
-    self._busy_future = future
-
-    try:
-      await self._query(command)
-      await future
-    finally:
-      self._busy_future = None
+      try:
+        await self._query(command)
+        await asyncio.shield(self._run_future)
+      finally:
+        self._run_future = None
 
   async def get_unique_id(self):
     """
     Returns the unique id of this device.
 
     Returns
       The unique id of this device, such as `...`.
@@ -261,37 +189,80 @@
 
     Parameters
       delay: The delay, in seconds. The resolution is 1 ms.
     """
 
     await self._run(f"M{round(delay * 1000)}R")
 
+  async def wait_error(self):
+    await self._error_event.wait()
+
   async def __aenter__(self):
-    assert not self._closing
+    await self.open()
+    return self
+
+  @aexit_handler
+  async def __aexit__(self, failed: bool):
+    if not failed:
+      async with (self._query_lock, self._run_lock):
+        await self.close()
+    else:
+      await self.close()
+
+  async def open(self):
+    if self._read_task:
+      raise AMFDeviceConnectionError
 
-  async def __aexit__(self, exc_type, exc, tb):
-    await self.close()
+    self._read_task = asyncio.create_task(self._read_loop())
+
+    try:
+      # Set answer mode to asynchronous
+      await self._query("!501")
+    except Exception:
+      # Avoid preventing __aexit__() from being called
+      await self.close()
+      raise
+
+  async def close(self):
+    """
+    Closes the device.
+
+    Raises
+      AMFDeviceConnectionLostError: If the device was already closed.
+    """
+
+    if self._closing or (not self._read_task):
+      raise AMFDeviceConnectionError
+
+    self._closing = True
+
+    # Cancel the read task, if any
+
+    self._read_task.cancel()
+
+    try:
+      await self._read_task
+    except asyncio.CancelledError:
+      pass
+    finally:
+      del self._read_task
+
+    self._serial.close()
 
   @staticmethod
-  def list(*, all: bool = False):
+  def list():
     """
     Lists visible devices.
 
-    Parameters
-      all: Whether to include devices that do not have recognized vendor and product ids.
-
     Yields
       Instances of `AMFDeviceInfo`.
     """
 
     for item in serial.tools.list_ports.comports():
-      # if all or (item.vid, item.pid) == (0x03eb, 0x2404):
-      if all:
-        yield AMFDeviceInfo(address=item.device)
+      yield AMFDeviceInfo(address=item.device)
 
 
 __all__ = [
   'AMFDevice',
   'AMFDeviceConnectionError',
-  'AMFDeviceConnectionLostError',
   'AMFDeviceInfo'
 ]
```

### Comparing `amf-rotary-valve-0.1.0/amf_rotary_valve.egg-info/PKG-INFO` & `amf-rotary-valve-0.2.0/amf_rotary_valve.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amf-rotary-valve
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package that provides control of AMF rotary valves
 License: EUPL-1.2
 Project-URL: repository, https://github.com/slietar/amf-rotary-valve
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # amf-rotary-valve
@@ -23,27 +23,27 @@
 
 
 ## Usage
 
 ```py
 from amf_rotary_valve import AMFDevice
 
-device = OkolabDevice(address="COM3")
-device = OkolabDevice(address="/dev/tty.usbmodem1101")
+device = AMFDevice(address="COM3")
+device = AMFDevice(address="/dev/tty.usbmodem1101")
 ```
 
 ```py
 async with device:
   await device.home()
 
   valve_count = await device.get_valve_count()
   current_valve = await device.get_valve()
 
   # Rotate to the next valve
   await device.rotate(current_valve % valve_count + 1)
 ```
 
 ```py
-for info in OkolabDevice.list():
-  async with (device := info.create())
+for info in AMFDevice.list():
+  async with info.create() as device:
     print(await device.get_unique_id())
 ```
```

### Comparing `amf-rotary-valve-0.1.0/readme.md` & `amf-rotary-valve-0.2.0/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 
 ## Usage
 
 ```py
 from amf_rotary_valve import AMFDevice
 
-device = OkolabDevice(address="COM3")
-device = OkolabDevice(address="/dev/tty.usbmodem1101")
+device = AMFDevice(address="COM3")
+device = AMFDevice(address="/dev/tty.usbmodem1101")
 ```
 
 ```py
 async with device:
   await device.home()
 
   valve_count = await device.get_valve_count()
   current_valve = await device.get_valve()
 
   # Rotate to the next valve
   await device.rotate(current_valve % valve_count + 1)
 ```
 
 ```py
-for info in OkolabDevice.list():
-  async with (device := info.create())
+for info in AMFDevice.list():
+  async with info.create() as device:
     print(await device.get_unique_id())
 ```
```

