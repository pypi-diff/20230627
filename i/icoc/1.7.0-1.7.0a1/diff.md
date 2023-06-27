# Comparing `tmp/icoc-1.7.0.tar.gz` & `tmp/icoc-1.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icoc-1.7.0.tar", last modified: Tue Jun 27 11:46:59 2023, max compression
+gzip compressed data, was "icoc-1.7.0a1.tar", last modified: Tue Jun 20 10:06:16 2023, max compression
```

## Comparing `icoc-1.7.0.tar` & `icoc-1.7.0a1.tar`

### file list

```diff
@@ -1,107 +1,103 @@
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.887798 icoc-1.7.0/
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.874656 icoc-1.7.0/.github/
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.876672 icoc-1.7.0/.github/workflows/
--rw-r--r--   0 rene       (501) staff       (20)     1375 2023-06-26 13:34:38.000000 icoc-1.7.0/.github/workflows/documentation.yaml
--rw-r--r--   0 rene       (501) staff       (20)      854 2023-06-07 10:26:30.000000 icoc-1.7.0/.github/workflows/tests.yaml
--rw-r--r--   0 rene       (501) staff       (20)       68 2023-06-26 13:34:38.000000 icoc-1.7.0/MANIFEST.in
--rw-r--r--   0 rene       (501) staff       (20)     2864 2023-06-27 11:46:59.887673 icoc-1.7.0/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     1993 2023-06-26 13:34:38.000000 icoc-1.7.0/ReadMe.md
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.877641 icoc-1.7.0/icoc.egg-info/
--rw-r--r--   0 rene       (501) staff       (20)     2864 2023-06-27 11:46:59.000000 icoc-1.7.0/icoc.egg-info/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     2447 2023-06-27 11:46:59.000000 icoc-1.7.0/icoc.egg-info/SOURCES.txt
--rw-r--r--   0 rene       (501) staff       (20)        1 2023-06-27 11:46:59.000000 icoc-1.7.0/icoc.egg-info/dependency_links.txt
--rw-r--r--   0 rene       (501) staff       (20)      480 2023-06-27 11:46:59.000000 icoc-1.7.0/icoc.egg-info/entry_points.txt
--rw-r--r--   0 rene       (501) staff       (20)      368 2023-06-27 11:46:59.000000 icoc-1.7.0/icoc.egg-info/requires.txt
--rw-r--r--   0 rene       (501) staff       (20)        9 2023-06-27 11:46:59.000000 icoc-1.7.0/icoc.egg-info/top_level.txt
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.877802 icoc-1.7.0/mytoolit/
--rw-r--r--   0 rene       (501) staff       (20)       22 2023-06-27 10:45:51.000000 icoc-1.7.0/mytoolit/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.879364 icoc-1.7.0/mytoolit/can/
--rw-r--r--   0 rene       (501) staff       (20)      470 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/can/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    12214 2023-06-01 13:30:24.000000 icoc-1.7.0/mytoolit/can/adc.py
--rw-r--r--   0 rene       (501) staff       (20)     5692 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/can/calibration.py
--rw-r--r--   0 rene       (501) staff       (20)     9978 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/can/command.py
--rw-r--r--   0 rene       (501) staff       (20)      199 2023-01-17 15:27:35.000000 icoc-1.7.0/mytoolit/can/error.py
--rw-r--r--   0 rene       (501) staff       (20)    15799 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/can/identifier.py
--rw-r--r--   0 rene       (501) staff       (20)    21969 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/can/message.py
--rw-r--r--   0 rene       (501) staff       (20)   156735 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/can/network.py
--rw-r--r--   0 rene       (501) staff       (20)     4348 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/can/node.py
--rw-r--r--   0 rene       (501) staff       (20)     2909 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/can/sensor.py
--rw-r--r--   0 rene       (501) staff       (20)    14009 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/can/status.py
--rw-r--r--   0 rene       (501) staff       (20)    28506 2023-06-19 14:26:07.000000 icoc-1.7.0/mytoolit/can/streaming.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.880091 icoc-1.7.0/mytoolit/cmdline/
--rw-r--r--   0 rene       (501) staff       (20)      195 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/cmdline/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    10154 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/cmdline/commander.py
--rw-r--r--   0 rene       (501) staff       (20)     8872 2023-06-19 14:05:00.000000 icoc-1.7.0/mytoolit/cmdline/icon.py
--rw-r--r--   0 rene       (501) staff       (20)     8859 2023-06-13 11:42:48.000000 icoc-1.7.0/mytoolit/cmdline/parse.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.880562 icoc-1.7.0/mytoolit/config/
--rw-r--r--   0 rene       (501) staff       (20)      132 2023-06-19 12:39:06.000000 icoc-1.7.0/mytoolit/config/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    14090 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/config/config.py
--rwxr-xr-x   0 rene       (501) staff       (20)    13145 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/config/config.yaml
--rw-r--r--   0 rene       (501) staff       (20)     1897 2023-06-27 09:44:17.000000 icoc-1.7.0/mytoolit/config/user.yaml
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.880787 icoc-1.7.0/mytoolit/eeprom/
--rw-r--r--   0 rene       (501) staff       (20)      121 2021-03-31 08:39:06.000000 icoc-1.7.0/mytoolit/eeprom/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3405 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/eeprom/eeprom_status.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.881125 icoc-1.7.0/mytoolit/experiments/
--rw-r--r--   0 rene       (501) staff       (20)     2513 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/experiments/RF_tests.py
--rw-r--r--   0 rene       (501) staff       (20)     2465 2023-05-15 09:35:35.000000 icoc-1.7.0/mytoolit/experiments/new.py
--rw-r--r--   0 rene       (501) staff       (20)     1570 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/experiments/old.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.881924 icoc-1.7.0/mytoolit/measurement/
--rw-r--r--   0 rene       (501) staff       (20)      295 2023-03-02 11:57:58.000000 icoc-1.7.0/mytoolit/measurement/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     2149 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/measurement/acceleration.py
--rw-r--r--   0 rene       (501) staff       (20)      104 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/measurement/constants.py
--rw-r--r--   0 rene       (501) staff       (20)     2663 2023-03-06 15:54:45.000000 icoc-1.7.0/mytoolit/measurement/sensor.py
--rw-r--r--   0 rene       (501) staff       (20)    10915 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/measurement/storage.py
--rw-r--r--   0 rene       (501) staff       (20)     1638 2023-06-19 14:26:07.000000 icoc-1.7.0/mytoolit/measurement/units.py
--rw-r--r--   0 rene       (501) staff       (20)     1654 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/measurement/voltage.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.883749 icoc-1.7.0/mytoolit/old/
--rw-r--r--   0 rene       (501) staff       (20)    19142 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/old/MyToolItCommands.py
--rw-r--r--   0 rene       (501) staff       (20)     2065 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/old/MyToolItNetworkNumbers.py
--rw-r--r--   0 rene       (501) staff       (20)     1985 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/old/MyToolItSth.py
--rw-r--r--   0 rene       (501) staff       (20)      224 2021-05-12 07:38:00.000000 icoc-1.7.0/mytoolit/old/MyToolItStu.py
--rw-r--r--   0 rene       (501) staff       (20)     9404 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/old/Plotter.py
--rw-r--r--   0 rene       (501) staff       (20)     8642 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/old/SthLimits.py
--rw-r--r--   0 rene       (501) staff       (20)      151 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/old/StuLimits.py
--rw-r--r--   0 rene       (501) staff       (20)        0 2021-03-31 08:39:06.000000 icoc-1.7.0/mytoolit/old/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    40867 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/old/cli.py
--rw-r--r--   0 rene       (501) staff       (20)   102855 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/old/network.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.884808 icoc-1.7.0/mytoolit/old/test/
--rw-r--r--   0 rene       (501) staff       (20)    35677 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/old/test/HardwareSth.py
--rw-r--r--   0 rene       (501) staff       (20)   371486 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/old/test/MyToolItTestSth.py
--rw-r--r--   0 rene       (501) staff       (20)    16040 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/old/test/MyToolItTestSthManually.py
--rw-r--r--   0 rene       (501) staff       (20)    76128 2023-06-19 14:26:07.000000 icoc-1.7.0/mytoolit/old/test/MyToolItTestStu.py
--rw-r--r--   0 rene       (501) staff       (20)     6176 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/old/test/MyToolItTestStuManually.py
--rw-r--r--   0 rene       (501) staff       (20)        0 2021-07-12 14:02:41.000000 icoc-1.7.0/mytoolit/old/test/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      389 2021-09-29 13:59:48.000000 icoc-1.7.0/mytoolit/old/test/testSignal.py
--rw-r--r--   0 rene       (501) staff       (20)    25157 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/old/ui.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.885487 icoc-1.7.0/mytoolit/report/
--rw-r--r--   0 rene       (501) staff       (20)     7454 2021-03-31 08:39:06.000000 icoc-1.7.0/mytoolit/report/MyTooliT.pdf
--rw-r--r--   0 rene       (501) staff       (20)      108 2021-03-31 08:39:06.000000 icoc-1.7.0/mytoolit/report/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     6538 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/report/forms.py
--rw-r--r--   0 rene       (501) staff       (20)     2278 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/report/pdf.py
--rw-r--r--   0 rene       (501) staff       (20)     7991 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/report/report.py
--rw-r--r--   0 rene       (501) staff       (20)     5230 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/report/style.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.885843 icoc-1.7.0/mytoolit/scripts/
--rw-r--r--   0 rene       (501) staff       (20)     4965 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/scripts/eeprom.py
--rw-r--r--   0 rene       (501) staff       (20)      667 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/scripts/mac.py
--rw-r--r--   0 rene       (501) staff       (20)      650 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/scripts/name.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.885951 icoc-1.7.0/mytoolit/test/
--rw-r--r--   0 rene       (501) staff       (20)       13 2021-03-31 08:39:06.000000 icoc-1.7.0/mytoolit/test/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.886638 icoc-1.7.0/mytoolit/test/production/
--rw-r--r--   0 rene       (501) staff       (20)      148 2022-01-27 22:57:57.000000 icoc-1.7.0/mytoolit/test/production/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    21279 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/test/production/node.py
--rw-r--r--   0 rene       (501) staff       (20)     4831 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/test/production/sensor_node.py
--rw-r--r--   0 rene       (501) staff       (20)     6525 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/test/production/smh.py
--rw-r--r--   0 rene       (501) staff       (20)    18722 2023-06-19 14:26:07.000000 icoc-1.7.0/mytoolit/test/production/sth.py
--rw-r--r--   0 rene       (501) staff       (20)     3591 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/test/production/stu.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.886970 icoc-1.7.0/mytoolit/test/unit/
--rw-r--r--   0 rene       (501) staff       (20)      187 2021-03-31 08:39:06.000000 icoc-1.7.0/mytoolit/test/unit/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3860 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/test/unit/extended_test_result.py
--rw-r--r--   0 rene       (501) staff       (20)      576 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/test/unit/extended_test_runner.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-27 11:46:59.887508 icoc-1.7.0/mytoolit/utility/
--rw-r--r--   0 rene       (501) staff       (20)      208 2023-06-19 14:26:07.000000 icoc-1.7.0/mytoolit/utility/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1455 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/utility/data.py
--rw-r--r--   0 rene       (501) staff       (20)     1067 2023-06-26 13:34:38.000000 icoc-1.7.0/mytoolit/utility/environment.py
--rw-r--r--   0 rene       (501) staff       (20)     1268 2023-01-17 10:19:15.000000 icoc-1.7.0/mytoolit/utility/naming.py
--rw-r--r--   0 rene       (501) staff       (20)     3360 2023-06-13 11:42:48.000000 icoc-1.7.0/mytoolit/utility/open.py
--rw-r--r--   0 rene       (501) staff       (20)     2543 2023-06-26 13:34:38.000000 icoc-1.7.0/pyproject.toml
--rw-r--r--   0 rene       (501) staff       (20)       38 2023-06-27 11:46:59.887834 icoc-1.7.0/setup.cfg
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.660578 icoc-1.7.0a1/
+-rw-r--r--   0 rene       (501) staff       (20)       73 2022-12-15 11:26:52.000000 icoc-1.7.0a1/MANIFEST.in
+-rw-r--r--   0 rene       (501) staff       (20)     2862 2023-06-20 10:06:16.651791 icoc-1.7.0a1/PKG-INFO
+-rw-r--r--   0 rene       (501) staff       (20)     1989 2022-12-21 12:29:41.000000 icoc-1.7.0a1/ReadMe.md
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.634987 icoc-1.7.0a1/icoc.egg-info/
+-rw-r--r--   0 rene       (501) staff       (20)     2862 2023-06-20 10:06:16.000000 icoc-1.7.0a1/icoc.egg-info/PKG-INFO
+-rw-r--r--   0 rene       (501) staff       (20)     2381 2023-06-20 10:06:16.000000 icoc-1.7.0a1/icoc.egg-info/SOURCES.txt
+-rw-r--r--   0 rene       (501) staff       (20)        1 2023-06-20 10:06:16.000000 icoc-1.7.0a1/icoc.egg-info/dependency_links.txt
+-rw-r--r--   0 rene       (501) staff       (20)      521 2023-06-20 10:06:16.000000 icoc-1.7.0a1/icoc.egg-info/entry_points.txt
+-rw-r--r--   0 rene       (501) staff       (20)      279 2023-06-20 10:06:16.000000 icoc-1.7.0a1/icoc.egg-info/requires.txt
+-rw-r--r--   0 rene       (501) staff       (20)        9 2023-06-20 10:06:16.000000 icoc-1.7.0a1/icoc.egg-info/top_level.txt
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.635121 icoc-1.7.0a1/mytoolit/
+-rw-r--r--   0 rene       (501) staff       (20)       30 2023-06-20 09:59:26.000000 icoc-1.7.0a1/mytoolit/__init__.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.638472 icoc-1.7.0a1/mytoolit/can/
+-rw-r--r--   0 rene       (501) staff       (20)      470 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/can/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    12214 2023-06-01 13:30:24.000000 icoc-1.7.0a1/mytoolit/can/adc.py
+-rw-r--r--   0 rene       (501) staff       (20)     5692 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/can/calibration.py
+-rw-r--r--   0 rene       (501) staff       (20)     9978 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/can/command.py
+-rw-r--r--   0 rene       (501) staff       (20)      199 2023-01-17 15:27:35.000000 icoc-1.7.0a1/mytoolit/can/error.py
+-rw-r--r--   0 rene       (501) staff       (20)    15799 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/can/identifier.py
+-rw-r--r--   0 rene       (501) staff       (20)    21929 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/can/message.py
+-rw-r--r--   0 rene       (501) staff       (20)   155346 2023-06-13 15:04:43.000000 icoc-1.7.0a1/mytoolit/can/network.py
+-rw-r--r--   0 rene       (501) staff       (20)     4348 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/can/node.py
+-rw-r--r--   0 rene       (501) staff       (20)     2909 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/can/sensor.py
+-rw-r--r--   0 rene       (501) staff       (20)    14009 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/can/status.py
+-rw-r--r--   0 rene       (501) staff       (20)    28506 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/can/streaming.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.639269 icoc-1.7.0a1/mytoolit/cmdline/
+-rw-r--r--   0 rene       (501) staff       (20)      195 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/cmdline/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    10178 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/cmdline/commander.py
+-rw-r--r--   0 rene       (501) staff       (20)     8872 2023-06-19 14:05:00.000000 icoc-1.7.0a1/mytoolit/cmdline/icon.py
+-rw-r--r--   0 rene       (501) staff       (20)     8859 2023-06-13 11:42:48.000000 icoc-1.7.0a1/mytoolit/cmdline/parse.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.639731 icoc-1.7.0a1/mytoolit/config/
+-rw-r--r--   0 rene       (501) staff       (20)      132 2023-06-19 12:39:06.000000 icoc-1.7.0a1/mytoolit/config/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    14893 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/config/config.py
+-rwxr-xr-x   0 rene       (501) staff       (20)    13767 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/config/config.yaml
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.640133 icoc-1.7.0a1/mytoolit/eeprom/
+-rw-r--r--   0 rene       (501) staff       (20)      121 2021-03-31 08:39:06.000000 icoc-1.7.0a1/mytoolit/eeprom/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     3405 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/eeprom/eeprom_status.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.640716 icoc-1.7.0a1/mytoolit/experiments/
+-rw-r--r--   0 rene       (501) staff       (20)     2513 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/experiments/RF_tests.py
+-rw-r--r--   0 rene       (501) staff       (20)     2465 2023-05-15 09:35:35.000000 icoc-1.7.0a1/mytoolit/experiments/new.py
+-rw-r--r--   0 rene       (501) staff       (20)     1570 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/experiments/old.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.642154 icoc-1.7.0a1/mytoolit/measurement/
+-rw-r--r--   0 rene       (501) staff       (20)      295 2023-03-02 11:57:58.000000 icoc-1.7.0a1/mytoolit/measurement/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     2149 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/measurement/acceleration.py
+-rw-r--r--   0 rene       (501) staff       (20)      104 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/measurement/constants.py
+-rw-r--r--   0 rene       (501) staff       (20)     2663 2023-03-06 15:54:45.000000 icoc-1.7.0a1/mytoolit/measurement/sensor.py
+-rw-r--r--   0 rene       (501) staff       (20)    11109 2023-06-05 09:30:04.000000 icoc-1.7.0a1/mytoolit/measurement/storage.py
+-rw-r--r--   0 rene       (501) staff       (20)     1638 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/measurement/units.py
+-rw-r--r--   0 rene       (501) staff       (20)     1654 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/measurement/voltage.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.644806 icoc-1.7.0a1/mytoolit/old/
+-rw-r--r--   0 rene       (501) staff       (20)    19144 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/MyToolItCommands.py
+-rw-r--r--   0 rene       (501) staff       (20)     2065 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/MyToolItNetworkNumbers.py
+-rw-r--r--   0 rene       (501) staff       (20)     1985 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/MyToolItSth.py
+-rw-r--r--   0 rene       (501) staff       (20)      224 2021-05-12 07:38:00.000000 icoc-1.7.0a1/mytoolit/old/MyToolItStu.py
+-rw-r--r--   0 rene       (501) staff       (20)     9120 2023-05-24 13:55:10.000000 icoc-1.7.0a1/mytoolit/old/Plotter.py
+-rw-r--r--   0 rene       (501) staff       (20)     8642 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/SthLimits.py
+-rw-r--r--   0 rene       (501) staff       (20)      151 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/StuLimits.py
+-rw-r--r--   0 rene       (501) staff       (20)        0 2021-03-31 08:39:06.000000 icoc-1.7.0a1/mytoolit/old/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    40927 2023-04-18 11:42:04.000000 icoc-1.7.0a1/mytoolit/old/cli.py
+-rw-r--r--   0 rene       (501) staff       (20)   102819 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/network.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.647237 icoc-1.7.0a1/mytoolit/old/test/
+-rw-r--r--   0 rene       (501) staff       (20)    35677 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/test/HardwareSth.py
+-rw-r--r--   0 rene       (501) staff       (20)   370829 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/old/test/MyToolItTestSth.py
+-rw-r--r--   0 rene       (501) staff       (20)    16040 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/test/MyToolItTestSthManually.py
+-rw-r--r--   0 rene       (501) staff       (20)    76128 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/old/test/MyToolItTestStu.py
+-rw-r--r--   0 rene       (501) staff       (20)     6176 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/test/MyToolItTestStuManually.py
+-rw-r--r--   0 rene       (501) staff       (20)        0 2021-07-12 14:02:41.000000 icoc-1.7.0a1/mytoolit/old/test/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      389 2021-09-29 13:59:48.000000 icoc-1.7.0a1/mytoolit/old/test/testSignal.py
+-rw-r--r--   0 rene       (501) staff       (20)    25157 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/old/ui.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.648356 icoc-1.7.0a1/mytoolit/report/
+-rw-r--r--   0 rene       (501) staff       (20)     7454 2021-03-31 08:39:06.000000 icoc-1.7.0a1/mytoolit/report/MyTooliT.pdf
+-rw-r--r--   0 rene       (501) staff       (20)      108 2021-03-31 08:39:06.000000 icoc-1.7.0a1/mytoolit/report/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     6538 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/report/forms.py
+-rw-r--r--   0 rene       (501) staff       (20)     2278 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/report/pdf.py
+-rw-r--r--   0 rene       (501) staff       (20)     7974 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/report/report.py
+-rw-r--r--   0 rene       (501) staff       (20)     5230 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/report/style.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.648886 icoc-1.7.0a1/mytoolit/scripts/
+-rw-r--r--   0 rene       (501) staff       (20)     1107 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/scripts/clean.py
+-rw-r--r--   0 rene       (501) staff       (20)     4965 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/scripts/eeprom.py
+-rw-r--r--   0 rene       (501) staff       (20)      667 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/scripts/mac.py
+-rw-r--r--   0 rene       (501) staff       (20)      650 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/scripts/name.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.649023 icoc-1.7.0a1/mytoolit/test/
+-rw-r--r--   0 rene       (501) staff       (20)       13 2021-03-31 08:39:06.000000 icoc-1.7.0a1/mytoolit/test/__init__.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.650412 icoc-1.7.0a1/mytoolit/test/production/
+-rw-r--r--   0 rene       (501) staff       (20)      148 2022-01-27 22:57:57.000000 icoc-1.7.0a1/mytoolit/test/production/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    21337 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/test/production/node.py
+-rw-r--r--   0 rene       (501) staff       (20)     4831 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/test/production/sensor_node.py
+-rw-r--r--   0 rene       (501) staff       (20)     6525 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/test/production/smh.py
+-rw-r--r--   0 rene       (501) staff       (20)    18722 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/test/production/sth.py
+-rw-r--r--   0 rene       (501) staff       (20)     3591 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/test/production/stu.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.650882 icoc-1.7.0a1/mytoolit/test/unit/
+-rw-r--r--   0 rene       (501) staff       (20)      187 2021-03-31 08:39:06.000000 icoc-1.7.0a1/mytoolit/test/unit/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     3860 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/test/unit/extended_test_result.py
+-rw-r--r--   0 rene       (501) staff       (20)      576 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/test/unit/extended_test_runner.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-06-20 10:06:16.651582 icoc-1.7.0a1/mytoolit/utility/
+-rw-r--r--   0 rene       (501) staff       (20)      208 2023-06-19 14:26:07.000000 icoc-1.7.0a1/mytoolit/utility/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     1455 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/utility/data.py
+-rw-r--r--   0 rene       (501) staff       (20)     1083 2023-06-19 12:54:40.000000 icoc-1.7.0a1/mytoolit/utility/environment.py
+-rw-r--r--   0 rene       (501) staff       (20)     1268 2023-01-17 10:19:15.000000 icoc-1.7.0a1/mytoolit/utility/naming.py
+-rw-r--r--   0 rene       (501) staff       (20)     3360 2023-06-13 11:42:48.000000 icoc-1.7.0a1/mytoolit/utility/open.py
+-rw-r--r--   0 rene       (501) staff       (20)     2497 2023-06-19 14:26:07.000000 icoc-1.7.0a1/pyproject.toml
+-rw-r--r--   0 rene       (501) staff       (20)       38 2023-06-20 10:06:16.660638 icoc-1.7.0a1/setup.cfg
```

### Comparing `icoc-1.7.0/PKG-INFO` & `icoc-1.7.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icoc
-Version: 1.7.0
+Version: 1.7.0a1
 Summary: Control and test software for sensory tool holders (STH), sensor milling heads (SMH) and stationary transceiver units (STU)
 Author-email: Clemens Burgstaller <burgstaller@ift.at>, René Schwaiger <rene.schwaiger@ift.at>
 Project-URL: Documentation, https://mytoolit.github.io/ICOc/
 Project-URL: Source, https://github.com/mytoolit/ICOc/
 Keywords: smart-tool,smh,stu,sth,tool-holder
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Other/Proprietary License
@@ -44,11 +44,11 @@
 - HTML (`make html`),
 - EPUB (`make epub`), and
 - PDF (`make pdf`)
 
 version of the documentation. The output will be stored in the folder `Bookdown` in the root of the repository. If you want to build all versions of the documentation, just use the command
 
 ```
-make doc
+make
 ```
 
 in the repo root.
```

### Comparing `icoc-1.7.0/ReadMe.md` & `icoc-1.7.0a1/ReadMe.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 - HTML (`make html`),
 - EPUB (`make epub`), and
 - PDF (`make pdf`)
 
 version of the documentation. The output will be stored in the folder `Bookdown` in the root of the repository. If you want to build all versions of the documentation, just use the command
 
 ```
-make doc
+make
 ```
 
 in the repo root.
```

### Comparing `icoc-1.7.0/icoc.egg-info/PKG-INFO` & `icoc-1.7.0a1/icoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icoc
-Version: 1.7.0
+Version: 1.7.0a1
 Summary: Control and test software for sensory tool holders (STH), sensor milling heads (SMH) and stationary transceiver units (STU)
 Author-email: Clemens Burgstaller <burgstaller@ift.at>, René Schwaiger <rene.schwaiger@ift.at>
 Project-URL: Documentation, https://mytoolit.github.io/ICOc/
 Project-URL: Source, https://github.com/mytoolit/ICOc/
 Keywords: smart-tool,smh,stu,sth,tool-holder
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Other/Proprietary License
@@ -44,11 +44,11 @@
 - HTML (`make html`),
 - EPUB (`make epub`), and
 - PDF (`make pdf`)
 
 version of the documentation. The output will be stored in the folder `Bookdown` in the root of the repository. If you want to build all versions of the documentation, just use the command
 
 ```
-make doc
+make
 ```
 
 in the repo root.
```

### Comparing `icoc-1.7.0/icoc.egg-info/SOURCES.txt` & `icoc-1.7.0a1/icoc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 MANIFEST.in
 ReadMe.md
 pyproject.toml
-.github/workflows/documentation.yaml
-.github/workflows/tests.yaml
 icoc.egg-info/PKG-INFO
 icoc.egg-info/SOURCES.txt
 icoc.egg-info/dependency_links.txt
 icoc.egg-info/entry_points.txt
 icoc.egg-info/requires.txt
 icoc.egg-info/top_level.txt
 mytoolit/__init__.py
@@ -25,15 +23,14 @@
 mytoolit/cmdline/__init__.py
 mytoolit/cmdline/commander.py
 mytoolit/cmdline/icon.py
 mytoolit/cmdline/parse.py
 mytoolit/config/__init__.py
 mytoolit/config/config.py
 mytoolit/config/config.yaml
-mytoolit/config/user.yaml
 mytoolit/eeprom/__init__.py
 mytoolit/eeprom/eeprom_status.py
 mytoolit/experiments/RF_tests.py
 mytoolit/experiments/new.py
 mytoolit/experiments/old.py
 mytoolit/measurement/__init__.py
 mytoolit/measurement/acceleration.py
@@ -62,14 +59,15 @@
 mytoolit/old/test/testSignal.py
 mytoolit/report/MyTooliT.pdf
 mytoolit/report/__init__.py
 mytoolit/report/forms.py
 mytoolit/report/pdf.py
 mytoolit/report/report.py
 mytoolit/report/style.py
+mytoolit/scripts/clean.py
 mytoolit/scripts/eeprom.py
 mytoolit/scripts/mac.py
 mytoolit/scripts/name.py
 mytoolit/test/__init__.py
 mytoolit/test/production/__init__.py
 mytoolit/test/production/node.py
 mytoolit/test/production/sensor_node.py
```

### Comparing `icoc-1.7.0/mytoolit/can/adc.py` & `icoc-1.7.0a1/mytoolit/can/adc.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/can/calibration.py` & `icoc-1.7.0a1/mytoolit/can/calibration.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/can/command.py` & `icoc-1.7.0a1/mytoolit/can/command.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/can/identifier.py` & `icoc-1.7.0a1/mytoolit/can/identifier.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/can/message.py` & `icoc-1.7.0a1/mytoolit/can/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,19 +335,17 @@
         data_explanation = ""
 
         block_command = identifier.block_command_name()
 
         StreamingFormatClass = (
             StreamingFormat
             if block_command == "Data"
-            else (
-                StreamingFormatVoltage
-                if block_command == "Voltage"
-                else StreamingFormat
-            )
+            else StreamingFormatVoltage
+            if block_command == "Voltage"
+            else StreamingFormat
         )
         streaming_format: StreamingFormat = StreamingFormatClass(self.data[0])
         data_explanation += repr(streaming_format)
 
         if identifier.is_acknowledgment() and len(self.data) >= 2:
             sequence_counter = self.data[1]
             explanations = [f"Sequence Counter: {sequence_counter}"]
```

### Comparing `icoc-1.7.0/mytoolit/can/network.py` & `icoc-1.7.0a1/mytoolit/can/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -- Imports ------------------------------------------------------------------
 
 from __future__ import annotations
 
 from asyncio import get_running_loop, Queue, sleep, TimeoutError, wait_for
 from datetime import date
 from logging import getLogger, FileHandler, Formatter
+from pathlib import Path
 from struct import pack, unpack
 from sys import platform
 from time import time
 from types import TracebackType
 from typing import List, NamedTuple, Optional, Sequence, Type, Union
 
 from can import Bus, Listener, Message as CANMessage, Notifier
@@ -113,15 +114,16 @@
     def __init__(self):
         """Initialize the logger"""
 
         logger = getLogger("network.can")
         # We use `Logger` in the code below, since the `.logger` attribute
         # stores internal DynaConf data
         logger.setLevel(settings.Logger.can.level)
-        handler = FileHandler("can.log", "w", "utf-8", delay=True)
+        repo_root = Path(__file__).parent.parent.parent
+        handler = FileHandler(repo_root / "can.log", "w", "utf-8", delay=True)
         handler.setFormatter(Formatter("{asctime} {message}", style="{"))
         logger.addHandler(handler)
 
     def on_message_received(self, message: CANMessage) -> None:
         """React to a received message on the bus
 
         Parameters
@@ -921,23 +923,17 @@
 
         The (Bluetooth broadcast) name of the device
 
         Example
         -------
 
         >>> from asyncio import run, sleep
-        >>> from platform import system
 
         Get Bluetooth advertisement name of device “0” from STU 1
 
-        >>> if system() == 'Linux':
-        ...    async def reset():
-        ...        async with Network() as network:
-        ...            await network.reset_node('STU 1')
-        ...    run(reset())
         >>> async def get_bluetooth_device_name():
         ...     async with Network() as network:
         ...         await network.activate_bluetooth('STU 1')
         ...         # Wait for device scan in node STU 1 to take place
         ...         await sleep(2)
         ...         # We assume that at least one STH is available
         ...         return await network.get_name('STU 1', device_number=0)
@@ -2559,23 +2555,17 @@
 
         The voltage of the acceleration sensor in Volt
 
         Example
         -------
 
         >>> from asyncio import run
-        >>> from platform import system
 
         Read the acceleration voltage of STH 1
 
-        >>> if system() == 'Linux':
-        ...    async def reset():
-        ...        async with Network() as network:
-        ...            await network.reset_node('STU 1')
-        ...    run(reset())
         >>> async def read_acceleration_voltage():
         ...     async with Network() as network:
         ...         await network.connect_sensor_device(0)
         ...
         ...         before = await network.read_acceleration_voltage()
         ...         await network.activate_acceleration_self_test()
         ...         between = await network.read_acceleration_voltage()
@@ -3311,23 +3301,17 @@
 
         The current value of advertisement time 1 in milliseconds
 
         Example
         -------
 
         >>> from asyncio import run
-        >>> from platform import system
 
         Read advertisement time 1 of STH 1
 
-        >>> if system() == 'Linux':
-        ...    async def reset():
-        ...        async with Network() as network:
-        ...            await network.reset_node('STU 1')
-        ...    run(reset())
         >>> async def read_advertisement_time_1():
         ...     async with Network() as network:
         ...         await network.connect_sensor_device(0)
         ...         return await network.read_eeprom_advertisement_time_1()
         >>> advertisement_time = run(read_advertisement_time_1())
         >>> isinstance(advertisement_time, float)
         True
@@ -3353,23 +3337,17 @@
         milliseconds:
             The value for advertisement time 1 in milliseconds
 
         Example
         -------
 
         >>> from asyncio import run
-        >>> from platform import system
 
         Write and read advertisement time 1 of STH 1
 
-        >>> if system() == 'Linux':
-        ...    async def reset():
-        ...        async with Network() as network:
-        ...            await network.reset_node('STU 1')
-        ...    run(reset())
         >>> async def write_read_advertisement_time_1(milliseconds):
         ...     async with Network() as network:
         ...         await network.connect_sensor_device(0)
         ...         await network.write_eeprom_advertisement_time_1(
         ...                 milliseconds)
         ...         return await network.read_eeprom_advertisement_time_1()
         >>> run(write_read_advertisement_time_1(1250))
@@ -3456,23 +3434,17 @@
 
         The current value of advertisement time 2 in milliseconds
 
         Example
         -------
 
         >>> from asyncio import run
-        >>> from platform import system
 
         Read advertisement time 2 of STH 1
 
-        >>> if system() == 'Linux':
-        ...    async def reset():
-        ...        async with Network() as network:
-        ...            await network.reset_node('STU 1')
-        ...    run(reset())
         >>> async def read_advertisement_time_2():
         ...     async with Network() as network:
         ...         await network.connect_sensor_device(0)
         ...         return await network.read_eeprom_advertisement_time_2()
         >>> advertisement_time = run(read_advertisement_time_2())
         >>> isinstance(advertisement_time, float)
         True
@@ -4851,23 +4823,17 @@
             The (negative) offset of the acceleration value in multiples of g₀
 
         Example
         -------
 
         >>> from asyncio import run
         >>> from math import isclose
-        >>> from platform import system
 
         Write and read the acceleration offset of STH 1
 
-        >>> if system() == 'Linux':
-        ...    async def reset():
-        ...        async with Network() as network:
-        ...            await network.reset_node('STU 1')
-        ...    run(reset())
         >>> async def write_read_y_axis_acceleration_offset(offset):
         ...     async with Network() as network:
         ...         await network.connect_sensor_device(0)
         ...         await network.write_eeprom_y_axis_acceleration_offset(
         ...                 offset)
         ...         return (await
         ...                 network.read_eeprom_y_axis_acceleration_offset())
```

### Comparing `icoc-1.7.0/mytoolit/can/node.py` & `icoc-1.7.0a1/mytoolit/can/node.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/can/sensor.py` & `icoc-1.7.0a1/mytoolit/can/sensor.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/can/status.py` & `icoc-1.7.0a1/mytoolit/can/status.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/can/streaming.py` & `icoc-1.7.0a1/mytoolit/can/streaming.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/cmdline/commander.py` & `icoc-1.7.0a1/mytoolit/cmdline/commander.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,17 @@
         """
 
         path = settings.commands.path
         operating_system = system()
         paths = (
             path.linux
             if operating_system == "Linux"
-            else path.mac if operating_system == "Darwin" else path.windows
+            else path.mac
+            if operating_system == "Darwin"
+            else path.windows
         )
 
         environ["PATH"] += pathsep + pathsep.join(paths)
 
     def _run_command(
         self,
         command: List[str],
```

### Comparing `icoc-1.7.0/mytoolit/cmdline/icon.py` & `icoc-1.7.0a1/mytoolit/cmdline/icon.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/cmdline/parse.py` & `icoc-1.7.0a1/mytoolit/cmdline/parse.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/config/config.py` & `icoc-1.7.0a1/mytoolit/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from platform import system
 from sys import stderr
 from typing import List, Optional
 
 from dynaconf import Dynaconf, ValidationError, Validator
 from platformdirs import site_config_dir, user_config_dir
 
-from mytoolit.utility.open import open_file, UnableToOpenError
+from mytoolit.utility.open import open_file
 
 # -- Classes ------------------------------------------------------------------
 
 
 class ConfigurationUtility:
     """Access configuration data"""
 
@@ -45,40 +45,48 @@
 
         # Create file, if it does not exist already
         if not filepath.exists():
             filepath.parent.mkdir(
                 exist_ok=True,
                 parents=True,
             )
-
-            default_user_config = (
-                files("mytoolit.config").joinpath("user.yaml").read_text()
-            )
-
             with filepath.open("w", encoding="utf8") as config_file:
-                config_file.write(default_user_config)
+                config_file.write("""\
+# This file contains configuration values for the ICOc package.
+# For a list of available settings you can change, please
+# take a look at the default configuration. The latest version
+# of the default configuration is available here:
+#
+# https://github.com/MyTooliT/ICOc/blob/master/mytoolit/config/config.yaml
+#
+# Settings in this file will overwrite values from the default configuration.
+# In the case of maps and lists this might not be what you want. To change
+# this behavior you can set `dynaconf_merge` to true, either globally or for
+# specific maps or lists. For more information, please take a look at the
+# Dynaconf documentation about this topic: https://www.dynaconf.com/merging
+
+# Enable merging (of maps and lists) globally
+dynaconf_merge: true
+
+# —— <Example> ————————————————————————————————————————————————————————————————
+# Change the (test) operator name to “User Config”
+# If you do not want to change the operator name,
+# please delete the two lines below.
+operator:
+  name: User Config
+# —— </Example> ———————————————————————————————————————————————————————————————
+""")
 
         open_file(filepath)
 
     @classmethod
     def open_user_config(cls):
         """Open the current users configuration file"""
 
-        try:
-            cls.open_config_file(cls.user_config_filepath)
-        except UnableToOpenError as error:
-            print(
-                (
-                    f"Unable to open user configuration: {error}"
-                    "\nTo work around this problem please open "
-                    f"“{cls.user_config_filepath}” in your favorite text "
-                    "editor"
-                ),
-                file=stderr,
-            )
+        cls.open_config_file(cls.user_config_filepath)
 
 
 class SettingsIncorrectError(Exception):
     """Raised when the configuration is incorrect"""
 
 
 class Settings(Dynaconf):
@@ -420,15 +428,15 @@
         """
 
         directory = self.output_directory()
 
         if directory.exists() and not directory.is_dir():
             raise NotADirectoryError(
                 f"The output directory “{directory}” points to an "
-                "existing file not a directory"
+                "existing file not an directory"
             )
 
         if not directory.is_dir():
             try:
                 makedirs(str(directory))
             except OSError as error:
                 raise OSError(
```

### Comparing `icoc-1.7.0/mytoolit/eeprom/eeprom_status.py` & `icoc-1.7.0a1/mytoolit/eeprom/eeprom_status.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/experiments/RF_tests.py` & `icoc-1.7.0a1/mytoolit/experiments/RF_tests.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/experiments/new.py` & `icoc-1.7.0a1/mytoolit/experiments/new.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/experiments/old.py` & `icoc-1.7.0a1/mytoolit/experiments/old.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/measurement/acceleration.py` & `icoc-1.7.0a1/mytoolit/measurement/acceleration.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/measurement/sensor.py` & `icoc-1.7.0a1/mytoolit/measurement/sensor.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/measurement/storage.py` & `icoc-1.7.0a1/mytoolit/measurement/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,21 @@
         >>> filepath = Path("test.hdf5")
         >>> with Storage(filepath) as storage:
         ...     pass
         >>> filepath.unlink()
 
         """
 
-        self.filepath = Path(filepath).expanduser().resolve()
+        repository = Path(__file__).parent.parent.parent
+        filepath = Path(filepath).expanduser()
+        self.filepath = (
+            filepath
+            if filepath.is_absolute()
+            else repository.joinpath(filepath)
+        ).resolve()
 
         self.hdf: Optional[File] = None
         self.acceleration: Optional[Node] = None
         self.start_time: Optional[float] = None
 
     def __enter__(self) -> Storage:
         """Open the HDF file for writing"""
```

### Comparing `icoc-1.7.0/mytoolit/measurement/units.py` & `icoc-1.7.0a1/mytoolit/measurement/units.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/measurement/voltage.py` & `icoc-1.7.0a1/mytoolit/measurement/voltage.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/old/MyToolItCommands.py` & `icoc-1.7.0a1/mytoolit/old/MyToolItCommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     "MacAddress": 17,
     "DeviceConnectMacAddr": 18,
     "SelfAddressing": 255,
 }
 
 BluetoothTime = {
     "Connect": 20,
-    "Out": 4 * 5,
+    "Out": (4 * 5),
     "Disconnect": 2,
     "GetDeviceNumber": 2,
     "DeviceConnect": 6,
     "TestConnect": 4,
 }
 
 SystemCommandRouting = {
```

### Comparing `icoc-1.7.0/mytoolit/old/MyToolItNetworkNumbers.py` & `icoc-1.7.0a1/mytoolit/old/MyToolItNetworkNumbers.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/old/MyToolItSth.py` & `icoc-1.7.0a1/mytoolit/old/MyToolItSth.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     "AdcConfigAllPrescalerMax": 4,
     "ConTimeNormalMaxMs": 5000,
     "ConTimeSleep1MaxMs": 6000,
     "ConTimeSleep2MaxMs": 7000,
     "ConTimeMaximumMs": 15000,
     "DisconnectedCurrentMax": 0.8,  # in mA
     "EnergyMode1CurrentMax": 0.5,  # in mA
-    "EnergyMode2CurrentMax": 0.48,  # in mA
-    "EnergyModeMaxCurrentMax": 0.48,  # in mA
+    "EnergyMode2CurrentMax": 0.47,  # in mA
+    "EnergyModeMaxCurrentMax": 0.47,  # in mA
     "EnergyConnectedCurrentMax": 10,  # in mA
     "EnergyMeasuringCurrentMax": 17,  # in mA
     "EnergyMeasuringLedOffCurrentMax": 17,  # in mA
 }
 
 SleepTime = {
     "Min": 10000,
```

### Comparing `icoc-1.7.0/mytoolit/old/Plotter.py` & `icoc-1.7.0a1/mytoolit/old/Plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,17 @@
 
 
 def vPlotter(iSocketPort, log_level):
     global cDict
 
     logger = getLogger(__name__)
     logger.setLevel(log_level)
-    handler = FileHandler("plotter.log", delay=True)
+    handler = FileHandler(
+        Path(__file__).parent.parent.parent / "plotter.log", delay=True
+    )
     handler.setFormatter(
         Formatter("{asctime} {levelname} {name} {message}", style="{")
     )
     logger.addHandler(handler)
 
     logger.info("Application started")
     sPloterSocketInit(iSocketPort)
@@ -255,52 +257,40 @@
 
     # Adjust limits if new data goes beyond bounds
     if update_bounds:
         min_bound = min(
             [
                 value
                 for value in (
-                    (
-                        np.min(yX_data) - np.std(yX_data)
-                        if yX_data is not None
-                        else None
-                    ),
-                    (
-                        np.min(yY_data) - np.std(yY_data)
-                        if yY_data is not None
-                        else None
-                    ),
-                    (
-                        np.min(yZ_data) - np.std(yZ_data)
-                        if yZ_data is not None
-                        else None
-                    ),
+                    np.min(yX_data) - np.std(yX_data)
+                    if yX_data is not None
+                    else None,
+                    np.min(yY_data) - np.std(yY_data)
+                    if yY_data is not None
+                    else None,
+                    np.min(yZ_data) - np.std(yZ_data)
+                    if yZ_data is not None
+                    else None,
                 )
                 if value is not None
             ]
         )
         max_bound = max(
             [
                 value
                 for value in (
-                    (
-                        np.max(yX_data) + np.std(yX_data)
-                        if yX_data is not None
-                        else None
-                    ),
-                    (
-                        np.max(yY_data) + np.std(yY_data)
-                        if yY_data is not None
-                        else None
-                    ),
-                    (
-                        np.max(yZ_data) + np.std(yZ_data)
-                        if yZ_data is not None
-                        else None
-                    ),
+                    np.max(yX_data) + np.std(yX_data)
+                    if yX_data is not None
+                    else None,
+                    np.max(yY_data) + np.std(yY_data)
+                    if yY_data is not None
+                    else None,
+                    np.max(yZ_data) + np.std(yZ_data)
+                    if yZ_data is not None
+                    else None,
                 )
                 if value is not None
             ]
         )
         plt.ylim(min_bound, max_bound)
 
     # this pauses the data so the figure/axis can catch up - the amount of
```

### Comparing `icoc-1.7.0/mytoolit/old/SthLimits.py` & `icoc-1.7.0a1/mytoolit/old/SthLimits.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/old/cli.py` & `icoc-1.7.0a1/mytoolit/old/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,17 @@
         except (NotADirectoryError, OSError) as error:
             raise error
 
         self.parse_arguments()
 
         self.logger = getLogger(__name__)
         self.logger.setLevel(self.args.log.upper())
-        handler = FileHandler("cli.log", delay=True)
+        handler = FileHandler(
+            Path(__file__).parent.parent.parent / "cli.log", delay=True
+        )
         handler.setFormatter(
             Formatter("{asctime} {levelname} {name} {message}", style="{")
         )
         self.logger.addHandler(handler)
         self.logger.info("Initialized logger")
 
         self.KeyBoardInterrupt = False
```

### Comparing `icoc-1.7.0/mytoolit/old/network.py` & `icoc-1.7.0a1/mytoolit/old/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,27 +127,29 @@
         # General purpose logger
         self.logger = getLogger(__name__)
         self.logger.setLevel(log_level)
         repo_root = Path(__file__).parent.parent.parent
         handler: Union[FileHandler, StreamHandler] = (
             StreamHandler()
             if log_destination is None
-            else FileHandler(log_destination, "w", "utf-8", delay=True)
+            else FileHandler(
+                repo_root / log_destination, "w", "utf-8", delay=True
+            )
         )
         handler.setFormatter(
             Formatter("{asctime} {levelname} {name} {message}", style="{")
         )
         self.logger.addHandler(handler)
 
         # Logger for CAN messages
         logger = getLogger("can")
         # We use `Logger` in the code below, since the `.logger` attribute
         # stores internal DynaConf data
-        logger.setLevel(settings.Logger.can.level.upper())
-        handler = FileHandler("can.log", "w", "utf-8", delay=True)
+        logger.setLevel(settings.Logger.can.level)
+        handler = FileHandler(repo_root / "can.log", "w", "utf-8", delay=True)
         handler.setFormatter(Formatter("{asctime} {message}", style="{"))
         logger.addHandler(handler)
 
         self.logger.info(datetime.now().isoformat())
         self.start_time = int(round(time() * 1000))
         self.pcan = PCANBasic()
         self.m_PcanHandle = PCAN_USBBUS1
@@ -1230,17 +1232,17 @@
         statistics["Quantil95"] = self.streamingValueStatisticsQuantile(
             sortArray, 0.95
         )
         statistics["Quantil99"] = self.streamingValueStatisticsQuantile(
             sortArray, 0.99
         )
         statistics["Maximum"] = sortArray[-1]
-        statistics["ArithmeticAverage"] = (
-            self.streamingValueStatisticsArithmeticAverage(sortArray)
-        )
+        statistics[
+            "ArithmeticAverage"
+        ] = self.streamingValueStatisticsArithmeticAverage(sortArray)
         statistics["StandardDeviation"] = (
             self.streamingValueStatisticsVariance(sortArray) ** 0.5
         )
         statistics["Variance"] = self.streamingValueStatisticsVariance(
             sortArray
         )
         statistics["Skewness"] = self.streamingValueStatisticsMomentOrder(
@@ -1379,26 +1381,22 @@
         )
         dataSetsVoltage = self.data_sets(
             self.VoltageConfig.b.bNumber1,
             self.VoltageConfig.b.bNumber2,
             self.VoltageConfig.b.bNumber3,
         )
         dataPointsAcc = sum(
-            (
-                self.AccConfig.b.bNumber1,
-                self.AccConfig.b.bNumber2,
-                self.AccConfig.b.bNumber3,
-            )
+            self.AccConfig.b.bNumber1,
+            self.AccConfig.b.bNumber2,
+            self.AccConfig.b.bNumber3,
         )
         dataPointsVoltage = sum(
-            (
-                self.VoltageConfig.b.bNumber1,
-                self.VoltageConfig.b.bNumber2,
-                self.VoltageConfig.b.bNumber3,
-            )
+            self.VoltageConfig.b.bNumber1,
+            self.VoltageConfig.b.bNumber2,
+            self.VoltageConfig.b.bNumber3,
         )
         totalDataPoints = dataPointsAcc + dataPointsVoltage
         msgAcc = samplingRate / totalDataPoints
         if 0 < dataSetsAcc:
             msgAcc /= dataSetsAcc
         else:
             msgAcc = 0
```

### Comparing `icoc-1.7.0/mytoolit/old/test/HardwareSth.py` & `icoc-1.7.0a1/mytoolit/old/test/HardwareSth.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/old/test/MyToolItTestSth.py` & `icoc-1.7.0a1/mytoolit/old/test/MyToolItTestSth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1969,18 +1969,16 @@
         )
         self.assertLessEqual(
             float(sCurrentAverage), TestConfig["EnergyMeasuringCurrentMax"]
         )
         self.assertEqual(sCurrentUnit, "mA")
 
     def test0019PowerConsumptionMeasuringLedOff(self):
-        # fmt: off
         """Power Consumption - Reset conditions, LED turned off (⏱ 85 seconds)
         """
-        # fmt: on
         try:
             os.remove("Aem6.txt")
         except:
             pass
         self.TurnOffLed()
         self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
@@ -2282,18 +2280,16 @@
                 self.assertEqual(readD[3], 0)
                 self.assertEqual(readD[4], 0)
                 self.assertEqual(readD[5], 0)
                 self.assertEqual(readD[6], 0)
                 self.assertEqual(readD[7], 0)
 
     def test0032CalibrationFactorsKDWriteThenRead(self):
-        # fmt: off
         """Write all calibration factors and read them afterwards (⏱ 15 seconds)
         """
-        # fmt: on
         b0 = 2 - 1
         b1 = 8 - 1
         b2 = 32 - 1
         b3 = 128 - 1
         for _keyKD, valueKD in CalibrationFactor.items():
             for i in range(1, 4):
                 b0 += 1
@@ -4989,18 +4985,16 @@
             self.tSthLimits.iAdcAccYTolerance,
             self.tSthLimits.iAdcAccZMiddle,
             self.tSthLimits.iAdcAccZTolerance,
             self.tSthLimits.fAcceleration,
         )
 
     def test0346MixedStreamingAccXYZVoltBat(self):
-        # fmt: off
         """Mixed Streaming - AccX + AccY + AccZ + VoltageBattery (⏱ 25 seconds)
         """
-        # fmt: on
         self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Voltage"],
             DataSets[3],
             1,
             0,
             0,
@@ -5096,18 +5090,16 @@
             self.tSthLimits.iAdcAccYTolerance,
             self.tSthLimits.iAdcAccZMiddle,
             self.tSthLimits.iAdcAccZTolerance,
             self.tSthLimits.fAcceleration,
         )
 
     def test0347StreamingAccXSingleBattery(self):
-        # fmt: off
         """Stream x-acceleration & read sampling point for battery (⏱ 20 seconds)
         """
-        # fmt: on
         indexStart = self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Data"],
             DataSets[3],
             1,
             0,
             0,
@@ -5182,18 +5174,16 @@
         )
         self.assertGreater(
             calcRate * self.tSthLimits.uSamplingToleranceHigh,
             samplingPointsAccX,
         )
 
     def test0348StreamingAccYSingleBattery(self):
-        # fmt: off
         """Stream y-acceleration & read sampling point for battery (⏱ 20 seconds)
         """
-        # fmt: on
         indexStart = self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Data"],
             DataSets[3],
             0,
             1,
             0,
@@ -5268,18 +5258,16 @@
         )
         self.assertGreater(
             calcRate * self.tSthLimits.uSamplingToleranceHigh,
             samplingPointsAccY,
         )
 
     def test0349StreamingAccZSingleBattery(self):
-        # fmt: off
         """Stream z-acceleration & read sampling point for battery (⏱ 20 seconds)
         """
-        # fmt: on
         indexStart = self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Data"],
             DataSets[3],
             0,
             0,
             1,
@@ -5354,18 +5342,16 @@
         )
         self.assertGreater(
             calcRate * self.tSthLimits.uSamplingToleranceHigh,
             samplingPointsAccZ,
         )
 
     def test0350StreamingBatterySingleAccX(self):
-        # fmt: off
         """Stream Battery & receive single sampling point for AccX (⏱ 20 seconds)
         """
-        # fmt: on
         for _i in range(0, 1):
             indexStart = self.Can.streamingStart(
                 MyToolItNetworkNr["STH1"],
                 MyToolItStreaming["Voltage"],
                 DataSets[3],
                 1,
                 0,
@@ -5441,18 +5427,16 @@
             )
             self.assertGreater(
                 calcRate * self.tSthLimits.uSamplingToleranceHigh,
                 samplingPointsBattery,
             )
 
     def test0351StreamingBatterySingleAccY(self):
-        # fmt: off
         """Stream Battery & receive single sampling point for AccY (⏱ 20 seconds)
         """
-        # fmt: on
 
         indexStart = self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Voltage"],
             DataSets[3],
             1,
             0,
@@ -5528,18 +5512,16 @@
         )
         self.assertGreater(
             calcRate * self.tSthLimits.uSamplingToleranceHigh,
             samplingPointsBattery,
         )
 
     def test0352StreamingBatterySingleAccZ(self):
-        # fmt: off
         """Stream Battery & receive single sampling point for AccZ (⏱ 20 seconds)
         """
-        # fmt: on
         indexStart = self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Voltage"],
             DataSets[3],
             1,
             0,
             0,
@@ -5614,18 +5596,16 @@
         )
         self.assertGreater(
             calcRate * self.tSthLimits.uSamplingToleranceHigh,
             samplingPointsBattery,
         )
 
     def test0353StreamingBatterySingleAccYZ(self):
-        # fmt: off
         """Stream Battery & receive single sampling point for AccYZ (⏱ 20 seconds)
         """
-        # fmt: on
         indexStart = self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Voltage"],
             DataSets[3],
             1,
             0,
             0,
@@ -5701,18 +5681,16 @@
         )
         self.assertGreater(
             calcRate * self.tSthLimits.uSamplingToleranceHigh,
             samplingPointsBattery,
         )
 
     def test0354StreamingBatterySingleAccXZ(self):
-        # fmt: off
         """Stream Battery & receive single sampling point for AccXZ (⏱ 20 seconds)
         """
-        # fmt: on
         indexStart = self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Voltage"],
             DataSets[3],
             1,
             0,
             0,
@@ -5788,18 +5766,16 @@
         )
         self.assertGreater(
             calcRate * self.tSthLimits.uSamplingToleranceHigh,
             samplingPointsBattery,
         )
 
     def test0355StreamingBatterySingleAccXY(self):
-        # fmt: off
         """Stream Battery & receive single sampling point for AccXY (⏱ 20 seconds)
         """
-        # fmt: on
 
         indexStart = self.Can.streamingStart(
             MyToolItNetworkNr["STH1"],
             MyToolItStreaming["Voltage"],
             DataSets[3],
             1,
             0,
@@ -6325,15 +6301,16 @@
             calcRate * self.tSthLimits.uSamplingToleranceHigh,
             samplingPointsAccY,
         )
         self.assertEqual(samplingPointsAccY, samplingPointsAccZ)
         self.assertEqual(samplingPointsAccX, samplingPointsAccZ)
 
     def test0370StreamingOnfOff(self):
-        """Stream Start and Stop -> Test communication protocol (⏱ 3 minutes)"""
+        """Stream Start and Stop -> Test communication protocol (⏱ 3 minutes)
+        """
         _runs = 100
         # single stream, data set 3
         for _i in range(0, _runs):
             self.Can.streamingStart(
                 MyToolItNetworkNr["STH1"],
                 MyToolItStreaming["Data"],
                 DataSets[3],
@@ -9634,18 +9611,16 @@
             self.assertEqual(stateStartVoltage[i], ErrorPayloadAssumed[i])
             self.assertEqual(stateStartVss[i], ErrorPayloadAssumed[i])
             self.assertEqual(stateStartAvdd[i], ErrorPayloadAssumed[i])
             self.assertEqual(stateStartOpa1[i], ErrorPayloadAssumed[i])
             self.assertEqual(stateStartOpa2[i], ErrorPayloadAssumed[i])
 
     def test0605StateCalibrationMeasurementReset(self):
-        # fmt: off
         """Check Reset Subcommand of Calibration Measurement Command (⏱ 6 seconds)
         """
-        # fmt: on
         ackInjectX = self.Can.calibMeasurement(
             MyToolItNetworkNr["STH1"],
             CalibMeassurementActionNr["Activate"],
             CalibMeassurementTypeNr["Acc"],
             1,
             AdcReference["VDD"],
         )
@@ -9908,18 +9883,16 @@
         self.Can.logger.info(
             "Watchdog Counter after second reset: " + str(WDogCounter3)
         )
         self.assertEqual(WDogCounter1, WDogCounter2)
         self.assertEqual(WDogCounter1, WDogCounter3)
 
     def test0703ProductionDate(self):
-        # fmt: off
         """Write actual production date and Check ProductionDate (⏱ 7 seconds)
         """
-        # fmt: on
         sDate = date.today()
         sDate = str(sDate).replace("-", "")
         au8ProductionDate = []
         for element in sDate:
             au8ProductionDate.append(ord(element))
         au8Payload = [5, 20, 4, 0]
         au8Payload.extend(au8ProductionDate[:4])
@@ -10143,18 +10116,16 @@
         )
         self.assertEqual(
             u32EepromWriteRequestCounterTestStart + 2,
             u32EepromWriteRequestCounterTestEnd,
         )
 
     def test0753EepromWriteRequestCounterPageSwitches(self):
-        # fmt: off
         """Check that page switched do not yield to Writing EEPROM (⏱ 30 seconds)
         """
-        # fmt: on
         time.sleep(1)
         uLoopRuns = 5
         u32EepromWriteRequestCounterTestStart = (
             self.Can.u32EepromWriteRequestCounter(MyToolItNetworkNr["STH1"])
         )
         for _i in range(0, uLoopRuns):
             for sPage in EepromPage:
@@ -10188,18 +10159,16 @@
         )
         self.assertEqual(
             u32EepromWriteRequestCounterTestStart,
             u32EepromWriteRequestCounterTestEnd,
         )  # +1 due to incrementing at first write
 
     def test0754EepromWriteRequestCounterPageWriteSwitches(self):
-        # fmt: off
         """Check that page switched with previews writes yield into to Writing EEPROM with the correct number of writes (⏱ 15 seconds)
         """
-        # fmt: on
         time.sleep(2)
         uLoopRuns = 5
         uPageStart = 10
         uPageRuns = 6
         u32EepromWriteRequestCounterTestStart = (
             self.Can.u32EepromWriteRequestCounter(MyToolItNetworkNr["STH1"])
         )
@@ -10516,18 +10485,16 @@
         self.Can.CanTimeStampStart(self._resetStu()["CanTime"])
         self.Can.logger.info("Connect to STH")
         self.Can.bBlueToothConnectPollingName(
             MyToolItNetworkNr["STU1"], settings.sth.name
         )
 
     def test0900ErrorCmdVerbotenSth1(self):
-        # fmt: off
         """Test that nothing happens when sending Command 0x0000 to STH1 (⏱ 22 seconds)
         """
-        # fmt: on
         cmd = self.Can.CanCmd(0, 0, 1, 0)
         message = self.Can.CanMessage20(
             cmd, MyToolItNetworkNr["SPU1"], MyToolItNetworkNr["STH1"], []
         )
         msgAck = self.Can.tWriteFrameWaitAckRetries(
             message, waitMs=1000, retries=3, bErrorExit=False
         )
@@ -10554,18 +10521,16 @@
         )
         msgAck = self.Can.tWriteFrameWaitAckRetries(
             message, waitMs=1000, retries=3, bErrorExit=False
         )
         self.assertEqual("Error", msgAck)
 
     def test0901ErrorRequestErrorSth1(self):
-        # fmt: off
         """Test that nothing happens when sending Request(1) and bError(1) to STH1 (⏱ 15 seconds)
         """
-        # fmt: on
         cmd = self.Can.CanCmd(
             MyToolItBlock["System"], MyToolItSystem["Reset"], 1, 1
         )
         message = self.Can.CanMessage20(
             cmd, MyToolItNetworkNr["SPU1"], MyToolItNetworkNr["STH1"], []
         )
         msgAck = self.Can.tWriteFrameWaitAckRetries(
```

### Comparing `icoc-1.7.0/mytoolit/old/test/MyToolItTestSthManually.py` & `icoc-1.7.0a1/mytoolit/old/test/MyToolItTestSthManually.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/old/test/MyToolItTestStu.py` & `icoc-1.7.0a1/mytoolit/old/test/MyToolItTestStu.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/old/test/MyToolItTestStuManually.py` & `icoc-1.7.0a1/mytoolit/old/test/MyToolItTestStuManually.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/old/ui.py` & `icoc-1.7.0a1/mytoolit/old/ui.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/report/MyTooliT.pdf` & `icoc-1.7.0a1/mytoolit/report/MyTooliT.pdf`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/report/forms.py` & `icoc-1.7.0a1/mytoolit/report/forms.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/report/pdf.py` & `icoc-1.7.0a1/mytoolit/report/pdf.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/report/report.py` & `icoc-1.7.0a1/mytoolit/report/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -- Imports ------------------------------------------------------------------
 
 from functools import partial
-from importlib.resources import as_file, files
+from pathlib import Path
 from typing import List
 
 from reportlab.lib.units import cm
 from reportlab.platypus import (
     Flowable,
     ListFlowable,
     Paragraph,
@@ -31,20 +31,20 @@
     page_width = defaultPageSize[0]
     page_height = defaultPageSize[1]
     logo_width = 370
     logo_height = 75
     logo_offset = 50
     title_offset = logo_offset + logo_height + 20
 
-    with as_file(files("mytoolit.report") / "MyTooliT.pdf") as logo_filepath:
-        PDFImage(logo_filepath, logo_width, logo_height).drawOn(
-            canvas,
-            (page_width - logo_width) / 2,
-            page_height - logo_offset - logo_height,
-        )
+    logo_filepath = Path("mytoolit") / "report" / "MyTooliT.pdf"
+    PDFImage(logo_filepath, logo_width, logo_height).drawOn(
+        canvas,
+        (page_width - logo_width) / 2,
+        page_height - logo_offset - logo_height,
+    )
 
     style = get_style_sheet()
 
     center_width = page_width / 2
 
     heading1 = style["Heading1"]
     canvas.setFont(heading1.fontName, heading1.fontSize)
@@ -73,25 +73,23 @@
             A text that specifies the node (e.g. STH) for which a report
             should be generated
 
         """
 
         self.node = node
         self.document = SimpleDocTemplate(
-            f"{node} Test.pdf",
+            str(Path(__file__).parent.parent.parent / f"{node} Test.pdf"),
             author="MyTooliT",
             title="Test Report",
             subject="{} Test".format(
                 "Sensory Tool Holder"
                 if node == "STH"
-                else (
-                    "Sensory Milling Head"
-                    if node == "SMH"
-                    else "Stationary Transceiver Unit"
-                )
+                else "Sensory Milling Head"
+                if node == "SMH"
+                else "Stationary Transceiver Unit"
             ),
         )
         self.story = [Spacer(1, 3 * cm)]
         self.styles = get_style_sheet()
 
         self.general = []
         self.attributes = []
@@ -256,15 +254,15 @@
 
 if __name__ == "__main__":
     from platform import system
     from subprocess import run
 
     # Create a example test report
     node = "STH"
-    pdf_path = f"{node} Test.pdf"
+    pdf_path = str(Path(__file__).parent.parent.parent / f"{node} Test.pdf")
     report = Report(node)
 
     report.add_checkbox_list(
         title="Checkbox Title", boxes=["First box", "Second box"]
     )
 
     report.build()
```

### Comparing `icoc-1.7.0/mytoolit/report/style.py` & `icoc-1.7.0a1/mytoolit/report/style.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/scripts/eeprom.py` & `icoc-1.7.0a1/mytoolit/scripts/eeprom.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/scripts/mac.py` & `icoc-1.7.0a1/mytoolit/scripts/mac.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/scripts/name.py` & `icoc-1.7.0a1/mytoolit/scripts/name.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/test/production/node.py` & `icoc-1.7.0a1/mytoolit/test/production/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,16 @@
             The serial number of the programming board
 
         chip:
             The name of the chip that should be flashed
 
         """
 
-        image_filepath = Path(flash_location).expanduser().resolve()
+        repository_root = Path(__file__).parent.parent.parent.parent
+        image_filepath = repository_root / flash_location
         self.assertTrue(
             image_filepath.is_file(),
             f"Firmware file {image_filepath} does not exist",
         )
 
         commander = Commander(
             serial_number=programmmer_serial_number, chip=chip
```

### Comparing `icoc-1.7.0/mytoolit/test/production/sensor_node.py` & `icoc-1.7.0a1/mytoolit/test/production/sensor_node.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/test/production/smh.py` & `icoc-1.7.0a1/mytoolit/test/production/smh.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/test/production/sth.py` & `icoc-1.7.0a1/mytoolit/test/production/sth.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/test/production/stu.py` & `icoc-1.7.0a1/mytoolit/test/production/stu.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/test/unit/extended_test_result.py` & `icoc-1.7.0a1/mytoolit/test/unit/extended_test_result.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/test/unit/extended_test_runner.py` & `icoc-1.7.0a1/mytoolit/test/unit/extended_test_runner.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/utility/data.py` & `icoc-1.7.0a1/mytoolit/utility/data.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/utility/environment.py` & `icoc-1.7.0a1/mytoolit/utility/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     """
 
     path = settings.commands.path
     operating_system = system()
     paths = (
         path.linux
         if operating_system == "Linux"
-        else path.mac if operating_system == "Darwin" else path.windows
+        else path.mac
+        if operating_system == "Darwin"
+        else path.windows
     )
     environ["PATH"] += pathsep + pathsep.join(paths)
 
 
 # -- Main ---------------------------------------------------------------------
 
 if __name__ == "__main__":
```

### Comparing `icoc-1.7.0/mytoolit/utility/naming.py` & `icoc-1.7.0a1/mytoolit/utility/naming.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/mytoolit/utility/open.py` & `icoc-1.7.0a1/mytoolit/utility/open.py`

 * *Files identical despite different names*

### Comparing `icoc-1.7.0/pyproject.toml` & `icoc-1.7.0a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Programming Language :: Python",
 ]
 
 dependencies = [
-  "bidict>=0.22.1,<2",
-  "dynaconf>=3.1.12,<4",
-  "matplotlib>=3.7.1,<4",
-  "netaddr>=0.8.0,<2",
-  "pdfrw>=0.4,<2",
-  "pint>=0.22,<2",
-  "platformdirs>=3.5.0,<4",
-  "python-can[pcan]>=4,<5",
-  "pywin32>=306; os_name == 'nt'",
-  "reportlab>=4.0.4,<5",
-  "tables>=3.6,<4",
-  "tqdm>=4.65,<5",
-  "semantic_version>=2.10,<3",
-  "windows-curses>=2.3.1,<3; os_name == 'nt'",
+  "bidict",
+  "dynaconf>=3.1.12",
+  "matplotlib",
+  "netaddr",
+  "pdfrw",
+  "pint>=0.22",
+  "platformdirs>=3.5.0",
+  "python-can[pcan]>=4.0",
+  "pywin32; os_name == 'nt'",
+  "reportlab",
+  "tables>=3.6",
+  "tqdm>=4.65",
+  "semantic_version",
+  "windows-curses; os_name == 'nt'",
 ]
 description = """Control and test software for sensory tool holders (STH), \
                  sensor milling heads (SMH) and stationary transceiver units \
                  (STU)"""
 dynamic = ["version"]
 keywords = [
     "smart-tool",
@@ -60,14 +60,15 @@
     "pytest",
 ]
 
 [project.scripts]
 icoc = "mytoolit.old.ui:main"
 icon = "mytoolit.cmdline.icon:main"
 check-eeprom = "mytoolit.scripts.eeprom:main"
+clean-repo = "mytoolit.scripts.clean:main"
 test-smh = "mytoolit.test.production.smh:main"
 test-sth = "mytoolit.test.production.sth:main"
 test-sth-verification = "mytoolit.old.test.MyToolItTestSth:main"
 test-stu-verification = "mytoolit.old.test.MyToolItTestStu:main"
 test-stu = "mytoolit.test.production.stu:main"
 convert-base64-mac = "mytoolit.scripts.name:main"
 convert-mac-base64 = "mytoolit.scripts.mac:main"
```

