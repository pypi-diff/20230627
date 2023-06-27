# Comparing `tmp/srsinst.sr542-0.0.4.tar.gz` & `tmp/srsinst.sr542-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument drivers to GIT\sr542\dist\.tmp-vpln9xgx\srsinst.sr542-0.0.4.tar", last modified: Thu Jun 22 23:39:49 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument drivers to GIT\sr542\dist\.tmp-w9oe2cao\srsinst.sr542-0.1.0.tar", last modified: Tue Jun 27 00:48:15 2023, max compression
```

## Comparing `srsinst.sr542-0.0.4.tar` & `srsinst.sr542-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.090114 srsinst.sr542-0.0.4/
--rw-rw-rw-   0        0        0     1968 2023-02-10 18:32:29.000000 srsinst.sr542-0.0.4/.gitignore
--rw-rw-rw-   0        0        0     1109 2023-02-22 20:10:02.000000 srsinst.sr542-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      979 2023-06-22 23:39:49.090114 srsinst.sr542-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-02-22 18:05:50.000000 srsinst.sr542-0.0.4/README.md
--rw-rw-rw-   0        0        0     1184 2023-06-21 20:03:57.000000 srsinst.sr542-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 23:39:49.090114 srsinst.sr542-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-02-22 20:10:14.000000 srsinst.sr542-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.056980 srsinst.sr542-0.0.4/srsinst/
-drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.080111 srsinst.sr542-0.0.4/srsinst/sr542/
--rw-rw-rw-   0        0        0      141 2023-06-22 23:38:27.000000 srsinst.sr542-0.0.4/srsinst/sr542/__init__.py
--rw-rw-rw-   0        0        0      485 2023-02-22 18:12:00.000000 srsinst.sr542-0.0.4/srsinst/sr542/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.090114 srsinst.sr542-0.0.4/srsinst/sr542/instruments/
--rw-rw-rw-   0        0        0     6234 2023-06-21 21:19:56.000000 srsinst.sr542-0.0.4/srsinst/sr542/instruments/components.py
--rw-rw-rw-   0        0        0      699 2023-04-06 22:20:23.000000 srsinst.sr542-0.0.4/srsinst/sr542/instruments/get_instruments.py
--rw-rw-rw-   0        0        0     1005 2023-02-24 22:33:04.000000 srsinst.sr542-0.0.4/srsinst/sr542/instruments/keys.py
--rw-rw-rw-   0        0        0     1111 2023-02-24 18:57:33.000000 srsinst.sr542-0.0.4/srsinst/sr542/instruments/sr542.py
--rw-rw-rw-   0        0        0     1270 2023-02-23 00:10:07.000000 srsinst.sr542-0.0.4/srsinst/sr542/sr542 with sr860.taskconfig
--rw-rw-rw-   0        0        0       62 2023-02-22 20:14:03.000000 srsinst.sr542-0.0.4/srsinst/sr542/sr542.taskconfig
-drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.080111 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/
--rw-rw-rw-   0        0        0      979 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-06-22 23:39:49.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 00:48:15.198834 srsinst.sr542-0.1.0/
+-rw-rw-rw-   0        0        0     1968 2023-02-10 18:32:29.000000 srsinst.sr542-0.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1109 2023-02-22 20:10:02.000000 srsinst.sr542-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5662 2023-06-27 00:48:15.198834 srsinst.sr542-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4863 2023-06-27 00:43:18.000000 srsinst.sr542-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1184 2023-06-21 20:03:57.000000 srsinst.sr542-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 00:48:15.198834 srsinst.sr542-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-02-22 20:10:14.000000 srsinst.sr542-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 00:48:15.184430 srsinst.sr542-0.1.0/srsinst/
+drwxrwxrwx   0        0        0        0 2023-06-27 00:48:15.198834 srsinst.sr542-0.1.0/srsinst/sr542/
+-rw-rw-rw-   0        0        0      141 2023-06-27 00:43:55.000000 srsinst.sr542-0.1.0/srsinst/sr542/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-02-22 18:12:00.000000 srsinst.sr542-0.1.0/srsinst/sr542/__main__.py
+-rw-rw-rw-   0        0        0      258 2023-06-27 00:43:18.000000 srsinst.sr542-0.1.0/srsinst/sr542/dutyFactorControl.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-27 00:48:15.198834 srsinst.sr542-0.1.0/srsinst/sr542/instruments/
+-rw-rw-rw-   0        0        0     6242 2023-06-27 00:43:18.000000 srsinst.sr542-0.1.0/srsinst/sr542/instruments/components.py
+-rw-rw-rw-   0        0        0      699 2023-04-06 22:20:23.000000 srsinst.sr542-0.1.0/srsinst/sr542/instruments/get_instruments.py
+-rw-rw-rw-   0        0        0     1005 2023-02-24 22:33:04.000000 srsinst.sr542-0.1.0/srsinst/sr542/instruments/keys.py
+-rw-rw-rw-   0        0        0     1111 2023-02-24 18:57:33.000000 srsinst.sr542-0.1.0/srsinst/sr542/instruments/sr542.py
+-rw-rw-rw-   0        0        0     1270 2023-02-23 00:10:07.000000 srsinst.sr542-0.1.0/srsinst/sr542/sr542 with sr860.taskconfig
+-rw-rw-rw-   0        0        0       62 2023-02-22 20:14:03.000000 srsinst.sr542-0.1.0/srsinst/sr542/sr542.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-27 00:48:15.198834 srsinst.sr542-0.1.0/srsinst/sr542/tasks/
+-rw-rw-rw-   0        0        0     4799 2023-06-27 00:43:18.000000 srsinst.sr542-0.1.0/srsinst/sr542/tasks/dutyfactorcontrol.py
+drwxrwxrwx   0        0        0        0 2023-06-27 00:48:15.188834 srsinst.sr542-0.1.0/srsinst.sr542.egg-info/
+-rw-rw-rw-   0        0        0     5662 2023-06-27 00:48:15.000000 srsinst.sr542-0.1.0/srsinst.sr542.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-06-27 00:48:15.000000 srsinst.sr542-0.1.0/srsinst.sr542.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 00:48:15.000000 srsinst.sr542-0.1.0/srsinst.sr542.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-27 00:48:15.000000 srsinst.sr542-0.1.0/srsinst.sr542.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-06-27 00:48:15.000000 srsinst.sr542-0.1.0/srsinst.sr542.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 00:48:15.000000 srsinst.sr542-0.1.0/srsinst.sr542.egg-info/top_level.txt
```

### Comparing `srsinst.sr542-0.0.4/.gitignore` & `srsinst.sr542-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.4/LICENSE.txt` & `srsinst.sr542-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.4/pyproject.toml` & `srsinst.sr542-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.4/srsinst/sr542/instruments/components.py` & `srsinst.sr542-0.1.0/srsinst/sr542/instruments/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         Keys.DIFF: 5,
         Keys.CTRL: 6,
     }
     motor_state = DictCommand('MOTR', OffOnDict)
 
     def __init__(self, parent):
         super().__init__(parent)
-        self.frequency_monitor = FloatIndexCommand('MFRQ', 6, 0, Operate.FrequencyMonitorDict)
+        self.frequency_monitor = FloatIndexGetCommand('MFRQ', 6, 0, Operate.FrequencyMonitorDict)
         self.slots = IntIndexGetCommand('SLOT', 1, 0, Operate.SlotDict)
         self.add_parent_to_index_commands()
 
     def run(self):
         self.motor_state = Keys.ON
 
     def stop(self):
@@ -145,15 +145,16 @@
         Keys.PL: 3,
         Keys.CMAX: 4,
         Keys.TMAX: 5,
         Keys.ChopperHeadMemoryFail: 6,
         Keys.ChopperHeadDisconnect: 7
     }
 
-    last_error = IntCommand('LERR')
+    last_error = IntGetCommand('LERR')
+
     status_byte = IntGetCommand('*STB')
     status_enable_byte = IntCommand('*SRE')
     event_status_byte = IntGetCommand('*ESR')
     event_enable_byte = IntCommand('*ESE')
     chopper_condition_byte = IntGetCommand('CHCR')
     chopper_condition_positive_transition_byte = IntCommand('CHPT')
     chopper_condition_negative_transition_byte = IntCommand('CHNT')
```

### Comparing `srsinst.sr542-0.0.4/srsinst/sr542/instruments/get_instruments.py` & `srsinst.sr542-0.1.0/srsinst/sr542/instruments/get_instruments.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.4/srsinst/sr542/instruments/keys.py` & `srsinst.sr542-0.1.0/srsinst/sr542/instruments/keys.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.4/srsinst/sr542/instruments/sr542.py` & `srsinst.sr542-0.1.0/srsinst/sr542/instruments/sr542.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.4/srsinst/sr542/sr542 with sr860.taskconfig` & `srsinst.sr542-0.1.0/srsinst/sr542/sr542 with sr860.taskconfig`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.4/srsinst.sr542.egg-info/SOURCES.txt` & `srsinst.sr542-0.1.0/srsinst.sr542.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,13 +8,15 @@
 srsinst.sr542.egg-info/SOURCES.txt
 srsinst.sr542.egg-info/dependency_links.txt
 srsinst.sr542.egg-info/entry_points.txt
 srsinst.sr542.egg-info/requires.txt
 srsinst.sr542.egg-info/top_level.txt
 srsinst/sr542/__init__.py
 srsinst/sr542/__main__.py
+srsinst/sr542/dutyFactorControl.taskconfig
 srsinst/sr542/sr542 with sr860.taskconfig
 srsinst/sr542/sr542.taskconfig
 srsinst/sr542/instruments/components.py
 srsinst/sr542/instruments/get_instruments.py
 srsinst/sr542/instruments/keys.py
-srsinst/sr542/instruments/sr542.py
+srsinst/sr542/instruments/sr542.py
+srsinst/sr542/tasks/dutyfactorcontrol.py
```

