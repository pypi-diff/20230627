# Comparing `tmp/pydwm1001-0.1.1.tar.gz` & `tmp/pydwm1001-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwm1001-0.1.1.tar", last modified: Thu Jun 22 20:18:36 2023, max compression
+gzip compressed data, was "pydwm1001-0.2.0.tar", last modified: Tue Jun 27 19:48:14 2023, max compression
```

## Comparing `pydwm1001-0.1.1.tar` & `pydwm1001-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-22 20:18:36.056072 pydwm1001-0.1.1/
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     1111 2023-06-21 13:38:46.000000 pydwm1001-0.1.1/LICENSE
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      637 2023-06-22 20:18:36.056072 pydwm1001-0.1.1/PKG-INFO
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      103 2023-06-21 13:38:46.000000 pydwm1001-0.1.1/README.md
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     3691 2023-06-22 15:03:34.000000 pydwm1001-0.1.1/dwm1001.py
-drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-22 20:18:36.056072 pydwm1001-0.1.1/pydwm1001.egg-info/
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      637 2023-06-22 20:18:36.000000 pydwm1001-0.1.1/pydwm1001.egg-info/PKG-INFO
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      229 2023-06-22 20:18:36.000000 pydwm1001-0.1.1/pydwm1001.egg-info/SOURCES.txt
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        1 2023-06-22 20:18:36.000000 pydwm1001-0.1.1/pydwm1001.egg-info/dependency_links.txt
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        9 2023-06-22 20:18:36.000000 pydwm1001-0.1.1/pydwm1001.egg-info/requires.txt
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        8 2023-06-22 20:18:36.000000 pydwm1001-0.1.1/pydwm1001.egg-info/top_level.txt
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      640 2023-06-22 20:16:21.000000 pydwm1001-0.1.1/pyproject.toml
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)       38 2023-06-22 20:18:36.056072 pydwm1001-0.1.1/setup.cfg
-drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-22 20:18:36.056072 pydwm1001-0.1.1/tests/
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     2745 2023-06-22 15:03:34.000000 pydwm1001-0.1.1/tests/test_dwm1001.py
+drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     1111 2023-06-21 13:38:46.000000 pydwm1001-0.2.0/LICENSE
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      637 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/PKG-INFO
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      103 2023-06-21 13:38:46.000000 pydwm1001-0.2.0/README.md
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     4194 2023-06-27 19:29:56.000000 pydwm1001-0.2.0/dwm1001.py
+drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/pydwm1001.egg-info/
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      637 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/PKG-INFO
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      229 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/SOURCES.txt
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        1 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/dependency_links.txt
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        9 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/requires.txt
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        8 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/top_level.txt
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      640 2023-06-27 19:29:56.000000 pydwm1001-0.2.0/pyproject.toml
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)       38 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/setup.cfg
+drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/tests/
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     2745 2023-06-22 15:03:34.000000 pydwm1001-0.2.0/tests/test_dwm1001.py
```

### Comparing `pydwm1001-0.1.1/LICENSE` & `pydwm1001-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwm1001-0.1.1/PKG-INFO` & `pydwm1001-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.1.1/dwm1001.py` & `pydwm1001-0.2.0/dwm1001.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,25 +105,39 @@
 
         position_data = [float(substr) for substr in report[3:6]]
         position_data.append(int(report[6]))
 
         return TagId(report[2]), TagPosition(*position_data)
 
 
-class Tag:
+class Tag(UartDwm1001):
     def __init__(self, serial_handle) -> None:
         self.serial_handle = serial_handle
 
-        self.serial_handle.write(ShellCommand.DOUBLE_ENTER.value)
-        time.sleep(1)
-        self.serial_handle.write(ShellCommand.LEP)
+        # Device may not have shutdown properly previously
+        self.reset()
+        self.enter_shell_mode()
+
+    def start_position_reporting(self) -> None:
+        self.send_shell_command(ShellCommand.LEP)
+
+        # The first line after invoking the command will have part of
+        # the shell prompt mixed in, which would mess up parsing.
+        self.serial_handle.reset_input_buffer()
+
+    def stop_position_reporting(self) -> None:
+        self.send_shell_command(ShellCommand.ENTER)
 
     @property
     def position(self) -> TagPosition:
         report = self.serial_handle.readline().decode().split(",")
 
-        if len(report) != 5 or report[0] != "POS":
-            raise ValueError("Could not parse position report.")
+        if len(report) != 5:
+            raise ParsingError("Position report has unexpected length.")
+
+        if report[0] != "POS":
+            raise ParsingError("Position report has incorrect tag.")
 
-        position_data = [float(substr) for substr in report[1:]]
+        position_data = [float(substr) for substr in report[1:4]]
+        position_data.append(int(report[4]))
 
         return TagPosition(*position_data)
```

### Comparing `pydwm1001-0.1.1/pydwm1001.egg-info/PKG-INFO` & `pydwm1001-0.2.0/pydwm1001.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.1.1/pyproject.toml` & `pydwm1001-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydwm1001"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Adam Morrissett", email="morrissettal2@vcu.edu" },
 ]
 description = "A Python library for interfacing with DWM1001"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pydwm1001-0.1.1/tests/test_dwm1001.py` & `pydwm1001-0.2.0/tests/test_dwm1001.py`

 * *Files identical despite different names*

