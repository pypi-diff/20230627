# Comparing `tmp/piwaterflow-0.6.0.tar.gz` & `tmp/piwaterflow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.6.0.tar", last modified: Tue Jun 20 07:22:40 2023, max compression
+gzip compressed data, was "piwaterflow-1.0.0.tar", last modified: Tue Jun 27 17:37:08 2023, max compression
```

## Comparing `piwaterflow-0.6.0.tar` & `piwaterflow-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/piwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/config_waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/piwaterflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/piwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_000_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_001_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_002_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_003_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_004_events.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:37:08.865872 piwaterflow-1.0.0/
+-rw-rw-rw-   0        0        0     1430 2023-06-27 17:37:08.864872 piwaterflow-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-05-05 10:59:47.000000 piwaterflow-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:37:08.802871 piwaterflow-1.0.0/piwaterflow/
+-rw-rw-rw-   0        0        0      122 2023-06-26 12:27:27.000000 piwaterflow-1.0.0/piwaterflow/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-06-19 06:30:06.000000 piwaterflow-1.0.0/piwaterflow/__main__.py
+-rw-rw-rw-   0        0        0      709 2023-06-19 06:30:06.000000 piwaterflow-1.0.0/piwaterflow/config-template.yml
+-rw-rw-rw-   0        0        0     1202 2023-06-19 06:30:06.000000 piwaterflow-1.0.0/piwaterflow/config_waterflow.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:37:08.849870 piwaterflow-1.0.0/piwaterflow/tests/
+-rw-rw-rw-   0        0        0        0 2022-12-20 17:07:56.000000 piwaterflow-1.0.0/piwaterflow/tests/__init__.py
+-rw-rw-rw-   0        0        0      724 2023-05-05 10:59:47.000000 piwaterflow-1.0.0/piwaterflow/tests/test_000.py
+-rw-rw-rw-   0        0        0    24760 2023-06-26 12:25:04.000000 piwaterflow-1.0.0/piwaterflow/waterflow.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:37:08.838871 piwaterflow-1.0.0/piwaterflow.egg-info/
+-rw-rw-rw-   0        0        0     1430 2023-06-27 17:37:08.000000 piwaterflow-1.0.0/piwaterflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-06-27 17:37:08.000000 piwaterflow-1.0.0/piwaterflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:37:08.000000 piwaterflow-1.0.0/piwaterflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-06-27 17:37:08.000000 piwaterflow-1.0.0/piwaterflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-27 17:37:08.000000 piwaterflow-1.0.0/piwaterflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:37:08.865872 piwaterflow-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-06-27 12:45:14.000000 piwaterflow-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:37:08.862872 piwaterflow-1.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-05 10:59:47.000000 piwaterflow-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4975 2023-06-19 06:30:06.000000 piwaterflow-1.0.0/tests/test_000_loop.py
+-rw-rw-rw-   0        0        0     2309 2023-06-19 06:30:06.000000 piwaterflow-1.0.0/tests/test_001_forward.py
+-rw-rw-rw-   0        0        0     2531 2023-06-19 06:30:06.000000 piwaterflow-1.0.0/tests/test_002_reverse.py
+-rw-rw-rw-   0        0        0     1092 2023-05-31 12:49:45.000000 piwaterflow-1.0.0/tests/test_003_lock.py
+-rw-rw-rw-   0        0        0     1100 2023-06-19 06:30:06.000000 piwaterflow-1.0.0/tests/test_004_events.py
```

### Comparing `piwaterflow-0.6.0/PKG-INFO` & `piwaterflow-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: piwaterflow
-Version: 0.6.0
-Summary: Raspberry Pi Waterflow resilient system
-Home-page: https://github.com/Phornee/piwaterflow
-Author: Ismael Raya
-Author-email: phornee@gmail.com
-License: UNKNOWN
-Description: # PiWaterflow
-        This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
-        It's intended to be executed periodically (i.e. cron every 5 minutes).
-        - Requirements:
-          - Raspberry Pi (any model)
-          - Relays to control the valves
-          - Optional control relay to enable alternative power inverter
-        - It supports 2 watering programs every day.
-          - Programs can be forced at any time.
-        - Valves can be manually triggered.
-        - Programs, forced programs and manual Valves can be manually stopped.
-        - Metrics can be emitted to influxdb to register actions (programs and valves).
-        - This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
-        
-        TODO:
-        - Abort watering if humidity is above threshold (90% default). Send email warning
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: piwaterflow
+Version: 1.0.0
+Summary: Raspberry Pi Waterflow resilient system
+Home-page: https://github.com/Phornee/piwaterflow
+Author: Ismael Raya
+Author-email: phornee@gmail.com
+License: UNKNOWN
+Description: # PiWaterflow
+        This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
+        It's intended to be executed periodically (i.e. cron every 5 minutes).
+        - Requirements:
+          - Raspberry Pi (any model)
+          - Relays to control the valves
+          - Optional control relay to enable alternative power inverter
+        - It supports 2 watering programs every day.
+          - Programs can be forced at any time.
+        - Valves can be manually triggered.
+        - Programs, forced programs and manual Valves can be manually stopped.
+        - Metrics can be emitted to influxdb to register actions (programs and valves).
+        - This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
+        
+        TODO:
+        - Abort watering if humidity is above threshold (90% default). Send email warning
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `piwaterflow-0.6.0/README.md` & `piwaterflow-1.0.0/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# PiWaterflow
-This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
-It's intended to be executed periodically (i.e. cron every 5 minutes).
-- Requirements:
-  - Raspberry Pi (any model)
-  - Relays to control the valves
-  - Optional control relay to enable alternative power inverter
-- It supports 2 watering programs every day.
-  - Programs can be forced at any time.
-- Valves can be manually triggered.
-- Programs, forced programs and manual Valves can be manually stopped.
-- Metrics can be emitted to influxdb to register actions (programs and valves).
-- This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
-
-TODO:
+# PiWaterflow
+This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
+It's intended to be executed periodically (i.e. cron every 5 minutes).
+- Requirements:
+  - Raspberry Pi (any model)
+  - Relays to control the valves
+  - Optional control relay to enable alternative power inverter
+- It supports 2 watering programs every day.
+  - Programs can be forced at any time.
+- Valves can be manually triggered.
+- Programs, forced programs and manual Valves can be manually stopped.
+- Metrics can be emitted to influxdb to register actions (programs and valves).
+- This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
+
+TODO:
 - Abort watering if humidity is above threshold (90% default). Send email warning
```

### Comparing `piwaterflow-0.6.0/piwaterflow/config-template.yml` & `piwaterflow-1.0.0/piwaterflow/config-template.yml`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-logpath: log
-loop_freq: 1
-inverter_relay_pin: 31
-external_ac_signal_pin: 10
-programs:
-  - name: first
-    enabled: true
-    start_time: '09:51'
-    valves:
-        - name: main
-          time: 14 # In minutes
-        - name: grass
-          time: 2 # In minutes
-  - name: second
-    enabled: true
-    start_time: '19:04'
-    valves:
-        - name: main
-          time: 0 # In minutes
-        - name: grass
-          time: 2 # In minutes
-valves:
-  main:
-    pin: 33
-  grass:
-    pin: 35
-max_valve_time: 10 # In minutes
-humidity_threshold: 90
-metrics: false
-max_loop_time: 20 # In minutes
-influxdbconn:
-  host: xxxxxxx
-  bucket: xxxxxxx
-  user: xxxxxxx
-  password: xxxxxxx
-
+logpath: log
+loop_freq: 1
+inverter_relay_pin: 31
+external_ac_signal_pin: 10
+programs:
+  - name: first
+    enabled: true
+    start_time: '09:51'
+    valves:
+        - name: main
+          time: 14 # In minutes
+        - name: grass
+          time: 2 # In minutes
+  - name: second
+    enabled: true
+    start_time: '19:04'
+    valves:
+        - name: main
+          time: 0 # In minutes
+        - name: grass
+          time: 2 # In minutes
+valves:
+  main:
+    pin: 33
+  grass:
+    pin: 35
+max_valve_time: 10 # In minutes
+humidity_threshold: 90
+metrics: false
+max_loop_time: 20 # In minutes
+influxdbconn:
+  host: xxxxxxx
+  bucket: xxxxxxx
+  user: xxxxxxx
+  password: xxxxxxx
+
```

### Comparing `piwaterflow-0.6.0/piwaterflow/tests/test_000.py` & `piwaterflow-1.0.0/piwaterflow/tests/test_000.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import unittest
-import os
-import sys
-import inspect
-from pathlib import Path
-
-THIS_FOLDER = os.path.dirname(inspect.getfile(inspect.currentframe()))
-sys.path.insert(0, os.path.dirname(THIS_FOLDER))
-from waterflow import Waterflow  #noqa 
-
-
-class Testing(unittest.TestCase):
-    # templates_path = "{}/templates".format(Path().absolute())
-    # static_path = "{}/static".format(Path().absolute())
-    # service = HomeServices(template_folder=templates_path, static_folder=static_path, db_connector='mock')
-    # client = service.getApp().test_client()
-
-    def test_influx_down(self):
-        pass
-        # self.assertEqual(response.status_code, 200)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+import os
+import sys
+import inspect
+from pathlib import Path
+
+THIS_FOLDER = os.path.dirname(inspect.getfile(inspect.currentframe()))
+sys.path.insert(0, os.path.dirname(THIS_FOLDER))
+from waterflow import Waterflow  #noqa 
+
+
+class Testing(unittest.TestCase):
+    # templates_path = "{}/templates".format(Path().absolute())
+    # static_path = "{}/static".format(Path().absolute())
+    # service = HomeServices(template_folder=templates_path, static_folder=static_path, db_connector='mock')
+    # client = service.getApp().test_client()
+
+    def test_influx_down(self):
+        pass
+        # self.assertEqual(response.status_code, 200)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `piwaterflow-0.6.0/piwaterflow/waterflow.py` & `piwaterflow-1.0.0/piwaterflow/waterflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Loop for watering system. It will properly activate watering valves according to the schedulling set
     in the config file
     All times are local to the watering system location
 """
 import os
+import re
 import time
 import shutil
 from datetime import datetime, timedelta
 from pathlib import Path
 import json
 import logging
 
@@ -19,15 +20,15 @@
 from .config_waterflow import WaterflowConfig
 
 class Waterflow():
     """ Waterflow class that manages a loop system to activate/deactivate watering valves.
         This should run in a raspberry pi or similar, with watering valves connected through relays.
         At this moment it can support up to 2 valves, and 2 different programs alnog the day.
         Those programs/valves can be switched on/off in a forced way apart from the programs.
-        This is autonomous, and could be controlled by directly changing the programs´configuration in the
+        This is autonomous, and could be controlled by directly changing the programs' configuration in the
         config.yml file.
         However, it can work together with the piwwwwaterflow package that serves a http page to remotely control
         the waterflow system.
     """
     def __init__(self, template_config_path: str = None, fake_now: datetime = None, dry_run: bool = False):
         """__init__ of the function
         Args:
@@ -555,7 +556,20 @@
                 self._add_event('Exception', str(ex))
                 raise RuntimeError(ex) from ex
             finally:
                 GPIO.cleanup()
                 self.release_lock()
         else:
             self.logger.error('Loop executed while locked by previous execution.')
+
+    @classmethod
+    def get_version(cls) -> str:
+        """ Gets version string from the init file
+        Returns:
+            str: Version string
+        """
+        version_file = os.path.join(Path(__file__).parent.resolve(), '__init__.py')
+        with open(version_file, 'r',  encoding="utf-8") as initfile_lines:
+            content = initfile_lines.read()
+            version = re.search(r'__version__ = ["|\'](.*?)["|\']', content).group(1)
+            return version
+        raise RuntimeError(f'Unable to find version string in {version_file}.')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `piwaterflow-0.6.0/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-1.0.0/piwaterflow.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: piwaterflow
-Version: 0.6.0
-Summary: Raspberry Pi Waterflow resilient system
-Home-page: https://github.com/Phornee/piwaterflow
-Author: Ismael Raya
-Author-email: phornee@gmail.com
-License: UNKNOWN
-Description: # PiWaterflow
-        This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
-        It's intended to be executed periodically (i.e. cron every 5 minutes).
-        - Requirements:
-          - Raspberry Pi (any model)
-          - Relays to control the valves
-          - Optional control relay to enable alternative power inverter
-        - It supports 2 watering programs every day.
-          - Programs can be forced at any time.
-        - Valves can be manually triggered.
-        - Programs, forced programs and manual Valves can be manually stopped.
-        - Metrics can be emitted to influxdb to register actions (programs and valves).
-        - This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
-        
-        TODO:
-        - Abort watering if humidity is above threshold (90% default). Send email warning
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: piwaterflow
+Version: 1.0.0
+Summary: Raspberry Pi Waterflow resilient system
+Home-page: https://github.com/Phornee/piwaterflow
+Author: Ismael Raya
+Author-email: phornee@gmail.com
+License: UNKNOWN
+Description: # PiWaterflow
+        This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
+        It's intended to be executed periodically (i.e. cron every 5 minutes).
+        - Requirements:
+          - Raspberry Pi (any model)
+          - Relays to control the valves
+          - Optional control relay to enable alternative power inverter
+        - It supports 2 watering programs every day.
+          - Programs can be forced at any time.
+        - Valves can be manually triggered.
+        - Programs, forced programs and manual Valves can be manually stopped.
+        - Metrics can be emitted to influxdb to register actions (programs and valves).
+        - This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
+        
+        TODO:
+        - Abort watering if humidity is above threshold (90% default). Send email warning
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `piwaterflow-0.6.0/piwaterflow.egg-info/SOURCES.txt` & `piwaterflow-1.0.0/piwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.6.0/tests/test_000_loop.py` & `piwaterflow-1.0.0/tests/test_000_loop.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-""" Unittesting """
-import unittest
-from pathlib import Path
-import gc
-
-from piwaterflow import Waterflow
-
-
-class Testing(unittest.TestCase):
-    """ Unittesting class
-    """
-    def setUp(self):
-        template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
-        self.waterflow = Waterflow(template_config_path=template_config_path, dry_run=True)
-
-    def tearDown(self):
-        del self.waterflow
-        gc.collect()
-
-    def test_0000_loop_noprog(self):
-        """ Test the loop and main high-level functionalities. No program will run at that time
-        """
-        self.waterflow.loop(Waterflow.str_to_time('2023-05-27 08:30:00'))
-
-        events = self.waterflow._read_events() # pylint: disable=protected-access
-        if events:
-            self.assertEqual(len(events), 1)
-            self.assertTrue(events[0][1] == "LastProg" and events[0][2] == "2023-05-27 09:51:00")
-        else:
-            self.fail("not the right events generated.")
-
-    def test_0001_loop_prog(self):
-        """ Test the loop and main high-level functionalities. Program will run at that time
-        """
-        self.waterflow._write_last_program_time(Waterflow.str_to_time('2023-05-26 23:59:00')) # pylint: disable=protected-access
-        self.waterflow.loop(Waterflow.str_to_time('2023-05-27 09:52:00'))
-
-        events = self.waterflow._read_events() # pylint: disable=protected-access
-        if events:
-            self.assertEqual(len(events), 8)
-            self.assertTrue(events[0][1] == "ExecProg" and events[0][2] == "first")
-            self.assertTrue(events[1][1] == "InverterON" and events[1][2] is None)
-            self.assertTrue(events[2][1] == "ValveON" and events[2][2] == "main")
-            self.assertTrue(events[3][1] == "ValveOFF" and events[3][2] == "main")
-            self.assertTrue(events[4][1] == "ValveON" and events[4][2] == "grass")
-            self.assertTrue(events[5][1] == "ValveOFF" and events[5][2] == "grass")
-            self.assertTrue(events[6][1] == "InverterOFF" and events[6][2] is None)
-            self.assertTrue(events[7][1] == "LastProg" and events[7][2] == "2023-05-27 19:04:00")
-        else:
-            self.fail("not the right events generated.")
-
-    def test_0002_loop_prog_forced(self):
-        """ Test the loop and main high-level functionalities. Program will run at that time
-        """
-        self.waterflow._write_last_program_time(Waterflow.str_to_time('2023-05-26 23:59:00')) # pylint: disable=protected-access
-        self.waterflow.force('program', 'first')
-        self.waterflow.loop(Waterflow.str_to_time('2023-05-27 09:52:00'))
-
-        events = self.waterflow._read_events() # pylint: disable=protected-access
-        if events:
-            self.assertEqual(len(events), 9)
-            self.assertTrue(events[0][1] == "ForcedProg" and events[0][2] == "first")
-            self.assertTrue(events[1][1] == "ExecProg" and events[1][2] == "first")
-            self.assertTrue(events[2][1] == "InverterON" and events[2][2] is None)
-            self.assertTrue(events[3][1] == "ValveON" and events[3][2] == "main")
-            self.assertTrue(events[4][1] == "ValveOFF" and events[4][2] == "main")
-            self.assertTrue(events[5][1] == "ValveON" and events[5][2] == "grass")
-            self.assertTrue(events[6][1] == "ValveOFF" and events[6][2] == "grass")
-            self.assertTrue(events[7][1] == "InverterOFF" and events[7][2] is None)
-            self.assertTrue(events[8][1] == "LastProg" and events[8][2] == "2023-05-27 19:04:00")
-        else:
-            self.fail("not the right events generated.")
-
-    def test_0003_loop_valve_forced(self):
-        """ Test the loop and main high-level functionalities. Program will run at that time
-        """
-        self.waterflow._write_last_program_time(Waterflow.str_to_time('2023-05-26 23:59:00')) # pylint: disable=protected-access
-        self.waterflow.force('valve', 'grass')
-        self.waterflow.loop(Waterflow.str_to_time('2023-05-27 09:52:00'))
-
-        events = self.waterflow._read_events() # pylint: disable=protected-access
-        if events:
-            self.assertEqual(len(events), 7)
-            self.assertTrue(events[0][1] == "ForcedValve" and events[0][2] == "grass")
-            self.assertTrue(events[1][1] == "ExecValve" and events[1][2] == "grass")
-            self.assertTrue(events[2][1] == "InverterON" and events[2][2] is None)
-            self.assertTrue(events[3][1] == "ValveON" and events[3][2] == "grass")
-            self.assertTrue(events[4][1] == "ValveOFF" and events[4][2] == "grass")
-            self.assertTrue(events[5][1] == "InverterOFF" and events[5][2] is None)
-            self.assertTrue(events[6][1] == "LastProg" and events[6][2] == "2023-05-27 19:04:00")
-        else:
-            self.fail("not the right events generated.")
-
-if __name__ == '__main__':
-    unittest.main()
-
+""" Unittesting """
+import unittest
+from pathlib import Path
+import gc
+
+from piwaterflow import Waterflow
+
+
+class Testing(unittest.TestCase):
+    """ Unittesting class
+    """
+    def setUp(self):
+        template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
+        self.waterflow = Waterflow(template_config_path=template_config_path, dry_run=True)
+
+    def tearDown(self):
+        del self.waterflow
+        gc.collect()
+
+    def test_0000_loop_noprog(self):
+        """ Test the loop and main high-level functionalities. No program will run at that time
+        """
+        self.waterflow.loop(Waterflow.str_to_time('2023-05-27 08:30:00'))
+
+        events = self.waterflow._read_events() # pylint: disable=protected-access
+        if events:
+            self.assertEqual(len(events), 1)
+            self.assertTrue(events[0][1] == "LastProg" and events[0][2] == "2023-05-27 09:51:00")
+        else:
+            self.fail("not the right events generated.")
+
+    def test_0001_loop_prog(self):
+        """ Test the loop and main high-level functionalities. Program will run at that time
+        """
+        self.waterflow._write_last_program_time(Waterflow.str_to_time('2023-05-26 23:59:00')) # pylint: disable=protected-access
+        self.waterflow.loop(Waterflow.str_to_time('2023-05-27 09:52:00'))
+
+        events = self.waterflow._read_events() # pylint: disable=protected-access
+        if events:
+            self.assertEqual(len(events), 8)
+            self.assertTrue(events[0][1] == "ExecProg" and events[0][2] == "first")
+            self.assertTrue(events[1][1] == "InverterON" and events[1][2] is None)
+            self.assertTrue(events[2][1] == "ValveON" and events[2][2] == "main")
+            self.assertTrue(events[3][1] == "ValveOFF" and events[3][2] == "main")
+            self.assertTrue(events[4][1] == "ValveON" and events[4][2] == "grass")
+            self.assertTrue(events[5][1] == "ValveOFF" and events[5][2] == "grass")
+            self.assertTrue(events[6][1] == "InverterOFF" and events[6][2] is None)
+            self.assertTrue(events[7][1] == "LastProg" and events[7][2] == "2023-05-27 19:04:00")
+        else:
+            self.fail("not the right events generated.")
+
+    def test_0002_loop_prog_forced(self):
+        """ Test the loop and main high-level functionalities. Program will run at that time
+        """
+        self.waterflow._write_last_program_time(Waterflow.str_to_time('2023-05-26 23:59:00')) # pylint: disable=protected-access
+        self.waterflow.force('program', 'first')
+        self.waterflow.loop(Waterflow.str_to_time('2023-05-27 09:52:00'))
+
+        events = self.waterflow._read_events() # pylint: disable=protected-access
+        if events:
+            self.assertEqual(len(events), 9)
+            self.assertTrue(events[0][1] == "ForcedProg" and events[0][2] == "first")
+            self.assertTrue(events[1][1] == "ExecProg" and events[1][2] == "first")
+            self.assertTrue(events[2][1] == "InverterON" and events[2][2] is None)
+            self.assertTrue(events[3][1] == "ValveON" and events[3][2] == "main")
+            self.assertTrue(events[4][1] == "ValveOFF" and events[4][2] == "main")
+            self.assertTrue(events[5][1] == "ValveON" and events[5][2] == "grass")
+            self.assertTrue(events[6][1] == "ValveOFF" and events[6][2] == "grass")
+            self.assertTrue(events[7][1] == "InverterOFF" and events[7][2] is None)
+            self.assertTrue(events[8][1] == "LastProg" and events[8][2] == "2023-05-27 19:04:00")
+        else:
+            self.fail("not the right events generated.")
+
+    def test_0003_loop_valve_forced(self):
+        """ Test the loop and main high-level functionalities. Program will run at that time
+        """
+        self.waterflow._write_last_program_time(Waterflow.str_to_time('2023-05-26 23:59:00')) # pylint: disable=protected-access
+        self.waterflow.force('valve', 'grass')
+        self.waterflow.loop(Waterflow.str_to_time('2023-05-27 09:52:00'))
+
+        events = self.waterflow._read_events() # pylint: disable=protected-access
+        if events:
+            self.assertEqual(len(events), 7)
+            self.assertTrue(events[0][1] == "ForcedValve" and events[0][2] == "grass")
+            self.assertTrue(events[1][1] == "ExecValve" and events[1][2] == "grass")
+            self.assertTrue(events[2][1] == "InverterON" and events[2][2] is None)
+            self.assertTrue(events[3][1] == "ValveON" and events[3][2] == "grass")
+            self.assertTrue(events[4][1] == "ValveOFF" and events[4][2] == "grass")
+            self.assertTrue(events[5][1] == "InverterOFF" and events[5][2] is None)
+            self.assertTrue(events[6][1] == "LastProg" and events[6][2] == "2023-05-27 19:04:00")
+        else:
+            self.fail("not the right events generated.")
+
+if __name__ == '__main__':
+    unittest.main()
+
```

### Comparing `piwaterflow-0.6.0/tests/test_001_forward.py` & `piwaterflow-1.0.0/tests/test_001_forward.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-""" Unittesting """
-import unittest
-from pathlib import Path
-from datetime import datetime
-
-from piwaterflow import Waterflow
-
-
-class Testing(unittest.TestCase):
-    """ Unittesting class
-    """
-    def setUp(self):
-        template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
-        self.waterflow = Waterflow(template_config_path=template_config_path,
-                                   fake_now = Waterflow.str_to_time('2023-04-27 00:01:00'),
-                                   dry_run=True)
-
-    def test_0011_recalc_next_program(self):
-        """ Test the recalc_next_program function
-        """
-        last_program_time = Waterflow.str_to_time('2023-04-26 23:30:27')
-        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
-        self.assertTrue(time_prog == datetime(2023, 4, 27, 9, 51).astimezone())
-        self.assertTrue(program_name == 'first')
-
-        # Checks if _recalc_next_program works fine if last_program is today before first program
-        last_program_time = Waterflow.str_to_time('2023-04-27 00:30:00')
-        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
-        self.assertTrue(time_prog == datetime(2023, 4, 27, 9, 51).astimezone())
-        self.assertTrue(program_name == 'first')
-
-        # Checks if _recalc_next_program works fine if last_program is between two programs
-        last_program_time = Waterflow.str_to_time('2023-04-27 10:30:00')
-        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
-        self.assertTrue(time_prog == datetime(2023, 4, 27, 19, 4).astimezone())
-        self.assertTrue(program_name == 'second')
-
-        # Checks if _recalc_next_program works fine if last_program is after all  programs
-        last_program_time = Waterflow.str_to_time('2023-04-27 23:59:00')
-        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
-        self.assertTrue(time_prog == datetime(2023, 4, 28, 9, 51).astimezone())
-        self.assertTrue(program_name == 'first')
-
-if __name__ == '__main__':
-    unittest.main()
+""" Unittesting """
+import unittest
+from pathlib import Path
+from datetime import datetime
+
+from piwaterflow import Waterflow
+
+
+class Testing(unittest.TestCase):
+    """ Unittesting class
+    """
+    def setUp(self):
+        template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
+        self.waterflow = Waterflow(template_config_path=template_config_path,
+                                   fake_now = Waterflow.str_to_time('2023-04-27 00:01:00'),
+                                   dry_run=True)
+
+    def test_0011_recalc_next_program(self):
+        """ Test the recalc_next_program function
+        """
+        last_program_time = Waterflow.str_to_time('2023-04-26 23:30:27')
+        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
+        self.assertTrue(time_prog == datetime(2023, 4, 27, 9, 51).astimezone())
+        self.assertTrue(program_name == 'first')
+
+        # Checks if _recalc_next_program works fine if last_program is today before first program
+        last_program_time = Waterflow.str_to_time('2023-04-27 00:30:00')
+        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
+        self.assertTrue(time_prog == datetime(2023, 4, 27, 9, 51).astimezone())
+        self.assertTrue(program_name == 'first')
+
+        # Checks if _recalc_next_program works fine if last_program is between two programs
+        last_program_time = Waterflow.str_to_time('2023-04-27 10:30:00')
+        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
+        self.assertTrue(time_prog == datetime(2023, 4, 27, 19, 4).astimezone())
+        self.assertTrue(program_name == 'second')
+
+        # Checks if _recalc_next_program works fine if last_program is after all  programs
+        last_program_time = Waterflow.str_to_time('2023-04-27 23:59:00')
+        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
+        self.assertTrue(time_prog == datetime(2023, 4, 28, 9, 51).astimezone())
+        self.assertTrue(program_name == 'first')
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `piwaterflow-0.6.0/tests/test_002_reverse.py` & `piwaterflow-1.0.0/tests/test_002_reverse.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-""" Unittesting """
-import unittest
-from pathlib import Path
-from datetime import datetime
-
-from piwaterflow import Waterflow
-
-
-class Testing(unittest.TestCase):
-    """ Unittesting class
-    """
-    def setUp(self):
-        template_config_path = f'{Path(__file__).parent}/data/config-template_reverse.yml'
-        self.waterflow = Waterflow(template_config_path=template_config_path, 
-                                   fake_now=Waterflow.str_to_time('2023-04-27 00:01:00'),
-                                   dry_run=True)
-
-    def test_0021_recalc_next_program(self):
-        """ Test the recalc_next_program function
-        """
-        # Checks if _recalc_next_program works fine if last_program was "yesterday"
-        last_program_time_utc = Waterflow.str_to_time('2023-04-26 23:30:27')
-        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
-        self.assertTrue(time_utc == datetime(2023, 4, 27, 5, 6).astimezone())
-        self.assertTrue(program_name == 'second')
-
-        # Checks if _recalc_next_program works fine if last_program is today before first program
-        last_program_time_utc = Waterflow.str_to_time('2023-04-27 00:30:00') # pylint: disable=protected-access
-        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
-        self.assertTrue(time_utc == datetime(2023, 4, 27, 5, 6).astimezone())
-        self.assertTrue(program_name == 'second')
-
-        # Checks if _recalc_next_program works fine if last_program is between two programs
-        last_program_time_utc = Waterflow.str_to_time('2023-04-27 10:30:00') # pylint: disable=protected-access
-        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
-        self.assertTrue(time_utc == datetime(2023, 4, 27, 23, 30).astimezone())
-        self.assertTrue(program_name == 'first')
-
-        # Checks if _recalc_next_program works fine if last_program is after all  programs
-        last_program_time_utc = Waterflow.str_to_time('2023-04-27 23:59:00') # pylint: disable=protected-access
-        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
-        self.assertTrue(time_utc == datetime(2023, 4, 28, 5, 6,).astimezone())
-        self.assertTrue(program_name == 'second')
-
-if __name__ == '__main__':
-    unittest.main()
+""" Unittesting """
+import unittest
+from pathlib import Path
+from datetime import datetime
+
+from piwaterflow import Waterflow
+
+
+class Testing(unittest.TestCase):
+    """ Unittesting class
+    """
+    def setUp(self):
+        template_config_path = f'{Path(__file__).parent}/data/config-template_reverse.yml'
+        self.waterflow = Waterflow(template_config_path=template_config_path, 
+                                   fake_now=Waterflow.str_to_time('2023-04-27 00:01:00'),
+                                   dry_run=True)
+
+    def test_0021_recalc_next_program(self):
+        """ Test the recalc_next_program function
+        """
+        # Checks if _recalc_next_program works fine if last_program was "yesterday"
+        last_program_time_utc = Waterflow.str_to_time('2023-04-26 23:30:27')
+        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
+        self.assertTrue(time_utc == datetime(2023, 4, 27, 5, 6).astimezone())
+        self.assertTrue(program_name == 'second')
+
+        # Checks if _recalc_next_program works fine if last_program is today before first program
+        last_program_time_utc = Waterflow.str_to_time('2023-04-27 00:30:00') # pylint: disable=protected-access
+        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
+        self.assertTrue(time_utc == datetime(2023, 4, 27, 5, 6).astimezone())
+        self.assertTrue(program_name == 'second')
+
+        # Checks if _recalc_next_program works fine if last_program is between two programs
+        last_program_time_utc = Waterflow.str_to_time('2023-04-27 10:30:00') # pylint: disable=protected-access
+        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
+        self.assertTrue(time_utc == datetime(2023, 4, 27, 23, 30).astimezone())
+        self.assertTrue(program_name == 'first')
+
+        # Checks if _recalc_next_program works fine if last_program is after all  programs
+        last_program_time_utc = Waterflow.str_to_time('2023-04-27 23:59:00') # pylint: disable=protected-access
+        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
+        self.assertTrue(time_utc == datetime(2023, 4, 28, 5, 6,).astimezone())
+        self.assertTrue(program_name == 'second')
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `piwaterflow-0.6.0/tests/test_004_events.py` & `piwaterflow-1.0.0/tests/test_004_events.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-""" Unittesting """
-import unittest
-from pathlib import Path
-import gc
-
-from piwaterflow import Waterflow
-
-
-class Testing(unittest.TestCase):
-    """ Unittesting class
-    """
-    def setUp(self):
-        template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
-        self.waterflow = Waterflow(template_config_path=template_config_path, dry_run=True)
-
-    def tearDown(self):
-        del self.waterflow
-        gc.collect()
-
-    def test_0000_read_write_events(self):
-        """ Test the loop and main high-level functionalities. No program will run at that time
-        """
-        self.waterflow._add_event('LastProg', '2023-05-27 09:51:00') # pylint: disable=protected-access
-
-        events = self.waterflow._read_events() # pylint: disable=protected-access
-        if events:
-            self.assertEqual(len(events), 1)
-            self.assertTrue(events[0][1] == "LastProg" and events[0][2] == "2023-05-27 09:51:00")
-        else:
-            self.fail("not the right events generated.")
-
-if __name__ == '__main__':
-    unittest.main()
-
+""" Unittesting """
+import unittest
+from pathlib import Path
+import gc
+
+from piwaterflow import Waterflow
+
+
+class Testing(unittest.TestCase):
+    """ Unittesting class
+    """
+    def setUp(self):
+        template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
+        self.waterflow = Waterflow(template_config_path=template_config_path, dry_run=True)
+
+    def tearDown(self):
+        del self.waterflow
+        gc.collect()
+
+    def test_0000_read_write_events(self):
+        """ Test the loop and main high-level functionalities. No program will run at that time
+        """
+        self.waterflow._add_event('LastProg', '2023-05-27 09:51:00') # pylint: disable=protected-access
+
+        events = self.waterflow._read_events() # pylint: disable=protected-access
+        if events:
+            self.assertEqual(len(events), 1)
+            self.assertTrue(events[0][1] == "LastProg" and events[0][2] == "2023-05-27 09:51:00")
+        else:
+            self.fail("not the right events generated.")
+
+if __name__ == '__main__':
+    unittest.main()
+
```

