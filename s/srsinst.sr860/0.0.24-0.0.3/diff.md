# Comparing `tmp/srsinst.sr860-0.0.24.tar.gz` & `tmp/srsinst.sr860-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument drivers to GIT\sr860\dist\.tmp-0vxopuff\srsinst.sr860-0.0.24.tar", last modified: Tue Jun 27 19:44:39 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument_library\sr860\dist\.tmp-2mym4ve8\srsinst.sr860-0.0.3.tar", last modified: Mon Jan  9 18:20:53 2023, max compression
```

## Comparing `srsinst.sr860-0.0.24.tar` & `srsinst.sr860-0.0.3.tar`

### file list

```diff
@@ -1,62 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.347699 srsinst.sr860-0.0.24/
--rw-rw-rw-   0        0        0     1968 2023-02-10 18:32:29.000000 srsinst.sr860-0.0.24/.gitignore
--rw-rw-rw-   0        0        0     1107 2023-01-03 17:25:41.000000 srsinst.sr860-0.0.24/LICENSE.txt
--rw-rw-rw-   0        0        0     8485 2023-06-27 19:44:39.337704 srsinst.sr860-0.0.24/PKG-INFO
--rw-rw-rw-   0        0        0     7686 2023-06-16 00:22:36.000000 srsinst.sr860-0.0.24/README.md
--rw-rw-rw-   0        0        0   102698 2023-02-10 20:16:01.000000 srsinst.sr860-0.0.24/SR860_screenshot.png
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.262512 srsinst.sr860-0.0.24/docs/
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.262512 srsinst.sr860-0.0.24/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.287763 srsinst.sr860-0.0.24/docs/_static/image/
--rw-rw-rw-   0        0        0   102698 2023-02-10 20:16:01.000000 srsinst.sr860-0.0.24/docs/_static/image/SR860_screenshot.png
--rw-rw-rw-   0        0        0     1239 2023-06-27 19:42:15.000000 srsinst.sr860-0.0.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 19:44:39.347699 srsinst.sr860-0.0.24/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.sr860-0.0.24/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.262512 srsinst.sr860-0.0.24/srsinst/
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.307744 srsinst.sr860-0.0.24/srsinst/sr860/
--rw-rw-rw-   0        0        0      268 2023-06-27 19:38:14.000000 srsinst.sr860-0.0.24/srsinst/sr860/__init__.py
--rw-rw-rw-   0        0        0      485 2023-04-07 00:54:32.000000 srsinst.sr860-0.0.24/srsinst/sr860/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.307744 srsinst.sr860-0.0.24/srsinst/sr860/instruments/
--rw-rw-rw-   0        0        0        0 2023-05-10 22:15:31.000000 srsinst.sr860-0.0.24/srsinst/sr860/instruments/__init__.py
--rw-rw-rw-   0        0        0    27334 2023-06-26 20:38:16.000000 srsinst.sr860-0.0.24/srsinst/sr860/instruments/components.py
--rw-rw-rw-   0        0        0      699 2023-05-10 22:14:20.000000 srsinst.sr860-0.0.24/srsinst/sr860/instruments/get_instruments.py
--rw-rw-rw-   0        0        0     3633 2023-03-27 23:07:35.000000 srsinst.sr860-0.0.24/srsinst/sr860/instruments/keys.py
--rw-rw-rw-   0        0        0     4010 2023-06-16 00:33:27.000000 srsinst.sr860-0.0.24/srsinst/sr860/instruments/sr860.py
--rw-rw-rw-   0        0        0     3664 2023-05-03 17:28:13.000000 srsinst.sr860-0.0.24/srsinst/sr860/instruments/visainterface.py
--rw-rw-rw-   0        0        0     3031 2023-05-03 17:28:13.000000 srsinst.sr860-0.0.24/srsinst/sr860/instruments/vxi11interface.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.317715 srsinst.sr860-0.0.24/srsinst/sr860/plots/
--rw-rw-rw-   0        0        0        0 2023-01-27 17:16:28.000000 srsinst.sr860-0.0.24/srsinst/sr860/plots/__init__.py
--rw-rw-rw-   0        0        0     8462 2023-04-06 22:20:58.000000 srsinst.sr860-0.0.24/srsinst/sr860/plots/timeplot.py
--rw-rw-rw-   0        0        0     4263 2023-03-24 17:49:17.000000 srsinst.sr860-0.0.24/srsinst/sr860/plots/twobytwosharexplot.py
--rw-rw-rw-   0        0        0     2021 2023-03-08 18:03:43.000000 srsinst.sr860-0.0.24/srsinst/sr860/sr860 with sr542.taskconfig
--rw-rw-rw-   0        0        0     3338 2023-06-21 20:57:39.000000 srsinst.sr860-0.0.24/srsinst/sr860/sr860.taskconfig
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.337704 srsinst.sr860-0.0.24/srsinst/sr860/tasks/
--rw-rw-rw-   0        0        0        0 2022-12-22 20:08:49.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/__init__.py
--rw-rw-rw-   0        0        0     1026 2023-06-21 20:39:39.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/assignparametertochannel.py
--rw-rw-rw-   0        0        0     1361 2023-03-06 17:34:08.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/autofunctiontask.py
--rw-rw-rw-   0        0        0     1219 2023-06-21 20:39:39.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/auxoutputtask.py
--rw-rw-rw-   0        0        0     2314 2023-06-21 20:42:05.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/configurereferencetask.py
--rw-rw-rw-   0        0        0     1423 2023-06-21 20:42:55.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/configuresineoutputtask.py
--rw-rw-rw-   0        0        0     2635 2023-06-21 20:38:38.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/datatransferfromdatachannelstask.py
--rw-rw-rw-   0        0        0     1207 2023-06-21 20:36:25.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/scanauxout1task.py
--rw-rw-rw-   0        0        0     1207 2023-06-21 20:37:19.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/scanauxout2task.py
--rw-rw-rw-   0        0        0     1643 2023-06-21 20:29:35.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/scanfrequencytask.py
--rw-rw-rw-   0        0        0     1553 2023-06-21 20:43:26.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/scanrefamplitudetask.py
--rw-rw-rw-   0        0        0     1425 2023-06-21 20:43:55.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/scanrefoffsettask.py
--rw-rw-rw-   0        0        0     1642 2023-06-21 20:44:08.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/selecttimebasetask.py
--rw-rw-rw-   0        0        0     2311 2023-06-21 20:45:34.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/setreferencetochoptask.py
--rw-rw-rw-   0        0        0     2227 2023-06-21 20:46:33.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/setreferencetodualtask.py
--rw-rw-rw-   0        0        0     2072 2023-06-21 20:47:31.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/setreferencetoexternaltask.py
--rw-rw-rw-   0        0        0     7458 2023-06-27 19:36:53.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/setreferencetoexternalwithsr542task.py
--rw-rw-rw-   0        0        0     1791 2023-06-21 20:49:26.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/setreferencetointernaltask.py
--rw-rw-rw-   0        0        0     1081 2023-03-27 23:44:46.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/sidntesttask.py
--rw-rw-rw-   0        0        0     1626 2023-06-21 20:34:58.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/signaltocurrentmodetask.py
--rw-rw-rw-   0        0        0     1998 2023-06-21 20:34:58.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/signaltovoltagemodetask.py
--rw-rw-rw-   0        0        0     1342 2023-04-11 00:34:19.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/simulatedplot.py
--rw-rw-rw-   0        0        0     3313 2023-06-21 20:50:04.000000 srsinst.sr860-0.0.24/srsinst/sr860/tasks/streamingtask.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:44:39.297727 srsinst.sr860-0.0.24/srsinst.sr860.egg-info/
--rw-rw-rw-   0        0        0     8485 2023-06-27 19:44:39.000000 srsinst.sr860-0.0.24/srsinst.sr860.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1858 2023-06-27 19:44:39.000000 srsinst.sr860-0.0.24/srsinst.sr860.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 19:44:39.000000 srsinst.sr860-0.0.24/srsinst.sr860.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-27 19:44:39.000000 srsinst.sr860-0.0.24/srsinst.sr860.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-06-27 19:44:39.000000 srsinst.sr860-0.0.24/srsinst.sr860.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 19:44:39.000000 srsinst.sr860-0.0.24/srsinst.sr860.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-09 18:20:53.941327 srsinst.sr860-0.0.3/
+-rw-rw-rw-   0        0        0     1107 2023-01-03 17:25:41.000000 srsinst.sr860-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      998 2023-01-09 18:20:53.940328 srsinst.sr860-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-01-03 19:57:55.000000 srsinst.sr860-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-01-09 18:20:53.941327 srsinst.sr860-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2164 2023-01-03 20:12:50.000000 srsinst.sr860-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-09 18:20:53.907944 srsinst.sr860-0.0.3/srsinst/
+drwxrwxrwx   0        0        0        0 2023-01-09 18:20:53.922542 srsinst.sr860-0.0.3/srsinst/sr860/
+-rw-rw-rw-   0        0        0      245 2023-01-09 16:43:19.000000 srsinst.sr860-0.0.3/srsinst/sr860/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-01-03 17:25:41.000000 srsinst.sr860-0.0.3/srsinst/sr860/__main__.py
+drwxrwxrwx   0        0        0        0 2023-01-09 18:20:53.926168 srsinst.sr860-0.0.3/srsinst/sr860/instruments/
+-rw-rw-rw-   0        0        0       42 2022-12-22 20:12:34.000000 srsinst.sr860-0.0.3/srsinst/sr860/instruments/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-01-03 19:07:42.000000 srsinst.sr860-0.0.3/srsinst/sr860/instruments/get_instruments.py
+drwxrwxrwx   0        0        0        0 2023-01-09 18:20:53.932811 srsinst.sr860-0.0.3/srsinst/sr860/instruments/sr865/
+-rw-rw-rw-   0        0        0        0 2022-12-14 17:44:52.000000 srsinst.sr860-0.0.3/srsinst/sr860/instruments/sr865/__init__.py
+-rw-rw-rw-   0        0        0     3674 2023-01-03 19:35:03.000000 srsinst.sr860-0.0.3/srsinst/sr860/instruments/sr865/components.py
+-rw-rw-rw-   0        0        0     1506 2023-01-05 17:55:06.000000 srsinst.sr860-0.0.3/srsinst/sr860/instruments/sr865/sr865.py
+-rw-rw-rw-   0        0        0     3105 2023-01-06 17:05:26.000000 srsinst.sr860-0.0.3/srsinst/sr860/instruments/sr865/visainterface.py
+-rw-rw-rw-   0        0        0     2461 2023-01-06 18:08:51.000000 srsinst.sr860-0.0.3/srsinst/sr860/instruments/sr865/vxi11interface.py
+drwxrwxrwx   0        0        0        0 2023-01-09 18:20:53.933810 srsinst.sr860-0.0.3/srsinst/sr860/plots/
+-rw-rw-rw-   0        0        0     5328 2023-01-04 00:29:47.000000 srsinst.sr860-0.0.3/srsinst/sr860/plots/twobytwosharexplot.py
+-rw-rw-rw-   0        0        0      250 2022-12-23 17:29:49.000000 srsinst.sr860-0.0.3/srsinst/sr860/sr860.taskconfig
+drwxrwxrwx   0        0        0        0 2023-01-09 18:20:53.940328 srsinst.sr860-0.0.3/srsinst/sr860/tasks/
+-rw-rw-rw-   0        0        0        0 2022-12-22 20:08:49.000000 srsinst.sr860-0.0.3/srsinst/sr860/tasks/__init__.py
+-rw-rw-rw-   0        0        0     2262 2023-01-03 18:28:27.000000 srsinst.sr860-0.0.3/srsinst/sr860/tasks/sidntesttask.py
+-rw-rw-rw-   0        0        0     1313 2023-01-03 17:47:56.000000 srsinst.sr860-0.0.3/srsinst/sr860/tasks/simulatedplot.py
+-rw-rw-rw-   0        0        0     3402 2023-01-03 19:44:47.000000 srsinst.sr860-0.0.3/srsinst/sr860/tasks/streamingtask.py
+drwxrwxrwx   0        0        0        0 2023-01-09 18:20:53.918526 srsinst.sr860-0.0.3/srsinst.sr860.egg-info/
+-rw-rw-rw-   0        0        0      998 2023-01-09 18:20:53.000000 srsinst.sr860-0.0.3/srsinst.sr860.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      834 2023-01-09 18:20:53.000000 srsinst.sr860-0.0.3/srsinst.sr860.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-09 18:20:53.000000 srsinst.sr860-0.0.3/srsinst.sr860.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-01-09 18:20:53.000000 srsinst.sr860-0.0.3/srsinst.sr860.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       59 2023-01-09 18:20:53.000000 srsinst.sr860-0.0.3/srsinst.sr860.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-01-09 18:20:53.000000 srsinst.sr860-0.0.3/srsinst.sr860.egg-info/top_level.txt
```

### Comparing `srsinst.sr860-0.0.24/LICENSE.txt` & `srsinst.sr860-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.0.24/srsinst/sr860/instruments/get_instruments.py` & `srsinst.sr860-0.0.3/srsinst/sr860/instruments/get_instruments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
-from srsgui import Task
-from .sr860 import SR860
+from srsgui.task import Task
+from .sr865.sr865 import SR865
 
 logger = logging.getLogger(__name__)
 
 
-def get_sr860(task: Task, name=None) -> SR860:
+def get_sr865(task: Task, name=None) -> SR865:
     """
     Instead of using task.get_instrument() directly in a Task subclass,
     Defining a wrapper function with a instrument return type will help
     a context-sensitive editors display  attributes available
     for the instrument class.
     """
     if name is None:
         inst = list(task.inst_dict.values())[0]
     else:
         inst = task.get_instrument(name)
 
-    if issubclass(type(inst), SR860):
+    if issubclass(type(inst), SR865):
         return inst
     else:
-        logger.error('{} is not {}'.format(type(inst), SR860))
+        logger.error('{} is not {}'.format(type(inst), SR865))
         return None
```

### Comparing `srsinst.sr860-0.0.24/srsinst/sr860/instruments/visainterface.py` & `srsinst.sr860-0.0.3/srsinst/sr860/instruments/sr865/visainterface.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,23 +35,23 @@
             self._resource_name = resource
         except Exception as e:
             raise InstCommunicationError('Failed to connect {}'.format(resource))
         else:
             self._is_connected = True
 
             if self._connect_callback:
-                self._connect_callback('Connected VISA: {}'
-                                       .format(self._resource_name))
+                self._connect_callback('Connected serial port: {} Baud rate: {}'
+                                       .format(self._port, self._baud_rate))
 
     def disconnect(self):
         self._visa.close()
         self._is_connected = False
         self._resource_name = None
         if self._disconnect_callback:
-            self._disconnect_callback('Disconnected VISA: {}'.format(self._resource_name))
+            self._disconnect_callback('Disconnected serial port: {}'.format(self._port))
 
     @staticmethod
     def parse_parameter_string(param_string):
         connect_parameters = []
         params = param_string.split(':', 1)
         interface_type = params[0].strip().lower()
         if interface_type != VisaInterface.NAME:
@@ -62,54 +62,37 @@
             connect_parameters.append(interface_type)  # 'visa'
             connect_parameters.append(params[1])  # resource string
         return connect_parameters
 
     def _send(self, cmd):
         self._visa.write(cmd)
 
-    def _write_binary(self, binary_array):
-        if type(binary_array) not in (bytes, bytearray):
-            raise TypeError('_write_binary requires bytes or bytearray')
-        self._visa.write_raw(binary_array)
-
     def _recv(self):
         reply = self._visa.read()
         return reply
 
     def _read_binary(self, length=-1):
         reply = self._visa.read_bytes(length)
         return reply
 
     def query_text(self, cmd):
-        with self.get_lock():
-            reply = self._visa.query(cmd)
-        if self._query_callback:
-            self._query_callback('Queried Cmd: {} Reply: {}'.format(cmd, reply))
-
+        reply = self._visa.query(cmd)
         return reply
 
     def clear_buffer(self):
         self._visa.clear()
 
     def get_visa_instrument(self):
         return self._visa
 
     def get_info(self):
         return {'type': self.type,
                 'resource_name': self._resource_name,
                 }
 
-    def set_timeout(self, timeout):
-        self._timeout = timeout
-        if self._visa:
-            self._visa.timeout = self._timeout * 1000
-
-    def get_timeout(self):
-        return self._timeout
-
     @classmethod
     def find(cls):
         if not VISA_AVAILABLE:
             return ['No PyVisa installed']
         if not cls.rm:
             return []
```

### Comparing `srsinst.sr860-0.0.24/srsinst/sr860/instruments/vxi11interface.py` & `srsinst.sr860-0.0.3/srsinst/sr860/instruments/sr865/vxi11interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,23 +24,21 @@
             self._vxi = vxi11.Instrument(ip_address)
             print(self._vxi.ask('*IDN?'))
             self._ip_address = ip_address
             self._is_connected = True
             if self._connect_callback:
                 self._connect_callback('Connected VXI11 to {}'
                                        .format(self._ip_address))
-
+            
         except Exception as e:
             logger.error(e)
-
+            
     def disconnect(self):
         self._vxi.close()
         self._is_connected = False
-        if self._disconnect_callback:
-            self._disconnect_callback('Disconnected VXI11 from : {}'.format(self._ip_address))
 
     @staticmethod
     def parse_parameter_string(param_string):
         connect_parameters = []
         params = param_string.split(':')
         num = len(params)
         interface_type = params[0].strip().lower()
@@ -52,48 +50,34 @@
             connect_parameters.append(interface_type)  # 'serial'
             connect_parameters.append(params[1])  # IP address
         return connect_parameters
 
     def _send(self, cmd):
         self._vxi.write(cmd)
 
-    def _write_binary(self, binary_array):
-        if type(binary_array) not in (bytes, bytearray):
-            raise TypeError('_write_binary requires bytes or bytearray')
-        self._vxi.write_raw(binary_array)
-
     def _recv(self):
         reply = self._vxi.read()
         return reply
 
     def _read_binary(self, length=-1):
         """
         Read a fixed number of bytes. VXI11 read_raw returns all the data contained
         in the last packet that covers the length of data.
         It could return larger than the specified size of data.
         """
         reply = self._vxi.read_raw(length)
         return reply
 
     def query_text(self, cmd):
-        with self.get_lock():
-            reply = self._vxi.ask(cmd)
+        reply = self._vxi.ask(cmd)
         if self._query_callback:
             self._query_callback('Queried Cmd: {} Reply: {}'.format(cmd, reply))
 
         return reply
 
-    def set_timeout(self, timeout):
-        self._timeout = timeout
-        if self._vxi:
-            self._vxi.timeout = timeout * 1000
-
-    def get_timeout(self):
-        return self._timeout
-
     def clear_buffer(self):
         self._vxi.clear()
 
     def get_info(self):
         return {'type': self.type,
                 'ip_address': self._ip_address,
                 }
```

### Comparing `srsinst.sr860-0.0.24/srsinst/sr860/tasks/simulatedplot.py` & `srsinst.sr860-0.0.3/srsinst/sr860/tasks/simulatedplot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import time
 import math
 import numpy as np
 from srsgui import Task
-from srsinst.sr860.plots.twobytwosharexplot import TwoByTwoShareXPlot
-from srsinst.sr860.instruments.components import DataStreamBuffer
+from plots.twobytwosharexplot import TwoByTwoShareXPlot
 
 
 class SimulatedPlotTask(Task):
     input_parameters={}
 
     def setup(self):
         # storage for data generation
         self.dr = 1e-3
         self.dt = 1e-3
 
         self.figure = self.get_figure()
-        self.data = DataStreamBuffer(10000000)
-        self.plot = TwoByTwoShareXPlot(self.figure, self.data)
+        self.plot = TwoByTwoShareXPlot(self.figure)
+        self.plot.set_buffer_size(10000000)
 
     def test(self):
         while True:
+            if not self.is_running():
+                break
+
             r, th = self.calc_chunk()
-            self.delay(0.001)
+            time.sleep(0.001)
 
             x = r * np.sin(th)
             y = r * np.cos(th)
 
-            self.data.add_data_block(x, y, r, th)
+            self.plot.add_data_block(x, y, r, th)
             self.notify_data_available()  # parent calls update() method
 
+
     def update(self, data):
         if self.plot.request_plot_update():
             self.request_figure_update()
 
     def cleanup(self):
         pass
```

### Comparing `srsinst.sr860-0.0.24/srsinst/sr860/tasks/streamingtask.py` & `srsinst.sr860-0.0.3/srsinst/sr860/tasks/streamingtask.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,93 @@
 
 import time
+import logging
+import socket
+
+import numpy as np
+from  struct import unpack_from
 
 from srsgui import Task
-from srsgui import IntegerInput, FloatInput, ListInput, IntegerListInput
+from srsgui import IntegerInput, FloatInput, ListInput
 
-from srsinst.sr860 import SR860, get_sr860
-from srsinst.sr860.instruments.components import DataStream
+from instruments import get_sr865
 
-from srsinst.sr860.plots.twobytwosharexplot import TwoByTwoShareXPlot
+from plots.twobytwosharexplot import TwoByTwoShareXPlot
 
 
 class StreamingTask(Task):
     Duration = 'duration'
     Channels = 'Channels'
     DataFormat = 'data format'
     PacketSize = 'packet size'
     Rate = 'rate divider'
     Port = 'udp port'
 
     input_parameters = {
-        Duration:   IntegerInput(3600, ' s', 1, 360000, 1),
-        Channels:   ListInput(list(DataStream.ChannelDict.keys()), 1),
-        DataFormat: ListInput(list(DataStream.FormatDict.keys())),
-        PacketSize: IntegerListInput([1024, 512, 256, 128]),
-        Rate:       IntegerInput(4, '  (2^n) ', 0, 20, 1),
-        Port:       IntegerInput(1865, '', 1024, 65535, 1)
+        Duration: IntegerInput(3600, ' s', 1, 360000, 1),
+        Channels: ListInput(['X', 'X, Y', 'R, Theta', 'X, Y, R, Theta'], 1),
+        DataFormat: ListInput(['Float32', 'Int16']),
+        PacketSize: ListInput(['1024', '512', '256', '128']),
+        Rate: IntegerInput(4, '  (1/2^n) ', 0, 20, 1),
+        Port: IntegerInput(8086, '', 1024, 65535, 1)
     }
 
     def setup(self):
-        self.logger = self.get_logger(__name__)
-        self.lia = get_sr860(self)
+        self.logger = logging.getLogger(__file__)
+        self.lia = get_sr865(self)
         print(self.lia.query_text('*idn?'))
 
+        self.params = self.get_all_input_parameters()
+
         self.lia.stream.enable = False
         self.lia.stream.option = 2
-        self.lia.stream.channel = self.input_parameters[self.Channels].text
-        self.lia.stream.format = self.input_parameters[self.DataFormat].text
-        self.lia.stream.packet_size = self.input_parameters[self.PacketSize].get_value()
-        self.lia.stream.rate = self.get_input_parameter(self.Rate)
-        self.lia.stream.port = self.get_input_parameter(self.Port)
+        self.lia.stream.channel = self.params[self.Channels]
+        self.lia.stream.format = self.params[self.DataFormat]
+        self.lia.stream.packet_size = self.params[self.PacketSize]
+        self.lia.stream.rate = self.params[self.Rate]
+        self.lia.stream.port = self.params[self.Port]
 
-        self.duration_value = self.get_input_parameter(self.Duration)
         self.max_rate = self.lia.stream.max_rate
         self.sample_rate = self.max_rate / 2 ** self.lia.stream.rate
-        self.packet_size = self.lia.stream.packet_size
+        self.packet_size = int(list(self.lia.stream.PacketSizeDict.keys())[self.lia.stream.packet_size])
         self.logger.info('Channels: {}, Data format: {}, Packet_size: {}, Rate: {:.3f} Hz, Port: {}'
-                         .format(self.lia.stream.channel,
-                                 self.lia.stream.format,
+                         .format(list(self.lia.stream.ChannelDict.keys())[self.lia.stream.channel],
+                                 list(self.lia.stream.FormatDict.keys())[self.lia.stream.format],
                                  self.packet_size,
                                  self.sample_rate,
                                  self.lia.stream.port,
                                  )
                          )
 
-        self.plot = TwoByTwoShareXPlot(self.figure, self.lia.stream.data)
+        self.plot = TwoByTwoShareXPlot(self.figure)
 
         # Mark the time 0
         self.init_time = time.time()
 
     def test(self):
-        if self.get_input_parameter(self.Channels) == 0:
+        if self.params[self.Channels] == 0:
             raise ValueError('Channel X is not allowed,Choose other multiple channels')
 
         self.last_p_id = 0
         self.lia.stream.start()
-        while time.time() - self.init_time < self.duration_value:
-            block, p_id = self.lia.stream.receive_packet()
-            self.lia.stream.data.add_data_block(*block)
-
-            if self.last_p_id and p_id - self.last_p_id > 1:
-                self.logger.warning('{} missing packet(s) before ID:{}'
-                                    .format(p_id - self.last_p_id - 1, p_id))
-            self.last_p_id = p_id
-            self.notify_data_available()
-
-            if not self.is_running():
-                break
+        try:
+            while time.time() - self.init_time < self.params[self.Duration]:
+                if not self.is_running():
+                    break
+
+                block, p_id = self.lia.stream.receive_packet()
+                self.plot.add_data_block(*block)
+
+                if self.last_p_id and p_id - self.last_p_id > 1:
+                    self.logger.warning('{} missing packet(s) before ID:{}'
+                                        .format(p_id - self.last_p_id - 1, p_id))
+                self.last_p_id = p_id
+                self.notify_data_available()
+        except Exception as e:
+            self.logger.error(e)
 
     def update(self, data):
         if self.plot.request_plot_update():
             self.request_figure_update()
 
     def cleanup(self):
         self.lia.stream.stop()
```

