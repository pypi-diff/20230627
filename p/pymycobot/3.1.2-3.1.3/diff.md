# Comparing `tmp/pymycobot-3.1.2.tar.gz` & `tmp/pymycobot-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.1.2.tar", last modified: Thu Jun 15 07:11:33 2023, max compression
+gzip compressed data, was "pymycobot-3.1.3.tar", last modified: Tue Jun 27 03:25:27 2023, max compression
```

## Comparing `pymycobot-3.1.2.tar` & `pymycobot-3.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:11:33.694346 pymycobot-3.1.2/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.2/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    59099 2023-06-15 07:11:33.693335 pymycobot-3.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 07:11:33.663475 pymycobot-3.1.2/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.2/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1554 2023-06-15 07:09:04.000000 pymycobot-3.1.2/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.2/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    12276 2023-06-15 06:45:38.000000 pymycobot-3.1.2/pymycobot/common.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.2/pymycobot/error.py
--rw-rw-rw-   0        0        0    33758 2023-06-15 06:42:33.000000 pymycobot-3.1.2/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.2/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.2/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.2/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     9015 2023-06-12 07:33:26.000000 pymycobot-3.1.2/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13315 2023-04-14 05:34:53.000000 pymycobot-3.1.2/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.2/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.2/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.2/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7503 2023-06-15 06:42:39.000000 pymycobot-3.1.2/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.2/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8483 2023-05-23 05:43:01.000000 pymycobot-3.1.2/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.2/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19631 2023-05-24 08:27:45.000000 pymycobot-3.1.2/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.2/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:11:33.691332 pymycobot-3.1.2/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    59099 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 07:11:33.695731 pymycobot-3.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:25:27.086076 pymycobot-3.1.3/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.3/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    59140 2023-06-27 03:25:27.085080 pymycobot-3.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 03:25:27.054361 pymycobot-3.1.3/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.3/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1554 2023-06-27 03:25:13.000000 pymycobot-3.1.3/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.3/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    12276 2023-06-15 06:45:38.000000 pymycobot-3.1.3/pymycobot/common.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.3/pymycobot/error.py
+-rw-rw-rw-   0        0        0    33758 2023-06-15 06:42:33.000000 pymycobot-3.1.3/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.3/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.3/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.3/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     9080 2023-06-27 03:24:18.000000 pymycobot-3.1.3/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13314 2023-06-27 03:24:50.000000 pymycobot-3.1.3/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.3/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.3/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.3/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     7566 2023-06-27 03:24:05.000000 pymycobot-3.1.3/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.3/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     8548 2023-06-27 03:24:57.000000 pymycobot-3.1.3/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.3/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.3/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.3/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:25:27.083077 pymycobot-3.1.3/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    59140 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 03:25:27.086076 pymycobot-3.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.3/setup.py
```

### Comparing `pymycobot-3.1.2/LICENSE` & `pymycobot-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/PKG-INFO` & `pymycobot-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -2701,7 +2703,9 @@
 
 
 ### start()
 Start playing
 
 ---
 More demo can go to [here](../demo).
+
+
```

### Comparing `pymycobot-3.1.2/README.md` & `pymycobot-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/Interface.py` & `pymycobot-3.1.3/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/__init__.py` & `pymycobot-3.1.3/pymycobot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.1.2"
+__version__ = "3.1.3"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.1.2/pymycobot/bluet.py` & `pymycobot-3.1.3/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/common.py` & `pymycobot-3.1.3/pymycobot/common.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/error.py` & `pymycobot-3.1.3/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/generate.py` & `pymycobot-3.1.3/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/log.py` & `pymycobot-3.1.3/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/myarm.py` & `pymycobot-3.1.3/pymycobot/myarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,8 +251,11 @@
                 1 - Turn on transparent transmission. verify all data.\n
                 2 - Turn on transparent transmission, only verify the configuration information of communication forwarding mode (default is 0)
         """
         return self._mesg(ProtocolCode.GET_SSID_PWD, mode)
     
     def close(self):
         self._serial_port.close()
+        
+    def open(self):
+        self._serial_port.open()
```

### Comparing `pymycobot-3.1.2/pymycobot/mybuddy.py` & `pymycobot-3.1.3/pymycobot/mybuddy.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,8 +391,8 @@
     def close(self):
         self._serial_port.close()   
             
     def open(self):
         self._serial_port.open()
         
     def is_open(self):
-        return self._serial_port.isOpen()
+        return self._serial_port.is_open
```

### Comparing `pymycobot-3.1.2/pymycobot/mybuddybluetooth.py` & `pymycobot-3.1.3/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/mybuddyemoticon.py` & `pymycobot-3.1.3/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/mybuddysocket.py` & `pymycobot-3.1.3/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/mycobot.py` & `pymycobot-3.1.3/pymycobot/mycobot.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,7 +209,10 @@
     # Other
     def wait(self, t):
         time.sleep(t)
         return self
     
     def close(self):
         self._serial_port.close()
+        
+    def open(self):
+        self._serial_port.open()
```

### Comparing `pymycobot-3.1.2/pymycobot/mycobotsocket.py` & `pymycobot-3.1.3/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/mypalletizer.py` & `pymycobot-3.1.3/pymycobot/mypalletizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,7 +241,10 @@
             
         """
         data_list = [[25, 21], [26, 32]]
         return self._mesg(ProtocolCode.GET_ACCEI_DATA, data_list[1] if value else data_list[0], has_reply=True)
     
     def close(self):
         self._serial_port.close()
+        
+    def open(self):
+        self._serial_port.open()
```

### Comparing `pymycobot-3.1.2/pymycobot/mypalletizersocket.py` & `pymycobot-3.1.3/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot/ultraArm.py` & `pymycobot-3.1.3/pymycobot/ultraArm.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,7 +577,10 @@
                         print("Retry receive...")
             command = ""
 
         self.set_speed_mode(2)  # Acceleration / deceleration mode
         
     def close(self):
         self._serial_port.close()
+        
+    def open(self):
+        self._serial_port.open()
```

### Comparing `pymycobot-3.1.2/pymycobot/utils.py` & `pymycobot-3.1.3/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.1.3/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -2701,7 +2703,9 @@
 
 
 ### start()
 Start playing
 
 ---
 More demo can go to [here](../demo).
+
+
```

### Comparing `pymycobot-3.1.2/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.1.3/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.2/setup.py` & `pymycobot-3.1.3/setup.py`

 * *Files identical despite different names*

