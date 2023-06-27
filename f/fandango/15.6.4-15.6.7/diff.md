# Comparing `tmp/fandango-15.6.4.tar.gz` & `tmp/fandango-15.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fandango-15.6.4.tar", last modified: Wed Feb  8 13:07:52 2023, max compression
+gzip compressed data, was "dist/fandango-15.6.7.tar", last modified: Tue Feb 28 18:15:22 2023, max compression
```

## Comparing `fandango-15.6.4.tar` & `fandango-15.6.7.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:52.000000 fandango-15.6.4/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      556 2022-05-25 08:42:07.000000 fandango-15.6.4/AUTHORS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3691 2022-05-25 08:42:07.000000 fandango-15.6.4/LICENSE
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      106 2022-05-25 08:42:07.000000 fandango-15.6.4/MANIFEST.in
--rw-r--r--   0 srubio    (1206) Control   (1200)     1272 2023-02-08 13:07:52.000000 fandango-15.6.4/PKG-INFO
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    12517 2022-11-29 16:25:41.000000 fandango-15.6.4/README.md
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:51.000000 fandango-15.6.4/fandango/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    52702 2022-05-25 08:42:07.000000 fandango-15.6.4/fandango/CHANGELOG
--rwxr-xr-x   0 srubio    (1206) Control   (1200)        7 2023-02-08 13:06:20.000000 fandango-15.6.4/fandango/VERSION
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     9232 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    58353 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/arrays.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    79005 2023-01-16 16:13:01.000000 fandango-15.6.4/fandango/callbacks.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    19336 2023-02-08 12:59:51.000000 fandango-15.6.4/fandango/db.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2702 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/debug.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:51.000000 fandango-15.6.4/fandango/device/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3760 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/device/DDebug.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    27004 2023-01-20 14:02:51.000000 fandango-15.6.4/fandango/device/Dev4Tango.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      238 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/device/DynamicDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    16925 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/device/FolderDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3630 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/device/FolderGUI.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    19656 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/device/WorkerDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      503 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/device/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    11697 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/devslist.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    33112 2022-12-12 16:43:35.000000 fandango-15.6.4/fandango/dicts.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4952 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/doc.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)   143322 2023-02-06 16:01:41.000000 fandango-15.6.4/fandango/dynamic.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    15081 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/excepts.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    57329 2023-01-17 16:35:17.000000 fandango-15.6.4/fandango/functional.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:51.000000 fandango-15.6.4/fandango/interface/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    11571 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/interface/CopyCatDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      297 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/interface/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     9345 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/interface/inheritance.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    22513 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/linos.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    18859 2022-12-16 08:49:20.000000 fandango-15.6.4/fandango/log.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    43106 2023-01-17 14:55:52.000000 fandango-15.6.4/fandango/objects.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     3747 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/pipes.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    86503 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/qt.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:51.000000 fandango-15.6.4/fandango/scripts/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2062 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/scripts/CopyCatDS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3171 2023-01-20 10:03:43.000000 fandango-15.6.4/fandango/scripts/DynamicDS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2059 2022-08-29 16:35:46.000000 fandango-15.6.4/fandango/scripts/FolderDS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2059 2022-08-29 16:35:46.000000 fandango-15.6.4/fandango/scripts/WorkerDS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      118 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/scripts/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    12037 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/scripts/csv2tango
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     8042 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/scripts/fandango
--rwxr-xr-x   0 srubio    (1206) Control   (1200)       93 2022-08-29 16:35:46.000000 fandango-15.6.4/fandango/scripts/folder-gui
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4788 2022-12-02 16:46:35.000000 fandango-15.6.4/fandango/scripts/my2to3.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1107 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/scripts/sardanact
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    44592 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/scripts/servers_lite.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1944 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/scripts/setup.ds.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     7704 2022-11-29 16:25:41.000000 fandango-15.6.4/fandango/scripts/tango2csv
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1764 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/scripts/tango2json
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      106 2022-08-29 16:35:46.000000 fandango-15.6.4/fandango/scripts/tango_cleanup
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2177 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/scripts/tango_create_device.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4053 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/scripts/tango_create_starter.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      321 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/scripts/tango_host
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     5284 2022-12-19 12:44:47.000000 fandango-15.6.4/fandango/scripts/tango_monitor
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2800 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/scripts/tango_property
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4849 2022-12-02 16:38:01.000000 fandango-15.6.4/fandango/scripts/tango_servers
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    48193 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/servers.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:51.000000 fandango-15.6.4/fandango/tango/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      462 2022-12-02 16:46:43.000000 fandango-15.6.4/fandango/tango/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     9766 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/tango/command.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    24719 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/tango/defaults.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    26945 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/tango/dynattr.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    13208 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/tango/export.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    56490 2022-12-21 14:27:38.000000 fandango-15.6.4/fandango/tango/methods.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    17024 2023-01-23 16:41:56.000000 fandango-15.6.4/fandango/tango/search.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    27175 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/tango/tangoeval.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:52.000000 fandango-15.6.4/fandango/testing/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/testing/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1254 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/testing/check_callbacks.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2164 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/testing/check_fandango.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     7260 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/testing/checkmodule.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3598 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/testing/gen_test_file.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4305 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/testing/simulation.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    69703 2022-12-02 16:46:35.000000 fandango-15.6.4/fandango/threads.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    13096 2022-11-29 16:25:42.000000 fandango-15.6.4/fandango/web.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:52.000000 fandango-15.6.4/fandango/widget/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2022-05-25 08:42:08.000000 fandango-15.6.4/fandango/widget/__init__.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:51.000000 fandango-15.6.4/fandango.egg-info/
--rw-r--r--   0 srubio    (1206) Control   (1200)     1272 2023-02-08 13:07:50.000000 fandango-15.6.4/fandango.egg-info/PKG-INFO
--rw-r--r--   0 srubio    (1206) Control   (1200)     2269 2023-02-08 13:07:50.000000 fandango-15.6.4/fandango.egg-info/SOURCES.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        1 2023-02-08 13:07:50.000000 fandango-15.6.4/fandango.egg-info/dependency_links.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       20 2023-02-08 13:07:50.000000 fandango-15.6.4/fandango.egg-info/entry_points.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        1 2022-08-29 16:49:35.000000 fandango-15.6.4/fandango.egg-info/not-zip-safe
--rw-r--r--   0 srubio    (1206) Control   (1200)       62 2023-02-08 13:07:50.000000 fandango-15.6.4/fandango.egg-info/requires.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       15 2023-02-08 13:07:50.000000 fandango-15.6.4/fandango.egg-info/top_level.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       67 2023-02-08 13:07:52.000000 fandango-15.6.4/setup.cfg
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     8044 2022-12-02 16:46:35.000000 fandango-15.6.4/setup.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:52.000000 fandango-15.6.4/tests/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-11-29 16:25:42.000000 fandango-15.6.4/tests/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    34621 2022-11-29 16:25:42.000000 fandango-15.6.4/tests/definitions.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-08 13:07:52.000000 fandango-15.6.4/tests/dependencies/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-11-29 16:25:42.000000 fandango-15.6.4/tests/dependencies/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)      175 2022-11-29 16:25:42.000000 fandango-15.6.4/tests/dependencies/dummy_module.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    42849 2022-11-29 16:25:42.000000 fandango-15.6.4/tests/test_functional.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    21320 2022-11-29 16:25:42.000000 fandango-15.6.4/tests/test_functional_auto_gen.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    14830 2022-11-29 16:25:42.000000 fandango-15.6.4/tests/test_functional_skip.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    14133 2022-11-29 16:25:42.000000 fandango-15.6.4/tests/test_objects.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      556 2022-05-25 08:42:07.000000 fandango-15.6.7/AUTHORS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3691 2022-05-25 08:42:07.000000 fandango-15.6.7/LICENSE
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      106 2022-05-25 08:42:07.000000 fandango-15.6.7/MANIFEST.in
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1272 2023-02-28 18:15:22.000000 fandango-15.6.7/PKG-INFO
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    12517 2022-11-29 16:25:41.000000 fandango-15.6.7/README.md
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:21.000000 fandango-15.6.7/fandango/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    52702 2022-05-25 08:42:07.000000 fandango-15.6.7/fandango/CHANGELOG
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)        7 2023-02-27 15:25:02.000000 fandango-15.6.7/fandango/VERSION
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     9232 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    58353 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/arrays.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    79005 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/callbacks.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    19336 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/db.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2702 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/debug.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/fandango/device/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3760 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/device/DDebug.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    27004 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/device/Dev4Tango.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      238 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/device/DynamicDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    16925 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/device/FolderDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3630 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/device/FolderGUI.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    19656 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/device/WorkerDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      503 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/device/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    11697 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/devslist.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    33112 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/dicts.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4952 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/doc.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)   143202 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/dynamic.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    15081 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/excepts.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    57329 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/functional.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/fandango/interface/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    11571 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/interface/CopyCatDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      297 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/interface/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     9345 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/interface/inheritance.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    22513 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/linos.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    18859 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/log.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    43106 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/objects.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     3747 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/pipes.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    86512 2023-02-24 14:23:53.000000 fandango-15.6.7/fandango/qt.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/fandango/scripts/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2062 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/scripts/CopyCatDS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3171 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/scripts/DynamicDS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2059 2022-08-29 16:35:46.000000 fandango-15.6.7/fandango/scripts/FolderDS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2059 2022-08-29 16:35:46.000000 fandango-15.6.7/fandango/scripts/WorkerDS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      118 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/scripts/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    12037 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/scripts/csv2tango
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     8042 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/scripts/fandango
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)       93 2022-08-29 16:35:46.000000 fandango-15.6.7/fandango/scripts/folder-gui
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4788 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/scripts/my2to3.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1107 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/scripts/sardanact
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    44592 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/scripts/servers_lite.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1944 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/scripts/setup.ds.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     7704 2022-11-29 16:25:41.000000 fandango-15.6.7/fandango/scripts/tango2csv
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1764 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/scripts/tango2json
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      106 2022-08-29 16:35:46.000000 fandango-15.6.7/fandango/scripts/tango_cleanup
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2177 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/scripts/tango_create_device.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4053 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/scripts/tango_create_starter.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      321 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/scripts/tango_host
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     5284 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/scripts/tango_monitor
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2800 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/scripts/tango_property
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4849 2022-12-02 16:38:01.000000 fandango-15.6.7/fandango/scripts/tango_servers
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    48193 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/servers.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/fandango/tango/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      462 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/tango/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     9766 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/tango/command.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    24719 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/tango/defaults.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    26945 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/tango/dynattr.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    13208 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/tango/export.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    56490 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/tango/methods.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    17024 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/tango/search.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    27254 2023-02-27 15:24:44.000000 fandango-15.6.7/fandango/tango/tangoeval.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/fandango/testing/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/testing/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1254 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/testing/check_callbacks.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2164 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/testing/check_fandango.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     7260 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/testing/checkmodule.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3598 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/testing/gen_test_file.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4305 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/testing/simulation.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    69703 2023-02-24 14:21:59.000000 fandango-15.6.7/fandango/threads.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    13096 2022-11-29 16:25:42.000000 fandango-15.6.7/fandango/web.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/fandango/widget/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2022-05-25 08:42:08.000000 fandango-15.6.7/fandango/widget/__init__.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/fandango.egg-info/
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1272 2023-02-28 18:15:20.000000 fandango-15.6.7/fandango.egg-info/PKG-INFO
+-rw-r--r--   0 srubio    (1206) Control   (1200)     2269 2023-02-28 18:15:20.000000 fandango-15.6.7/fandango.egg-info/SOURCES.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        1 2023-02-28 18:15:20.000000 fandango-15.6.7/fandango.egg-info/dependency_links.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       20 2023-02-28 18:15:20.000000 fandango-15.6.7/fandango.egg-info/entry_points.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        1 2022-08-29 16:49:35.000000 fandango-15.6.7/fandango.egg-info/not-zip-safe
+-rw-r--r--   0 srubio    (1206) Control   (1200)       62 2023-02-28 18:15:20.000000 fandango-15.6.7/fandango.egg-info/requires.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       15 2023-02-28 18:15:20.000000 fandango-15.6.7/fandango.egg-info/top_level.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       67 2023-02-28 18:15:22.000000 fandango-15.6.7/setup.cfg
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     8044 2023-02-24 14:21:59.000000 fandango-15.6.7/setup.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/tests/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-11-29 16:25:42.000000 fandango-15.6.7/tests/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    34621 2022-11-29 16:25:42.000000 fandango-15.6.7/tests/definitions.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-02-28 18:15:22.000000 fandango-15.6.7/tests/dependencies/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-11-29 16:25:42.000000 fandango-15.6.7/tests/dependencies/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)      175 2022-11-29 16:25:42.000000 fandango-15.6.7/tests/dependencies/dummy_module.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    42849 2022-11-29 16:25:42.000000 fandango-15.6.7/tests/test_functional.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    21320 2022-11-29 16:25:42.000000 fandango-15.6.7/tests/test_functional_auto_gen.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    14830 2022-11-29 16:25:42.000000 fandango-15.6.7/tests/test_functional_skip.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    14133 2022-11-29 16:25:42.000000 fandango-15.6.7/tests/test_objects.py
```

### Comparing `fandango-15.6.4/AUTHORS` & `fandango-15.6.7/AUTHORS`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/LICENSE` & `fandango-15.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/PKG-INFO` & `fandango-15.6.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fandango
-Version: 15.6.4
+Version: 15.6.7
 Summary: Simplify the configuration of big Tango control systems
 Home-page: UNKNOWN
 Author: Sergi Rubio
 Author-email: srubio@cells.es
 License: UNKNOWN
 Description: Fandango is a Python module created to simplify the configuration of big control systems; implementing the behavior of Jive (configuration) and/or Astor (deployment) tools in methods that could be called from scripts using regexp and wildcards. Fandango provides functional methods, classes and utilities to develop high-level device servers and APIs for Tango control system.
 Platform: Linux,Windows XP/Vista/7/8
```

### Comparing `fandango-15.6.4/README.md` & `fandango-15.6.7/README.md`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/CHANGELOG` & `fandango-15.6.7/fandango/CHANGELOG`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/__init__.py` & `fandango-15.6.7/fandango/__init__.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/arrays.py` & `fandango-15.6.7/fandango/arrays.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/callbacks.py` & `fandango-15.6.7/fandango/callbacks.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/db.py` & `fandango-15.6.7/fandango/db.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/debug.py` & `fandango-15.6.7/fandango/debug.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/device/DDebug.py` & `fandango-15.6.7/fandango/device/DDebug.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/device/Dev4Tango.py` & `fandango-15.6.7/fandango/device/Dev4Tango.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/device/FolderDS.py` & `fandango-15.6.7/fandango/device/FolderDS.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/device/FolderGUI.py` & `fandango-15.6.7/fandango/device/FolderGUI.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/device/WorkerDS.py` & `fandango-15.6.7/fandango/device/WorkerDS.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/devslist.py` & `fandango-15.6.7/fandango/devslist.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/dicts.py` & `fandango-15.6.7/fandango/dicts.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/doc.py` & `fandango-15.6.7/fandango/doc.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/dynamic.py` & `fandango-15.6.7/fandango/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,30 @@
 from fandango.tango.dynattr import *
 import fandango.objects as objects
 from fandango.excepts import *
 from fandango.objects import self_locked, Cached
 from fandango.linos import listdir
 from fandango.dicts import SortedDict, CaselessDefaultDict, defaultdict, CaselessDict
 from fandango.log import Logger, shortstr
-from fandango.callbacks import EventSource, EventListener
 import fandango.functional as fun
-from fandango.functional import *
+from fandango.functional import (
+    clmatch,
+    clsearch,
+    clsub,
+    kmap,
+    lowstr,
+    isSequence,
+    isCallable,
+    isMapping,
+    isString,
+    list2lines,
+    time2str,
+    str2time,
+    notNone,
+)
 
 
 USE_STATIC_METHODS = False
 
 MEM_CHECK = str(os.environ.get("PYMEMCHECK")).lower() in ("yes", "true", "1")
 if MEM_CHECK and "HEAPY" not in locals():
     try:
@@ -142,15 +155,15 @@
     import gc
 
 # if 'LatestDeviceImpl' not in dir(PyTango): PyTango.LatestDeviceImpl = PyTango.Device_4Impl
 if "DeviceClass" not in dir(PyTango):
     PyTango.DeviceClass = PyTango.PyDeviceClass
 
 MAX_ARRAY_SIZE = 8192
-EVENT_TYPES = "(true|yes|push|forward|archive|[0-9]+)$"
+EVENT_TYPES = "(true|yes|push|archive|[0-9]+)$"
 
 
 class DynamicDSImpl(PyTango.LatestDeviceImpl,Logger):
 
     EXTENSIONS = dict(list(ft.EXTENSIONS.items()))
 
     def __init__(
@@ -296,15 +309,15 @@
             True,
             self.set_status(self.get_status() + status),
         ]
 
         # Advance methods for evaluating formulas
         self._locals["self"] = self
         self._locals["EVAL"] = lambda formula: self.evaluateFormula(formula)
-        self._locals["MATCH"] = lambda expr, cad: matchCl(expr, cad)
+        self._locals["MATCH"] = lambda expr, cad: fun.matchCl(expr, cad)
         self._locals["DELAY"] = lambda secs: fn.wait(secs)
         self._locals["FILE"] = lambda filename: DynamicDS.open_file(
             filename, device=self
         )  # This command will allow to setup attributes from config files
         self._locals["FORMULA"] = self.get_attr_formula
         self._locals["MODELS"] = self.get_attr_models
         self._locals["time2str"] = fn.time2str
@@ -396,15 +409,15 @@
             DynamicDSClass.device_property_list,
         ):
 
             for prop, value in list(d.items()):
                 if not hasattr(self, prop):
                     if "Array" in str(value[0]):
                         value = value[-1]
-                    elif value and isSequence(value[-1]):
+                    elif value and fun.isSequence(value[-1]):
                         value = value[-1][0]
                     else:
                         value = value and value[-1]
                     dct[prop] = value
 
                 self.debug("default %s: %s" % (prop, value))
         if update:
@@ -848,15 +861,15 @@
                 setattr(self, _is_allowed.__name__, _is_allowed)
 
                 max_size = (
                     hasattr(self, "DynamicSpectrumSize") and self.DynamicSpectrumSize
                 )
                 AttrType = (
                     PyTango.AttrWriteType.READ_WRITE
-                    if "WRITE" in re.split("[\[\(\]\)\ =,\+]", formula)
+                    if "WRITE" in fun.re.split("[\[\(\]\)\ =,\+]", formula)
                     else PyTango.AttrWriteType.READ
                 )
 
                 for typename, dyntype in list(DynamicDSTypes.items()):
 
                     if dyntype.match(formula):
 
@@ -1001,15 +1014,15 @@
                 if create and events:
                     # THIS IS CONFIGURING EVENTS TO BE "MANUAL",
                     # pushed=True, filtered=False (ignore Jive settings)
                     self.set_change_event(aname.lower(), True, False)
                     if "archive" in events:
                         self.set_archive_event(aname.lower(), True, False)
 
-                if isNumber(events) and aname not in new_polled_attrs:
+                if fun.isNumber(events) and aname not in new_polled_attrs:
                     new_polled_attrs[aname] = int(events)
 
             elif self.dyn_values[aname].keep:
                 self._locals[aname] = None
 
             ## END OF ATTR CONFIG LOOP
 
@@ -1066,15 +1079,15 @@
         ):
             # Both State and MemUsage shall be polled to have events!
             events = self.check_attribute_events(x)
             if events and x not in new_polled_attrs:
                 # To be added at next restart
                 self.warning("%s events will be polled (%s)" % (x, events))
                 new_polled_attrs[x] = (
-                    int(events) if isNumber(events) else self.DEFAULT_POLLING_PERIOD
+                    int(events) if fun.isNumber(events) else self.DEFAULT_POLLING_PERIOD
                 )
             if x != "state":
                 self.set_change_event(x, True, False)
                 if "archive" in events:
                     self.set_archive_event(x, True, False)
         try:
             self.check_polled_attributes(new_attr=new_polled_attrs)
@@ -1110,16 +1123,14 @@
         In the first two cases, the value specified applies to all attributes.
 
         In the last case, each config applies only to the specified attribute.
 
         Setting yes/true will enable only change events if configured from Jive.
 
         Setting archive will enable both change and archive events.
-        
-        Setting forward will enable subscription on XAttr and push
 
         Setting push will also enable the pushing from code.
         """
         self.UseEvents = list(filter(bool, (u.split("#")[0].strip().lower() 
             for u in self.UseEvents))
         )
         self.debug("check_attribute_events(%s,%s,%s)" % (aname, poll, self.UseEvents))
@@ -1205,17 +1216,17 @@
             elif new_quality is not None and q != new_quality:
                 self.info(
                     "In check_changed_event(%s,%s): %s != %s"
                     % (aname, shortstr(new_value), q, new_quality)
                 )
                 return True
 
-            elif isSequence(new_value) or isSequence(v):
+            elif fun.isSequence(new_value) or fun.isSequence(v):
                 # Event pushed ignoring cabs/crel config!
-                v, new_value = notNone(v, []), notNone(new_value, [])
+                v, new_value = fun.notNone(v, []), fun.notNone(new_value, [])
 
                 changed = len(v) != len(new_value) or any(
                     v != vv for v, vv in zip(v, new_value)
                 )
 
                 self.info(
                     "In check_changed_event(%s,%s != %s): changed = %s"
@@ -1243,15 +1254,15 @@
                     finally:
                         self.info(
                             "In check_changed_event(%s,%s != %s): changed=%s"
                             % (aname, shortstr(new_value), shortstr(v), changed)
                         )
                         return changed
 
-                if clsearch("(push|forward)", events):  # UseEvents = push #on any change
+                if clsearch("push", events):  # UseEvents = push #on any change
                     # cabs,crel = 1e-12,1e-12
                     if v != new_value:  # It should be only if UseEvents=push
                         self.info(
                             "In check_changed_event(%s,%s): changed=True,"
                             " push on any change" % (aname, shortstr(new_value))
                         )
                         return True
@@ -1309,16 +1320,16 @@
                 fs = (formula + "\n" + self.dyn_qualities.get(a, "")).lower()
 
                 # Get dependencies from existing attributes
                 for k, v in list(self.dyn_values.items()):
                     ks = k.lower().strip()
                     if a == ks:
                         continue
-                    if ks in re.split("[^'\"_0-9a-zA-Z]", fs):
-                        # searchCl("(^|[^'\"_0-9a-z])%s($|[^'\"_0-9a-z])"%k,formula):
+                    if ks in fun.re.split("[^'\"_0-9a-zA-Z]", fs):
+                        # fun.searchCl("(^|[^'\"_0-9a-z])%s($|[^'\"_0-9a-z])"%k,formula):
                         self.dyn_values[aname].dependencies.add(k)
                         # Dependencies are case sensitive
                         self.dyn_values[k].keep = True
 
                 if isMapping(self.CheckDependencies):
                     for k, v in list(self.CheckDependencies.items()):
                         if clmatch(k, aname) or clmatch(k, formula):
@@ -1486,15 +1497,15 @@
         # THIS CHANGE MUST BE TESTED AGAINST PYTANGO7!!!! For Scalar/Spectrum/Image R/W Attrs!!
         try:  # PyTango8
             data = attr.get_write_value()
         except:
             data = []
             attr.get_write_value(data)
 
-        if isSequence(data) and self.dyn_values[aname].type.dimx == 1:
+        if fun.isSequence(data) and self.dyn_values[aname].type.dimx == 1:
             data = data[0]
         elif self.dyn_values[aname].type.dimy != 1:
             x = attr.get_max_dim_x()
             data = [data[i : i + x] for i in range(len(data))[::x]]
 
         self.setAttr(aname, data)
         # self.dyn_values[aname].update(result,time.time(),PyTango.AttrQuality.ATTR_VALID)
@@ -1518,23 +1529,23 @@
             aname = self.get_attr_name(aname)
             self.info(
                 "push_dyn_attr(v,t,q,e,c,q=%s)"
                 % str((shortstr(value), date, quality, events, changed, queued))
             )
             queued = queued and self.MaxEventStream
 
-            if clmatch("state$", aname):
+            if fun.clmatch("state$", aname):
                 aname = "State"
                 events, changed = True, True
                 value = value if value is not None else self.get_state()
                 date, quality = time.time(), AttrQuality.ATTR_VALID
 
             t = self.dyn_values.get(aname, DynamicAttribute())
             value = notNone(value, t.value)
-            date = notNone(date, now())
+            date = notNone(date, fun.now())
             quality = notNone(quality, t.quality)
 
             if events is None:
                 # That call parses the contents of UseEvents property
                 events = self.check_attribute_events(aname)
             if changed is None:
                 changed = self.check_changed_event(
@@ -1564,15 +1575,15 @@
                     self._events_lock.release()
                 return "queued"
             else:
                 if aname.lower() in ("state", "status"):
                     self.push_change_event(aname)
                 else:
                     self.push_change_event(aname, value, date, quality)
-                if clsearch("archive", events):
+                if fun.clsearch("archive", events):
                     if aname.lower() in ("state", "status"):
                         self.push_archive_event(aname)
                     else:
                         self.push_archive_event(aname, value, date, quality)
 
                 return "pushed"
 
@@ -1632,15 +1643,15 @@
                 if (not WRITE and not push and not deps)
                 else None
             )
             if cache is not None:
                 self.debug(
                     "Returning cached (%s) value for %s: %s(%s)"
                     % (
-                        time2str(cache.time),
+                        fun.time2str(cache.time),
                         aname,
                         type(cache.value),
                         shortstr(cache.value),
                     )
                 )
                 return cache.value
 
@@ -1703,17 +1714,17 @@
             if not WRITE and formula in self.Lambdas:
                 ## LAMBDAS CAN BE USED ONLY ON READ_ONLY FORMULAS!
                 f = self.Lambdas[formula]
                 self.info(
                     "In evalAttr(forced_push=%s) ... using Lambdas[%s] = %s"
                     % (push, formula, f)
                 )
-                if isString(f):
+                if fun.isString(f):
                     f = self._locals.get(f, self.__getattr__(f, None))
-                result = f() if isCallable(f) else f
+                result = f() if fun.isCallable(f) else f
 
             else:
 
                 if WRITE:
                     self.debug(
                         "%s::evalAttr(WRITE): Attribute=%s; formula=%s; VALUE=%s"
                         % (self.get_name(), aname, formula, shortstr(VALUE))
@@ -1839,15 +1850,15 @@
             s = traceback.format_exc()
             self.error(s)
             if "not defined" in str(s):
                 print('locals: %s' % str(sorted(self._locals.keys())))
             raise e  # Exception(s)
 
         finally:
-            self._eval_times[aname] = now() - tstart
+            self._eval_times[aname] = fun.now() - tstart
             self._locals["ATTRIBUTE"] = ""
 
     def evalCommand(self, cmd, argin=None):
         """This method will execute a command declared using DynamicCommands property"""
         k = cmd if "/" in cmd else self.get_name() + "/" + cmd
         assert k in list(
             self.dyn_comms.keys()
@@ -1868,15 +1879,15 @@
             % (isinstance(formula, str) and formula or "code")
         )
         # MODIFIIED!! to use pure DynamicAttributes
         # Attr = lambda a: self.dyn_values[a].value
         if formula in self.Lambdas:
             self.info("DynamicDS.evalState: using Lambdas")
             f = self.Lambdas[formula]
-            return f() if isCallable(f) else f
+            return f() if fun.isCallable(f) else f
 
         t = time.time() - self.time0
         for k, v in list(self.dyn_values.items()):
             self._locals[k] = v  # .value #Updating Last Attribute Values
         __locals = {}  # __locals=locals().copy() #Low priority: local variables
         __locals.update(self._locals)  # Cached objects
         __locals.update(
@@ -2000,15 +2011,15 @@
         MaxEventStream must be configured
         """
         try:
             c = 0
             self._events_lock.acquire()
             while self._events_last:
                 self._events_last.pop(0)
-            t0 = now()
+            t0 = fun.now()
             if not self.MaxEventStream or not self.check_attribute_events("state"):
                 self.debug("Events not queued ...")
                 return 0
             self.debug("*" * 80)
             self.debug(
                 "In processEvents(%d/%d)"
                 % (self.MaxEventStream, self._events_queue.qsize())
@@ -2209,15 +2220,15 @@
                 value = self.getXAttr(aname, default, write, wvalue)
             elif al == "state":
                 value = self.get_state()
             elif al == "status":
                 value = self.get_status()
             elif al in list(map(lowstr, self.dyn_values.keys())):
                 value = self.evalAttr(
-                    aname, WRITE=write, VALUE=notNone(wvalue, default)
+                    aname, WRITE=write, VALUE=fun.notNone(wvalue, default)
                 )
             else:
                 # Getting an Static attribute that match:
                 method = getattr(
                     self, "read_%s" % aname, getattr(self, "read_%s" % al, None)
                 )
                 if method is not None:
@@ -2299,15 +2310,15 @@
             value = argin[1]
         aname = argin[0]
         is_write = self._locals.get("WRITE")
 
         self.debug("VAR(%s,%s,%s,%s & %s)" % (aname, value, default, WRITE, is_write))
 
         if WRITE and is_write:
-            value = notNone(self._locals.get("VALUE"), value)
+            value = fun.notNone(self._locals.get("VALUE"), value)
             self.debug("Writing %s into %s" % (value, aname))
 
         if value is not None:
             self.variables[aname] = value
 
         elif self.variables.get(aname) is None:
             self.variables[aname] = default
@@ -2394,26 +2405,22 @@
                     if listener: #Done here to catch first event
                         self._external_listeners[full_name].add(listener)
 
                     if full_name not in self._external_attributes:
                         self.debug("%s.getXAttr: creating %s proxy to %s"
                             % (listener,"PyTango",full_name,))
 
-                        cap = EventSource(
+                        cap = ft.CachedAttributeProxy(
                             full_name, keeptime=max((100, self.KeepTime))
                         )  # keeptime=self.KeepTime)
                         self._external_attributes[full_name] = cap
-                        evs = self.check_attribute_events(listener)
-                        if clsearch("forward", evs) and ft.check_attribute_events(full_name):
-                            evs = "change"
-                        else:
-                            evs = ""
-                        cap.addListener(self, use_events = evs,
-                            #use_polling = not evs and self.PollingPeriod,
-                            )
+                        cap.addListener(self, use_events = "change"
+                                if self.check_attribute_events(listener)
+                                and fn.tango.check_attribute_events(full_name)
+                                else "")
                         
                     else:
                         self.debug("%s.getXAttr: using %s proxy to %s"
                             % (listener,"PyTango",full_name,))
                     if write:
                         self.info("getXAttr(Write): %s(%s)" % (type(wvalue), wvalue))
                         self._external_attributes[full_name].write(wvalue)
@@ -2574,22 +2581,22 @@
                 self.error(msg)
                 # Exceptions are not re_thrown to allow other commands to be evaluated if this fails.
             finally:
                 if hasattr(self, "myClass") and self.myClass:
                     self.myClass.DynDev = self  # NOT REDUNDANT: If a call to another device in the same server occurs this pointer could have been modified.
             return result
         else:
-            if isString(cmd):
+            if fun.isString(cmd):
                 if "/" not in cmd:
                     device = self.get_name()
                 else:
                     device, cmd = cmd.rsplit("/", 1)
             else:
                 device = self.get_name()
-            if isString(feedback) and "/" not in feedback:
+            if fun.isString(feedback) and "/" not in feedback:
                 feedback = device + "/" + feedback
             return ft.TangoCommand(
                 command=cmd, device=device, feedback=feedback, timeout=10.0, wait=10.0
             ).execute(args, expected=expected)
 
     @staticmethod
     def open_file(filename, device=None):
@@ -2755,15 +2762,15 @@
 
     def Help(self, str_format="text"):
         """This command returns help for this device class and its parents"""
         return ft.get_device_help(self, str_format)
 
     def setPauseEvents(self, argin):
         ov = self._events_paused
-        self._events_paused = bool(clmatch("yes|true", argin))
+        self._events_paused = bool(fun.clmatch("yes|true", argin))
         if not self._events_paused and ov:
             for a, v in list(self.dyn_values.items()):
                 events = self.check_attribute_events(a)
                 self.push_dyn_attr(aname, events=events, changed=1, queued=1)
 
         return str(self.check_attribute_events("state"))
 
@@ -3128,15 +3135,14 @@
         ],
         "UseEvents": [
             PyTango.DevVarStringArray,
             "Value of this property will be yes/true,no/false or a list of "
             "attributes that will trigger push_event (if configured from jive). "
             "If UseEvents=always, it will be always pushed, "
             "if UseEvents=push, will always push on any change, ignoring config, "
-            "if UseEvents=forward, XAttr will subscribe and push incoming events, "
             "if UseEvents=True, then Tango DB config prevails, and is checked",
             ["false"],
         ],
         "MaxEventStream": [
             PyTango.DevLong,
             "Max number of events to be pushed by processEvents()",
             [0],
```

### Comparing `fandango-15.6.4/fandango/excepts.py` & `fandango-15.6.7/fandango/excepts.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/functional.py` & `fandango-15.6.7/fandango/functional.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/interface/CopyCatDS.py` & `fandango-15.6.7/fandango/interface/CopyCatDS.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/interface/inheritance.py` & `fandango-15.6.7/fandango/interface/inheritance.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/linos.py` & `fandango-15.6.7/fandango/linos.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/log.py` & `fandango-15.6.7/fandango/log.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/objects.py` & `fandango-15.6.7/fandango/objects.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/pipes.py` & `fandango-15.6.7/fandango/pipes.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/qt.py` & `fandango-15.6.7/fandango/qt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1402,21 +1402,21 @@
             call_back = self.getDragEventCallback()
             mimeData = call_back()
 
             if not isinstance(mimeData, Qt.QMimeData):
                 txt = str(mimeData)
                 mimeData = Qt.QMimeData()
                 if getattr(self, "Mimetype", None):
-                    mimeData.setData(self.Mimetype, txt)
+                    mimeData.setData(self.Mimetype, txt.encode())
                 mimeData.setText(txt)  # Order is not trivial, preferred must go first
 
             drag = Qt.QDrag(self)
             drag.setMimeData(mimeData)
             drag.setHotSpot(event.pos() - self.rect().topLeft())
-            dropAction = drag.start(Qt.Qt.CopyAction)
+            dropAction = drag.exec_(Qt.Qt.CopyAction)
             # tracer('Out of Draggable(%s).mouseMoveEvent'%self._qt_klass__)
 
         def setModel(self, model):
             self._model = model
 
         def getModel(self):
             return getattr(self, "_model", None)
```

### Comparing `fandango-15.6.4/fandango/scripts/CopyCatDS` & `fandango-15.6.7/fandango/scripts/CopyCatDS`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/DynamicDS` & `fandango-15.6.7/fandango/scripts/DynamicDS`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/FolderDS` & `fandango-15.6.7/fandango/scripts/FolderDS`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/WorkerDS` & `fandango-15.6.7/fandango/scripts/WorkerDS`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/csv2tango` & `fandango-15.6.7/fandango/scripts/csv2tango`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/fandango` & `fandango-15.6.7/fandango/scripts/fandango`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/my2to3.py` & `fandango-15.6.7/fandango/scripts/my2to3.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/sardanact` & `fandango-15.6.7/fandango/scripts/sardanact`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/servers_lite.py` & `fandango-15.6.7/fandango/scripts/servers_lite.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/setup.ds.py` & `fandango-15.6.7/fandango/scripts/setup.ds.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/tango2csv` & `fandango-15.6.7/fandango/scripts/tango2csv`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/tango2json` & `fandango-15.6.7/fandango/scripts/tango2json`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/tango_create_device.py` & `fandango-15.6.7/fandango/scripts/tango_create_device.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/tango_create_starter.py` & `fandango-15.6.7/fandango/scripts/tango_create_starter.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/tango_monitor` & `fandango-15.6.7/fandango/scripts/tango_monitor`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/tango_property` & `fandango-15.6.7/fandango/scripts/tango_property`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/scripts/tango_servers` & `fandango-15.6.7/fandango/scripts/tango_servers`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/servers.py` & `fandango-15.6.7/fandango/servers.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/tango/command.py` & `fandango-15.6.7/fandango/tango/command.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/tango/defaults.py` & `fandango-15.6.7/fandango/tango/defaults.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/tango/dynattr.py` & `fandango-15.6.7/fandango/tango/dynattr.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/tango/export.py` & `fandango-15.6.7/fandango/tango/export.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/tango/methods.py` & `fandango-15.6.7/fandango/tango/methods.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/tango/search.py` & `fandango-15.6.7/fandango/tango/search.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/tango/tangoeval.py` & `fandango-15.6.7/fandango/tango/tangoeval.py`

 * *Files 1% similar despite different names*

```diff
@@ -661,19 +661,21 @@
                 # Used from alarm messages
                 self.last[target] = self.previous[var_name]
             except Exception as e:
                 self.trace("eval(r=%s): Unable to obtain %s values" % (r, target))
                 self.last[target] = e
                 raise e
         self.trace("formula = %s" % (self.source))
-        self.trace(
-            "previous.items():\n"
-            + "\n".join(str((str(k), str(i))) for k, i in list(self.previous.items()))
-        )
-        self.result = eval(self.source, dict(self.previous), self._locals)
+        self.trace("previous.items():\n"
+            + "\n".join(str((str(k), str(i))) 
+            for k, i in list(self.previous.items())))
+            
+        lcs = dict(self.previous)
+        lcs.update(self._locals)
+        self.result = eval(self.source, lcs) #use globals to pass variables in py3
         self.trace("result = %s" % str(self.result))
         return self.result
 
     pass
 
 
 #######################################################################################
```

### Comparing `fandango-15.6.4/fandango/testing/check_callbacks.py` & `fandango-15.6.7/fandango/testing/check_callbacks.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/testing/check_fandango.py` & `fandango-15.6.7/fandango/testing/check_fandango.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/testing/checkmodule.py` & `fandango-15.6.7/fandango/testing/checkmodule.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/testing/gen_test_file.py` & `fandango-15.6.7/fandango/testing/gen_test_file.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/testing/simulation.py` & `fandango-15.6.7/fandango/testing/simulation.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/threads.py` & `fandango-15.6.7/fandango/threads.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango/web.py` & `fandango-15.6.7/fandango/web.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/fandango.egg-info/PKG-INFO` & `fandango-15.6.7/fandango.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fandango
-Version: 15.6.4
+Version: 15.6.7
 Summary: Simplify the configuration of big Tango control systems
 Home-page: UNKNOWN
 Author: Sergi Rubio
 Author-email: srubio@cells.es
 License: UNKNOWN
 Description: Fandango is a Python module created to simplify the configuration of big control systems; implementing the behavior of Jive (configuration) and/or Astor (deployment) tools in methods that could be called from scripts using regexp and wildcards. Fandango provides functional methods, classes and utilities to develop high-level device servers and APIs for Tango control system.
 Platform: Linux,Windows XP/Vista/7/8
```

### Comparing `fandango-15.6.4/fandango.egg-info/SOURCES.txt` & `fandango-15.6.7/fandango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/setup.py` & `fandango-15.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/tests/definitions.py` & `fandango-15.6.7/tests/definitions.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/tests/test_functional.py` & `fandango-15.6.7/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/tests/test_functional_auto_gen.py` & `fandango-15.6.7/tests/test_functional_auto_gen.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/tests/test_functional_skip.py` & `fandango-15.6.7/tests/test_functional_skip.py`

 * *Files identical despite different names*

### Comparing `fandango-15.6.4/tests/test_objects.py` & `fandango-15.6.7/tests/test_objects.py`

 * *Files identical despite different names*

