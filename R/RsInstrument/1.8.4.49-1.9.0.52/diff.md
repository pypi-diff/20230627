# Comparing `tmp/RsInstrument-1.8.4.49.tar.gz` & `tmp/RsInstrument-1.9.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsInstrument-1.8.4.49.tar", last modified: Fri Nov 13 18:09:10 2020, max compression
+gzip compressed data, was "dist\RsInstrument-1.9.0.52.tar", last modified: Mon Nov 30 15:42:58 2020, max compression
```

## Comparing `RsInstrument-1.8.4.49.tar` & `RsInstrument-1.9.0.52.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2020-11-13 18:09:10.187106 RsInstrument-1.8.4.49/
--rw-rw-rw-   0        0        0     3606 2020-11-13 18:09:10.187106 RsInstrument-1.8.4.49/PKG-INFO
--rw-rw-rw-   0        0        0     2692 2020-11-13 18:09:06.000000 RsInstrument-1.8.4.49/README.md
-drwxrwxrwx   0        0        0        0 2020-11-13 18:09:10.128291 RsInstrument-1.8.4.49/RsInstrument/
-drwxrwxrwx   0        0        0        0 2020-11-13 18:09:10.141227 RsInstrument-1.8.4.49/RsInstrument/Fixed_Files/
--rw-rw-rw-   0        0        0     2132 2019-11-12 15:26:07.000000 RsInstrument-1.8.4.49/RsInstrument/Fixed_Files/Events.py
--rw-rw-rw-   0        0        0     4646 2019-11-14 07:57:49.000000 RsInstrument-1.8.4.49/RsInstrument/Fixed_Files/Reliability.py
--rw-rw-rw-   0        0        0    16240 2020-07-06 14:21:35.000000 RsInstrument-1.8.4.49/RsInstrument/Fixed_Files/Utilities.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsInstrument-1.8.4.49/RsInstrument/Fixed_Files/__init__.py
-drwxrwxrwx   0        0        0        0 2020-11-13 18:09:10.185110 RsInstrument-1.8.4.49/RsInstrument/Internal/
--rw-rw-rw-   0        0        0      560 2019-11-07 07:13:43.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4106 2020-10-08 12:02:42.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0      996 2019-11-12 15:18:27.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1028 2019-11-12 15:18:54.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9241 2020-07-06 14:21:35.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     4876 2019-11-14 07:57:49.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3433 2019-11-12 15:19:15.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2502 2019-11-12 15:19:15.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5309 2020-06-23 00:20:32.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    17684 2020-11-12 10:41:37.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3278 2020-07-06 14:21:35.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     3778 2019-11-14 07:57:49.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0     9637 2020-11-12 10:38:18.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/Core.py
--rw-rw-rw-   0        0        0    33883 2020-11-09 11:14:59.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/Instrument.py
--rw-rw-rw-   0        0        0     4021 2020-10-07 15:04:41.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2161 2019-11-12 15:21:08.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0     5258 2020-09-30 14:11:32.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3467 2020-06-23 00:20:32.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4435 2019-11-12 15:21:08.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0     3747 2020-06-23 00:20:32.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4847 2019-11-12 15:21:08.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     5074 2019-11-12 15:21:08.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1069 2019-11-12 15:21:08.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/StructBase.py
--rw-rw-rw-   0        0        0     2634 2019-11-11 06:33:43.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/Types.py
--rw-rw-rw-   0        0        0     4669 2019-11-11 06:33:43.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/Utilities.py
--rw-rw-rw-   0        0        0     5025 2020-09-30 12:56:05.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    43208 2020-09-30 14:11:32.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     6215 2020-06-23 00:20:32.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsInstrument-1.8.4.49/RsInstrument/Internal/__init__.py
--rw-rw-rw-   0        0        0    21771 2020-11-13 18:09:06.000000 RsInstrument-1.8.4.49/RsInstrument/RsInstrument.py
--rw-rw-rw-   0        0        0      684 2020-11-13 18:09:06.000000 RsInstrument-1.8.4.49/RsInstrument/__init__.py
-drwxrwxrwx   0        0        0        0 2020-11-13 18:09:10.135244 RsInstrument-1.8.4.49/RsInstrument.egg-info/
--rw-rw-rw-   0        0        0     3606 2020-11-13 18:09:10.000000 RsInstrument-1.8.4.49/RsInstrument.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2020-11-13 18:09:10.000000 RsInstrument-1.8.4.49/RsInstrument.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-13 18:09:10.000000 RsInstrument-1.8.4.49/RsInstrument.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-11-13 18:09:10.000000 RsInstrument-1.8.4.49/RsInstrument.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2020-11-13 18:09:10.000000 RsInstrument-1.8.4.49/RsInstrument.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-11-13 18:09:10.188141 RsInstrument-1.8.4.49/setup.cfg
--rw-rw-rw-   0        0        0      937 2020-11-13 18:09:06.000000 RsInstrument-1.8.4.49/setup.py
+drwxrwxrwx   0        0        0        0 2020-11-30 15:42:58.601021 RsInstrument-1.9.0.52/
+-rw-rw-rw-   0        0        0     3843 2020-11-30 15:42:58.601021 RsInstrument-1.9.0.52/PKG-INFO
+-rw-rw-rw-   0        0        0     2888 2020-11-30 15:42:35.000000 RsInstrument-1.9.0.52/README.md
+drwxrwxrwx   0        0        0        0 2020-11-30 15:42:58.490733 RsInstrument-1.9.0.52/RsInstrument/
+drwxrwxrwx   0        0        0        0 2020-11-30 15:42:58.515133 RsInstrument-1.9.0.52/RsInstrument/Fixed_Files/
+-rw-rw-rw-   0        0        0     2132 2019-11-12 15:26:07.000000 RsInstrument-1.9.0.52/RsInstrument/Fixed_Files/Events.py
+-rw-rw-rw-   0        0        0     4646 2019-11-14 07:57:49.000000 RsInstrument-1.9.0.52/RsInstrument/Fixed_Files/Reliability.py
+-rw-rw-rw-   0        0        0    17351 2020-11-29 19:13:32.000000 RsInstrument-1.9.0.52/RsInstrument/Fixed_Files/Utilities.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsInstrument-1.9.0.52/RsInstrument/Fixed_Files/__init__.py
+drwxrwxrwx   0        0        0        0 2020-11-30 15:42:58.597119 RsInstrument-1.9.0.52/RsInstrument/Internal/
+-rw-rw-rw-   0        0        0      560 2019-11-07 07:13:43.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4106 2020-10-08 12:02:42.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1086 2020-11-26 22:31:32.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1028 2019-11-12 15:18:54.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9241 2020-07-06 14:21:35.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5762 2020-11-24 16:30:50.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3433 2019-11-12 15:19:15.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2502 2019-11-12 15:19:15.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5309 2020-06-23 00:20:32.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    20352 2020-11-24 14:08:00.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3693 2020-11-24 16:11:43.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4489 2020-11-24 14:31:29.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    10071 2020-11-29 15:15:21.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/Core.py
+-rw-rw-rw-   0        0        0    35553 2020-11-29 19:45:00.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4021 2020-10-07 15:04:41.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2161 2019-11-12 15:21:08.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0     5258 2020-09-30 14:11:32.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3467 2020-06-23 00:20:32.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4435 2019-11-12 15:21:08.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0     3747 2020-06-23 00:20:32.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4847 2019-11-12 15:21:08.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5074 2019-11-12 15:21:08.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1069 2019-11-12 15:21:08.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3002 2020-11-24 16:13:14.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/Types.py
+-rw-rw-rw-   0        0        0     4669 2019-11-11 06:33:43.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5025 2020-09-30 12:56:05.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    44245 2020-11-29 17:25:52.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7136 2020-11-29 16:50:27.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsInstrument-1.9.0.52/RsInstrument/Internal/__init__.py
+-rw-rw-rw-   0        0        0    22882 2020-11-29 19:13:05.000000 RsInstrument-1.9.0.52/RsInstrument/RsInstrument.py
+-rw-rw-rw-   0        0        0      684 2020-11-30 15:42:54.000000 RsInstrument-1.9.0.52/RsInstrument/__init__.py
+drwxrwxrwx   0        0        0        0 2020-11-30 15:42:58.503421 RsInstrument-1.9.0.52/RsInstrument.egg-info/
+-rw-rw-rw-   0        0        0     3843 2020-11-30 15:42:58.000000 RsInstrument-1.9.0.52/RsInstrument.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1557 2020-11-30 15:42:58.000000 RsInstrument-1.9.0.52/RsInstrument.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-11-30 15:42:58.000000 RsInstrument-1.9.0.52/RsInstrument.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2020-11-30 15:42:58.000000 RsInstrument-1.9.0.52/RsInstrument.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2020-11-30 15:42:58.000000 RsInstrument-1.9.0.52/RsInstrument.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-11-30 15:42:58.601997 RsInstrument-1.9.0.52/setup.cfg
+-rw-rw-rw-   0        0        0      960 2020-11-30 15:42:54.000000 RsInstrument-1.9.0.52/setup.py
```

### Comparing `RsInstrument-1.8.4.49/PKG-INFO` & `RsInstrument-1.9.0.52/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: RsInstrument
-Version: 1.8.4.49
-Summary: VISA or Socket communication module for Rohde & Schwarz instruments
+Version: 1.9.0.52
+Summary: VISA or Socket Communication Module for Rohde & Schwarz Instruments
 Home-page: https://gitlab.com/miki2-2-2/rsinstrument
-Author: Rohde & Schwarz 2020
+Author: Rohde & Schwarz GmbH & Co. KG
 Author-email: Customer.Support@rohde-schwarz.com
 License: MIT
 Description: RsInstrument module provides convenient way of communicating with R&S instruments.
         
         Check out the full documentation here: https://rsinstrument.readthedocs.io/
         
         Version history:
         
+            Version 1.9.0.52 (29.11.2020)
+                - Added Thread-locking for sessions. Related new methods: get_lock(), assign_lock(), clear_lock()
+                - Added read-only property 'resource_name'
+        
             Version 1.8.4.49 (13.11.2020)
                 - Changed Authors and copyright
                 - Code changes only relevant for the auto-generated drivers
                 - Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
         
             Version 1.8.3.46 (09.11.2020)
                 - Fixed parsing of the instrument errors when an error message contains two double quotes
```

### Comparing `RsInstrument-1.8.4.49/README.md` & `RsInstrument-1.9.0.52/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 RsInstrument module provides convenient way of communicating with R&S instruments.
 
 Check out the full documentation here: https://rsinstrument.readthedocs.io/
 
 Version history:
 
+    Version 1.9.0.52 (29.11.2020)
+        - Added Thread-locking for sessions. Related new methods: get_lock(), assign_lock(), clear_lock()
+        - Added read-only property 'resource_name'
+
     Version 1.8.4.49 (13.11.2020)
         - Changed Authors and copyright
         - Code changes only relevant for the auto-generated drivers
         - Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
 
     Version 1.8.3.46 (09.11.2020)
         - Fixed parsing of the instrument errors when an error message contains two double quotes
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Fixed_Files/Events.py` & `RsInstrument-1.9.0.52/RsInstrument/Fixed_Files/Events.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Fixed_Files/Reliability.py` & `RsInstrument-1.9.0.52/RsInstrument/Fixed_Files/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Fixed_Files/Utilities.py` & `RsInstrument-1.9.0.52/RsInstrument/Fixed_Files/Utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List, Tuple
+import threading
 
 from ..Internal import Core
 from ..Internal import Conversions as Conv
 
 
 class Utilities:
 	"""Common utility class.
@@ -126,14 +127,19 @@
 		"""SCPI command: *TST?
 		Performs instrument's selftest.
 		Returns tuple (code:int, message: str). Code 0 means the self-test passed.
 		You can define the custom timeout in milliseconds. If you do not define it, the default selftest timeout is used (usually 60 secs)."""
 		return self._core.io.self_test(timeout)
 
 	@property
+	def resource_name(self) -> int:
+		"""Returns the resource name used in the constructor"""
+		return self._core.io.resource_name
+
+	@property
 	def opc_timeout(self) -> int:
 		"""See the opc_timeout.setter."""
 		return self._core.io.opc_timeout
 
 	@opc_timeout.setter
 	def opc_timeout(self, value: int) -> None:
 		"""Sets / Gets timeout in milliseconds for all the operations that use OPC synchronization."""
@@ -332,7 +338,24 @@
 		Set the append_to_pc_file to True if you want to append the read content to the end of the existing PC file"""
 		cmd = f"MMEM:DATA? '{source_instr_file}'"
 		self.query_bin_block_to_file(cmd, target_pc_file, append_to_pc_file)
 
 	def get_last_sent_cmd(self) -> str:
 		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
 		return self._core.get_last_sent_cmd()
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the thread lock for the current session. By default:
+			- If you create standard new RsInstrument instance with new VISA session, the session gets a new thread lock.
+				You can assign it to other RsInstrument sessions in order to share one physical instrument with a multi-thread access.
+			- If you create new RsInstrument from an existing session, the thread lock is shared automatically making both instances multi-thread safe.
+			You can always assign new thread lock by calling RsInstrument.assign_lock()
+		"""
+		return self._core.io.get_lock()
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the provided thread lock."""
+		self._core.io.assign_lock(lock)
+
+	def clear_lock(self):
+		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
+		self._core.io.clear_lock()
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ArgLinkedEventArgs.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ArgLinkedEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ArgSingle.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ArgSingle.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ArgSingleSuppressed.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ArgSingleSuppressed.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ArgStringComposer.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ArgStringComposer.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ArgStruct.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ArgStruct.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 
 	@classmethod
 	def scalar_int(cls, name: str, intern_link: str = None):
 		"""Describes mandatory scalar integer argument."""
 		return cls(name, DataType.Integer, None, False, False, 1, intern_link)
 
 	@classmethod
+	def scalar_int_ext(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar extended integer argument."""
+		return cls(name, DataType.IntegerExt, None, False, False, 1, intern_link)
+
+	@classmethod
 	def scalar_str(cls, name: str, intern_link: str = None):
 		"""Describes mandatory scalar string argument."""
 		return cls(name, DataType.String, None, False, False, 1, intern_link)
 
 	@classmethod
 	def scalar_raw_str(cls, name: str, intern_link: str = None):
 		"""Describes mandatory scalar raw string argument."""
@@ -43,14 +48,19 @@
 
 	@classmethod
 	def scalar_float(cls, name: str, intern_link: str = None):
 		"""Describes mandatory scalar float argument."""
 		return cls(name, DataType.Float, None, False, False, 1, intern_link)
 
 	@classmethod
+	def scalar_float_ext(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar extended float argument."""
+		return cls(name, DataType.FloatExt, None, False, False, 1, intern_link)
+
+	@classmethod
 	def scalar_enum(cls, name: str, enum_type, intern_link: str = None):
 		"""Describes mandatory scalar float argument."""
 		return cls(name, DataType.Enum, enum_type, False, False, 1, intern_link)
 
 	@classmethod
 	def scalar_str_optional(cls, name: str, intern_link: str = None):
 		"""Describes optional scalar string argument."""
@@ -64,30 +74,40 @@
 	@classmethod
 	def scalar_bool_optional(cls, name: str, intern_link: str = None):
 		"""Describes optional scalar boolean argument."""
 		return cls(name, DataType.Boolean, None, True, False, 1, intern_link)
 
 	@classmethod
 	def scalar_int_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar boolean argument."""
+		"""Describes optional scalar integer argument."""
 		return cls(name, DataType.Integer, None, True, False, 1, intern_link)
 
 	@classmethod
+	def scalar_int_ext_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar extended integer argument."""
+		return cls(name, DataType.IntegerExt, None, True, False, 1, intern_link)
+
+	@classmethod
 	def scalar_float_optional(cls, name: str, intern_link: str = None):
 		"""Describes optional scalar float argument."""
 		return cls(name, DataType.Float, None, True, False, 1, intern_link)
 
 	@classmethod
+	def scalar_float_ext_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar extended float argument."""
+		return cls(name, DataType.FloatExt, None, True, False, 1, intern_link)
+
+	@classmethod
 	def scalar_enum_optional(cls, name: str, enum_type, intern_link: str = None):
 		"""Describes optional scalar float argument."""
 		return cls(name, DataType.Enum, enum_type, True, False, 1, intern_link)
 
 	def __str__(self):
 		opt = '~' if self.is_optional else ''
-		name = f" '{self.name}'" if self.name is not '' else ''
+		name = f" '{self.name}'" if self.name != '' else ''
 		out = f"StructArg {opt}{self.data_type.name}{name}"
 
 		if self.is_open_list is False and self.repetition > 1:
 			out += f' [{self.repetition}]'
 		elif self.is_open_list is True:
 			out += f' [{self.repetition}...]'
 		if self.intern_link:
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ArgStructList.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ArgStructList.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ArgStructStringParser.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ArgStructStringParser.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/CommandsGroup.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/CommandsGroup.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/Conversions.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/Conversions.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,40 +135,67 @@
 		return float32_list_to_bytes(floats, True)
 	elif fmt == BinFloatFormat.Double_8bytes:
 		return double64_list_to_bytes(floats)
 	elif fmt == BinFloatFormat.Double_8bytes_swapped:
 		return double64_list_to_bytes(floats, True)
 
 
+pure_bool_true_lookup = frozenset(['on', 'On', 'ON', 'true', 'True', 'TRUE'])
 bool_true_lookup = frozenset(['1', 'on', 'On', 'ON', 'true', 'True', 'TRUE'])
 bool_false_lookup = frozenset(['0', 'off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
+pure_bool_false_lookup = frozenset(['off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
 
 
 def str_to_bool(string: str) -> bool:
 	"""Converts string to boolean value.
 	The function robust, and case insensitive.
 	If the string can not be converted to a boolean, the function returns False."""
 	assert_string_data(string)
 	if string in bool_true_lookup:
 		return True
 	if string in bool_false_lookup:
 		return False
+	# If leading/trailing spaces
 	string = string.strip()
 	if string in bool_true_lookup:
 		return True
 	if string in bool_false_lookup:
 		return False
+	# If enclosed by brackets
 	string = Utilities.trim_str_response(string)
 	if string in bool_true_lookup:
 		return True
 	if string in bool_false_lookup:
 		return False
 	return False
 
 
+def string_to_pure_bool(string: str) -> bool or None:
+	"""Converts string to boolean value. Compare to str_to_bool(), the values '1' and '0' are not considered boolean.
+	Also, if the method can not convert the string to boolean, it returns None."""
+	assert_string_data(string)
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	# If leading/trailing spaces
+	string = string.strip()
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	# If enclosed by brackets
+	string = Utilities.trim_str_response(string)
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	return None
+
+
 number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
 number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
 number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
 number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
 number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
 int_neg_inf = -(sys.maxsize - 1)
 enum_spec_prefixes = {'_minus': '-', '_plus': '+', '_': ''}
@@ -217,28 +244,38 @@
 	assert_string_data(string)
 	if string in number_plus_inf_lookup or string in number_max_lookup:
 		return sys.maxsize
 	if string in number_minus_inf_lookup or string in number_min_lookup or string in number_nan_lookup:
 		return int_neg_inf
 	if string == 'OFF':
 		return int_neg_inf + 1
+	if string == 'ON':
+		return int_neg_inf + 2
 	if string == 'OK':
 		return sys.maxsize - 1
 	if string == 'DC':
 		# noinspection PyTypeChecker
 		return int_neg_inf / 100
 	if string == 'ULEU':
 		return int(sys.maxsize / 10)
 	if string == 'ULEL':
 		# noinspection PyTypeChecker
 		return int_neg_inf / 10
 	# noinspection PyTypeChecker
 	return None
 
 
+def str_to_int_or_bool(string: str) -> int or bool:
+	"""Similar to str_to_int, but for special values "ON/OFF" the function returns boolean"""
+	result = string_to_pure_bool(string)
+	if result is not None:
+		return result
+	return str_to_int(string)
+
+
 def str_to_float(string: str) -> float:
 	"""Converts string to float value.
 	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
 	assert_string_data(string)
 	string = string.strip()
 	if string == '':
 		return 0.0
@@ -250,27 +287,37 @@
 		return math.nan
 	if string in number_max_lookup:
 		return sys.float_info.max
 	if string in number_min_lookup:
 		return -sys.float_info.max
 	if string == 'OFF':
 		return -sys.float_info.epsilon
+	if string == 'ON':
+		return -2*sys.float_info.epsilon
 	if string == 'OK':
 		return sys.float_info.epsilon
 	if string == 'DC' or string == '':
 		return -sys.float_info.max / 100
 	if string == 'ULEU':
 		return sys.float_info.max / 10
 	if string == 'ULEL':
 		return -sys.float_info.max / 10
 	if string == 'Simulating':
 		return 0.0
 	return float(string)
 
 
+def str_to_float_or_bool(string: str) -> float or bool:
+	"""Similar to str_to_float, but for special values "ON/OFF" the function returns boolean"""
+	result = string_to_pure_bool(string)
+	if result is not None:
+		return result
+	return str_to_float(string)
+
+
 def float_to_str(value: float) -> str:
 	"""Converts double number to string using {.12g} formatter."""
 	return format(value, ".12g")
 
 
 def bool_to_str(value: bool) -> str:
 	"""Converts boolean to 'ON' or 'OFF' string."""
@@ -338,14 +385,30 @@
 		return str(x)
 	elif isinstance(x, float):
 		return float_to_str(x)
 	else:
 		raise Exception(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
 
 
+def decimal_or_bool_value_to_str(x: int or float or bool) -> str:
+	"""Converts scalar decimal value to string.
+	Supported element types:
+	- int
+	- float
+	- boolean"""
+	if type(x) is bool:
+		return bool_to_str(x)
+	if isinstance(x, int):
+		return str(x)
+	elif isinstance(x, float):
+		return float_to_str(x)
+	else:
+		raise Exception(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
+
+
 def value_to_str(x: int or bool or float or str or Enum) -> str:
 	"""Converts scalar value to string.
 	Supported element types:
 	- int
 	- bool
 	- float
 	- string
@@ -388,51 +451,64 @@
 
 
 def str_to_float_list(string: str) -> List[float]:
 	"""Converts string with comma-separated values to list of Floats."""
 	assert_string_data(string)
 	if not string:
 		return []
-
 	result = [*map(str_to_float, string.split(','))]
 	return result
 
 
+def str_to_float_or_bool_list(string: str) -> List[float or bool]:
+	"""Converts string with comma-separated values to list of float or boolean values."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_float_or_bool, string.split(','))]
+	return result
+
+
 def str_to_int_list(string: str) -> List[int]:
 	"""Converts string with comma-separated values to list of Integers."""
 	assert_string_data(string)
 	if not string:
 		return []
-
 	result = [*map(str_to_int, string.split(','))]
 	return result
 
 
+def str_to_int_or_bool_list(string: str) -> List[int or bool]:
+	"""Converts string with comma-separated values to list of integer or boolean values."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_int_or_bool, string.split(','))]
+	return result
+
+
 def str_to_bool_list(string: str) -> List[bool]:
 	"""Converts string with comma-separated values to list of booleans."""
 	assert_string_data(string)
 	if not string:
 		return []
-
 	result = [*map(str_to_bool, string.split(','))]
 	return result
 
 
 def str_to_str_list(string: str, clear_one_empty_item: bool = False) -> List[str]:
 	"""Converts string with comma-separated values to list of strings.
 	Each element is trimmed by trim_str_response().
 	If the clear_one_empty_item is set to True (default is False), and the result is exactly one empty string item, the method returns empty list."""
 	assert_string_data(string)
 	if not string:
 		return []
-
 	result = [*map(Utilities.trim_str_response, string.split(','))]
 	if clear_one_empty_item and len(result) == 1 and result[0] == '':
 		return []
-
 	return result
 
 
 def _find_in_enum_members(item: str, enum_members: List[str]) -> int:
 	"""Matches a string in the provided list of member strings.
 	The item must be not fully matched.
 	The item is matched if a member string starts with the item (the item is a prefix of the member).
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ConverterFromScpiString.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ConverterFromScpiString.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import Enum
 
-from .Conversions import str_to_str_list, str_to_bool, str_to_bool_list, str_to_int, str_to_int_list, str_to_float, str_to_float_list, str_to_scalar_enum_helper, str_to_list_enum_helper
+from .Conversions import str_to_bool, str_to_int, str_to_int_or_bool, str_to_float, str_to_float_or_bool, str_to_scalar_enum_helper
+from .Conversions import str_to_str_list, str_to_bool_list, str_to_int_list, str_to_int_or_bool_list, str_to_float_list, str_to_float_or_bool_list, str_to_list_enum_helper
 from .Types import DataType
 from .Utilities import trim_str_response
 
 
 class ConverterFromScpiString:
 	"""Converter from SCPI response string to argument value
 	For list argument types, you must use the method get_one_element_value in a loop for each element.
@@ -20,26 +21,39 @@
 		self.enum_type = enum_type
 		self.data_type = data_type
 		self.element_type = self.data_type.element_type
 
 		if self.element_type == DataType.RawString:
 			self.converter = trim_str_response
 			self.list_converter = str_to_str_list
+
 		elif self.element_type == DataType.String:
 			self.converter = trim_str_response
 			self.list_converter = str_to_str_list
+
 		elif self.element_type == DataType.Boolean:
 			self.converter = str_to_bool
 			self.list_converter = str_to_bool_list
+
 		elif self.element_type == DataType.Integer:
 			self.converter = str_to_int
 			self.list_converter = str_to_int_list
+
+		elif self.element_type == DataType.IntegerExt:
+			self.converter = str_to_int_or_bool
+			self.list_converter = str_to_int_or_bool_list
+
 		elif self.element_type == DataType.Float:
 			self.converter = str_to_float
 			self.list_converter = str_to_float_list
+
+		elif self.element_type == DataType.FloatExt:
+			self.converter = str_to_float_or_bool
+			self.list_converter = str_to_float_or_bool_list
+
 		elif self.element_type == DataType.Enum:
 			assert self.enum_type, f"For data type enum, you have to define the enum_type variable."
 			# noinspection PyTypeChecker
 			self.enum_members = [x.name for x in self.enum_type]
 		else:
 			raise Exception(f"Unsupported data type '{data_type}'")
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/ConverterToScpiString.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/ConverterToScpiString.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,14 +37,22 @@
 	# For integer and float, allow them to be mixed
 	elif data_type == DataType.IntegerList or data_type == DataType.FloatList:
 		assert all((isinstance(x, int) or isinstance(x, float)) and type(x) != bool for x in data), f"Expected command parameter list of numbers, detected one or more elements of non-number type. Value: {data}"
 		return list_to_csv_str(data)
 	elif data_type == DataType.Integer or data_type == DataType.Float:
 		assert (isinstance(data, int) or isinstance(data, float)) and type(data) != bool, f"Expected command parameter number, actual data type: {type(data)}. Value: {data}"
 		return value_to_str(data)
+
+	# For integer and float extended, allow them to be mixed including the boolean type
+	elif data_type == DataType.IntegerExtList or data_type == DataType.FloatExtList:
+		assert all((isinstance(x, int) or isinstance(x, float) or isinstance(x, bool)) for x in data), f"Expected command parameter list of numbers or booleans, detected one or more elements of non-number type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.IntegerExt or data_type == DataType.FloatExt:
+		assert (isinstance(data, int) or isinstance(data, float) or isinstance(data, bool)), f"Expected command parameter number or boolean, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
 	else:
 		raise Exception(f"Unsupported data type: '{type(data_type)}'.")
 
 
 class ConverterToScpiString:
 	"""Converter from argument value to SCPI string.
 	Provides method get_value(arg_value) -> str
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/Core.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/Core.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 class Core(object):
 	"""Main driver component. Provides: \n
 		- Main core constructor
 		- 'io' interface for all the write / query operations
 		- Command parameters string composer for single arguments...
 		- Link handlers adding / changing / deleting
 
+		1.7.7 (build 42) 26.11.2020
+			- Extended ArgSingleList.compose_cmd_string() to 9 arguments
+
+		1.7.6 (build 41) 23.11.2020
+			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray
+
 		1.7.5 (build 40) 12.11.2020
 			- Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
 
 		1.7.4 (build 39) 11.09.2020
 			- Fixed parsing of the instrument errors when an error message contains two double quotes
 
 		1.7.3 (build 38) 21.10.2020
@@ -71,15 +77,15 @@
 			reset: bool = False,
 			driver_options: str = None,
 			user_options: str = None,
 			direct_session: object = None):
 		"""Initializes new driver session. For cleaner code, use the class methods: \n
 		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
 
-		self.core_version = '1.7.5'
+		self.core_version = '1.7.6'
 		self.simulating = False
 		self.supported_idn_patterns = []
 		self.supported_instr_models = []
 
 		self._args_single_list = ArgSingleList()
 		sett_dr = self._parse_init_settings_string(driver_options)
 		self._apply_settings_to_core(sett_dr)
@@ -102,21 +108,24 @@
 			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
 			False  # OPC query after each setting
 		)
 
 		self._instrumentSettings.apply_option_settings(sett_dr)
 		self._instrumentSettings.apply_option_settings(sett_user)
 
+		# Resolve the direct_session to handle. Options for direct_session type:
+		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
+		# - string in case of a simulation session
 		handle = direct_session
 		if handle:
 			# Check if the entered 'direct_session' is either the driver object or the Visa session
 			if hasattr(direct_session, 'get_session_handle'):
 				assert hasattr(direct_session, '_core'), f"Direct session is a class type. It must be an instance of the top-level driver class."
 				handle = direct_session.get_session_handle()
-			# Check if the handle is not simulation mode string
+			# Check if the handle is not a simulation mode string
 			if isinstance(handle, str):
 				if "Simulating session, resource name " in handle:
 					self.simulating = True
 					handle = None
 
 		self.io = Instrument(resource_name, self.simulating, self._instrumentSettings, handle)
 		self.io.query_instr_status = True
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/Instrument.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/Instrument.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import threading
 from enum import Enum
 from typing import List, Callable, Tuple, Dict
 
 from . import Utilities, InstrumentSettings, InstrumentOptions, InstrumentErrors, Conversions as Conv
 from .ArgSingleSuppressed import ArgSingleSuppressed
 from .ArgStructList import ArgStructList
 from .InternalLinker import InternalLinker
@@ -26,14 +27,15 @@
 		self._global_repcaps: Dict[str, RepeatedCapability] = {}
 		self._linker = InternalLinker()
 		# noinspection PyTypeChecker
 		self.on_write_handler: Callable = None
 		# noinspection PyTypeChecker
 		self.on_read_handler: Callable = None
 		self._io_events_include_data: bool = False
+		self._lock = None
 
 		# Fixed settings
 		self.selftest_timeout = 100000 if settings.selftest_timeout == 0 else settings.selftest_timeout
 		self.idn_model_full_name = settings.idn_model_full_name
 		self.instr_options_parse_mode = settings.instr_options_parse_mode
 
 		# Changeable settings
@@ -49,27 +51,30 @@
 		self.manufacturer: str = 'Rohde&Schwarz'
 		self.model: str = 'R&S Instrument'
 		self.serial_number: str = '100001'
 		self.firmware_version: str = '1.00'
 
 		if self._simulating:
 			self._session = VisaSessionSim(resource_name, settings, direct_session)
+			self._lock = self._session.get_lock()
 			self._instr_options = InstrumentOptions.Options('K0', InstrumentOptions.ParseMode.KeepOriginal)
 			self._session.write("*OPT K0")
 			return
 
 		self._session = VisaSession(resource_name, settings, direct_session)
-		self._session.clear_before_read()
-		self.idn_string = Utilities.trim_str_response(self._session.query_str('*IDN?')).strip()
-
-		# NRP-Z session coercing
-		if self._session.is_rsnrp_session():
-			settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
-			self.stb_in_error_check = False
-		self.instr_options_parse_mode = settings.instr_options_parse_mode
+		self._lock = self._session.get_lock()
+		with self._lock:
+			self._session.clear_before_read()
+			self.idn_string = Utilities.trim_str_response(self._session.query_str('*IDN?')).strip()
+
+			# NRP-Z session coercing
+			if self._session.is_rsnrp_session():
+				settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
+				self.stb_in_error_check = False
+			self.instr_options_parse_mode = settings.instr_options_parse_mode
 
 	def __str__(self):
 		if self._simulating:
 			return f"Simulated, Model: '{self.model}', ResourceName: '{self.resource_name}'"
 		else:
 			return f"Instrument Model: '{self.model}', ResourceName: '{self.resource_name}'"
 
@@ -87,14 +92,27 @@
 	def get_last_sent_cmd(self) -> str:
 		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
 		if self._simulating:
 			# noinspection PyUnresolvedReferences
 			return self._session.get_last_sent_cmd()
 		raise Exception("get_last_sent_cmd() can only be used in simulation mode")
 
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the thread lock provided from by the user. Trickles down to the VisaSession."""
+		self._lock = lock
+		self._session.assign_lock(lock)
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
+	def clear_lock(self):
+		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
+		self.assign_lock(threading.RLock())
+
 	@property
 	def visa_manufacturer(self) -> str:
 		"""Returns the visa manufacturer of the current session."""
 		return self._session.manufacturer
 
 	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
 		"""Adds / Updates link handler for the entered link_name.
@@ -206,18 +224,19 @@
 
 	def _query_options_and_parse(self, mode: InstrumentOptions.ParseMode) -> None:
 		"""Queries *OPT? and parses it based on the ParseMode."""
 		if mode == InstrumentOptions.ParseMode.Skip:
 			self._instr_options = InstrumentOptions.Options('', mode)
 			return
 		if self._simulating is False:
-			opts = self._session.query_str_no_tout_err('*OPT?', 1000)
-			if opts is None:
-				opts = 'Cannot read the instrument options - *OPT? query is not supported'
-			self._instr_options = InstrumentOptions.Options(opts, mode)
+			with self._lock:
+				opts = self._session.query_str_no_tout_err('*OPT?', 1000)
+				if opts is None:
+					opts = 'Cannot read the instrument options - *OPT? query is not supported'
+				self._instr_options = InstrumentOptions.Options(opts, mode)
 
 	@staticmethod
 	def _parse_err_query_response(response: str) -> str:
 		"""Parses entered response string to string error message without the error code.
 		E.g.: response = '-110,"Command error"' returns: 'Command error'."""
 		m = re.match(r'(-?[\d]+).*?"(.*)"', response)
 		if m:
@@ -250,232 +269,258 @@
 		for name, value in self._global_repcaps.items():
 			cmd_value = value.get_cmd_string_value()
 			cmd = cmd.replace(name, cmd_value)
 		return cmd
 
 	def query_opc(self) -> bool:
 		"""Sends *OPC? query and returns the result."""
-		self.start_send_read_event('*OPC?', False)
-		opc: bool = self._session.query_opc()
-		self.end_send_read_event()
-		return opc
+		with self._lock:
+			self.start_send_read_event('*OPC?', False)
+			opc: bool = self._session.query_opc()
+			self.end_send_read_event()
+			return opc
 
 	def query_all_syst_errors(self, include_codes=True) -> List[str]:
 		"""Returns all errors in the instrument's error queue.
 		If include_codes is False, you only get the error messages without the error codes."""
-		self.start_send_read_event('SYST:ERROR?', False)
-		errors = self._session.query_all_syst_errors()
-		if include_codes is False and errors is not None:
-			errors = [self._parse_err_query_response(x) for x in errors]
-		self.end_send_read_event()
-		return errors
+		with self._lock:
+			self.start_send_read_event('SYST:ERROR?', False)
+			errors = self._session.query_all_syst_errors()
+			if include_codes is False and errors is not None:
+				errors = [self._parse_err_query_response(x) for x in errors]
+			self.end_send_read_event()
+			return errors
 
 	def check_status(self) -> None:
 		"""Throws InstrumentStatusException in case of an error in the instrument's error queue.
 		The procedure is skipped, if the QueryInstrumentStatus is set to false."""
-		if not self.query_instr_status:
-			return
-		call_syst_error = self._session.error_in_error_queue() if self.stb_in_error_check else True
-		if call_syst_error:
-			errors = self.query_all_syst_errors(False)
-			InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, errors)
+		with self._lock:
+			if not self.query_instr_status:
+				return
+			call_syst_error = self._session.error_in_error_queue() if self.stb_in_error_check else True
+			if call_syst_error:
+				errors = self.query_all_syst_errors(False)
+				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, errors)
 
 	def clear_status(self) -> None:
 		"""Clears instrument's status subsystem."""
-		self._session.clear()
-		self._session.clear_before_read()
+		with self._lock:
+			self._session.clear()
+			self._session.clear_before_read()
 
 	def reset(self) -> None:
 		"""Resets the instrument and clears its status."""
-		self.write("*RST")
-		self.query_opc()
-		self.clear_status()
-		self.check_status()
+		with self._lock:
+			self.write("*RST")
+			self.query_opc()
+			self.clear_status()
+			self.check_status()
 
 	def write(self, cmd: str) -> None:
 		"""Writes string command to the instrument."""
-		cmd = self._replace_global_repcaps(cmd)
-		self._session.write(cmd)
-		if self.opc_query_after_write:
-			self._session.query_opc()
-		if self.on_write_handler:
-			self.send_write_str_event(cmd, False)
-		self.check_status()
+		with self._lock:
+			cmd = self._replace_global_repcaps(cmd)
+			self._session.write(cmd)
+			if self.opc_query_after_write:
+				self._session.query_opc()
+			if self.on_write_handler:
+				self.send_write_str_event(cmd, False)
+			self.check_status()
 
 	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
 		"""Writes a OPC-synced command.
 		Also performs error checking if the property self.query_instr_status is set to True.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		cmd = self._replace_global_repcaps(cmd)
-		self._session.write_with_opc(cmd, timeout)
-		self._session.query_and_clear_esr()
-		if self.on_write_handler:
-			self.send_write_str_event(cmd, True)
-		self.check_status()
+		with self._lock:
+			cmd = self._replace_global_repcaps(cmd)
+			self._session.write_with_opc(cmd, timeout)
+			self._session.query_and_clear_esr()
+			if self.on_write_handler:
+				self.send_write_str_event(cmd, True)
+			self.check_status()
 
 	def write_struct(self, cmd: str, struct: object) -> None:
 		"""Writes command to the instrument with the parameter composed from the entered structure."""
-		worker = ArgStructList(struct)
-		param = worker.compose_cmd_string()
-		cmd += f' {param}'.rstrip()
-		self.write(cmd)
+		with self._lock:
+			worker = ArgStructList(struct)
+			param = worker.compose_cmd_string()
+			cmd += f' {param}'.rstrip()
+			self.write(cmd)
 
 	def write_struct_with_opc(self, cmd: str, struct: object, timeout: int = None) -> None:
 		"""Writes OPC-synced command to the instrument with the parameter composed from the entered structure.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		worker = ArgStructList(struct)
-		param = worker.compose_cmd_string()
-		cmd += f' {param}'.rstrip()
-		self.write_with_opc(cmd, timeout)
+		with self._lock:
+			worker = ArgStructList(struct)
+			param = worker.compose_cmd_string()
+			cmd += f' {param}'.rstrip()
+			self.write_with_opc(cmd, timeout)
 
 	def query_str(self, query: str) -> str:
 		"""Sends a query and reads response from the instrument.
 		The response is trimmed of any trailing LF characters and has no length limit."""
-		query = self._replace_global_repcaps(query)
-		self.start_send_read_event(query, False)
-		response = self._session.query_str(query)
-		self.end_send_read_event()
-		self.check_status()
-		return response
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			response = self._session.query_str(query)
+			self.end_send_read_event()
+			self.check_status()
+			return response
 
 	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
 		"""Sends a OPC-synced query.
 		Also performs error checking if the self.query_instr_status is true.
 		The response is trimmed of any trailing LF characters and has no length limit.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		query = self._replace_global_repcaps(query)
-		self.start_send_read_event(query, True)
-		response = self._session.query_str_with_opc(query, timeout)
-		self.end_send_read_event()
-		self._session.query_and_clear_esr()
-		self.check_status()
-		return response
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			response = self._session.query_str_with_opc(query, timeout)
+			self.end_send_read_event()
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return response
 
 	def query_bin_block_to_stream(self, query: str, stream: StreamWriter) -> None:
 		"""Queries binary data block to the provided stream.
 		Use it for querying data from instrument to a variable or a file.
 		Throws an exception if the returned data was not a binary data."""
-		query = self._replace_global_repcaps(query)
-		self.start_send_read_event(query, False)
-		self._session.query_bin_block(query, stream, True)
-		self.end_send_read_event()
-		self.check_status()
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			self._session.query_bin_block(query, stream, True)
+			self.end_send_read_event()
+			self.check_status()
 
 	def query_bin_block(self, query: str) -> bytes:
 		"""Queries binary data block to bytes and returns data as bytes.
 		Throws an exception if the returned data was not a binary data."""
-		writer = StreamWriter.as_bin_var()
-		self.query_bin_block_to_stream(query, writer)
-		return writer.content
+		with self._lock:
+			writer = StreamWriter.as_bin_var()
+			self.query_bin_block_to_stream(query, writer)
+			return writer.content
 
 	def query_bin_block_to_file(self, cmd: str, file_path: str, append: bool = False) -> None:
 		"""Queries binary data block to the provided file.
 		If append is False, any existing file content is discarded.
 		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
 		Throws an exception if the returned data was not a binary data."""
-		with StreamWriter.as_bin_file(file_path, append) as writer:
-			self.query_bin_block_to_stream(cmd, writer)
+		with self._lock:
+			with StreamWriter.as_bin_file(file_path, append) as writer:
+				self.query_bin_block_to_stream(cmd, writer)
 
 	def query_bin_block_to_stream_with_opc(self, query: str, stream: StreamWriter, timeout: int = None) -> None:
 		"""Sends a OPC-synced query and returns data the provided stream.
 		Use it for querying data from instrument to a variable or a file.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		query = self._replace_global_repcaps(query)
-		self.start_send_read_event(query, True)
-		self._session.query_bin_block_with_opc(query, stream, True, timeout)
-		self.end_send_read_event()
-		self._session.query_and_clear_esr()
-		self.check_status()
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			self._session.query_bin_block_with_opc(query, stream, True, timeout)
+			self.end_send_read_event()
+			self._session.query_and_clear_esr()
+			self.check_status()
 
 	def query_bin_block_with_opc(self, query: str, timeout: int = None) -> bytes:
 		"""Sends a OPC-synced query and returns data as bytes.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		with StreamWriter.as_bin_var() as stream:
-			self.query_bin_block_to_stream_with_opc(query, stream, timeout)
-			return stream.content
+		with self._lock:
+			with StreamWriter.as_bin_var() as stream:
+				self.query_bin_block_to_stream_with_opc(query, stream, timeout)
+				return stream.content
 
 	def query_bin_block_to_file_with_opc(self, cmd: str, file_path: str, append: bool = False, timeout: int = None) -> None:
 		"""Sends a OPC-synced query and writes the returned data to the provided file.
 		If append is False, any existing file content is discarded.
 		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
 		Throws an exception if the returned data was not a binary data."""
-		with StreamWriter.as_bin_file(file_path, append) as writer:
-			self.query_bin_block_to_stream_with_opc(cmd, writer, timeout)
+		with self._lock:
+			with StreamWriter.as_bin_file(file_path, append) as writer:
+				self.query_bin_block_to_stream_with_opc(cmd, writer, timeout)
 
 	def query_int(self, query: str) -> int:
 		"""Sends a query and reads response from the instrument as integer."""
-		string = self.query_str(query)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return 0
-		return Conv.str_to_int(string)
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0
+			return Conv.str_to_int(string)
 
 	def query_int_with_opc(self, query: str, timeout: int = None) -> int:
 		"""Sends a OPC-synced query and reads response from the instrument as integer number.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		string = self.query_str_with_opc(query, timeout)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return 0
-		return Conv.str_to_int(string)
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0
+			return Conv.str_to_int(string)
 
 	def query_float(self, query: str) -> float:
 		"""Sends a query and reads response from the instrument as float number."""
-		string = self.query_str(query)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return 0.0
-		return Conv.str_to_float(string)
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0.0
+			return Conv.str_to_float(string)
 
 	def query_float_with_opc(self, query: str, timeout: int = None) -> float:
 		"""Sends a OPC-synced query and reads response from the instrument as float number.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		string = self.query_str_with_opc(query, timeout)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return 0.0
-		return Conv.str_to_float(string)
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0.0
+			return Conv.str_to_float(string)
 
 	def query_bool(self, query: str) -> bool:
 		"""Sends a query and reads response from the instrument as boolean value."""
-		string = self.query_str(query)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return False
-		return Conv.str_to_bool(string)
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return False
+			return Conv.str_to_bool(string)
 
 	def query_bool_with_opc(self, query: str, timeout: int = None) -> bool:
 		"""Sends a OPC-synced query and reads response from the instrument as boolean value.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		string = self.query_str_with_opc(query, timeout)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return False
-		return Conv.str_to_bool(string)
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return False
+			return Conv.str_to_bool(string)
 
 	def query_str_list(self, query: str) -> List[str]:
 		"""Sends a query and reads response from the instrument as csv-list."""
-		string = self.query_str(query)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-		response = [trim_str_response(x) for x in string.split(',')]
-		return response
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
+			response = [trim_str_response(x) for x in string.split(',')]
+			return response
 
 	def query_str_list_with_opc(self, query: str, timeout: int = None) -> List[str]:
 		"""Sends a OPC-synced query and reads response from the instrument as csv-list.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		string = self.query_str_with_opc(query, timeout)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-		response = [trim_str_response(x) for x in string.split(',')]
-		return response
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
+			response = [trim_str_response(x) for x in string.split(',')]
+			return response
 
 	def write_bin_block_from_stream(self, cmd: str, stream: StreamReader) -> None:
 		"""Writes all the stream content as binary data block to the instrument.
 		Use it for writing data to instrument from a variable or a file.
 		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
-		if self.on_write_handler:
-			self.start_send_write_bin_event(cmd)
-		self._session.write_bin_block(cmd, stream)
-		self.end_send_write_bin_event()
-		self.check_status()
+		with self._lock:
+			if self.on_write_handler:
+				self.start_send_write_bin_event(cmd)
+			self._session.write_bin_block(cmd, stream)
+			self.end_send_write_bin_event()
+			self.check_status()
 
 	def write_bin_block(self, cmd: str, payload: bytes) -> None:
 		"""Writes all the payload as binary data block to the instrument.
 		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
 		self.write_bin_block_from_stream(cmd, StreamReader.as_bin_var(payload))
 
 	def write_bin_block_from_file(self, cmd: str, file_path: str) -> None:
@@ -484,166 +529,178 @@
 		with StreamReader.as_bin_file(file_path) as reader:
 			self.write_bin_block_from_stream(cmd, reader)
 
 	def query_bin_or_ascii_float_list(self, query: str) -> List[float]:
 		"""Queries a list of floating-point numbers that can be returned in ASCII format or in binary format.
 		- For ASCII format, the list numbers are decoded as comma-separated values.
 		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32)."""
-		query = self._replace_global_repcaps(query)
-		self.start_send_read_event(query, False)
-		stream = StreamWriter.as_bin_var()
-		self._session.query_bin_block(query, stream, False)
-		self.end_send_read_event()
-		if self._simulating and not self._session.cached_to_stream:
-			return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-		if stream.binary:
-			result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-		else:
-			result = Conv.str_to_float_list(stream.content)
-		self.check_status()
-		return result
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			stream = StreamWriter.as_bin_var()
+			self._session.query_bin_block(query, stream, False)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
+			else:
+				result = Conv.str_to_float_list(stream.content)
+			self.check_status()
+			return result
 
 	def query_bin_or_ascii_float_list_with_opc(self, query: str, timeout: int = None) -> List[float]:
 		"""Sends a OPC-synced query and reads a list of floating-point numbers that can be returned in ASCII format or in binary format.
 		- For ASCII format, the list numbers are decoded as comma-separated values.
 		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32).
 		If you do not provide timeout, the method uses current opc_timeout."""
-		query = self._replace_global_repcaps(query)
-		self.start_send_read_event(query, True)
-		stream = StreamWriter.as_bin_var()
-		self._session.query_bin_block_with_opc(query, stream, False, timeout)
-		self.end_send_read_event()
-		if self._simulating and not self._session.cached_to_stream:
-			return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-		if stream.binary:
-			result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-		else:
-			result = Conv.str_to_float_list(stream.content)
-		self._session.query_and_clear_esr()
-		self.check_status()
-		return result
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			stream = StreamWriter.as_bin_var()
+			self._session.query_bin_block_with_opc(query, stream, False, timeout)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
+			else:
+				result = Conv.str_to_float_list(stream.content)
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return result
 
 	def query_bin_or_ascii_float_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[float]:
 		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
 		The current implementation allows for the rest of the string to be only ASCII format."""
-		string = self.query_str(query)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-		response = self._linker.cut_from_response_string(suppressed, string, query)
-		return Conv.str_to_float_list(response)
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return Conv.str_to_float_list(response)
 
 	def query_bin_or_ascii_float_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[float]:
 		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
 		If you do not provide timeout, the method uses current opc_timeout.
 		The current implementation allows for the rest of the string to be only ASCII format."""
-		string = self.query_str_with_opc(query, timeout)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-		response = self._linker.cut_from_response_string(suppressed, string, query)
-		return Conv.str_to_float_list(response)
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return Conv.str_to_float_list(response)
 
 	def query_bin_or_ascii_int_list(self, query: str) -> List[int]:
 		"""Queries a list of integer numbers that can be returned in ASCII format or in binary format.
 		- For ASCII format, the list numbers are decoded as comma-separated values.
 		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32)."""
-		query = self._replace_global_repcaps(query)
-		self.start_send_read_event(query, False)
-		stream = StreamWriter.as_bin_var()
-		self._session.query_bin_block(query, stream, False)
-		self.end_send_read_event()
-		if self._simulating and not self._session.cached_to_stream:
-			return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-		if stream.binary:
-			result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-		else:
-			result = Conv.str_to_int_list(stream.content)
-		self.check_status()
-		return result
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			stream = StreamWriter.as_bin_var()
+			self._session.query_bin_block(query, stream, False)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
+			else:
+				result = Conv.str_to_int_list(stream.content)
+			self.check_status()
+			return result
 
 	def query_bin_or_ascii_int_list_with_opc(self, query: str, timeout: int = None) -> List[int]:
 		"""Sends a OPC-synced query and reads a list of integer numbers that can be returned in ASCII format or in binary format.
 		- For ASCII format, the list numbers are decoded as comma-separated values.
 		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32).
 		If you do not provide timeout, the method uses current opc_timeout."""
-		query = self._replace_global_repcaps(query)
-		self.start_send_read_event(query, True)
-		stream = StreamWriter.as_bin_var()
-		self._session.query_bin_block_with_opc(query, stream, False, timeout)
-		self.end_send_read_event()
-		if self._simulating and not self._session.cached_to_stream:
-			return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-		if stream.binary:
-			result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-		else:
-			result = Conv.str_to_int_list(stream.content)
-		self._session.query_and_clear_esr()
-		self.check_status()
-		return result
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			stream = StreamWriter.as_bin_var()
+			self._session.query_bin_block_with_opc(query, stream, False, timeout)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
+			else:
+				result = Conv.str_to_int_list(stream.content)
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return result
 
 	def query_bin_or_ascii_int_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[int]:
 		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
 		The current implementation allows for the rest of the string to be only ASCII format."""
-		response = self.query_str(query)
-		if self._simulating:
-			return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-		response = self._linker.cut_from_response_string(suppressed, response, query)
-		return Conv.str_to_int_list(response)
+		with self._lock:
+			response = self.query_str(query)
+			if self._simulating:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			response = self._linker.cut_from_response_string(suppressed, response, query)
+			return Conv.str_to_int_list(response)
 
 	def query_bin_or_ascii_int_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[int]:
 		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
 		If you do not provide timeout, the method uses current opc_timeout.
 		The current implementation allows for the rest of the string to be only ASCII format."""
-		response = self.query_str_with_opc(query, timeout)
-		if self._simulating:
-			return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-		response = self._linker.cut_from_response_string(suppressed, response, query)
-		return Conv.str_to_int_list(response)
+		with self._lock:
+			response = self.query_str_with_opc(query, timeout)
+			if self._simulating:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			response = self._linker.cut_from_response_string(suppressed, response, query)
+			return Conv.str_to_int_list(response)
 
 	def query_struct(self, query: str, struct: object) -> object:
 		"""Queries string of from instrument, and parses it based on the provided structure object.
 		THe method returns the copy of the entered object that it had modified."""
-		string = self.query_str(query)
-		if self._simulating and self._sim_cached_value_not_found(string):
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return struct
+			struct_list = ArgStructList(struct)
+			struct_list.parse_from_cmd_response(string)
+			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
 			return struct
-		struct_list = ArgStructList(struct)
-		struct_list.parse_from_cmd_response(string)
-		self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
-		return struct
 
 	def query_str_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> str:
 		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
-		string = self.query_str(query)
-		if self._simulating and self._sim_cached_value_not_found(string):
-			return string
-		response = self._linker.cut_from_response_string(suppressed, string, query)
-		return response
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return string
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return response
 
 	def self_test(self, timeout: int = None) -> Tuple[int, str]:
 		"""Performs instrument's selftest (*TST?).
 		Returns tuple (code:int, message: str). . Code 0 means the self-test passed.
 		You can define the custom timeout in milliseconds. If you do not define it, the default selftest timeout is used (usually 60 secs)."""
-		if timeout is None or timeout == 0:
-			timeout = self.selftest_timeout
-		response = self.query_str_with_opc('*TST?', timeout)
-		m = re.search(r'^(-?[\d]+)(,(.*))?', response)
-		if not m:
-			raise InstrumentErrors.UnexpectedResponseException(self.resource_name, f"Unexpected response to a '*TST?' self-test query: '{response}'")
-		code = Conv.str_to_int(m.group(1))
-		msg = Utilities.trim_str_response(m.group(3))
-		self.check_status()
-		return code, msg
+		with self._lock:
+			if timeout is None or timeout == 0:
+				timeout = self.selftest_timeout
+			response = self.query_str_with_opc('*TST?', timeout)
+			m = re.search(r'^(-?[\d]+)(,(.*))?', response)
+			if not m:
+				raise InstrumentErrors.UnexpectedResponseException(self.resource_name, f"Unexpected response to a '*TST?' self-test query: '{response}'")
+			code = Conv.str_to_int(m.group(1))
+			msg = Utilities.trim_str_response(m.group(3))
+			self.check_status()
+			return code, msg
 
 	def get_session_handle(self) -> object:
 		"""Returns the underlying pyvisa session."""
 		return self._session.get_session_handle()
 
 	def close(self) -> None:
 		"""Closes the Instrument session."""
-		self._session.close()
-		self._session = None
+		with self._lock:
+			self._session.close()
+			self._session = None
 
 	# Events part
 
 	@property
 	def io_events_include_data(self) -> bool:
 		"""If true, the read and write handlers also include read and written data."""
 		return self._io_events_include_data
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/InstrumentErrors.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/InstrumentErrors.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/InstrumentOptions.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/InstrumentOptions.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/InstrumentSettings.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/InstrumentSettings.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/InternalLinker.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/InternalLinker.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/IoTransferEventArgs.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/IoTransferEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/RepeatedCapability.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/RepeatedCapability.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/StreamReader.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/StreamReader.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/StreamWriter.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/StreamWriter.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/StructBase.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/StructBase.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/Types.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/Types.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,34 +3,40 @@
 
 
 class DataType(Enum):
 	"""Data type of a variable in the driver."""
 	String = auto()
 	RawString = auto()
 	Integer = auto()
+	IntegerExt = auto()
 	Boolean = auto()
 	Float = auto()
+	FloatExt = auto()
 	Enum = auto()
 	StringList = auto()
 	RawStringList = auto()
 	IntegerList = auto()
+	IntegerExtList = auto()
 	BooleanList = auto()
 	FloatList = auto()
+	FloatExtList = auto()
 	EnumList = auto()
 
 	@property
 	def is_list(self) -> bool:
 		"""Returns True, if the data type is a list."""
 		return self in frozenset(
 			{
 				DataType.StringList,
 				DataType.RawStringList,
 				DataType.IntegerList,
+				DataType.IntegerExtList,
 				DataType.BooleanList,
 				DataType.FloatList,
+				DataType.FloatExtList,
 				DataType.EnumList
 			})
 
 	@property
 	def is_scalar(self) -> bool:
 		"""Returns True, if the data type is a scalar."""
 		return not self.is_list
@@ -67,16 +73,20 @@
 			return DataType.RawString
 		elif self == DataType.RawStringList:
 			return DataType.RawString
 		elif self == DataType.BooleanList:
 			return DataType.Boolean
 		elif self == DataType.IntegerList:
 			return DataType.Integer
+		elif self == DataType.IntegerExtList:
+			return DataType.IntegerExt
 		elif self == DataType.FloatList:
 			return DataType.Float
+		elif self == DataType.FloatExtList:
+			return DataType.FloatExt
 		elif self == DataType.EnumList:
 			return DataType.Enum
 
 	def get_default_value(self, enm: Enum = None) -> Any:
 		"""Returns default value for the current type.
 		If the data type is Enum or EnumString, you have to provide the enum class."""
 		if self.is_list:
@@ -85,22 +95,15 @@
 			return ''
 		elif self == DataType.String:
 			return ''
 		elif self == DataType.Boolean:
 			return False
 		elif self == DataType.Integer:
 			return 0
+		elif self == DataType.IntegerExt:
+			return 0
 		elif self == DataType.Float:
 			return 0.0
+		elif self == DataType.FloatExt:
+			return 0.0
 		elif self == DataType.Enum:
 			return enm(0)
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/Utilities.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/Utilities.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/VisaPluginSocketIo.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/VisaPluginSocketIo.py`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/VisaSession.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/VisaSession.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 from enum import Enum, Flag
 from typing import Tuple, Callable, AnyStr
 import os.path
 import re
+import threading
 
 # noinspection PyPackageRequirements
 import pyvisa
 
 from .VisaPluginSocketIo import ResourceManager, SocketIo
 from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
 from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
@@ -59,14 +60,15 @@
 	"""Extended VISA class."""
 
 	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
 		self.reusing_session = direct_session is not None
 		# noinspection PyTypeChecker
 		self._data_chunk_size: int = None
 		self._std_bin_block_header_max_len: int = 999999999
+		self._lock = None
 		self.disable_opc_query: bool = settings.disable_opc_query
 		self.last_status = None
 		self.visa_library_name = None
 
 		# Implemented for interface compatibility with VisaSessionSim
 		self.cached_to_stream = False
 
@@ -90,25 +92,34 @@
 			# Check resource_name for the trailing (SelectVisa=..)
 			pure_resource_name, visa_select = self._get_pure_resource_name(resource_name)
 			if settings.visa_select is not None:
 				visa_select = settings.visa_select
 			self._rm = VisaSession.get_resource_manager(visa_select)
 			self.manufacturer = self._get_visa_manufacturer()
 
+			# Resource manager opening
 			try:
 				self._session = self._rm.open_resource(pure_resource_name)
 			except pyvisa.VisaIOError as e:
 				if e.error_code != pyvisa.constants.StatusCode.error_resource_not_found:
 					raise e
 				message = e.description
 				message += f"\nLibrary: {self._rm.visalib}\nManufacturer: {self.manufacturer}\nResource Name: '{resource_name}'"
 				raise InstrumentErrors.ResourceError(resource_name, message)
-
 			self._resource_name = resource_name
 
+		# Decide, whether to create a new thread lock or the existing one from the session
+		if hasattr(self._session, 'session_thread_rlock'):
+			rlock = self._session.session_thread_rlock
+			if isinstance(rlock, type(threading.RLock())):
+				self.assign_lock(rlock)
+		if self.get_lock() is None:
+			# The existing session did not have a thread lock, assign a new one
+			self.assign_lock(threading.RLock())
+
 		self._interface_type = SessionKind.unsupported
 		if self._session.interface_type == pyvisa.constants.InterfaceType.gpib or self._session.interface_type == pyvisa.constants.InterfaceType.gpib:
 			self._interface_type = SessionKind.gpib
 
 		elif self._session.interface_type == pyvisa.constants.InterfaceType.rsnrp:
 			self._interface_type = SessionKind.rs_nrp
 
@@ -234,14 +245,25 @@
 		except TypeError:
 			return self._rm.visalib.__class__.__name__
 
 	def is_rsnrp_session(self) -> bool:
 		"""Returns True, if the current session is a NRP-Z session"""
 		return self._interface_type == SessionKind.rs_nrp
 
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the provided thread lock by setting the pyvisa runtime session attribute 'session_thread_rlock'
+		This is done, because if the session is to be entered as an existing session to another RsInstrument object,
+		the lock must be shared as well. The lock is only used by the parent class Instrument."""
+		setattr(self._session, 'session_thread_rlock', lock)
+		self._lock = lock
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
 	@property
 	def visa_timeout(self) -> int:
 		"""See the visa_timeout.setter."""
 		return int(self._session.timeout)
 
 	@visa_timeout.setter
 	def visa_timeout(self, value: int) -> None:
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/Internal/VisaSessionSim.py` & `RsInstrument-1.9.0.52/RsInstrument/Internal/VisaSessionSim.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+import threading
 from typing import Callable, Dict, AnyStr
 
 from . import InstrumentSettings
 from .StreamReader import StreamReader
 from .StreamWriter import StreamWriter
 
 
 # noinspection PyMethodMayBeStatic,PyUnusedLocal
 class VisaSessionSim(object):
 	"""Visa session in simulation mode.
-	Provides the properties for the simulation mode"""
+	Provides the properties for the simulation mode.
+	Also serves as a cache for the SCPI command values: If you query a SCPI command value, it returns the last set value by that SCPI command."""
 
 	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
 		# noinspection PyTypeChecker
 		self._data_chunk_size: int = None
+		self._lock: threading.RLock = None
 
 		# Event handlers
 		# noinspection PyTypeChecker
 		self.on_read_chunk_handler: Callable = None
 		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
 		# noinspection PyTypeChecker
 		self.on_write_chunk_handler: Callable = None
@@ -37,14 +40,31 @@
 
 		# If the return value is written to a cache, this flag signals if it was a cached value
 		self.cached_to_stream = False
 
 		# cache command values dictionary
 		self._cmd_vals_cache: Dict[str, AnyStr] = {}
 
+		# Decide, whether to create a new thread lock or the existing one from the direct_session
+		if direct_session and hasattr(direct_session, 'session_thread_rlock'):
+			rlock = direct_session.session_thread_rlock
+			if isinstance(rlock, type(threading.RLock())):
+				self.assign_lock(rlock)
+		if self.get_lock() is None:
+			# The existing session did not have a thread lock, assign a new one
+			self.assign_lock(threading.RLock())
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the provided thread lock. The lock is only used by the parent class Instrument."""
+		self._lock = lock
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
 	def _update_cmd_vals_cache(self, cmd: str, param: AnyStr = None) -> None:
 		"""Parses out the parameter from the command and stores/updates them in the cache"""
 		aux = cmd.split(' ', 1)
 		if len(aux) < 2:
 			return
 		headers = aux[0].strip().lower()
 		param = aux[1].strip()
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/RsInstrument.py` & `RsInstrument-1.9.0.52/RsInstrument/RsInstrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import threading
 from typing import List, Tuple
 
 from .Fixed_Files import Events
 from .Internal.Core import Core
 from .Internal.Conversions import BinFloatFormat, BinIntFormat
 from .Internal import Conversions as Conv
 from .Internal.VisaSession import VisaSession
 
 
 class RsInstrument:
-	_driver_version_const = '1.8.4.49'
+	_driver_version_const = '1.9.0.52'
 	_driver_options_const = "SupportedInstrModels = All Rohde & Schwarz Instruments, SupportedIdnPatterns = Rohde(-|&)Schwarz/Hameg, SimulationIdnString = Rohde&Schwarz*SimulationDevice*100001*" + _driver_version_const
 
 	def __init__(
 			self, resource_name: str, id_query: bool = True, reset: bool = False, options: str = None, direct_session: object = None):
 		"""Initializes new RsInstrument session. \n
 		Parameter options tokens examples:
 			- 'Simulate=True' - starts the session in simulation mode. Default: False
@@ -197,14 +198,19 @@
 		"""SCPI command: *TST?
 		Performs instrument's selftest.
 		Returns tuple (code:int, message: str). Code 0 means the self-test passed.
 		You can define the custom timeout in milliseconds. If you do not define it, the default selftest timeout is used (usually 60 secs)."""
 		return self._core.io.self_test(timeout)
 
 	@property
+	def resource_name(self) -> int:
+		"""Returns the resource name used in the constructor"""
+		return self._core.io.resource_name
+
+	@property
 	def opc_timeout(self) -> int:
 		"""See the opc_timeout.setter"""
 		return self._core.io.opc_timeout
 
 	@opc_timeout.setter
 	def opc_timeout(self, value: int) -> None:
 		"""Sets / Gets timeout in milliseconds for all the operations that use OPC synchronization"""
@@ -404,14 +410,31 @@
 		cmd = f"MMEM:DATA? '{source_instr_file}'"
 		self.query_bin_block_to_file(cmd, target_pc_file, append_to_pc_file)
 
 	def get_last_sent_cmd(self) -> str:
 		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
 		return self._core.get_last_sent_cmd()
 
+	def get_lock(self) -> threading.RLock:
+		"""Returns the thread lock for the current session. By default:
+			- If you create standard new RsInstrument instance with new VISA session, the session gets a new thread lock.
+				You can assign it to other RsInstrument sessions in order to share one physical instrument with a multi-thread access.
+			- If you create new RsInstrument from an existing session, the thread lock is shared automatically making both instances multi-thread safe.
+			You can always assign new thread lock by calling RsInstrument.assign_lock()
+		"""
+		return self._core.io.get_lock()
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the provided thread lock."""
+		self._core.io.assign_lock(lock)
+
+	def clear_lock(self):
+		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
+		self._core.io.clear_lock()
+
 	@staticmethod
 	def assert_minimum_version(min_version: str) -> None:
 		"""Asserts that the driver version fulfills the minimum required version you have entered.
 		This way you make sure your installed driver is of the entered version or newer."""
 		min_version_list = min_version.split('.')
 		curr_version_list = RsInstrument._driver_version_const.split('.')
 		count_min = len(min_version_list)
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument/__init__.py` & `RsInstrument-1.9.0.52/RsInstrument/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """VISA communication interface for SCPI-based instrument remote control.
-	:version: 1.8.4.49
+	:version: 1.9.0.52
 	:copyright: 2020 by Rohde & Schwarz GMBH & Co. KG
 	:license: MIT, see LICENSE for more details.
 """
 
 
-__version__ = '1.8.4.49'
+__version__ = '1.9.0.52'
 
 # Main class
 from RsInstrument.RsInstrument import RsInstrument
 
 # Bin data format
 from RsInstrument.RsInstrument import BinFloatFormat, BinIntFormat
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument.egg-info/PKG-INFO` & `RsInstrument-1.9.0.52/RsInstrument.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: RsInstrument
-Version: 1.8.4.49
-Summary: VISA or Socket communication module for Rohde & Schwarz instruments
+Version: 1.9.0.52
+Summary: VISA or Socket Communication Module for Rohde & Schwarz Instruments
 Home-page: https://gitlab.com/miki2-2-2/rsinstrument
-Author: Rohde & Schwarz 2020
+Author: Rohde & Schwarz GmbH & Co. KG
 Author-email: Customer.Support@rohde-schwarz.com
 License: MIT
 Description: RsInstrument module provides convenient way of communicating with R&S instruments.
         
         Check out the full documentation here: https://rsinstrument.readthedocs.io/
         
         Version history:
         
+            Version 1.9.0.52 (29.11.2020)
+                - Added Thread-locking for sessions. Related new methods: get_lock(), assign_lock(), clear_lock()
+                - Added read-only property 'resource_name'
+        
             Version 1.8.4.49 (13.11.2020)
                 - Changed Authors and copyright
                 - Code changes only relevant for the auto-generated drivers
                 - Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
         
             Version 1.8.3.46 (09.11.2020)
                 - Fixed parsing of the instrument errors when an error message contains two double quotes
```

### Comparing `RsInstrument-1.8.4.49/RsInstrument.egg-info/SOURCES.txt` & `RsInstrument-1.9.0.52/RsInstrument.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RsInstrument-1.8.4.49/setup.py` & `RsInstrument-1.9.0.52/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="RsInstrument",
-    version="1.8.4.49",
-    description="VISA or Socket communication module for Rohde & Schwarz instruments",
+    version="1.9.0.52",
+    description="VISA or Socket Communication Module for Rohde & Schwarz Instruments",
     long_description=README,
     long_description_content_type="text/markdown",
-    author="Rohde & Schwarz 2020",
-	copyright="Copyright © Rohde & Schwarz 2020",
+    author="Rohde & Schwarz GmbH & Co. KG",
+	copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2020",
     author_email="Customer.Support@rohde-schwarz.com",
 	url="https://gitlab.com/miki2-2-2/rsinstrument",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
     ],
```

