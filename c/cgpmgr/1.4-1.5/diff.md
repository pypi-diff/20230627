# Comparing `tmp/cgpmgr-1.4.tar.gz` & `tmp/cgpmgr-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgpmgr-1.4.tar", last modified: Sat Jun 17 13:13:45 2023, max compression
+gzip compressed data, was "cgpmgr-1.5.tar", last modified: Tue Jun 27 14:41:01 2023, max compression
```

## Comparing `cgpmgr-1.4.tar` & `cgpmgr-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 13:13:45.200005 cgpmgr-1.4/
--rw-r--r--   0 pi        (1000) pi        (1000)    11342 2021-09-04 14:18:09.000000 cgpmgr-1.4/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-17 13:13:45.200005 cgpmgr-1.4/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     2812 2023-06-05 04:58:21.000000 cgpmgr-1.4/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 13:13:45.170005 cgpmgr-1.4/cgpmgr/
--rwxr-xr-x   0 pi        (1000) pi        (1000)       19 2021-09-05 05:17:17.000000 cgpmgr-1.4/cgpmgr/__init__.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)    30617 2023-06-17 13:11:23.000000 cgpmgr-1.4/cgpmgr/cli.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 13:13:45.190005 cgpmgr-1.4/cgpmgr.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      241 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       14 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-17 13:13:45.200005 cgpmgr-1.4/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)      478 2023-06-17 13:11:15.000000 cgpmgr-1.4/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 14:41:01.235649 cgpmgr-1.5/
+-rw-r--r--   0 pi        (1000) pi        (1000)    11342 2021-09-04 14:18:09.000000 cgpmgr-1.5/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-27 14:41:01.235649 cgpmgr-1.5/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     2812 2023-06-05 04:58:21.000000 cgpmgr-1.5/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 14:41:01.225649 cgpmgr-1.5/cgpmgr/
+-rwxr-xr-x   0 pi        (1000) pi        (1000)       19 2021-09-05 05:17:17.000000 cgpmgr-1.5/cgpmgr/__init__.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)    30617 2023-06-27 14:40:06.000000 cgpmgr-1.5/cgpmgr/cli.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 14:41:01.235649 cgpmgr-1.5/cgpmgr.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      241 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       14 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        7 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-27 14:41:01.235649 cgpmgr-1.5/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)      478 2023-06-27 14:40:06.000000 cgpmgr-1.5/setup.py
```

### Comparing `cgpmgr-1.4/LICENSE` & `cgpmgr-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cgpmgr-1.4/README.md` & `cgpmgr-1.5/README.md`

 * *Files identical despite different names*

### Comparing `cgpmgr-1.4/cgpmgr/cli.py` & `cgpmgr-1.5/cgpmgr/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Raspberry Pi/Jetson Nano電源管理 拡張基板 RPZ-PowerMGR用コントロールツール
 Indoor Corgi, https://www.indoorcorgielec.com
 GitHub: https://github.com/IndoorCorgi/cgpmgr
-Version 1.4
+Version 1.5
 
 必要環境:
 1) Raspberry Pi OS / Jetson Linux, Python3
 2) I2Cインターフェース
   Raspberry PiでI2Cを有効にする方法
   https://www.indoorcorgielec.com/resources/raspberry-pi/raspberry-pi-i2c/
 3) 電源管理 拡張基板 RPZ-PowerMGR
@@ -759,15 +759,15 @@
   else:
     s += '*, '
 
   if (sch[2] >> 7) == 0:
     if (sch[2] & 0x40) == 0:
       s += '{:02}, '.format(sch[2])
     else:
-      s += '{}, '.format((dow2str[sch[2] & 0x7 - 1]))
+      s += '{}, '.format(dow2str[(sch[2] & 0x7) - 1])
   else:
     s += '*, '
 
   if (sch[1] >> 7) == 0:
     s += '{:02}, '.format(sch[1])
   else:
     s += '*, '
```

