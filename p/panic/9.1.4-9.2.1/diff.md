# Comparing `tmp/panic-9.1.4.tar.gz` & `tmp/panic-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/panic-9.1.4.tar", last modified: Tue Feb 28 18:18:04 2023, max compression
+gzip compressed data, was "dist/panic-9.2.1.tar", last modified: Tue Jun 27 05:10:06 2023, max compression
```

## Comparing `panic-9.1.4.tar` & `panic-9.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:18:04.000000 panic-9.1.4/
--rw-r--r--   0 srubio    (1206) Control   (1200)     3685 2022-04-25 13:54:49.000000 panic-9.1.4/LICENSE
--rw-r--r--   0 srubio    (1206) Control   (1200)       79 2022-04-25 13:54:49.000000 panic-9.1.4/MANIFEST.in
--rw-r--r--   0 srubio    (1206) Control   (1200)      737 2023-02-28 18:18:04.000000 panic-9.1.4/PKG-INFO
--rw-r--r--   0 srubio    (1206) Control   (1200)     2552 2022-04-25 13:54:49.000000 panic-9.1.4/README.rst
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:18:04.000000 panic-9.1.4/bin/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      584 2023-02-23 14:53:43.000000 panic-9.1.4/bin/PyAlarm
--rwxr-xr-x   0 srubio    (1206) Control   (1200)       91 2023-02-22 19:24:39.000000 panic-9.1.4/bin/panic
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:18:04.000000 panic-9.1.4/extra/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-04-25 13:54:49.000000 panic-9.1.4/extra/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     4873 2023-02-22 19:22:00.000000 panic-9.1.4/extra/report.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:18:04.000000 panic-9.1.4/panic/
--rw-r--r--   0 srubio    (1206) Control   (1200)    11270 2023-02-22 19:22:00.000000 panic-9.1.4/panic/CHANGES
--rw-r--r--   0 srubio    (1206) Control   (1200)   128768 2023-02-22 16:19:59.000000 panic-9.1.4/panic/PyAlarm.ctsaal01.py
--rw-r--r--   0 srubio    (1206) Control   (1200)        6 2023-02-28 18:16:42.000000 panic-9.1.4/panic/VERSION
--rw-r--r--   0 srubio    (1206) Control   (1200)     1443 2023-02-22 19:22:00.000000 panic-9.1.4/panic/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    83850 2023-02-22 19:27:53.000000 panic-9.1.4/panic/alarmapi.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:18:04.000000 panic-9.1.4/panic/ds/
--rw-r--r--   0 srubio    (1206) Control   (1200)    13141 2023-02-22 19:22:00.000000 panic-9.1.4/panic/ds/PanicViewDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)   128841 2023-02-27 15:36:04.000000 panic-9.1.4/panic/ds/PyAlarm.py
--rw-r--r--   0 srubio    (1206) Control   (1200)       23 2023-02-23 14:16:32.000000 panic-9.1.4/panic/ds/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)       52 2023-02-23 14:59:27.000000 panic-9.1.4/panic/ds/__main__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    10493 2023-02-22 19:22:00.000000 panic-9.1.4/panic/ds/kpi.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     1801 2023-02-22 19:22:00.000000 panic-9.1.4/panic/engine.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:18:04.000000 panic-9.1.4/panic/gui/
--rw-r--r--   0 srubio    (1206) Control   (1200)      106 2023-02-22 19:24:39.000000 panic-9.1.4/panic/gui/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    16965 2023-02-22 19:24:39.000000 panic-9.1.4/panic/gui/actions.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    10024 2023-02-22 19:25:17.000000 panic-9.1.4/panic/gui/alarmhistory.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     8276 2023-02-22 19:28:40.000000 panic-9.1.4/panic/gui/devattrchange.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    31331 2023-02-22 19:30:08.000000 panic-9.1.4/panic/gui/editor.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    46877 2023-02-22 19:31:01.000000 panic-9.1.4/panic/gui/gui.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     1975 2023-02-22 19:24:39.000000 panic-9.1.4/panic/gui/htmlview.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:18:04.000000 panic-9.1.4/panic/gui/icon/
--rw-r--r--   0 srubio    (1206) Control   (1200)      628 2022-04-25 13:54:50.000000 panic-9.1.4/panic/gui/icon/panel-view.png
--rw-r--r--   0 srubio    (1206) Control   (1200)    26077 2022-04-25 13:54:50.000000 panic-9.1.4/panic/gui/icon/panic-6-banner.png
--rw-r--r--   0 srubio    (1206) Control   (1200)    19419 2022-04-25 13:54:50.000000 panic-9.1.4/panic/gui/icon/panic-6-banner.svg
--rw-r--r--   0 srubio    (1206) Control   (1200)    17102 2022-04-25 13:54:50.000000 panic-9.1.4/panic/gui/icon/panic-6-big.png
--rw-r--r--   0 srubio    (1206) Control   (1200)     3150 2022-04-25 13:54:50.000000 panic-9.1.4/panic/gui/icon/panic-6.png
--rw-r--r--   0 srubio    (1206) Control   (1200)    13278 2022-04-25 13:54:50.000000 panic-9.1.4/panic/gui/icon/panic-6.svg
--rw-r--r--   0 srubio    (1206) Control   (1200)     7793 2022-04-25 13:54:50.000000 panic-9.1.4/panic/gui/icon/panic-icon.gif
--rw-r--r--   0 srubio    (1206) Control   (1200)    31662 2022-04-25 13:54:50.000000 panic-9.1.4/panic/gui/icon/panic-icon.svg
--rw-r--r--   0 srubio    (1206) Control   (1200)    10603 2023-02-22 19:22:00.000000 panic-9.1.4/panic/gui/panel.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    12053 2023-02-22 19:24:39.000000 panic-9.1.4/panic/gui/phonebook.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     1910 2023-02-22 19:22:00.000000 panic-9.1.4/panic/gui/status.py
--rw-r--r--   0 srubio    (1206) Control   (1200)      802 2023-02-22 19:22:00.000000 panic-9.1.4/panic/gui/toolbar.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    23011 2023-02-22 19:24:39.000000 panic-9.1.4/panic/gui/ui_data.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    10635 2023-02-22 19:31:22.000000 panic-9.1.4/panic/gui/ui_gui.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    31856 2023-02-22 19:25:16.000000 panic-9.1.4/panic/gui/utils.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     3870 2023-02-22 19:24:39.000000 panic-9.1.4/panic/gui/views.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    14110 2023-02-22 19:22:00.000000 panic-9.1.4/panic/properties.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     7058 2023-02-22 19:22:00.000000 panic-9.1.4/panic/test.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    26887 2023-02-22 19:24:39.000000 panic-9.1.4/panic/view.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    19325 2023-02-22 19:31:54.000000 panic-9.1.4/panic/widgets.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:18:04.000000 panic-9.1.4/panic.egg-info/
--rw-r--r--   0 srubio    (1206) Control   (1200)      737 2023-02-28 18:18:04.000000 panic-9.1.4/panic.egg-info/PKG-INFO
--rw-r--r--   0 srubio    (1206) Control   (1200)     1108 2023-02-28 18:18:04.000000 panic-9.1.4/panic.egg-info/SOURCES.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        1 2023-02-28 18:18:04.000000 panic-9.1.4/panic.egg-info/dependency_links.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       20 2023-02-28 18:18:04.000000 panic-9.1.4/panic.egg-info/entry_points.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       24 2023-02-28 18:18:04.000000 panic-9.1.4/panic.egg-info/requires.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       12 2023-02-28 18:18:04.000000 panic-9.1.4/panic.egg-info/top_level.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       38 2023-02-28 18:18:04.000000 panic-9.1.4/setup.cfg
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1559 2023-02-23 14:03:39.000000 panic-9.1.4/setup.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-06-27 05:10:06.000000 panic-9.2.1/
+-rw-r--r--   0 srubio    (1206) Control   (1200)     3685 2023-06-20 07:10:38.000000 panic-9.2.1/LICENSE
+-rw-r--r--   0 srubio    (1206) Control   (1200)       79 2023-06-20 07:10:38.000000 panic-9.2.1/MANIFEST.in
+-rw-r--r--   0 srubio    (1206) Control   (1200)      737 2023-06-27 05:10:06.000000 panic-9.2.1/PKG-INFO
+-rw-r--r--   0 srubio    (1206) Control   (1200)     2552 2023-06-20 07:10:38.000000 panic-9.2.1/README.rst
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-06-27 05:10:05.000000 panic-9.2.1/bin/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      592 2023-06-20 07:10:38.000000 panic-9.2.1/bin/PyAlarm
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)       91 2023-06-20 07:10:38.000000 panic-9.2.1/bin/panic
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-06-27 05:10:05.000000 panic-9.2.1/panic/
+-rw-r--r--   0 srubio    (1206) Control   (1200)    11270 2023-06-20 07:10:39.000000 panic-9.2.1/panic/CHANGES
+-rw-r--r--   0 srubio    (1206) Control   (1200)   128768 2023-06-20 07:10:39.000000 panic-9.2.1/panic/PyAlarm.ctsaal01.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)        6 2023-06-21 16:12:00.000000 panic-9.2.1/panic/VERSION
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1534 2023-06-21 16:00:23.000000 panic-9.2.1/panic/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    84480 2023-06-21 16:02:53.000000 panic-9.2.1/panic/alarmapi.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-06-27 05:10:05.000000 panic-9.2.1/panic/ds/
+-rw-r--r--   0 srubio    (1206) Control   (1200)    13141 2023-06-20 07:10:39.000000 panic-9.2.1/panic/ds/PanicViewDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)   131353 2023-06-21 16:02:53.000000 panic-9.2.1/panic/ds/PyAlarm.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)       25 2023-06-20 07:10:39.000000 panic-9.2.1/panic/ds/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)       52 2023-06-20 07:10:39.000000 panic-9.2.1/panic/ds/__main__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    10493 2023-06-20 07:10:39.000000 panic-9.2.1/panic/ds/kpi.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1801 2023-06-20 07:10:39.000000 panic-9.2.1/panic/engine.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-06-27 05:10:05.000000 panic-9.2.1/panic/extra/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-06-21 15:59:35.000000 panic-9.2.1/panic/extra/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     4873 2023-06-21 15:59:35.000000 panic-9.2.1/panic/extra/report.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-06-27 05:10:06.000000 panic-9.2.1/panic/gui/
+-rw-r--r--   0 srubio    (1206) Control   (1200)      128 2023-06-21 16:08:37.000000 panic-9.2.1/panic/gui/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    17563 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/actions.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    10024 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/alarmhistory.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     8276 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/devattrchange.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    31331 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/editor.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    46928 2023-06-21 16:09:16.000000 panic-9.2.1/panic/gui/gui.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1975 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/htmlview.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-06-27 05:10:06.000000 panic-9.2.1/panic/gui/icon/
+-rw-r--r--   0 srubio    (1206) Control   (1200)      628 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/icon/panel-view.png
+-rw-r--r--   0 srubio    (1206) Control   (1200)    26077 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/icon/panic-6-banner.png
+-rw-r--r--   0 srubio    (1206) Control   (1200)    19419 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/icon/panic-6-banner.svg
+-rw-r--r--   0 srubio    (1206) Control   (1200)    17102 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/icon/panic-6-big.png
+-rw-r--r--   0 srubio    (1206) Control   (1200)     3150 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/icon/panic-6.png
+-rw-r--r--   0 srubio    (1206) Control   (1200)    13278 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/icon/panic-6.svg
+-rw-r--r--   0 srubio    (1206) Control   (1200)     7793 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/icon/panic-icon.gif
+-rw-r--r--   0 srubio    (1206) Control   (1200)    31662 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/icon/panic-icon.svg
+-rw-r--r--   0 srubio    (1206) Control   (1200)    10603 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/panel.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    12053 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/phonebook.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1910 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/status.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)      802 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/toolbar.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    23011 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/ui_data.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    10635 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/ui_gui.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    32757 2023-06-21 16:02:53.000000 panic-9.2.1/panic/gui/utils.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     3870 2023-06-20 07:10:40.000000 panic-9.2.1/panic/gui/views.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    14113 2023-06-21 15:59:35.000000 panic-9.2.1/panic/properties.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     7058 2023-06-20 07:10:39.000000 panic-9.2.1/panic/test.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    26887 2023-06-20 07:19:08.000000 panic-9.2.1/panic/view.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    19325 2023-06-20 07:10:39.000000 panic-9.2.1/panic/widgets.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-06-27 05:10:05.000000 panic-9.2.1/panic.egg-info/
+-rw-r--r--   0 srubio    (1206) Control   (1200)      737 2023-06-27 05:10:05.000000 panic-9.2.1/panic.egg-info/PKG-INFO
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1120 2023-06-27 05:10:05.000000 panic-9.2.1/panic.egg-info/SOURCES.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        1 2023-06-27 05:10:05.000000 panic-9.2.1/panic.egg-info/dependency_links.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       20 2023-06-27 05:10:05.000000 panic-9.2.1/panic.egg-info/entry_points.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       24 2023-06-27 05:10:05.000000 panic-9.2.1/panic.egg-info/requires.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        6 2023-06-27 05:10:05.000000 panic-9.2.1/panic.egg-info/top_level.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       38 2023-06-27 05:10:06.000000 panic-9.2.1/setup.cfg
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1559 2023-06-20 07:11:03.000000 panic-9.2.1/setup.py
```

### Comparing `panic-9.1.4/LICENSE` & `panic-9.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/PKG-INFO` & `panic-9.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: panic
-Version: 9.1.4
+Version: 9.2.1
 Summary: PANIC, a python Alarm System for TANGO
 Home-page: UNKNOWN
 Author: Sergi Rubio
 Author-email: srubio@cells.es
 Maintainer: Sergi Rubio
 Maintainer-email: srubio@cells.es
 License: UNKNOWN
```

### Comparing `panic-9.1.4/README.rst` & `panic-9.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/bin/PyAlarm` & `panic-9.2.1/bin/PyAlarm`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
    [ $(which screen 2>/dev/null) ] ; then
   echo "run detached"
   CMD="screen -dm -S $DS-$INSTANCE "
 else
   CMD=""
 fi
 
-CMD="${CMD} ${VPYTHON} -m panic.ds $INSTANCE $2"
+CMD="${CMD} ${VPYTHON} -m panic.ds.PyAlarm $INSTANCE $2"
 echo $CMD
 $CMD
```

### Comparing `panic-9.1.4/extra/report.py` & `panic-9.2.1/panic/extra/report.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/CHANGES` & `panic-9.2.1/panic/CHANGES`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/PyAlarm.ctsaal01.py` & `panic-9.2.1/panic/PyAlarm.ctsaal01.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/__init__.py` & `panic-9.2.1/panic/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,10 +39,16 @@
 # import view
 
 from .view import AlarmView
 from .properties import *
 from .alarmapi import *
 from .alarmapi import Alarm, AlarmAPI, AlarmDS, api, getAttrValue
 
+try:
+    from . import gui
+except:
+    print('Unable to import panic.gui')
+    gui = None
+
 # from utils import *
 
 _proxies = alarmapi._proxies
```

### Comparing `panic-9.1.4/panic/alarmapi.py` & `panic-9.2.1/panic/alarmapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 
     return substitute(new_message, substitutions, depth - 1)
 
 
 ###############################################################################
 # @todo: Tango access methods
 
+@fandango.CatchedArgs(throw=False)
 def getAttrValue(obj, default=Exception):
     """
     Extracts rvalue in tango/taurus3/4 compatible way
     If default = True, obj is returned
     If default = Exception, only exception objects are returned (else None)
     """
     rm = getattr(obj, 'read', None)
@@ -1129,15 +1130,16 @@
                     r[tag] = r[tag] or END_OF_TIME
         return r
 
     def get_acknowledged(self, alarm=None):
         if self._acknowledged is None:
             self._acknowledged = CachedAttributeProxy(
                 self.name + '/AcknowledgedAlarms', keeptime=3000.)
-        value = getAttrValue(self._acknowledged)
+        value = getAttrValue(self._acknowledged)# or []
+        #print('alarm(%s)._acknowledged: %s' % (alarm,value))
         if alarm is not None:
             return getattr(alarm, 'tag', alarm) in value
         else:
             return value
 
     def get_disabled(self, alarm=None):
         if self._disabled is None:
@@ -1246,14 +1248,16 @@
         if isinstance(k, Alarm):
             return self.__get_tag(k.tag)
         elif clmatch(retango, k):
             if ':' in k:
                 self.warning('[%s]: AlarmAPI does not support multi-host!' % k)
             else:
                 k = k.split('/')[-1]
+        if k not in self.alarms:
+            k = first((t for t in self.alarms if k.lower()==t.lower()),k)
         return k
 
     def __getitem__(self, k):  # *a,**k):
         return self.alarms.__getitem__(self.__get_tag(k))  # *a,**k)
 
     def __setitem__(self, k, v):
         return self.alarms.__setitem__(self.__get_tag(k), v)
@@ -1802,39 +1806,52 @@
         formula = self[exps[0]].formula
         for e in exps[1:]:
             r = e.partition('=')
             formula = formula.replace(r[0].strip(), r[-1].strip())
         return formula
 
     def split_formula(self, formula, keep_operators=False):
+        """
+        Split formula into individual sections separated by and/or
+        """
         f = self[formula].formula if formula in self else formula
         i, count, buff, final = 0, 0, '', []
+        x = 0
         while i < len(f):
-            s = f[i]
-            if s in '([{': count += 1
-            if s in ')]}': count -= 1
-            if not count and s in ' \t':
-                if f[i:i + 4].strip().lower() == 'or':
+            x += 1 #needed to prevent endless loops
+            if x>2048: 
+                break
+        
+            nx, s = '', f[i]
+            if s in '([{': 
+                count += 1
+            if s in ')]}': 
+                count -= 1
+            
+            if not count and (s in ' \t' or i>=len(f)-1):
+                # found free space or end of formula
+                #print('limit',i,'"%s"'%s,'"%s"'%buff,len(f.strip())-1)
+                if f[i:i + 4].strip().split()[0].lower() == 'or':
                     nx = 'or'
-                    i += len(nx) + 2
-                elif f[i:i + 5].strip().lower() == 'and':
+                elif f[i:i + 5].strip().split()[0].lower() == 'and':
                     nx = 'and'
-                    i += len(nx) + 2
-                else:
-                    nx = ''
-                if nx:
-                    final.append(buff.strip())
-                    if keep_operators:
-                        final.append(nx)
-                    buff = ''
-                    continue
 
             buff += s
+            
+            if not count and nx or i>=len(f)-1:
+                #print('append',i,buff,nx)
+                final.append(buff.strip())
+                if keep_operators:
+                    final.append(nx)
+                i += len(nx) + 2
+                buff = ''
+                continue ### i not incremented!?
+
             i += 1
-            nx = ''
+            
         return final
 
     def parse_alarms(self, formula):
         """
         Searches for alarm tags used in the formula
         """
         alnum = '(?:^|[^/a-zA-Z0-9-_])([a-zA-Z0-9-_]+)'  # (?:$|[^/a-zA-Z0-9-_])'
```

### Comparing `panic-9.1.4/panic/ds/PanicViewDS.py` & `panic-9.2.1/panic/ds/PanicViewDS.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/ds/PyAlarm.py` & `panic-9.2.1/panic/ds/PyAlarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,24 +158,24 @@
 #     Device States Description:
 #
 #   DevState.ON :     ActiveAlarms list is empty
 #   DevState.ALARM :  Size of ActiveAlarms is >=1
 # ==================================================================
 
 
-class PyAlarm(tango.Device_4Impl, fandango.log.Logger):
+class PyAlarm(tango.LatestDeviceImpl, fandango.log.Logger):
     # --------- Add your global variables here --------------------------
 
     Panic = None
 
     # --------------------------------------------------------------------------
     # Overriding Quality-based Tango state machine
     def set_state(self, state):
         self._state = state
-        tango.Device_4Impl.set_state(self, state)
+        tango.LatestDeviceImpl.set_state(self, state)
 
     def get_state(self):
         # @Tango6
         # This have been overriden as it seemed not well managed when connecting devices in a same server
         return self._state
 
     def dev_state(self):
@@ -187,15 +187,15 @@
         """ State redefinition is required to keep independency between 
         attribute configuration (max/min alarms) and the device State """
         # return self.get_state()
         return self._state
 
     def set_status(self, status):
         self._status = status
-        tango.Device_4Impl.set_status(self, status)
+        tango.LatestDeviceImpl.set_status(self, status)
 
     def get_status(self):
         return self._status
 
     def dev_status(self):
         return self._status
 
@@ -222,14 +222,15 @@
 
             elif self.worker and not (self.worker._process.is_alive()
                                       and self.worker._receiver.is_alive()):
                 self.set_state(tango.DevState.FAULT)
                 self.eval_status = 'Alarm Values not being processed!!!'
                 self.set_status(self.eval_status)
             else:
+                self.debug('StateMachine:get_enabled()')
                 if self.get_enabled():
                     self.set_state(tango.DevState.ALARM if actives
                                    else tango.DevState.ON)
                     status = "There are {}/{} active alarms\n".format(len(actives), len(self.Alarms))
 
                 else:
                     self.set_state(tango.DevState.DISABLE)
@@ -593,14 +594,15 @@
         if self.worker and self.worker.is_alive(): self.worker.stop()
         return
 
     ##@}
 
     ###########################################################################
 
+    @fandango.Cached(depth=2,expire=3.)
     def get_enabled(self, force=False):
         e = str(self.Enabled).lower().strip()
         last = self.PastValues.get('Enabled', (0, 0))
         # t is time passed since start
         t = int(time.time() - (self.TStarted + self.StartupDelay))
 
         if e in ('true', '1', 'yes', 'enabled'):
@@ -608,14 +610,15 @@
         elif e in ('', 'false', '0', 'no', 'none', 'disabled'):
             r = None
         elif e == 'nan':
             r = fandango.NaN
         elif fandango.matchCl('^[0-9]+$', e):
             r = t > int(e)
         elif not force and last[0] and (t - last[0]) < self.PollingPeriod:
+            # This condition is done now by Cached decorator
             # return last cached value
             return last[1]
         else:
             # Evaluating an alarm formula
             try:
                 self.FailedAlarms.pop('Enabled', None)
                 r = self.EvaluateFormula(self.Enabled, as_string=False, _locals={'t': t})
@@ -705,14 +708,15 @@
                                       not self.CheckDisabled(a[0]))  # copied without disabled alarms
                 finally:
                     self.lock.release()
                 self.debug('\n' +
                            'Enabled alarms to process in next {} s cycle (UseProcess={}): {} '
                            .format(self.PollingPeriod, self.UseProcess, [a[0] for a in myAlarms])
                            + '\n' + '#' * 80)
+                self.debug('updateAlarms:get_enabled()')
                 if not self.get_enabled(force=True):
                     self.info('ALARM SENDING IS DISABLED!!')
 
                 ###############################################################
                 # NOT using a subProcess and Using Taurus to update the variables
                 if not self.worker and self.UseTaurus:
                     try:  # When using Taurus it will minimize the CPU usage
@@ -772,15 +776,15 @@
         Process method called from updateAlarms for each alarm
         """
 
         now = self.last_attribute_check = time.time()
         ##########################################################
         alarm.get_state(force=True)
         WAS_OK = alarm.counter < self.AlarmThreshold
-        self.info('Checking alarm tag {}'.format(tag_name))
+        self.info('>>> process_alarm({})'.format(tag_name))
         self.debug(alarm.formula)
 
         # Cache management
         # try: del self.LastValues.pop(tag_name)
         # except: self.error(traceback.format_exc())
         self.LastValues[tag_name] = variables = {}
 
@@ -943,23 +947,26 @@
                     # self.PastValues[tag_name] = None
                     self.Alarms[tag_name].clear()
                     self.Alarms[tag_name].set_time()
                     self.info("Alarm {}:{} cleared".format(date, tag_name))
 
                     if tag_name in self.AcknowledgedAlarms:
                         self.AcknowledgedAlarms.remove(tag_name)
-
+                        
+                    result = True
+                
             self.alarm_attr_read(tag_name)  # pushing is done here
         except:
             s = traceback.format_exc()
             self.warning('free_alarm({}) failed!:1: {}'.format(tag_name, s))
         finally:
             self.lock.release()
 
         try:  # NOTIFICATION SHOULD NOT BE WITHIN THE LOCK
+            self.debug('free_alarm:get_enabled()')
             if was_active and self.get_enabled() and notify:
                 # This is executed only when called from ResetAlarm() command
                 # AutoReset notification is called from updateAlarms to include attribute values in report
                 self.send_alarm(tag_name, message=message or 'RESET', comment=comment)
 
         except:
             self.warning('free_alarm({}) failed!:2: {}'.format(tag_name, traceback.format_exc()))
@@ -979,15 +986,16 @@
          - Triggers snapshots for ALARMS
          - Saves HTML report
 
         ACKNOWLEDGE/RESET messages are not managed here, but in free_alarm
         """
         self.info('\n\n')
         self.info('=' * 80)
-        self.info(shortstr('In PyAlarm.send_alarm({},{},{})'.format(tag_name, message, values), 255))
+        self.info(shortstr('In PyAlarm.send_alarm({},{},{})'.format(
+            tag_name, message, values), 255))
         alarm = (self.Alarms.get(tag=tag_name) or [None])[0]
         try:
             if alarm and self.MaxMessagesPerAlarm and self.Alarms[tag_name].sent >= self.MaxMessagesPerAlarm:
                 # This counter is reset calling .clear() from free_alarm()
                 self.debug('*' * 80)
                 self.warning(
                     'Too many alarms ({}) already sent for {}!!!'.format(self.Alarms[tag_name].sent, tag_name))
@@ -1005,32 +1013,36 @@
                 self.info(('{} receivers:\n\t{}\n\tmail:{}\n\t'
                            'sms:{}\n\ttg:{}\n\taction[{}]: {}'.format(
                     tag_name, alarm.receivers, mail_receivers, sms_receivers,
                     tg_receivers, len(action_receivers), action_receivers)))
             finally:
                 self.lock.release()
 
-            self.info('\n\n')
+            self.info('\n%s.message: %s\n'%(tag_name,message))
             if message not in ('ALARM', 'REMINDER') and not self.AlertOnRecovery:
                 mail_receivers = sms_receivers = tg_receivers = []
 
             if alarm:
                 report = self.GenerateReport(tag_name, mail_receivers or '', message=message,
                                              user_comment=comment, values=values)
             else:
                 # Sending a test message (no alarm involved)
                 report = [message, tag_name + '-' + message, ','.join(mail_receivers)]
+            
+            self.debug('report: %s' % str(report)[:60])
 
+            self.debug('send_alarm:get_enabled()')
             if self.get_enabled():
 
                 def rcatched(method):
 
                     def _rcatched(*args, **kwargs):
 
-                        self.info('send_alarm({}) => {}({},{})'.format(tag_name, method, args, kwargs))
+                        self.debug('send_alarm({}) => {}({},{})'.format(
+                            tag_name, method, args, kwargs))
                         try:
                             r = method(*args, **kwargs)
                         except:
                             msg = getattr(method, '__name__', str(method))
                             msg = '{} crashed! \n{}'.format(msg, traceback.format_exc())
                             self.warning(msg)
                             report[0] += '\n' + '-' * 80 + '\n' + msg
@@ -1082,14 +1094,15 @@
                 # html logs
                 if self.parse_receivers(tag_name, 'HTML', receivers, message=message):
                     r = rcatched(self.GenerateReport)(tag_name, message=message,
                                                       values=values, html=True)
                     rcatched(self.SaveHtml)(r)
 
                 ## emails
+                self.debug('mail_receivers: ' + str(mail_receivers))
                 if mail_receivers:
                     r = rcatched(self.SendMail)(report)
 
                 self.info('-' * 80), self.update_flag_file()
 
             else:
                 self.info('=============> ALARM SENDING DISABLED!!')
@@ -1105,14 +1118,15 @@
                 self.Alarms[tag_name].last_sent = time.time()
 
             return report
 
         except Exception as e:
             self.warning('PyAlarm.send_alarm crashed with exception:\n{}'
                          .format(traceback.format_exc()))
+            sys.exit(-1)
         self.info('-' * 80)
         return ''
 
     def update_flag_file(self):
         ''' If there's Active Alarms writes a 1 to the file specified
         by FlagFile property, else writes 0 '''
         try:
@@ -1364,15 +1378,15 @@
 
     # ------------------------------------------------------------------
     #    Device constructor
     # ------------------------------------------------------------------
     def __init__(self, cl, name):
         # This code should be executed only at server_init() and not at device.init()
         print('In PyAlarm.__init__({},{})'.format(cl, name))
-        tango.Device_4Impl.__init__(self, cl, name)
+        tango.LatestDeviceImpl.__init__(self, cl, name)
         self.call__init__(fandango.log.Logger, name,
                           use_tango=True,  # already True by default, printf may cause I/O issues
                           format='%(levelname)-8s %(asctime)s %(name)s: %(message)s')
 
         self.setLogLevel('DEBUG')
         panic._proxies[name] = self
         init_callbacks(period_ms=50.)
@@ -1524,14 +1538,19 @@
                 ##this patch must be DEPRECATED
                 # if self.PollingPeriod>3600:
                 # self.warning('PERIODS IN MILLISECONDS ARE DEPRECATED!: '
                 # '{} ms >> {} s'
                 # %(self.PollingPeriod,self.PollingPeriod*1e-3))
                 ##Converting from ms to s
                 # self.PollingPeriod = self.PollingPeriod*1e-3
+                
+                try:
+                    self.get_enabled.__func__.expire = self.PollingPeriod
+                except Exception as e:
+                    print(str(e))
 
                 if (str(self.AlertOnRecovery).strip().lower()
                         in ('false', 'no', 'none')):
                     self.AlertOnRecovery = ''
 
                 if str(self.Reminder).strip().lower() == 'false': self.Reminder = 0
 
@@ -1561,15 +1580,16 @@
 
                 if self.UseProcess and PROCESS and not self.worker:
 
                     # Do not reduce worker timeout or you may have problems
                     # if main thread idles (e.g. Tango database is down)
                     self.info('Configuring WorkerProcess ...')
                     self.worker = WorkerProcess(self.Eval, start=True,
-                                                timeout=self.PollingPeriod * max((self.AlarmThreshold, 3)))
+                                        timeout = self.PollingPeriod 
+                                            * max((self.AlarmThreshold, 3)))
                     self.worker.send('set_timeout', 'set_timeout',
                                      self.EvalTimeout)
                     self.worker.command('import threading')
 
                     # ,timewait=0.05*self.PollingPeriod/len(self.Alarms))
                     self.worker.add('previous', target='dict([(k,str(v)) '
                                                        'for k,v in executor.previous.items()])',
@@ -1619,14 +1639,24 @@
 
             if not self.updateThread or not self.updateThread.is_alive():
                 self.pause.clear()
                 self.start()
 
             self.info('Ready to accept request ...')
             self.info('#' * 80)
+            if self.LogLevel == 'DEFAULT':
+                if any('-v%s'%s in str(sys.argv) for s in '23'):
+                    self.LogLevel = 'INFO'
+                elif any('-v%s'%s in str(sys.argv) for s in '456789'):
+                    self.LogLevel = 'DEBUG'
+                elif '-v0' in str(sys.argv):
+                    self.LogLevel = 'ERROR'
+                else:
+                    self.LogLevel = 'WARNING'
+                    
             self.setLogLevel(self.LogLevel)
 
         except Exception as e:
             self.info('Exception in PyAlarm.init_device(): \n{}'
                       .format(traceback.format_exc()))
             self.set_state(tango.DevState.FAULT)
             raise e
@@ -1636,20 +1666,20 @@
             self.kill.clear()
         return
 
     # ------------------------------------------------------------------
     #    Always excuted hook method
     # ------------------------------------------------------------------
     def always_executed_hook(self):
-        self.debug("In " + self.get_name() + "::always_excuted_hook()")
+        self.debug("In " + self.get_name() + "::always_executed_hook()")
         now = time.time()
         # Status/Events processed only once per second
         if (self.last_status + 1.) <= now:
             self.StateMachine()
-        self.debug("Out of " + self.get_name() + "::always_excuted_hook()")
+        self.debug("Out of " + self.get_name() + "::always_executed_hook()")
 
     # ==================================================================
     #
     #    PyAlarm read/write attribute methods
     #
     # ==================================================================
     # ------------------------------------------------------------------
@@ -1918,14 +1948,16 @@
                     STATE = True
                     raise Exception('UNKNOWN ALARM {}!!'.format(tag_name))
             else:
                 if 'debug' in str(self.getLogLevel()).lower():
                     self.Eval._trace = True
 
                 VALUE = self.Eval.eval(formula, _raise=RAISE)
+                
+            self.info('Result: ' + str(VALUE))
             ##################################################################
 
             if tag_name:  # not external
                 # variables value returned as process_alarms cache
                 variables.update(
                     self.get_last_values(alarm=tag_name, variables=varnames))
             else:
@@ -1959,15 +1991,15 @@
                     self.FailedAlarms[tag_name] = desc
                 self.info('-> Exceptions in Non-State attributes ({}) '
                           'do not trigger Alarm'.format(tag_name or formula))
 
         finally:
             self.lock.release() if lock else None
 
-        if external:
+        if as_string and external:
             return ('{} (IgnoreExceptions={},RethrowState={},'
                     'RethrowAttribute={})'
                     .format(VALUE, self.IgnoreExceptions, self.RethrowState,
                             self.RethrowAttribute))
         else:
             self.EvalTimes[tag_name] = time.time() - t0
             return str(VALUE) if as_string else VALUE
@@ -1984,15 +2016,20 @@
         self.info("In " + self.get_name() + "::ResetAlarm()")
         #    Add your own code here
         if len(argin) == 1:
             raise Exception('UserMessageRequiredAs2ndArgument')  # tag,userMessage = argin[0],''
         else:
             tag, userMessage = argin[:2]
 
-        argout = self.get_active_alarms() if self.free_alarm(tag, userMessage, message='RESET') else []
+        if self.EvaluateFormula(self.Alarms[tag].formula):
+            if userMessage != 'FORCED':
+                raise Exception('AlarmConditionsStillActive!')
+        
+        r = self.free_alarm(tag, userMessage, message='RESET')
+        argout = self.get_active_alarms() if r else []
         return argout
 
     # ------------------------------------------------------------------
     #    Acknowledge command:
     #
     #    Description: Acknowledge alarm no more reminders will be sent
     #
@@ -2233,15 +2270,15 @@
     #
     #    argin:  DevVarStringArray    tag,message,receivers,...,description
     #    argout: DevVarStringArray
     # ------------------------------------------------------------------
 
     def GenerateReport(self, tag, receivers='', message='DETAILS',
                        values=None, user_comment=None, html=False,
-                       evals=False, others=False, pasts=False):
+                       evals=False, others=False, pasts=False, sections=True):
         """
         When called from Tango a single argument is received; which is a list
         containing all arguments
 
         :param message: Can be one of MESSAGE_TYPES or a different text
         """
         self.info('In GenerateReport({},{},{})'.format(tag, receivers, message))
@@ -2310,22 +2347,40 @@
         elif message not in MESSAGE_TYPES:
             first_row = '\n\t{}'.format(message)
 
         report += first_row
         report += '\n\tAlarmDevice: {}'.format(self.get_name())
         report += '\n\tDescription: {}'.format(self.Alarms[tag].parse_description())
         report += '\n\tSeverity: {}'.format(self.Alarms[tag].parse_severity())
-        report += '\n\tFormula: {}'.format(self.Alarms[tag].formula)
+        
+        formula = self.Eval.parse_formula(
+            self.Alarms[tag].formula, macros=['COPY(%s)']) # apply macros
+        report += '\n\tFormula: {}'.format(formula)
+        
+        sections = sections and self.Panic.split_formula(formula)       
+        if sections:
+            try:
+                report += '\n'
+                for s in sections:
+                    try:
+                        s = self.Eval.parse_formula(s)
+                        r = str(self.EvaluateFormula(s,as_string=False))
+                    except Exception as e:
+                        r = str(e)
+                        
+                    report += '\nEval: \t%s\nResult: \t%s\n' % (s,r)
+            except:
+                self.error('Unable to parse sections')
+                traceback.print_exc()
 
         if values:
             report += '\n\n' + 'Values are: \n'
             if hasattr(values, 'items'):
                 try:
-                    invkey = lambda t: (t[-1], t[0])
-                    for k, v in sorted(values.items(), key=invkey):
+                    for k, v in sorted(values.items()):
                         m = fandango.tango.parse_tango_model(k)
                         dev = m and m.get('devicename')
                         attr = m and m.get('attribute')
                         if dev in self.Panic.devices and attr in self.Panic:
                             k = attr
                         elif k.lower().strip().endswith('/state'):
                             v = str(tango.DevState.values.get(v, v))
@@ -2335,32 +2390,42 @@
                 except:
                     msg = traceback.format_exc()
                     report += str(values).strip() or msg
                     self.error('Error parsing values for email:\n{}'.format(msg))
             else:
                 report += str(values).strip()
 
-        report += '\n\n' + 'Alarm receivers are:' + '\n\t{}'.format(alarm.receivers)
+        report += '\nAlarm receivers are:\n\t{}\n'.format(alarm.receivers)
+        
         if evals:
-            report += '\n\n' + 'EvalTimes are: \n {}\n'.format(self.EvalTimes)
+            report += '\nEvalTimes are: \n {}\n'.format(self.EvalTimes)
+            
         if others and len(actives) > 1:
             try:
                 report += ('\n\n' + 'Other Active Alarms are:'
                            + '\n\t'.join([''] + sorted(
                             ['{}:{}:{}'.format(k, time2str(v.active),
                                                self.Alarms[k].formula)
                              for k, v in self.Alarms.items() if v.active])))
             except:
                 pass
 
         if pasts and self.PastAlarms:
             report += ('\n\n' + 'Past Alarms were:' + '\n\t'.join(['']
-                                                                  + ['{}:{}'.format(','.join(k), time2str(d))
-                                                                     for d, k in
-                                                                     sorted(self.PastAlarms.items())[-10:]]))
+                    + ['{}:{}'.format(','.join(k), time2str(d))
+                        for d, k in
+                        sorted(self.PastAlarms.items())[-10:]]))
+        try:
+            cf = self.Panic.get_device(alarm.device).get_config()
+            report += '\n\nPyAlarm Configuration:\n'
+            for k in sorted(ALARM_CYCLE):
+                report += '\n\t%s.%s : %s' % (alarm.device,k,str(cf.get(k,None)))
+        except:
+            traceback.print_exc()
+            
         if html:
             result = [report, subject]
         else:
             result = [report, subject, ','.join(maillist)]
 
         self.Reports[tag] = {(tag, message, alarm.active, html): result}
         self.debug('Out of GenerateReport({},{},{})'.format(tag, receivers, message))
@@ -2371,14 +2436,15 @@
         sep = ';'  # ';' #','
         # setup = 'tag','description','formula'
         setup = SUMMARY_FIELDS
 
         [alarm.get_state(force=True) for alarm in self.Alarms.values()]
         attr_AlarmSummary_read = []
         for alarm in self.Alarms.values():
+            self.debug('GenerateSummary:get_enabled()')
             l = ['{}={}'.format(s, (str if s != 'time' else time2str)
             (getattr(alarm, s) if s != 'state' or self.get_enabled()
              else 'DSUPR')) for s in setup]
             attr_AlarmSummary_read.append(sep.join(l))
 
         # Should be True only when called from Commands
         if push:
@@ -2517,15 +2583,16 @@
                 self.info('Launching mail command: ' + shortstr(command, 512))
                 # & needed in Debian to avoid timeouts
                 os.system(command + ' &')
 
                 for m in argin[2].split(','):
                     self.SentEmails[m.lower()] += 1
 
-                return 'DONE'
+            return 'DONE'
+        
         except Exception:
             self.info('Exception in PyAlarm.SendMail(): \n{}'.format(traceback.format_exc()))
         return 'FAILED'
 
     # ------------------------------------------------------------------
     #    SaveHtml command:
     #
```

### Comparing `panic-9.1.4/panic/ds/kpi.py` & `panic-9.2.1/panic/ds/kpi.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/engine.py` & `panic-9.2.1/panic/engine.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/actions.py` & `panic-9.2.1/panic/gui/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,18 @@
             act.setEnabled(len(items) == 1)
             self.popMenu.addAction(getThemeIcon("applications-system"),
                                    "Advanced Config", lambda s=self: ShowConfig(s))
             self.popMenu.addSeparator()
             act = self.popMenu.addAction(
                 getThemeIcon("accessories-text-editor"), "TestDevice",
                 lambda d=alarm.device: testDevice(d))
+            
+            act = self.popMenu.addAction(
+                getThemeIcon("applications-system"), "Restart Server",
+                lambda d=alarm.device: restartServer(d))            
 
             act.setEnabled(len(items) == 1)
 
         # self.popMenu.addSeparator()
         # self.popMenu.addAction(getThemeIcon("process-stop"), "close App",self.close)
 
         if getattr(self, '_manager', None):
@@ -263,14 +267,24 @@
     return alarms
 
 
 def testDevice(device):
     import os
     os.system('tg_devtest %s &' % device)
 
+def restartServer(device):
+    astor = fn.Astor(device) 
+    devs = astor.get_all_devices()
+    v = QMessageBox.warning(self, 'Warning',
+                            'Following devices will be affected: \n%s'
+                                % '\n'.join(devs),
+                            QMessageBox.Ok | QMessageBox.Cancel)
+    if v == QMessageBox.Cancel:
+        return    
+    astor.restart_servers()
 
 def emitValueChanged(self):
     if hasattr(self, 'emitValueChanged'):
         self.emitValueChanged()
     elif hasattr(self, 'valueChanged'):
         self.valueChanged()
         # [o.get_acknowledged(force=True) for o in items]
```

### Comparing `panic-9.1.4/panic/gui/alarmhistory.py` & `panic-9.2.1/panic/gui/alarmhistory.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/devattrchange.py` & `panic-9.2.1/panic/gui/devattrchange.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/editor.py` & `panic-9.2.1/panic/gui/editor.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/gui.py` & `panic-9.2.1/panic/gui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,16 @@
 
 
 
 """
 
 OPEN_WINDOWS = []
 
-import panic.gui.utils as widgets
-
-widgets.TRACE_LEVEL = 0  # -1
+from . import utils
+utils.TRACE_LEVEL = 0  # -1
 
 ###########################################################################
 
 PARENT_CLASS = Qt.QWidget
 
 
 class QAlarmList(QAlarmManager, PARENT_CLASS):
@@ -113,32 +112,32 @@
         self.changed = True
         self.severities = []  # List to keep severities currently visible
 
         self.expert = False
         self.tools = {}  # Widgets dictionary
 
         self.scope = options.get('scope', '*')  # filters or '*'
-        exported = options.get('exported', '')
+        self.exported = options.get('exported', '')
         self.default_regEx = options.get('default', filters or '*')
         self.regEx = self.default_regEx
         self.NO_ICON = Qt.QIcon()
 
         refresh = int(options.get('refresh', self.REFRESH_TIME))
         self.REFRESH_TIME = refresh
         # AlarmRow.REFRESH_TIME = refresh
 
         # if self.regEx not in ('','*'):
         # print 'Setting RegExp filter: %s'%self.regEx
         # self._ui.regExLine.setText(str(self.regEx))
 
         print('AlarmGUI(%s, %s)' % (api, self.scope))
         self.api = api or panic.AlarmAPI(None)
-        self.api.load(self.scope, exported=exported)
+        self.api.load(self.scope, exported=self.exported)
         print('AlarmGUI(%s,%s): api done, %d devs, %d alarms' %
-              (self.scope, exported, len(self.api.devices),
+              (self.scope, self.exported, len(self.api.devices),
                len(self.api.alarms)))
 
         self.init_ui(parent, mainwindow)  # init_mw is called here
 
         # @TODO: api-based views are not multi-host
         self.view = panic.view.AlarmView(api=self.api,
                                          scope=self.scope,
@@ -243,15 +242,15 @@
             trace('onReload(%s)' % self.RELOAD_TIME)
             print('+' * 80)
             now = time.time()
             trace('%s -> AlarmGUI.onReload() after %f seconds' % (
                 now, now - self.last_reload))
             self.last_reload = now
             self._ui.listWidget.clearSelection()
-            self.api.load()
+            self.api.load(self.scope, exported=self.exported)
             if not self.api.keys():
                 trace('NO ALARMS FOUND IN DATABASE!?!?')
             self.setSecondCombo()
             # self.checkAlarmRows()
 
             # Updating the alarm list
             self.buildList(changed=False)
@@ -968,15 +967,15 @@
         tmw.toolsMenu.addAction(getThemeIcon("x-office-address-book"),
                                 "PhoneBook", alarmApp.tools['bookApp'].show)
         toolbar.addAction(getThemeIcon("x-office-address-book"),
                           "PhoneBook", alarmApp.tools['bookApp'].show)
 
         trend_action = (getThemeIcon(":/designer/qwtplot.png"),
                         'Trend',
-                        lambda: WindowManager.addWindow(widgets.get_archive_trend(show=True))
+                        lambda: WindowManager.addWindow(utils.get_archive_trend(show=True))
                         )
         tmw.toolsMenu.addAction(*trend_action)
         toolbar.addAction(*trend_action)
 
         alarmApp.tools['config'] = WindowManager.addWindow(
             dacWidget(container=tmw))
         tmw.toolsMenu.addAction(getThemeIcon("applications-system"),
@@ -1202,16 +1201,16 @@
         self._ui.deleteButton.setEnabled(self.expert)  # show()
         self.expert = check
         return
 
     ###########################################################################
 
 
-def main(args):
-    AlarmGUI.main(args)
+def main(args=None):
+    AlarmGUI.main(args or sys.argv[1:])
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
 
 try:
     from fandango.doc import get_fn_autodoc
```

### Comparing `panic-9.1.4/panic/gui/htmlview.py` & `panic-9.2.1/panic/gui/htmlview.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/icon/panel-view.png` & `panic-9.2.1/panic/gui/icon/panel-view.png`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/icon/panic-6-banner.png` & `panic-9.2.1/panic/gui/icon/panic-6-banner.png`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/icon/panic-6-banner.svg` & `panic-9.2.1/panic/gui/icon/panic-6-banner.svg`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/icon/panic-6-big.png` & `panic-9.2.1/panic/gui/icon/panic-6-big.png`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/icon/panic-6.png` & `panic-9.2.1/panic/gui/icon/panic-6.png`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/icon/panic-6.svg` & `panic-9.2.1/panic/gui/icon/panic-6.svg`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/icon/panic-icon.gif` & `panic-9.2.1/panic/gui/icon/panic-icon.gif`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/icon/panic-icon.svg` & `panic-9.2.1/panic/gui/icon/panic-icon.svg`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/panel.py` & `panic-9.2.1/panic/gui/panel.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/phonebook.py` & `panic-9.2.1/panic/gui/phonebook.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/status.py` & `panic-9.2.1/panic/gui/status.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/toolbar.py` & `panic-9.2.1/panic/gui/toolbar.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/ui_data.py` & `panic-9.2.1/panic/gui/ui_data.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/ui_gui.py` & `panic-9.2.1/panic/gui/ui_gui.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/gui/utils.py` & `panic-9.2.1/panic/gui/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,15 @@
             self.UserValidator, self.validator = '', None
             log, p = '', str(sys.path)
             try:
                 props = getPanicProperty(['UserValidator', 'PanicAdminUsers'])
                 self.UserValidator = fandango.first(props['UserValidator'], '')
                 self.AdminUsers = list(filter(bool,
                         map(str.strip, props['PanicAdminUsers'])))
+                
                 if self.UserValidator:
                     mod, klass = self.UserValidator.rsplit('.', 1)
                     mod = fandango.objects.loadModule(mod)
                     p = mod.__file__
                     klass = getattr(mod, klass)
                     self.validator = klass()
                     try:
@@ -261,17 +262,19 @@
             except:
                 traceback.print_exc()
                 print('iValidateWidget: {} module not found in {}'
                       .format(self.UserValidator or 'PyAlarm.UserValidator', p))
                 return -1
 
         if self.AdminUsers and not self.UserValidator:
-            raise Exception('iValidateWidget(PanicAdminUsers):'
-                            ' UserValidator property not defined')
+            raise Exception('iValidateWidget(PanicAdminUsers:%s):'
+                            ' UserValidator property not defined'
+                            % self.AdminUsers)
             return -1
+        
         if not self.AdminUsers and not self.UserValidator:
             # passwords not available
             return None
         users = sorted(self.api.get_admins_for_alarm(tag))
         if not users:
             # Not using passwords for this alarm
             self.last_users = None
@@ -610,20 +613,24 @@
         """
         text = getWidgetText(self.tf)
         self.formula = formula or multiline2line(text)
         self.tf.setPlainText(line2multiline(self.formula))
         if self.org_formula is None: self.org_formula = formula
         print('In AlarmFormula.updateFormula({},changed={})'
               .format(self.formula, formula != self.org_formula))
-        if self.formula:
-            self.test.formula = self.api.replace_alarms(self.formula)
-        if parse:
-            self.test.formula = self.test.parse_formula(self.test.formula)
-        new_text = line2multiline('{}'.format(self.test.formula))
-        self.tb.setToolTip(new_text)
+        try:
+            if self.formula:
+                self.test.formula = self.api.replace_alarms(self.formula)
+            if parse:
+                self.test.formula = self.test.parse_formula(self.test.formula)
+            new_text = line2multiline('{}'.format(self.test.formula))
+            self.tb.setToolTip(new_text)
+        except Exception as e:
+            print('Failed to parse formula (may contain errors): {}'.format(e))
+            
         return self.test.formula
 
     def updateResult(self, formula=''):
         print('In AlarmFormula.updateResult({}({}))'.format(type(formula), formula))
         formula = self.updateFormula(formula, parse=not self.device)
         if self.org_formula and formula != self.org_formula:
             print('\tformula changed!')
@@ -634,14 +641,28 @@
                 result = '{}: {}'.format(self.device,
                     self.api.evaluate(
                         formula if self.device else self.test.formula,
                         device=self.device, timeout=10000, _locals=self._locals))
             except Exception as e:
                 result = '{}: {}: {}'.format(self.device, type(e).__name__, e)
                 print(result)
+            try:
+                rn = ''
+                sections = self.api.split_formula(formula)
+                print('%d sections in formula' % len(sections))
+                for f in self.api.split_formula(formula):
+                    rn += '\n{}:\n\t{}'.format(f,
+                    self.api.evaluate(
+                        formula if self.device else self.test.formula,
+                        device=self.device, timeout=10000, _locals=self._locals))
+                    rn +='\n'
+            except Exception as e:
+                    rn = traceback.format_exc()
+            finally:
+                result += '\n\n' + rn
         else:
             result = traceback.format_exc()
             print(result)
         self.tb.setPlainText(result)
         self.tb.setParent(self, Qt.Qt.Dialog)
         self.tb.setWindowModality(Qt.Qt.WindowModal)
         self.tb.show()
@@ -698,16 +719,16 @@
                 if ':' in dev and not dev.startswith('tango://'):
                     dev = 'tango://' + dev
                 model.add(dev + '/' + attr)
 
         self.model = sorted(model)
         print('In AttributesPreview.updateAttributes({})'.format(model))
         self.form.setModel(model)
-        [tvalue.setLabelConfig("<attr_fullname>")
-         for tvalue in self.form.getItems()]
+        [tvalue.setLabelConfig('{dev.name}/{attr.name}')#"<attr_fullname>")
+            for tvalue in self.form.getItems()]
         print('In AttributesPreview.updateAttributes({})'.format('done'))
 
     ###########################################################################
 
 
 class AlarmPreview(Qt.QDialog):
```

### Comparing `panic-9.1.4/panic/gui/views.py` & `panic-9.2.1/panic/gui/views.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/properties.py` & `panic-9.2.1/panic/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,15 @@
     'VersionNumber':
         [PyTango.DevString,
          "API version used (device-managed)",
          ["6.1.1"]],
     'LogLevel':
         [PyTango.DevString,
          "stdout log filter",
-         ["INFO"]],
+         ["DEFAULT"]],
     'StartupDelay':
         [PyTango.DevLong,
          "Number of seconds that PyAlarm will wait before starting.",
          [0]],
     'EvalTimeout':
         [PyTango.DevLong,
          "Timeout for read_attribute calls, in milliseconds .",
```

### Comparing `panic-9.1.4/panic/test.py` & `panic-9.2.1/panic/test.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/view.py` & `panic-9.2.1/panic/view.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic/widgets.py` & `panic-9.2.1/panic/widgets.py`

 * *Files identical despite different names*

### Comparing `panic-9.1.4/panic.egg-info/PKG-INFO` & `panic-9.2.1/panic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: panic
-Version: 9.1.4
+Version: 9.2.1
 Summary: PANIC, a python Alarm System for TANGO
 Home-page: UNKNOWN
 Author: Sergi Rubio
 Author-email: srubio@cells.es
 Maintainer: Sergi Rubio
 Maintainer-email: srubio@cells.es
 License: UNKNOWN
```

### Comparing `panic-9.1.4/panic.egg-info/SOURCES.txt` & `panic-9.2.1/panic.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 ./bin/PyAlarm
 ./bin/panic
-extra/__init__.py
-extra/report.py
 panic/CHANGES
 panic/PyAlarm.ctsaal01.py
 panic/VERSION
 panic/__init__.py
 panic/alarmapi.py
 panic/engine.py
 panic/properties.py
@@ -23,14 +21,16 @@
 panic.egg-info/requires.txt
 panic.egg-info/top_level.txt
 panic/ds/PanicViewDS.py
 panic/ds/PyAlarm.py
 panic/ds/__init__.py
 panic/ds/__main__.py
 panic/ds/kpi.py
+panic/extra/__init__.py
+panic/extra/report.py
 panic/gui/__init__.py
 panic/gui/actions.py
 panic/gui/alarmhistory.py
 panic/gui/devattrchange.py
 panic/gui/editor.py
 panic/gui/gui.py
 panic/gui/htmlview.py
```

### Comparing `panic-9.1.4/setup.py` & `panic-9.2.1/setup.py`

 * *Files identical despite different names*

