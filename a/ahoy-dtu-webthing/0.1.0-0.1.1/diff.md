# Comparing `tmp/ahoy_dtu_webthing-0.1.0.tar.gz` & `tmp/ahoy_dtu_webthing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.1.0.tar", last modified: Tue Jun 27 04:44:20 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.1.1.tar", last modified: Tue Jun 27 04:57:46 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.1.0.tar` & `ahoy_dtu_webthing-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 04:44:20.000000 ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 04:44:09.000000 ahoy_dtu_webthing-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 04:44:20.740814 ahoy_dtu_webthing-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:57:46.065496 ahoy_dtu_webthing-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 04:57:34.000000 ahoy_dtu_webthing-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 04:57:46.065496 ahoy_dtu_webthing-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-27 04:57:34.000000 ahoy_dtu_webthing-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:57:46.065496 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 04:57:34.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-27 04:57:34.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-27 04:57:34.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-27 04:57:34.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:57:46.065496 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 04:57:46.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 04:57:46.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:57:46.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 04:57:46.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 04:57:46.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 04:57:46.000000 ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 04:57:34.000000 ahoy_dtu_webthing-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 04:57:46.065496 ahoy_dtu_webthing-0.1.1/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.1.0/LICENSE` & `ahoy_dtu_webthing-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.0/PKG-INFO` & `ahoy_dtu_webthing-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.1.0/README.md` & `ahoy_dtu_webthing-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing/dtu.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
         self.id = id
         self.channel = channels
         self.name = name
         self.serial = serial
         self.interval = interval
         self.p_dc = 0
+        self.p_dc1 = 0
+        self.p_dc2 = 0
         self.u_dc1 = 0
         self.u_dc2 = 0
         self.i_dc1 = 0
         self.i_dc2 = 0
         self.p_ac = 0
         self.u_ac = 0
         self.i_ac = 0
@@ -78,14 +80,16 @@
             response = requests.get(self.uri)
             inverter_measures = response.json()['inverter']
 
             p_ac = 0
             i_ac = 0
             u_ac  =0
             p_dc = 0
+            p_dc1 = None
+            p_dc2 = None
             u_dc1 = None
             u_dc2 = None
             i_dc1 = None
             i_dc2 = None
             efficiency = None
             temp = 0
             frequency = 0
@@ -111,39 +115,46 @@
                         u_dc2 = float(measure['val'])
                 elif measure['fld'] == 'I_DC':
                     if i_dc1 is None:
                         i_dc1 = float(measure['val'])
                     else:
                         i_dc2 = float(measure['val'])
                 elif measure['fld'] == 'P_DC':
-                    p_dc = float(measure['val'])
+                    if p_dc1 is None:
+                        p_dc1 = float(measure['val'])
+                    elif p_dc2 is None:
+                        p_dc2 = float(measure['val'])
+                    else:
+                        p_dc = float(measure['val'])
                 elif measure['fld'] == 'Efficiency':
                     efficiency = float(measure['val'])
                 elif measure['fld'] == 'Temp':
                     temp = float(measure['val'])
                 elif measure['fld'] == 'F_AC':
                     frequency = float(measure['val'])
 
-            self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, u_dc1, u_dc2, i_dc1, i_dc2, efficiency, temp, frequency)
+            self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, p_dc1, p_dc2, u_dc1, u_dc2, i_dc1, i_dc2, efficiency, temp, frequency)
 
     def set_power_limit(self, limit_watt: int):
         logging.info("inverter " + self.name + " set power limit to " + str(limit_watt) + " watt")
         requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_nonpersistent_absolute", "val": limit_watt})
 
-    def update(self, power_max: int, power_limit: int, p_ac: float, u_ac: float, i_ac: float, p_dc: float, u_dc1: float, u_dc2: float, i_dc1: float, i_dc2: float, efficiency: float, temp: float, frequency: float):
+    def update(self, power_max: int, power_limit: int, p_ac: float, u_ac: float, i_ac: float, p_dc: float, p_dc1:float, p_dc2: float, u_dc1: float, u_dc2: float, i_dc1: float, i_dc2: float, efficiency: float, temp: float, frequency: float):
         self.power_max = power_max
         self.power_limit = power_limit
         self.p_ac = p_ac
         self.u_ac = u_ac
         self.u_dc1 = u_dc1
         self.u_dc2 = u_dc2
         self.i_dc1 = i_dc1
         self.i_dc2 = i_dc2
         self.i_ac = i_ac
         self.p_dc = p_dc
+        self.p_dc1 = p_dc1
+        self.p_dc2 = p_dc2
         self.efficiency = efficiency
         self.temp = temp
         self.frequency = frequency
         self.last_update = datetime.now()
         self.__notify_Listener()
 
     def register_listener(self, listener):
```

### Comparing `ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.0/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.1.1/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

