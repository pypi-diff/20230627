# Comparing `tmp/ahoy_dtu_webthing-0.0.9.tar.gz` & `tmp/ahoy_dtu_webthing-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.0.9.tar", last modified: Mon Jun 19 20:37:29 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.1.0.tar", last modified: Tue Jun 27 04:44:20 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.0.9.tar` & `ahoy_dtu_webthing-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.0.9/LICENSE` & `ahoy_dtu_webthing-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.9/PKG-INFO` & `ahoy_dtu_webthing-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.0.9
+Version: 0.1.0
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.0.9/README.md` & `ahoy_dtu_webthing-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/dtu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,73 @@
 from threading import Thread
 import re
 import requests
+import logging
 from time import sleep
 from datetime import datetime
 
 class Inverter:
 
-    def __init__(self, base_uri: str, id: int, channels: int, name: str, serial: str):
+    def __init__(self, base_uri: str, id: int, channels: int, name: str, serial: str, interval: int):
+        self.is_running = True
         self.update_uri = re.sub("^/|/$", "", base_uri) + '/api/ctrl'
         self.uri = re.sub("^/|/$", "", base_uri) + '/api/record/live'
         self.index_uri = re.sub("^/|/$", "", base_uri) + '/api/index'
         self.config_uri = re.sub("^/|/$", "", base_uri) + '/api/record/config'
         self.inverter_uri = re.sub("^/|/$", "", base_uri) + '/api/inverter/list'
 
         self.id = id
         self.channel = channels
         self.name = name
         self.serial = serial
+        self.interval = interval
         self.p_dc = 0
+        self.u_dc1 = 0
+        self.u_dc2 = 0
+        self.i_dc1 = 0
+        self.i_dc2 = 0
         self.p_ac = 0
         self.u_ac = 0
         self.i_ac = 0
         self.temp = 0
+        self.frequency = 0
         self.efficiency = 0
         self.power_max = 0
         self.power_limit = 0
         self.last_update = datetime.fromtimestamp(0)
         self.is_available = False
         self.is_producing = False
         self.listener = None
-        self.refresh()
-        self.set_power_limit(self.power_max)
+        Thread(target=self.__periodic_refresh, daemon=True).start()
+
+    def close(self):
+        self.is_running = False
+
+    def __periodic_refresh(self):
+        while self.is_running:
+            try:
+                self.refresh()
+            except Exception as e:
+                logging.warning("error occurred refreshing inverter " + self.name + " " + str(e) + " (max " + str(self.power_max) + " watt)")
+            sleep(self.interval)
 
     def refresh(self):
-       # fetch inverter info
+        # fetch inverter info
         response = requests.get(self.index_uri)
         inverter_state = response.json()['inverter']
 
+        previous_is_available = self.is_available
         self.is_available = inverter_state[self.id]['is_avail']
+        if previous_is_available != self.is_available:
+            logging.info("inverter " + str(self.name) + " is " + ("" if self.is_available else "not ") + "available")
+
+        previous_is_producing = self.is_producing
         self.is_producing = inverter_state[self.id]['is_producing']
+        if previous_is_producing != self.is_producing:
+            logging.info("inverter " + str(self.name) + " is " + ("" if self.is_producing else "not ") + "producing")
 
         if self.is_producing:
             # fetch power limit
             response = requests.get(self.config_uri)
             inverter_configs = response.json()['inverter']
 
             # fetch inverter info
@@ -53,53 +78,75 @@
             response = requests.get(self.uri)
             inverter_measures = response.json()['inverter']
 
             p_ac = 0
             i_ac = 0
             u_ac  =0
             p_dc = 0
-            efficiency = 0
+            u_dc1 = None
+            u_dc2 = None
+            i_dc1 = None
+            i_dc2 = None
+            efficiency = None
             temp = 0
+            frequency = 0
             power_limit = 0
             power_max = sum(inverter_infos[self.id]['ch_max_pwr'])
 
             for config in inverter_configs[self.id]:
                 if config['fld'] == 'active_PowerLimit':
                     power_limit_percent = float(config['val'])
                     power_limit = int(power_max * power_limit_percent / 100)
 
             for measure in inverter_measures[self.id]:
                 if measure['fld'] == 'P_AC':
-                    p_ac = measure['val']
+                    p_ac = float(measure['val'])
                 elif measure['fld'] == 'I_AC':
-                    i_ac = measure['val']
+                    i_ac = float(measure['val'])
                 elif measure['fld'] == 'U_AC':
-                    u_ac = measure['val']
+                    u_ac = float(measure['val'])
+                elif measure['fld'] == 'U_DC':
+                    if u_dc1 is None:
+                        u_dc1 = float(measure['val'])
+                    else:
+                        u_dc2 = float(measure['val'])
+                elif measure['fld'] == 'I_DC':
+                    if i_dc1 is None:
+                        i_dc1 = float(measure['val'])
+                    else:
+                        i_dc2 = float(measure['val'])
                 elif measure['fld'] == 'P_DC':
-                    p_dc = measure['val']
+                    p_dc = float(measure['val'])
                 elif measure['fld'] == 'Efficiency':
-                    efficiency = measure['val']
+                    efficiency = float(measure['val'])
                 elif measure['fld'] == 'Temp':
-                    temp = measure['val']
+                    temp = float(measure['val'])
+                elif measure['fld'] == 'F_AC':
+                    frequency = float(measure['val'])
 
-            self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, efficiency, temp)
+            self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, u_dc1, u_dc2, i_dc1, i_dc2, efficiency, temp, frequency)
 
     def set_power_limit(self, limit_watt: int):
-        response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_nonpersistent_absolute", "val": limit_watt})
-        response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_persistent_absolute", "val": limit_watt})
+        logging.info("inverter " + self.name + " set power limit to " + str(limit_watt) + " watt")
+        requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_nonpersistent_absolute", "val": limit_watt})
 
-    def update(self, power_max: int, power_limit: int, p_ac: int, u_ac: int, i_ac: int, p_dc: int, efficiency: int, temp: int):
+    def update(self, power_max: int, power_limit: int, p_ac: float, u_ac: float, i_ac: float, p_dc: float, u_dc1: float, u_dc2: float, i_dc1: float, i_dc2: float, efficiency: float, temp: float, frequency: float):
         self.power_max = power_max
         self.power_limit = power_limit
         self.p_ac = p_ac
         self.u_ac = u_ac
+        self.u_dc1 = u_dc1
+        self.u_dc2 = u_dc2
+        self.i_dc1 = i_dc1
+        self.i_dc2 = i_dc2
         self.i_ac = i_ac
         self.p_dc = p_dc
         self.efficiency = efficiency
         self.temp = temp
+        self.frequency = frequency
         self.last_update = datetime.now()
         self.__notify_Listener()
 
     def register_listener(self, listener):
         self.listener = listener
 
     def __notify_Listener(self):
@@ -114,32 +161,22 @@
         return  self.__str__()
 
 
 
 class Dtu:
 
     def __init__(self, base_uri: str):
-        self.is_running = True
         self.base_uri = base_uri
         uri = re.sub("^/|/$", "", self.base_uri) + '/api/inverter/list'
         response = requests.get(uri)
         data = response.json()
-        self.interval = int(data['interval'])
-        self.inverters = [Inverter(self.base_uri, entry['id'], entry['channels'], entry['name'], entry['serial']) for entry in data['inverter']]
-        Thread(target=self.__periodic_refresh, daemon=True)
-
-    def __periodic_refresh(self):
-        while self.is_running:
-            try:
-                for inverter in self.inverters:
-                    inverter.refresh()
-            except Exception as e:
-                print(e)
-            sleep(self.interval)
+        interval = int(data['interval'])
+        self.inverters = [Inverter(self.base_uri, entry['id'], entry['channels'], entry['name'], entry['serial'], interval) for entry in data['inverter']]
 
     @staticmethod
     def connect(base_uri: str):
         return Dtu(base_uri)
 
     def close(self):
-        self.is_running = False
+        for inverter in self.inverters:
+            inverter.close()
```

### Comparing `ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,33 +52,33 @@
                      metadata={
                          'title': 'serial',
                          "type": "string",
                          'description': 'The serial number',
                          'readOnly': True,
                      }))
 
-        self.is_available = Value(inverter.is_available)
+        self.available = Value(inverter.is_available)
         self.add_property(
             Property(self,
                      'is_available',
-                     self.is_available,
+                     self.available,
                      metadata={
-                         'title': 'is_available',
+                         'title': 'available',
                          "type": "boolean",
                          'description': 'True, if is available',
                          'readOnly': True,
                      }))
 
-        self.is_producing = Value(inverter.is_producing)
+        self.producing = Value(inverter.is_producing)
         self.add_property(
             Property(self,
                  'is_producing',
-                 self.is_producing,
-                 metadata={
-                     'title': 'is_producing',
+                     self.producing,
+                     metadata={
+                     'title': 'producing',
                      "type": "boolean",
                      'description': 'True, if is producing',
                      'readOnly': True,
                  }))
 
         self.power_max = Value(inverter.power_max)
         self.add_property(
@@ -119,81 +119,146 @@
         self.p_dc = Value(inverter.p_dc)
         self.add_property(
             Property(self,
                      'p_dc',
                      self.p_dc,
                      metadata={
                          'title': 'Power DC',
-                         "type": "integer",
+                         "type": "number",
                          'description': 'The power DC [W]',
                          'readOnly': True,
                      }))
 
+        self.u_dc1 = Value(inverter.u_dc1)
+        self.add_property(
+            Property(self,
+                     'u_dc1',
+                     self.u_dc1,
+                     metadata={
+                         'title': 'Voltage DC - Channel 1',
+                         "type": "number",
+                         'description': 'The voltage DC channel 1 [V]',
+                         'readOnly': True,
+                     }))
+
+        self.u_dc2 = Value(inverter.u_dc2)
+        self.add_property(
+            Property(self,
+                     'u_dc2',
+                     self.u_dc2,
+                     metadata={
+                         'title': 'Voltage DC - Channel 2',
+                         "type": "number",
+                         'description': 'The voltage DC channel 2 [V]',
+                         'readOnly': True,
+                     }))
+
+        self.i_dc1 = Value(inverter.i_dc1)
+        self.add_property(
+            Property(self,
+                     'i_dc1',
+                     self.i_dc1,
+                     metadata={
+                         'title': 'Current DC - Channel 1',
+                         "type": "number",
+                         'description': 'The current DC channel 1 [A]',
+                         'readOnly': True,
+                     }))
+
+        self.i_dc2 = Value(inverter.i_dc2)
+        self.add_property(
+            Property(self,
+                     'i_dc2',
+                     self.i_dc2,
+                     metadata={
+                         'title': 'Current DC - Channel 2',
+                         "type": "number",
+                         'description': 'The current DC channel 2 [A]',
+                         'readOnly': True,
+                     }))
+
         self.p_ac = Value(inverter.p_ac)
         self.add_property(
             Property(self,
                      'p_ac',
                      self.p_ac,
                      metadata={
                          'title': 'Power AC',
-                         "type": "integer",
+                         "type": "number",
                          'description': 'The power AC [W]',
                          'readOnly': True,
                      }))
 
         self.u_ac = Value(inverter.u_ac)
         self.add_property(
             Property(self,
                      'u_ac',
                      self.u_ac,
                      metadata={
                          'title': 'Voltage AC',
-                         "type": "integer",
+                         "type": "number",
                          'description': 'The voltage AC [V]',
                          'readOnly': True,
                      }))
 
         self.i_ac = Value(inverter.i_ac)
         self.add_property(
             Property(self,
                      'i_ac',
                      self.i_ac,
                      metadata={
                          'title': 'Current AC',
-                         "type": "integer",
+                         "type": "number",
                          'description': 'The current AC [A]',
                          'readOnly': True,
                      }))
 
         self.efficiency = Value(inverter.efficiency)
         self.add_property(
             Property(self,
                      'efficiency',
                      self.efficiency,
                      metadata={
                          'title': 'Efficiency',
-                         "type": "integer",
+                         "type": "number",
                          'description': 'The efficiency [%]',
                          'readOnly': True,
                      }))
 
+        self.frequency = Value(inverter.frequency)
+        self.add_property(
+            Property(self,
+                     'frequency',
+                     self.frequency,
+                     metadata={
+                         'title': 'frequency',
+                         "type": "number",
+                         'description': 'The frequency [Hz]',
+                         'readOnly': True,
+                     }))
+
 
         self.ioloop = tornado.ioloop.IOLoop.current()
         self.inverter.register_listener(self.on_value_changed)
 
     def on_value_changed(self):
         self.ioloop.add_callback(self.__on_value_changed)
 
     def __on_value_changed(self):
-        self.is_producing.notify_of_external_update(self.inverter.is_producing)
-        self.is_available.notify_of_external_update(self.inverter.is_available)
+        self.producing.notify_of_external_update(self.inverter.is_producing)
+        self.available.notify_of_external_update(self.inverter.is_available)
         self.p_dc.notify_of_external_update(self.inverter.p_dc)
+        self.u_dc1.notify_of_external_update(self.inverter.u_dc1)
+        self.u_dc2.notify_of_external_update(self.inverter.u_dc2)
+        self.i_dc1.notify_of_external_update(self.inverter.i_dc1)
+        self.i_dc2.notify_of_external_update(self.inverter.i_dc2)
         self.p_ac.notify_of_external_update(self.inverter.p_ac)
         self.i_ac.notify_of_external_update(self.inverter.i_ac)
         self.u_ac.notify_of_external_update(self.inverter.u_ac)
+        self.frequency.notify_of_external_update(self.inverter.frequency)
         self.efficiency.notify_of_external_update(self.inverter.efficiency)
         self.last_update.notify_of_external_update(self.inverter.last_update.strftime("%Y-%m-%dT%H:%M:%S"))
         self.temp.notify_of_external_update(self.inverter.temp)
         self.power_max.notify_of_external_update(self.inverter.power_max)
         self.power_limit.notify_of_external_update(self.inverter.power_limit)
```

### Comparing `ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.0.9
+Version: 0.1.0
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

