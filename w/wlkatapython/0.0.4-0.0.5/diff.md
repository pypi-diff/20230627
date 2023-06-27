# Comparing `tmp/wlkatapython-0.0.4.tar.gz` & `tmp/wlkatapython-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkatapython-0.0.4.tar", last modified: Thu Jun  1 13:06:21 2023, max compression
+gzip compressed data, was "wlkatapython-0.0.5.tar", last modified: Tue Jun 27 08:16:54 2023, max compression
```

## Comparing `wlkatapython-0.0.4.tar` & `wlkatapython-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 13:06:21.236503 wlkatapython-0.0.4/
--rw-rw-rw-   0        0        0      367 2023-06-01 13:06:21.236503 wlkatapython-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 13:06:21.236503 wlkatapython-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-06-01 13:06:02.000000 wlkatapython-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:06:21.235501 wlkatapython-0.0.4/wlkatapython.egg-info/
--rw-rw-rw-   0        0        0      367 2023-06-01 13:06:21.000000 wlkatapython-0.0.4/wlkatapython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-06-01 13:06:21.000000 wlkatapython-0.0.4/wlkatapython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 13:06:21.000000 wlkatapython-0.0.4/wlkatapython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-01 13:06:21.000000 wlkatapython-0.0.4/wlkatapython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10136 2023-06-01 11:48:59.000000 wlkatapython-0.0.4/wlkatapython.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:16:54.243347 wlkatapython-0.0.5/
+-rw-rw-rw-   0        0        0      213 2023-06-27 08:16:54.242350 wlkatapython-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:16:54.243347 wlkatapython-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      290 2023-06-27 08:16:27.000000 wlkatapython-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:16:54.242350 wlkatapython-0.0.5/wlkatapython.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-27 08:16:54.000000 wlkatapython-0.0.5/wlkatapython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-06-27 08:16:54.000000 wlkatapython-0.0.5/wlkatapython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:16:54.000000 wlkatapython-0.0.5/wlkatapython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 08:16:54.000000 wlkatapython-0.0.5/wlkatapython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10108 2023-06-27 08:08:23.000000 wlkatapython-0.0.5/wlkatapython.py
```

### Comparing `wlkatapython-0.0.4/wlkatapython.py` & `wlkatapython-0.0.5/wlkatapython.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 '''
 wlkata python库包含USB口控制和RS485控制
-版本号0.0.2
+版本号0.0.5
 '''
-import serial
-import time
+
 import re
 
 class Wlkata_UART:
     def __init__(self):
         self.mirobot_state_all = {"state": "-1",
                                   "angle_A": -1, "angle_B": -1, "angle_C": -1, "angle_D": -1, "angle_X": -1, "angle_Y": -1,
                                   "angle_Z": -1,
@@ -75,15 +74,15 @@
     #停止当前程序
     def cancellation(self):
         self.sendMsg("o117")
 
     # 舵机夹爪指令
     def gripper(self, num):
         self.num = num
-        if self.num == ture:
+        if self.num == True:
             self.sendMsg("M3 S40")
         else:
             self.sendMsg("M3 S60")
 
     # 气泵控制
     def pump(self, num):
         self.num = num
@@ -279,8 +278,7 @@
 
     #运动模式查询
     def getmooe(self):
         self.getStatus()
         return self.mirobot_state_all["mooe"]
 
 
-
```

