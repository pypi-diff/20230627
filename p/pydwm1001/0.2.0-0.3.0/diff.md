# Comparing `tmp/pydwm1001-0.2.0.tar.gz` & `tmp/pydwm1001-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwm1001-0.2.0.tar", last modified: Tue Jun 27 19:48:14 2023, max compression
+gzip compressed data, was "pydwm1001-0.3.0.tar", last modified: Tue Jun 27 21:18:11 2023, max compression
```

## Comparing `pydwm1001-0.2.0.tar` & `pydwm1001-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     1111 2023-06-21 13:38:46.000000 pydwm1001-0.2.0/LICENSE
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      637 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/PKG-INFO
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      103 2023-06-21 13:38:46.000000 pydwm1001-0.2.0/README.md
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     4194 2023-06-27 19:29:56.000000 pydwm1001-0.2.0/dwm1001.py
-drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/pydwm1001.egg-info/
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      637 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/PKG-INFO
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      229 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/SOURCES.txt
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        1 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/dependency_links.txt
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        9 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/requires.txt
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        8 2023-06-27 19:48:14.000000 pydwm1001-0.2.0/pydwm1001.egg-info/top_level.txt
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      640 2023-06-27 19:29:56.000000 pydwm1001-0.2.0/pyproject.toml
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)       38 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/setup.cfg
-drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 19:48:14.783946 pydwm1001-0.2.0/tests/
--rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     2745 2023-06-22 15:03:34.000000 pydwm1001-0.2.0/tests/test_dwm1001.py
+drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 21:18:11.542565 pydwm1001-0.3.0/
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     1111 2023-06-21 13:38:46.000000 pydwm1001-0.3.0/LICENSE
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      637 2023-06-27 21:18:11.542565 pydwm1001-0.3.0/PKG-INFO
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      103 2023-06-21 13:38:46.000000 pydwm1001-0.3.0/README.md
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     4861 2023-06-27 21:16:08.000000 pydwm1001-0.3.0/dwm1001.py
+drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 21:18:11.542565 pydwm1001-0.3.0/pydwm1001.egg-info/
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      637 2023-06-27 21:18:11.000000 pydwm1001-0.3.0/pydwm1001.egg-info/PKG-INFO
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      229 2023-06-27 21:18:11.000000 pydwm1001-0.3.0/pydwm1001.egg-info/SOURCES.txt
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        1 2023-06-27 21:18:11.000000 pydwm1001-0.3.0/pydwm1001.egg-info/dependency_links.txt
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        9 2023-06-27 21:18:11.000000 pydwm1001-0.3.0/pydwm1001.egg-info/requires.txt
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)        8 2023-06-27 21:18:11.000000 pydwm1001-0.3.0/pydwm1001.egg-info/top_level.txt
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)      640 2023-06-27 21:16:08.000000 pydwm1001-0.3.0/pyproject.toml
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)       38 2023-06-27 21:18:11.542565 pydwm1001-0.3.0/setup.cfg
+drwx------   0 morrissettal2 (299664333) morrissettal2 (299664333)        0 2023-06-27 21:18:11.542565 pydwm1001-0.3.0/tests/
+-rw-------   0 morrissettal2 (299664333) morrissettal2 (299664333)     2745 2023-06-22 15:03:34.000000 pydwm1001-0.3.0/tests/test_dwm1001.py
```

### Comparing `pydwm1001-0.2.0/LICENSE` & `pydwm1001-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwm1001-0.2.0/PKG-INFO` & `pydwm1001-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.2.0/dwm1001.py` & `pydwm1001-0.3.0/dwm1001.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,19 +25,25 @@
             math.isclose(self.x_m, other.x_m)
             and math.isclose(self.y_m, other.y_m)
             and math.isclose(self.z_m, other.z_m)
             and self.quality == other.quality
         )
 
 
+@dataclass
+class SystemInfo:
+    address: int
+
+
 class ShellCommand(Enum):
     ENTER = b"\r"
     DOUBLE_ENTER = b"\r\r"
     LEP = b"lep"
     RESET = b"reset"
+    SI = b"si"  # System info
 
 
 class ParsingError(Exception):
     pass
 
 
 class UartDwm1001:
@@ -62,14 +68,15 @@
         time.sleep(self.RESET_DELAY_PERIOD)
 
     def enter_shell_mode(self) -> None:
         self.serial_handle.write(ShellCommand.DOUBLE_ENTER.value)
         self.serial_handle.flush()
 
         time.sleep(self.SHELL_STARTUP_DELAY_PERIOD)
+        self.serial_handle.reset_input_buffer()
 
     def exit_shell_mode(self) -> None:
         # If you quit shell mode (with `quit` command) without stopping
         # a running command, the command will automatically continue
         # when re-entering shell mode. This can be confusing, so we
         # reset the device instead to ensure previously-running commands
         # terminate.
@@ -124,14 +131,30 @@
         # the shell prompt mixed in, which would mess up parsing.
         self.serial_handle.reset_input_buffer()
 
     def stop_position_reporting(self) -> None:
         self.send_shell_command(ShellCommand.ENTER)
 
     @property
+    def tag_id(self) -> str:
+        self.send_shell_command(ShellCommand.SI)
+
+        report = []
+        for _ in range(9):
+            report.append(self.serial_handle.readline().decode())
+
+        # System info has a lot of lines, but we only care about the address
+        address_line = report[2]
+        address_text_start = address_line.find("addr=")
+        address_string = address_line[address_text_start:-1].strip()
+
+        # We only use the last four characters in the address
+        return address_string[-4:]
+
+    @property
     def position(self) -> TagPosition:
         report = self.serial_handle.readline().decode().split(",")
 
         if len(report) != 5:
             raise ParsingError("Position report has unexpected length.")
 
         if report[0] != "POS":
```

### Comparing `pydwm1001-0.2.0/pydwm1001.egg-info/PKG-INFO` & `pydwm1001-0.3.0/pydwm1001.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.2.0/pyproject.toml` & `pydwm1001-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydwm1001"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Adam Morrissett", email="morrissettal2@vcu.edu" },
 ]
 description = "A Python library for interfacing with DWM1001"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pydwm1001-0.2.0/tests/test_dwm1001.py` & `pydwm1001-0.3.0/tests/test_dwm1001.py`

 * *Files identical despite different names*

