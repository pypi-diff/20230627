# Comparing `tmp/idun_mock-0.1.1.tar.gz` & `tmp/idun_mock-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_mock-0.1.1.tar", max compression
+gzip compressed data, was "idun_mock-0.1.2.tar", max compression
```

## Comparing `idun_mock-0.1.1.tar` & `idun_mock-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1310 2023-06-16 09:25:29.881033 idun_mock-0.1.1/README.md
--rw-r--r--   0        0        0      148 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/__init__.py
--rw-r--r--   0        0        0     7795 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/client/__init__.py
--rw-r--r--   0        0        0     5631 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/client/__main__.py
--rw-r--r--   0        0        0      167 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/__init__.py
--rw-r--r--   0        0        0     8398 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/connection_pool.py
--rw-r--r--   0        0        0     4970 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/generator.py
--rw-r--r--   0        0        0     3081 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/igeb_test_packets-0.txt
--rw-r--r--   0        0        0    17548 2023-06-16 09:25:29.881033 idun_mock-0.1.1/idun_mock/data_generator/igeb_test_packets.txt
--rw-r--r--   0        0        0      765 2023-06-16 09:25:29.881033 idun_mock-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 idun_mock-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1310 2023-06-27 21:12:32.598105 idun_mock-0.1.2/README.md
+-rw-r--r--   0        0        0      148 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/__init__.py
+-rw-r--r--   0        0        0     7617 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/client/__init__.py
+-rw-r--r--   0        0        0     5631 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/client/__main__.py
+-rw-r--r--   0        0        0      167 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/__init__.py
+-rw-r--r--   0        0        0     8398 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/connection_pool.py
+-rw-r--r--   0        0        0     4930 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/generator.py
+-rw-r--r--   0        0        0     3081 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/igeb_test_packets-0.txt
+-rw-r--r--   0        0        0    17548 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/igeb_test_packets.txt
+-rw-r--r--   0        0        0      731 2023-06-27 21:12:32.598105 idun_mock-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 idun_mock-0.1.2/PKG-INFO
```

### Comparing `idun_mock-0.1.1/README.md` & `idun_mock-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.1/idun_mock/client/__init__.py` & `idun_mock-0.1.2/idun_mock/client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio, json, csv, httpx
 import websockets.exceptions
 from datetime import datetime
-from idun_data_models import GuardianRecording, json_pydantic
-from idun_data_models.api_data_model import DataStreams
+from idun_data_models import RecordingIn, RecordingConfig, DataStreams
 from idun_tools import logger
 from ..data_generator import generate_queue, GeneratorTime
 
 
 class MockGuardianDataGenerator:
     def __init__(self):
         self.message_queue = asyncio.Queue(maxsize=int(1e7))
@@ -50,33 +49,28 @@
     async def gather_recordingIDs(self) -> list[dict]:
         if len(self.recordingIDs) == 0:
             self.recordingIDs = await self.recordingID_queue.get()
         return self.recordingIDs
 
     async def register_recordings(self, rest_api_url: str) -> None:
         async def register_recording(client, deviceID, recordingID):
-            payload = (
-                json_pydantic(
-                    GuardianRecording(
-                        recordingID,
-                        deviceID,
-                        "mock data generator",
-                        DataStreams(bandpass_eeg=True),
-                    )
+            payload = RecordingIn(
+                recordingID=recordingID,
+                deviceID=deviceID,
+                displayName="mock data generator",
+                config=RecordingConfig(
+                    data_stream_subscription=DataStreams(bandpass_eeg=True)
                 ),
             )
-            # TODO: fix json_pydantic
-            if isinstance(payload, tuple):
-                payload = payload[0]
             logger.bind(payload=payload).info("Registering recording")
             await http_post(
                 client,
                 f"{rest_api_url}/api/recording/{deviceID}/recordings",
                 auth=(deviceID, ""),
-                content=payload,
+                content=payload.json(),
             )
 
         recordingIDs = await self.gather_recordingIDs()
         async with httpx.AsyncClient() as client, asyncio.TaskGroup() as tg:
             for i in recordingIDs:
                 tg.create_task(
                     register_recording(client, i["deviceID"], i["recordingID"])
@@ -102,15 +96,15 @@
 
         if stop is None:
             stop = self.stop
 
         async def may_block():
             message = await self.message_queue.get()
             try:
-                await websocket.send(json_pydantic(message))
+                await websocket.send(message.json())
             except websockets.exceptions.ConnectionClosedError:
                 await self.message_queue.put(message)
                 raise
 
         try:
             while not stop.is_set():
                 await asyncio.wait_for(may_block(), timeout=6.0)
```

### Comparing `idun_mock-0.1.1/idun_mock/client/__main__.py` & `idun_mock-0.1.2/idun_mock/client/__main__.py`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.1/idun_mock/data_generator/connection_pool.py` & `idun_mock-0.1.2/idun_mock/data_generator/connection_pool.py`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.1/idun_mock/data_generator/generator.py` & `idun_mock-0.1.2/idun_mock/data_generator/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import threading, random, time, asyncio
-from dataclasses import asdict
 from idun_data_models import Message
 from idun_tools import logger
 from .connection_pool import DeviceConnectionPool, GeneratorTime
 
 
 async def generate_queue(
     logger,
@@ -46,15 +45,15 @@
     )
     await recordingID_queue.put(connectionPool.allRecordingIDs())
     messageSet = set()
     while not stop.is_set() and not connectionPool.done():
         data = connectionPool.next_message()
         if data:
             try:
-                await asyncio.wait_for(message_queue.put(asdict(data)), timeout=6.0)
+                await asyncio.wait_for(message_queue.put(data), timeout=6.0)
                 messageSet.add(data)
                 await asyncio.sleep(delay / devices)
             except asyncio.TimeoutError:
                 if message_queue.full():
                     logger.error("Generator queue full! Stopping generation")
                 else:
                     logger.error("Generator timeout! Stopping generation")
@@ -88,15 +87,15 @@
         random_seed=random_seed,
     )
     messageSet = set()
     while not stop.is_set() and not connectionPool.done():
         data = connectionPool.next_message()
         if data:
             kinesis_client.put_record(
-                Data=asdict(data),
+                Data=data.dict(),
                 PartitionKey=data.deviceID,
             )
             messageSet.add(data)
     logger.info("> Stop generating test data")
     return messageSet
```

### Comparing `idun_mock-0.1.1/idun_mock/data_generator/igeb_test_packets-0.txt` & `idun_mock-0.1.2/idun_mock/data_generator/igeb_test_packets-0.txt`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.1/idun_mock/data_generator/igeb_test_packets.txt` & `idun_mock-0.1.2/idun_mock/data_generator/igeb_test_packets.txt`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.1/PKG-INFO` & `idun_mock-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: idun-mock
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mock a real IDUN Guardian device for testing purposes
 Author: Konstantinos Samaras-Tsakiris
 Author-email: konstantinos@iduntechnologies.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: dacite (>=1.8,<2.0)
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: idun_data_models (>=0.1.2,<0.2.0)
+Requires-Dist: httpx (>=0.24,<0.25)
+Requires-Dist: idun_data_models (>=0.2.0,<0.3.0)
 Requires-Dist: idun_tools (>=0.1.0,<0.2.0)
 Requires-Dist: websockets (>=11.0,<12.0)
 Description-Content-Type: text/markdown
 
 # IDUN Guardian mock library / client
 
 This is a client library for the IDUN Guardian which mocks out the physical device, intended for development and building tests for the IDUN Guardian.
```

