# Comparing `tmp/openhomedevice-2.1.tar.gz` & `tmp/openhomedevice-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhomedevice-2.1.tar", last modified: Wed Jun 14 19:58:16 2023, max compression
+gzip compressed data, was "openhomedevice-2.2.tar", last modified: Tue Jun 27 19:27:26 2023, max compression
```

## Comparing `openhomedevice-2.1.tar` & `openhomedevice-2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-14 19:58:16.480407 openhomedevice-2.1/
--rw-r--r--   0 barry      (502) staff       (20)     1076 2023-06-12 20:59:11.000000 openhomedevice-2.1/LICENSE.txt
--rw-r--r--   0 barry      (502) staff       (20)     7141 2023-06-14 19:58:16.480531 openhomedevice-2.1/PKG-INFO
--rw-r--r--   0 barry      (502) staff       (20)     6493 2023-06-14 19:55:10.000000 openhomedevice-2.1/README.md
-drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-14 19:58:16.478311 openhomedevice-2.1/openhomedevice/
--rw-r--r--   0 barry      (502) staff       (20)       43 2023-06-12 20:59:11.000000 openhomedevice-2.1/openhomedevice/__init__.py
--rw-r--r--   0 barry      (502) staff       (20)    10323 2023-06-14 19:50:16.000000 openhomedevice-2.1/openhomedevice/device.py
--rw-r--r--   0 barry      (502) staff       (20)     6482 2023-06-12 20:59:11.000000 openhomedevice-2.1/openhomedevice/didl_lite.py
-drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-14 19:58:16.480157 openhomedevice-2.1/openhomedevice.egg-info/
--rw-r--r--   0 barry      (502) staff       (20)     7141 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/PKG-INFO
--rw-r--r--   0 barry      (502) staff       (20)      309 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/SOURCES.txt
--rw-r--r--   0 barry      (502) staff       (20)        1 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/dependency_links.txt
--rw-r--r--   0 barry      (502) staff       (20)       36 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/requires.txt
--rw-r--r--   0 barry      (502) staff       (20)       15 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/top_level.txt
--rw-r--r--   0 barry      (502) staff       (20)       79 2023-06-14 19:58:16.480980 openhomedevice-2.1/setup.cfg
--rw-r--r--   0 barry      (502) staff       (20)      914 2023-06-14 18:34:31.000000 openhomedevice-2.1/setup.py
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-27 19:27:26.756592 openhomedevice-2.2/
+-rw-r--r--   0 barry      (502) staff       (20)     1076 2023-06-12 20:59:11.000000 openhomedevice-2.2/LICENSE.txt
+-rw-r--r--   0 barry      (502) staff       (20)     7238 2023-06-27 19:27:26.756750 openhomedevice-2.2/PKG-INFO
+-rw-r--r--   0 barry      (502) staff       (20)     6590 2023-06-27 19:20:23.000000 openhomedevice-2.2/README.md
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-27 19:27:26.753014 openhomedevice-2.2/openhomedevice/
+-rw-r--r--   0 barry      (502) staff       (20)       43 2023-06-12 20:59:11.000000 openhomedevice-2.2/openhomedevice/__init__.py
+-rw-r--r--   0 barry      (502) staff       (20)    10536 2023-06-27 19:26:31.000000 openhomedevice-2.2/openhomedevice/device.py
+-rw-r--r--   0 barry      (502) staff       (20)     6482 2023-06-12 20:59:11.000000 openhomedevice-2.2/openhomedevice/didl_lite.py
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-27 19:27:26.756093 openhomedevice-2.2/openhomedevice.egg-info/
+-rw-r--r--   0 barry      (502) staff       (20)     7238 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/PKG-INFO
+-rw-r--r--   0 barry      (502) staff       (20)      309 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/SOURCES.txt
+-rw-r--r--   0 barry      (502) staff       (20)        1 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/dependency_links.txt
+-rw-r--r--   0 barry      (502) staff       (20)       36 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/requires.txt
+-rw-r--r--   0 barry      (502) staff       (20)       15 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/top_level.txt
+-rw-r--r--   0 barry      (502) staff       (20)       79 2023-06-27 19:27:26.757273 openhomedevice-2.2/setup.cfg
+-rw-r--r--   0 barry      (502) staff       (20)      914 2023-06-27 19:21:27.000000 openhomedevice-2.2/setup.py
```

### Comparing `openhomedevice-2.1/LICENSE.txt` & `openhomedevice-2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openhomedevice-2.1/PKG-INFO` & `openhomedevice-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhomedevice
-Version: 2.1
+Version: 2.2
 Summary: Provides an API for requesting information from an Openhome device
 Home-page: https://github.com/bazwilliams/openhomedevice
 Author: Barry John Williams
 Author-email: barry@bjw.me.uk
 License: UNKNOWN
 Download-URL: https://github.com/bazwilliams/openhomedevice/tarball/2.1
 Keywords: upnp,dlna,openhome,linn,ds,music,render,async
@@ -65,14 +65,17 @@
     await software_status() #returns a dictionary with information about the current software
 ```
 
 #### Informational
 
 ```python
     uuid() #Unique identifier
+    manufacturer() #Manufacturer
+    model_name() #Model Name
+    friendly_name() #Friendly Name
     await name() #Name of device
     await room() #Name of room
     await is_in_standby() #returns true if in standby
     await transport_state() #returns one of Stopped, Playing, Paused or Buffering.
     volume_enabled #property true if the volume service is available
     await volume_level() #returns the volume setting or None if disabled
     await is_muted() #returns true if muted or None if disabled
```

### Comparing `openhomedevice-2.1/README.md` & `openhomedevice-2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     await software_status() #returns a dictionary with information about the current software
 ```
 
 #### Informational
 
 ```python
     uuid() #Unique identifier
+    manufacturer() #Manufacturer
+    model_name() #Model Name
+    friendly_name() #Friendly Name
     await name() #Name of device
     await room() #Name of room
     await is_in_standby() #returns true if in standby
     await transport_state() #returns one of Stopped, Playing, Paused or Buffering.
     volume_enabled #property true if the volume service is available
     await volume_level() #returns the volume setting or None if disabled
     await is_muted() #returns true if muted or None if disabled
```

### Comparing `openhomedevice-2.1/openhomedevice/device.py` & `openhomedevice-2.2/openhomedevice/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,23 @@
     #     while True:
     #         await asyncio.sleep(120)
     #         await self.server.event_handler.async_resubscribe_all()
 
     def uuid(self):
         return self.device.udn
 
+    def manufacturer(self):
+        return self.device.manufacturer
+    
+    def model_name(self):
+        return self.device.model_name
+    
+    def friendly_name(self):
+        return self.device.friendly_name
+
     async def name(self):
         action = self.product_service.action("Product")
         return (await action.async_call())["Name"]
 
     async def room(self):
         action = self.product_service.action("Product")
         return (await action.async_call())["Room"]
```

### Comparing `openhomedevice-2.1/openhomedevice/didl_lite.py` & `openhomedevice-2.2/openhomedevice/didl_lite.py`

 * *Files identical despite different names*

### Comparing `openhomedevice-2.1/openhomedevice.egg-info/PKG-INFO` & `openhomedevice-2.2/openhomedevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhomedevice
-Version: 2.1
+Version: 2.2
 Summary: Provides an API for requesting information from an Openhome device
 Home-page: https://github.com/bazwilliams/openhomedevice
 Author: Barry John Williams
 Author-email: barry@bjw.me.uk
 License: UNKNOWN
 Download-URL: https://github.com/bazwilliams/openhomedevice/tarball/2.1
 Keywords: upnp,dlna,openhome,linn,ds,music,render,async
@@ -65,14 +65,17 @@
     await software_status() #returns a dictionary with information about the current software
 ```
 
 #### Informational
 
 ```python
     uuid() #Unique identifier
+    manufacturer() #Manufacturer
+    model_name() #Model Name
+    friendly_name() #Friendly Name
     await name() #Name of device
     await room() #Name of room
     await is_in_standby() #returns true if in standby
     await transport_state() #returns one of Stopped, Playing, Paused or Buffering.
     volume_enabled #property true if the volume service is available
     await volume_level() #returns the volume setting or None if disabled
     await is_muted() #returns true if muted or None if disabled
```

### Comparing `openhomedevice-2.1/setup.py` & `openhomedevice-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'openhomedevice',
-  version = '2.1',
+  version = '2.2',
   author = 'Barry John Williams',
   author_email = 'barry@bjw.me.uk',
   description='Provides an API for requesting information from an Openhome device',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/bazwilliams/openhomedevice',
   packages=setuptools.find_packages(),
```

