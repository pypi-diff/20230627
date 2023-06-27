# Comparing `tmp/bytecore-1.0.0.tar.gz` & `tmp/bytecore-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecore-1.0.0.tar", last modified: Mon Jun 26 17:31:24 2023, max compression
+gzip compressed data, was "bytecore-1.0.1.tar", last modified: Tue Jun 27 16:31:24 2023, max compression
```

## Comparing `bytecore-1.0.0.tar` & `bytecore-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-26 17:31:24.600938 bytecore-1.0.0/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1074 2023-06-26 17:30:28.000000 bytecore-1.0.0/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14510 2023-06-26 17:31:24.600938 bytecore-1.0.0/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13933 2023-06-26 17:30:28.000000 bytecore-1.0.0/README.md
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      651 2023-06-26 17:30:28.000000 bytecore-1.0.0/pyproject.toml
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-26 17:31:24.600938 bytecore-1.0.0/setup.cfg
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-26 17:31:24.592938 bytecore-1.0.0/src/
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-26 17:31:24.596938 bytecore-1.0.0/src/bytecore/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4662 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/accumulator.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      799 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/bit.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1732 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/byte.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1769 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/byte_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      294 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/constant_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11455 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/control_unit.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      276 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/control_unit_state.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2620 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/cpu.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1024 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/emulator.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2737 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/memory.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      178 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/opcode.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1009 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/proxy_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1974 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/replay_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1146 2023-06-26 17:30:28.000000 bytecore-1.0.0/src/bytecore/state.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-26 17:31:24.596938 bytecore-1.0.0/src/bytecore.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14510 2023-06-26 17:31:24.000000 bytecore-1.0.0/src/bytecore.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      726 2023-06-26 17:31:24.000000 bytecore-1.0.0/src/bytecore.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-26 17:31:24.000000 bytecore-1.0.0/src/bytecore.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        9 2023-06-26 17:31:24.000000 bytecore-1.0.0/src/bytecore.egg-info/top_level.txt
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-26 17:31:24.600938 bytecore-1.0.0/tests/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1085 2023-06-26 17:30:28.000000 bytecore-1.0.0/tests/test_bit.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1106 2023-06-26 17:30:28.000000 bytecore-1.0.0/tests/test_byte.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1707 2023-06-26 17:30:28.000000 bytecore-1.0.0/tests/test_byte_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    15238 2023-06-26 17:30:28.000000 bytecore-1.0.0/tests/test_cpu.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9038 2023-06-26 17:30:28.000000 bytecore-1.0.0/tests/test_emulator.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3238 2023-06-26 17:30:28.000000 bytecore-1.0.0/tests/test_memory.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-27 16:31:24.631454 bytecore-1.0.1/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1074 2023-06-27 16:30:11.000000 bytecore-1.0.1/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14510 2023-06-27 16:31:24.631454 bytecore-1.0.1/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13933 2023-06-27 16:30:11.000000 bytecore-1.0.1/README.md
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      756 2023-06-27 16:30:11.000000 bytecore-1.0.1/pyproject.toml
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-27 16:31:24.631454 bytecore-1.0.1/setup.cfg
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-27 16:31:24.623454 bytecore-1.0.1/src/
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-27 16:31:24.631454 bytecore-1.0.1/src/bytecore/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4662 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/accumulator.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      799 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/bit.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1732 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/byte.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1769 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/byte_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      294 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/constant_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11455 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/control_unit.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      276 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/control_unit_state.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2620 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/cpu.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1024 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/emulator.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2737 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/memory.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      178 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/opcode.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1009 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/proxy_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/py.typed
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1974 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/replay_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1146 2023-06-27 16:30:11.000000 bytecore-1.0.1/src/bytecore/state.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-27 16:31:24.631454 bytecore-1.0.1/src/bytecore.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14510 2023-06-27 16:31:24.000000 bytecore-1.0.1/src/bytecore.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      748 2023-06-27 16:31:24.000000 bytecore-1.0.1/src/bytecore.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-27 16:31:24.000000 bytecore-1.0.1/src/bytecore.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        9 2023-06-27 16:31:24.000000 bytecore-1.0.1/src/bytecore.egg-info/top_level.txt
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-27 16:31:24.631454 bytecore-1.0.1/tests/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1085 2023-06-27 16:30:11.000000 bytecore-1.0.1/tests/test_bit.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1106 2023-06-27 16:30:11.000000 bytecore-1.0.1/tests/test_byte.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1707 2023-06-27 16:30:11.000000 bytecore-1.0.1/tests/test_byte_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    15238 2023-06-27 16:30:11.000000 bytecore-1.0.1/tests/test_cpu.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9038 2023-06-27 16:30:11.000000 bytecore-1.0.1/tests/test_emulator.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3238 2023-06-27 16:30:11.000000 bytecore-1.0.1/tests/test_memory.py
```

### Comparing `bytecore-1.0.0/LICENSE` & `bytecore-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/PKG-INFO` & `bytecore-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecore
-Version: 1.0.0
+Version: 1.0.1
 Summary: A minimal, 8-bit CPU emulator designed to help developers explore low-level computing concepts.
 Author-email: Joakim Winum Lien <joakim@winum.xyz>
 Project-URL: Homepage, https://github.com/joakimwinum/bytecore
 Project-URL: Bug Tracker, https://github.com/joakimwinum/bytecore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bytecore-1.0.0/README.md` & `bytecore-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/accumulator.py` & `bytecore-1.0.1/src/bytecore/accumulator.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/bit.py` & `bytecore-1.0.1/src/bytecore/bit.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/byte.py` & `bytecore-1.0.1/src/bytecore/byte.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/byte_register.py` & `bytecore-1.0.1/src/bytecore/byte_register.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/control_unit.py` & `bytecore-1.0.1/src/bytecore/control_unit.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/cpu.py` & `bytecore-1.0.1/src/bytecore/cpu.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/emulator.py` & `bytecore-1.0.1/src/bytecore/emulator.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/memory.py` & `bytecore-1.0.1/src/bytecore/memory.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/proxy_register.py` & `bytecore-1.0.1/src/bytecore/proxy_register.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/replay_register.py` & `bytecore-1.0.1/src/bytecore/replay_register.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore/state.py` & `bytecore-1.0.1/src/bytecore/state.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/src/bytecore.egg-info/PKG-INFO` & `bytecore-1.0.1/src/bytecore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecore
-Version: 1.0.0
+Version: 1.0.1
 Summary: A minimal, 8-bit CPU emulator designed to help developers explore low-level computing concepts.
 Author-email: Joakim Winum Lien <joakim@winum.xyz>
 Project-URL: Homepage, https://github.com/joakimwinum/bytecore
 Project-URL: Bug Tracker, https://github.com/joakimwinum/bytecore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bytecore-1.0.0/src/bytecore.egg-info/SOURCES.txt` & `bytecore-1.0.1/src/bytecore.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/bytecore/control_unit.py
 src/bytecore/control_unit_state.py
 src/bytecore/cpu.py
 src/bytecore/emulator.py
 src/bytecore/memory.py
 src/bytecore/opcode.py
 src/bytecore/proxy_register.py
+src/bytecore/py.typed
 src/bytecore/register.py
 src/bytecore/replay_register.py
 src/bytecore/state.py
 src/bytecore.egg-info/PKG-INFO
 src/bytecore.egg-info/SOURCES.txt
 src/bytecore.egg-info/dependency_links.txt
 src/bytecore.egg-info/top_level.txt
```

### Comparing `bytecore-1.0.0/tests/test_bit.py` & `bytecore-1.0.1/tests/test_bit.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/tests/test_byte.py` & `bytecore-1.0.1/tests/test_byte.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/tests/test_byte_register.py` & `bytecore-1.0.1/tests/test_byte_register.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/tests/test_cpu.py` & `bytecore-1.0.1/tests/test_cpu.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/tests/test_emulator.py` & `bytecore-1.0.1/tests/test_emulator.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.0.0/tests/test_memory.py` & `bytecore-1.0.1/tests/test_memory.py`

 * *Files identical despite different names*

