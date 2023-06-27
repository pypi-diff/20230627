# Comparing `tmp/ahoy_dtu_webthing-0.1.2.tar.gz` & `tmp/ahoy_dtu_webthing-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.1.2.tar", last modified: Tue Jun 27 05:04:05 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.1.3.tar", last modified: Tue Jun 27 05:04:42 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.1.2.tar` & `ahoy_dtu_webthing-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:04:05.232841 ahoy_dtu_webthing-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 05:03:52.000000 ahoy_dtu_webthing-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 05:04:05.232841 ahoy_dtu_webthing-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-27 05:03:52.000000 ahoy_dtu_webthing-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:04:05.232841 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 05:03:52.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-27 05:03:52.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-27 05:03:52.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-27 05:03:52.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:04:05.232841 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 05:04:05.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 05:04:05.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:04:05.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 05:04:05.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 05:04:05.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 05:04:05.000000 ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 05:03:52.000000 ahoy_dtu_webthing-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 05:04:05.232841 ahoy_dtu_webthing-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:04:42.160117 ahoy_dtu_webthing-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 05:04:26.000000 ahoy_dtu_webthing-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 05:04:42.164117 ahoy_dtu_webthing-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-27 05:04:26.000000 ahoy_dtu_webthing-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:04:42.160117 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 05:04:26.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-27 05:04:26.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-27 05:04:26.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-06-27 05:04:26.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:04:42.160117 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 05:04:42.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 05:04:42.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:04:42.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 05:04:42.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 05:04:42.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 05:04:42.000000 ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 05:04:26.000000 ahoy_dtu_webthing-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 05:04:42.164117 ahoy_dtu_webthing-0.1.3/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.1.2/LICENSE` & `ahoy_dtu_webthing-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.2/PKG-INFO` & `ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ahoy_dtu_webthing
-Version: 0.1.2
+Name: ahoy-dtu-webthing
+Version: 0.1.3
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.1.2/README.md` & `ahoy_dtu_webthing-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing/dtu.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.1.3/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,26 +112,14 @@
                      metadata={
                          'title': 'fetch_date',
                          "type": "string",
                          'description': 'The temperature [C]',
                          'readOnly': True,
                      }))
 
-        self.p_dc = Value(inverter.p_dc)
-        self.add_property(
-            Property(self,
-                     'p_dc',
-                     self.p_dc,
-                     metadata={
-                         'title': 'Power DC',
-                         "type": "number",
-                         'description': 'The power DC [W]',
-                         'readOnly': True,
-                     }))
-
         self.u_dc1 = Value(inverter.u_dc1)
         self.add_property(
             Property(self,
                      'u_dc1',
                      self.u_dc1,
                      metadata={
                          'title': 'Voltage DC - Channel 1',
@@ -172,14 +160,50 @@
                      metadata={
                          'title': 'Current DC - Channel 2',
                          "type": "number",
                          'description': 'The current DC channel 2 [A]',
                          'readOnly': True,
                      }))
 
+        self.p_dc = Value(inverter.p_dc)
+        self.add_property(
+            Property(self,
+                     'p_dc',
+                     self.p_dc,
+                     metadata={
+                         'title': 'Power DC',
+                         "type": "number",
+                         'description': 'The power DC [W]',
+                         'readOnly': True,
+                     }))
+
+        self.p_dc1 = Value(inverter.p_dc1)
+        self.add_property(
+            Property(self,
+                     'p_dc1',
+                     self.p_dc1,
+                     metadata={
+                         'title': 'Power DC channel 1',
+                         "type": "number",
+                         'description': 'The power DC channel 1 [W]',
+                         'readOnly': True,
+                     }))
+
+        self.p_dc2 = Value(inverter.p_dc2)
+        self.add_property(
+            Property(self,
+                     'p_dc2',
+                     self.p_dc2,
+                     metadata={
+                         'title': 'Power DC channel 2',
+                         "type": "number",
+                         'description': 'The power DC channel 2 [W]',
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
@@ -243,14 +267,16 @@
     def on_value_changed(self):
         self.ioloop.add_callback(self.__on_value_changed)
 
     def __on_value_changed(self):
         self.producing.notify_of_external_update(self.inverter.is_producing)
         self.available.notify_of_external_update(self.inverter.is_available)
         self.p_dc.notify_of_external_update(self.inverter.p_dc)
+        self.p_dc1.notify_of_external_update(self.inverter.p_dc1)
+        self.p_dc2.notify_of_external_update(self.inverter.p_dc2)
         self.u_dc1.notify_of_external_update(self.inverter.u_dc1)
         self.u_dc2.notify_of_external_update(self.inverter.u_dc2)
         self.i_dc1.notify_of_external_update(self.inverter.i_dc1)
         self.i_dc2.notify_of_external_update(self.inverter.i_dc2)
         self.p_ac.notify_of_external_update(self.inverter.p_ac)
         self.i_ac.notify_of_external_update(self.inverter.i_ac)
         self.u_ac.notify_of_external_update(self.inverter.u_ac)
```

### Comparing `ahoy_dtu_webthing-0.1.2/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ahoy-dtu-webthing
-Version: 0.1.2
+Name: ahoy_dtu_webthing
+Version: 0.1.3
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

