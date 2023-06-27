# Comparing `tmp/wlkatapython-0.0.5.tar.gz` & `tmp/wlkatapython-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkatapython-0.0.5.tar", last modified: Tue Jun 27 08:16:54 2023, max compression
+gzip compressed data, was "wlkatapython-0.0.6.tar", last modified: Tue Jun 27 08:25:05 2023, max compression
```

## Comparing `wlkatapython-0.0.5.tar` & `wlkatapython-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:16:54.243347 wlkatapython-0.0.5/
--rw-rw-rw-   0        0        0      213 2023-06-27 08:16:54.242350 wlkatapython-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-27 08:16:54.243347 wlkatapython-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      290 2023-06-27 08:16:27.000000 wlkatapython-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:16:54.242350 wlkatapython-0.0.5/wlkatapython.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-27 08:16:54.000000 wlkatapython-0.0.5/wlkatapython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-06-27 08:16:54.000000 wlkatapython-0.0.5/wlkatapython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:16:54.000000 wlkatapython-0.0.5/wlkatapython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 08:16:54.000000 wlkatapython-0.0.5/wlkatapython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10108 2023-06-27 08:08:23.000000 wlkatapython-0.0.5/wlkatapython.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:25:05.436064 wlkatapython-0.0.6/
+-rw-rw-rw-   0        0        0      208 2023-06-27 08:25:05.435060 wlkatapython-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:25:05.436064 wlkatapython-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      285 2023-06-27 08:24:28.000000 wlkatapython-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:25:05.435060 wlkatapython-0.0.6/wlkatapython.egg-info/
+-rw-rw-rw-   0        0        0      208 2023-06-27 08:25:05.000000 wlkatapython-0.0.6/wlkatapython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-06-27 08:25:05.000000 wlkatapython-0.0.6/wlkatapython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:25:05.000000 wlkatapython-0.0.6/wlkatapython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 08:25:05.000000 wlkatapython-0.0.6/wlkatapython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10136 2023-06-27 08:24:17.000000 wlkatapython-0.0.6/wlkatapython.py
```

### Comparing `wlkatapython-0.0.5/wlkatapython.py` & `wlkatapython-0.0.6/wlkatapython.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 '''
 wlkata python库包含USB口控制和RS485控制
-版本号0.0.5
+版本号0.0.6
 '''
 
 import re
+import time
+import serial
 
 class Wlkata_UART:
     def __init__(self):
         self.mirobot_state_all = {"state": "-1",
                                   "angle_A": -1, "angle_B": -1, "angle_C": -1, "angle_D": -1, "angle_X": -1, "angle_Y": -1,
                                   "angle_Z": -1,
                                   "coordinate_X": -1, "coordinate_Y": -1, "coordinate_Z": -1, "coordinate_RX": -1,
```

