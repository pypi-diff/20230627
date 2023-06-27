# Comparing `tmp/viam_sdk-0.4.2-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/viam_sdk-0.4.2rc1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9841528 bytes, number of entries: 375
+Zip file size: 9841542 bytes, number of entries: 375
 -rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx     1411 b- defN 80-Jan-01 00:00 viam/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 viam/components/__init__.py
 -rw-r--r--  2.0 unx     1075 b- defN 80-Jan-01 00:00 viam/components/arm/__init__.py
 -rw-r--r--  2.0 unx     2870 b- defN 80-Jan-01 00:00 viam/components/arm/arm.py
 -rw-r--r--  2.0 unx     3645 b- defN 80-Jan-01 00:00 viam/components/arm/client.py
 -rw-r--r--  2.0 unx     4951 b- defN 80-Jan-01 00:00 viam/components/arm/service.py
@@ -364,14 +364,14 @@
 -rw-r--r--  2.0 unx     2181 b- defN 80-Jan-01 00:00 viam/services/slam/client.py
 -rw-r--r--  2.0 unx     2757 b- defN 80-Jan-01 00:00 viam/services/slam/service.py
 -rw-r--r--  2.0 unx     1633 b- defN 80-Jan-01 00:00 viam/services/slam/slam.py
 -rw-r--r--  2.0 unx      426 b- defN 80-Jan-01 00:00 viam/services/vision/__init__.py
 -rw-r--r--  2.0 unx     5176 b- defN 80-Jan-01 00:00 viam/services/vision/client.py
 -rw-r--r--  2.0 unx     5076 b- defN 80-Jan-01 00:00 viam/services/vision/service.py
 -rw-r--r--  2.0 unx     4996 b- defN 80-Jan-01 00:00 viam/services/vision/vision.py
--rw-r--r--  2.0 unx     5286 b- defN 80-Jan-01 00:00 viam/sessions_client.py
+-rw-r--r--  2.0 unx     5149 b- defN 80-Jan-01 00:00 viam/sessions_client.py
 -rw-r--r--  2.0 unx     7927 b- defN 80-Jan-01 00:00 viam/utils.py
--rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     8730 b- defN 80-Jan-01 00:00 viam_sdk-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.4.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    34597 b- defN 16-Jan-01 00:00 viam_sdk-0.4.2.dist-info/RECORD
-375 files, 30136293 bytes uncompressed, 9785814 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.4.2rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8733 b- defN 80-Jan-01 00:00 viam_sdk-0.4.2rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.4.2rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    34609 b- defN 16-Jan-01 00:00 viam_sdk-0.4.2rc1.dist-info/RECORD
+375 files, 30136171 bytes uncompressed, 9785804 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1107,20 +1107,20 @@
 
 Filename: viam/sessions_client.py
 Comment: 
 
 Filename: viam/utils.py
 Comment: 
 
-Filename: viam_sdk-0.4.2.dist-info/LICENSE
+Filename: viam_sdk-0.4.2rc1.dist-info/LICENSE
 Comment: 
 
-Filename: viam_sdk-0.4.2.dist-info/METADATA
+Filename: viam_sdk-0.4.2rc1.dist-info/METADATA
 Comment: 
 
-Filename: viam_sdk-0.4.2.dist-info/WHEEL
+Filename: viam_sdk-0.4.2rc1.dist-info/WHEEL
 Comment: 
 
-Filename: viam_sdk-0.4.2.dist-info/RECORD
+Filename: viam_sdk-0.4.2rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## viam/sessions_client.py

```diff
@@ -32,14 +32,19 @@
 
 def loop_kwargs():
     if sys.version_info <= (3, 9):
         return {"loop": asyncio.get_running_loop()}
     return {}
 
 
+async def delay(coro, seconds):
+    await asyncio.sleep(seconds, **loop_kwargs())
+    await coro
+
+
 class SessionsClient:
     """
     A Session allows a client to express that it is actively connected and
     supports stopping actuating components when it's not.
     """
 
     _current_id: str = ""
@@ -107,30 +112,18 @@
                 if response.heartbeat_window is None:
                     raise GRPCError(status=Status.INTERNAL, message="Expected heartbeat window in response to start session")
 
                 self._supported = True
                 self._heartbeat_interval = response.heartbeat_window.ToTimedelta()
                 self._current_id = response.id
 
-        # tick once to ensure heartbeats are supported
         await self._heartbeat_tick()
 
-        if self._supported:
-            # We send heartbeats slightly faster than the interval window to
-            # ensure that we don't fall outside of it and expire the session.
-            wait = self._heartbeat_interval.total_seconds() / 5
-            asyncio.create_task(self._heartbeat_task(wait), name=f"{_TASK_PREFIX}-heartbeat")
-
         return self._metadata
 
-    async def _heartbeat_task(self, wait: float):
-        while self._supported:
-            await asyncio.sleep(wait)
-            await self._heartbeat_tick()
-
     async def _heartbeat_tick(self):
         if not self._supported:
             return
 
         while self._lock.locked():
             pass
 
@@ -142,14 +135,18 @@
         try:
             await self.client.SendSessionHeartbeat(request)
         except (GRPCError, StreamTerminatedError):
             LOGGER.debug("Heartbeat terminated", exc_info=True)
             self.reset()
         else:
             LOGGER.debug("Sent heartbeat successfully")
+            # We send heartbeats slightly faster than the interval window to
+            # ensure that we don't fall outside of it and expire the session.
+            wait = self._heartbeat_interval.total_seconds() / 5
+            asyncio.create_task(delay(self._heartbeat_tick(), wait), name=f"{_TASK_PREFIX}-heartbeat")
 
     @property
     def _metadata(self) -> _MetadataLike:
         if self._supported and self._current_id != "":
             return {SESSION_METADATA_KEY: self._current_id}
 
         return {}
```

## Comparing `viam_sdk-0.4.2.dist-info/LICENSE` & `viam_sdk-0.4.2rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `viam_sdk-0.4.2.dist-info/METADATA` & `viam_sdk-0.4.2rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viam-sdk
-Version: 0.4.2
+Version: 0.4.2rc1
 Summary: Viam Robotics Python SDK
 License: Apache-2.0
 Author: Naveed
 Author-email: naveed@viam.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `viam_sdk-0.4.2.dist-info/RECORD` & `viam_sdk-0.4.2rc1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -363,13 +363,13 @@
 viam/services/slam/client.py,sha256=co-PshdxsuJJVJPpJToTbhOy8H92fGtoB_AVjHFWwS8,2181
 viam/services/slam/service.py,sha256=nVgB7PxVPCYgOYt-6C7C9a6p_UD5jOfe0rsmIc-oZDQ,2757
 viam/services/slam/slam.py,sha256=872OV9JvSEvwWRBDiX-P8Zs87fNBp-5mbMx4ruot-gY,1633
 viam/services/vision/__init__.py,sha256=8DPwRKggv0cMb3Z4R5-pAHvbAIIMBfNYWUktuh58gyE,426
 viam/services/vision/client.py,sha256=EHiVW1R2JgS_DzyenmJzcIhQdtiegeUUBy2lYBpKemg,5176
 viam/services/vision/service.py,sha256=ae0zUVBi-QiNYoxfT7KurCUvdy0umdUdFVqMLprF_3c,5076
 viam/services/vision/vision.py,sha256=MFeEWjiS2Dp7ttqL3lmHTznxmGpoVEkIgYbWTuiZPPg,4996
-viam/sessions_client.py,sha256=Et7ipPP89RJ6PGjfwfstunDfZzGEmkrfDeldzBZ-Zso,5286
+viam/sessions_client.py,sha256=GUSKFmJnafDabxMsQQG2nuHPaiCUgjw42iHWJGg9qNA,5149
 viam/utils.py,sha256=gGoMOLkeJSerDIH2nPDydTfL7-p2AWqZCMU4jQEp0go,7927
-viam_sdk-0.4.2.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
-viam_sdk-0.4.2.dist-info/METADATA,sha256=ZVySQdGyXhKWtaUnqV-eybsZkuSgj9gsBDkQ8TVbVDk,8730
-viam_sdk-0.4.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-viam_sdk-0.4.2.dist-info/RECORD,,
+viam_sdk-0.4.2rc1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
+viam_sdk-0.4.2rc1.dist-info/METADATA,sha256=0pGX_HxGt1AYJqfKfYzLLnJGvO5PktVmD8Z0AW_glZg,8733
+viam_sdk-0.4.2rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+viam_sdk-0.4.2rc1.dist-info/RECORD,,
```

