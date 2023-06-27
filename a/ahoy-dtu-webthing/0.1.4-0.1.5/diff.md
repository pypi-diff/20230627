# Comparing `tmp/ahoy_dtu_webthing-0.1.4.tar.gz` & `tmp/ahoy_dtu_webthing-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.1.4.tar", last modified: Tue Jun 27 05:09:48 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.1.5.tar", last modified: Tue Jun 27 05:15:22 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.1.4.tar` & `ahoy_dtu_webthing-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:48.686747 ahoy_dtu_webthing-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 05:09:35.000000 ahoy_dtu_webthing-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 05:09:48.686747 ahoy_dtu_webthing-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-27 05:09:35.000000 ahoy_dtu_webthing-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:48.682747 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 05:09:35.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-27 05:09:35.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-27 05:09:35.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-06-27 05:09:35.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:48.686747 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 05:09:48.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 05:09:48.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:09:48.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 05:09:48.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 05:09:48.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 05:09:48.000000 ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 05:09:35.000000 ahoy_dtu_webthing-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 05:09:48.686747 ahoy_dtu_webthing-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:15:22.625698 ahoy_dtu_webthing-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 05:15:07.000000 ahoy_dtu_webthing-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 05:15:22.625698 ahoy_dtu_webthing-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-27 05:15:07.000000 ahoy_dtu_webthing-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:15:22.625698 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 05:15:07.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-27 05:15:07.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-27 05:15:07.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-06-27 05:15:07.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:15:22.625698 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 05:15:22.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 05:15:22.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:15:22.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 05:15:22.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 05:15:22.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 05:15:22.000000 ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 05:15:07.000000 ahoy_dtu_webthing-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 05:15:22.625698 ahoy_dtu_webthing-0.1.5/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.1.4/LICENSE` & `ahoy_dtu_webthing-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.4/PKG-INFO` & `ahoy_dtu_webthing-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.1.4/README.md` & `ahoy_dtu_webthing-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing/dtu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from threading import Thread
+from random import randint
 import re
 import requests
 import logging
 from time import sleep
 from datetime import datetime
 
 class Inverter:
@@ -41,14 +42,15 @@
         self.listener = None
         Thread(target=self.__periodic_refresh, daemon=True).start()
 
     def close(self):
         self.is_running = False
 
     def __periodic_refresh(self):
+        sleep(randint(0,self.interval))
         while self.is_running:
             try:
                 self.refresh()
             except Exception as e:
                 logging.warning("error occurred refreshing inverter " + self.name + " " + str(e) + " (max " + str(self.power_max) + " watt)")
             sleep(int(self.interval/2))
```

### Comparing `ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.4/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.1.5/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

