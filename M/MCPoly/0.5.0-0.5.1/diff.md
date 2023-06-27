# Comparing `tmp/MCPoly-0.5.0.tar.gz` & `tmp/MCPoly-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCPoly-0.5.0.tar", last modified: Mon Jun 19 08:26:12 2023, max compression
+gzip compressed data, was "MCPoly-0.5.1.tar", last modified: Tue Jun 27 14:13:38 2023, max compression
```

## Comparing `MCPoly-0.5.0.tar` & `MCPoly-0.5.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.045613 MCPoly-0.5.0/
--rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.5.0/LICENSE
--rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.5.0/MANIFEST.in
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.032032 MCPoly-0.5.0/MCPoly/
--rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-06-12 17:23:57.000000 MCPoly-0.5.0/MCPoly/.DS_Store
--rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.5.0/MCPoly/__init__.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.034875 MCPoly-0.5.0/MCPoly/lmpset/
--rw-r--r--   0 cxs454     (503) staff       (20)     5719 2023-06-18 16:08:00.000000 MCPoly-0.5.0/MCPoly/lmpset/DATAtoXYZ.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-12 14:51:59.000000 MCPoly-0.5.0/MCPoly/lmpset/DATAtomolTXT.py
--rw-r--r--   0 cxs454     (503) staff       (20)      169 2023-06-17 16:42:13.000000 MCPoly-0.5.0/MCPoly/lmpset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.5.0/MCPoly/lmpset/chain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.5.0/MCPoly/lmpset/infchain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    53042 2023-06-18 16:59:51.000000 MCPoly-0.5.0/MCPoly/lmpset/mould.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5425 2023-06-18 17:37:10.000000 MCPoly-0.5.0/MCPoly/lmpset/rebuild.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.037074 MCPoly-0.5.0/MCPoly/moldraw/
--rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.5.0/MCPoly/moldraw/C_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.5.0/MCPoly/moldraw/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.5.0/MCPoly/moldraw/bind_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.5.0/MCPoly/moldraw/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.5.0/MCPoly/moldraw/molecule.py
--rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.5.0/MCPoly/moldraw/sub_selection.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.040334 MCPoly-0.5.0/MCPoly/orcaset/
--rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.5.0/MCPoly/orcaset/XYZtoINP.py
--rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.5.0/MCPoly/orcaset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16739 2023-06-16 15:10:25.000000 MCPoly-0.5.0/MCPoly/orcaset/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     7592 2023-06-07 15:00:39.000000 MCPoly-0.5.0/MCPoly/orcaset/mgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.5.0/MCPoly/orcaset/multiorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.5.0/MCPoly/orcaset/orca.py
--rw-r--r--   0 cxs454     (503) staff       (20)    19721 2023-06-16 15:10:30.000000 MCPoly-0.5.0/MCPoly/orcaset/ssgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     9044 2023-06-09 09:20:04.000000 MCPoly-0.5.0/MCPoly/orcaset/ssorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.5.0/MCPoly/orcaset/view3dchoose.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.041807 MCPoly-0.5.0/MCPoly/sscurve/
--rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.5.0/MCPoly/sscurve/YModulus.py
--rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.5.0/MCPoly/sscurve/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.5.0/MCPoly/sscurve/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.5.0/MCPoly/sscurve/multiple.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.5.0/MCPoly/sscurve/single.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.042909 MCPoly-0.5.0/MCPoly/status/
--rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.5.0/MCPoly/status/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6192 2023-06-18 16:33:35.000000 MCPoly-0.5.0/MCPoly/status/echart.py
--rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.5.0/MCPoly/status/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)    21428 2023-06-18 17:31:17.000000 MCPoly-0.5.0/MCPoly/status/status.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.043338 MCPoly-0.5.0/MCPoly/version/
--rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.5.0/MCPoly/version/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)       33 2023-06-19 08:23:12.000000 MCPoly-0.5.0/MCPoly/version/version.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.043782 MCPoly-0.5.0/MCPoly/view3d/
--rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.5.0/MCPoly/view3d/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.5.0/MCPoly/view3d/view3d.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.044378 MCPoly-0.5.0/MCPoly/vis/
--rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.5.0/MCPoly/vis/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.5.0/MCPoly/vis/vis.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.032970 MCPoly-0.5.0/MCPoly.egg-info/
--rw-r--r--   0 cxs454     (503) staff       (20)     4135 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     1279 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/SOURCES.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/dependency_links.txt
--rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/requires.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-19 08:26:12.000000 MCPoly-0.5.0/MCPoly.egg-info/top_level.txt
--rw-r--r--   0 cxs454     (503) staff       (20)     4135 2023-06-19 08:26:12.045436 MCPoly-0.5.0/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     3773 2023-06-19 08:22:46.000000 MCPoly-0.5.0/README.md
--rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-19 08:26:12.045662 MCPoly-0.5.0/setup.cfg
--rw-r--r--   0 cxs454     (503) staff       (20)     1031 2023-06-19 08:23:22.000000 MCPoly-0.5.0/setup.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-19 08:26:12.045229 MCPoly-0.5.0/tests/
--rw-r--r--   0 cxs454     (503) staff       (20)     9627 2023-06-18 17:38:10.000000 MCPoly-0.5.0/tests/test_lmpset.py
--rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.5.0/tests/test_moldraw.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.5.0/tests/test_orcaset.py
--rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.5.0/tests/test_sscurve.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5246 2023-06-18 16:42:29.000000 MCPoly-0.5.0/tests/test_status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.945476 MCPoly-0.5.1/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.5.1/LICENSE
+-rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.5.1/MANIFEST.in
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.935717 MCPoly-0.5.1/MCPoly/
+-rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-06-12 17:23:57.000000 MCPoly-0.5.1/MCPoly/.DS_Store
+-rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.5.1/MCPoly/__init__.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.938301 MCPoly-0.5.1/MCPoly/lmpset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     5719 2023-06-18 16:08:00.000000 MCPoly-0.5.1/MCPoly/lmpset/DATAtoXYZ.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-12 14:51:59.000000 MCPoly-0.5.1/MCPoly/lmpset/DATAtomolTXT.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      169 2023-06-17 16:42:13.000000 MCPoly-0.5.1/MCPoly/lmpset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.5.1/MCPoly/lmpset/chain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.5.1/MCPoly/lmpset/infchain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    53042 2023-06-18 16:59:51.000000 MCPoly-0.5.1/MCPoly/lmpset/mould.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5402 2023-06-19 16:17:41.000000 MCPoly-0.5.1/MCPoly/lmpset/rebuild.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.939870 MCPoly-0.5.1/MCPoly/moldraw/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.5.1/MCPoly/moldraw/C_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.5.1/MCPoly/moldraw/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.5.1/MCPoly/moldraw/bind_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.5.1/MCPoly/moldraw/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.5.1/MCPoly/moldraw/molecule.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.5.1/MCPoly/moldraw/sub_selection.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.941424 MCPoly-0.5.1/MCPoly/orcaset/
+-rw-r--r--   0 cxs454     (503) staff       (20)    10729 2023-06-24 15:26:07.000000 MCPoly-0.5.1/MCPoly/orcaset/XYZtoINP.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.5.1/MCPoly/orcaset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    20688 2023-06-27 14:13:27.000000 MCPoly-0.5.1/MCPoly/orcaset/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     7792 2023-06-27 14:07:19.000000 MCPoly-0.5.1/MCPoly/orcaset/mgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.5.1/MCPoly/orcaset/multiorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2310 2023-06-27 14:02:40.000000 MCPoly-0.5.1/MCPoly/orcaset/orca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24435 2023-06-27 14:13:11.000000 MCPoly-0.5.1/MCPoly/orcaset/ssgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     9044 2023-06-09 09:20:04.000000 MCPoly-0.5.1/MCPoly/orcaset/ssorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.5.1/MCPoly/orcaset/view3dchoose.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.942262 MCPoly-0.5.1/MCPoly/sscurve/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.5.1/MCPoly/sscurve/YModulus.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.5.1/MCPoly/sscurve/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-06-22 12:33:27.000000 MCPoly-0.5.1/MCPoly/sscurve/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.5.1/MCPoly/sscurve/multiple.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.5.1/MCPoly/sscurve/single.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.943064 MCPoly-0.5.1/MCPoly/status/
+-rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.5.1/MCPoly/status/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6192 2023-06-18 16:33:35.000000 MCPoly-0.5.1/MCPoly/status/echart.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.5.1/MCPoly/status/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24351 2023-06-27 13:59:56.000000 MCPoly-0.5.1/MCPoly/status/status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.943467 MCPoly-0.5.1/MCPoly/version/
+-rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.5.1/MCPoly/version/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       33 2023-06-24 15:21:50.000000 MCPoly-0.5.1/MCPoly/version/version.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.943777 MCPoly-0.5.1/MCPoly/view3d/
+-rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.5.1/MCPoly/view3d/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.5.1/MCPoly/view3d/view3d.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.944104 MCPoly-0.5.1/MCPoly/vis/
+-rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.5.1/MCPoly/vis/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2112 2023-06-27 13:59:22.000000 MCPoly-0.5.1/MCPoly/vis/vis.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.936488 MCPoly-0.5.1/MCPoly.egg-info/
+-rw-r--r--   0 cxs454     (503) staff       (20)     4135 2023-06-27 14:13:38.000000 MCPoly-0.5.1/MCPoly.egg-info/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     1279 2023-06-27 14:13:38.000000 MCPoly-0.5.1/MCPoly.egg-info/SOURCES.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-27 14:13:38.000000 MCPoly-0.5.1/MCPoly.egg-info/dependency_links.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-27 14:13:38.000000 MCPoly-0.5.1/MCPoly.egg-info/requires.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-27 14:13:38.000000 MCPoly-0.5.1/MCPoly.egg-info/top_level.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)     4135 2023-06-27 14:13:38.945220 MCPoly-0.5.1/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     3773 2023-06-19 08:22:46.000000 MCPoly-0.5.1/README.md
+-rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-27 14:13:38.945542 MCPoly-0.5.1/setup.cfg
+-rw-r--r--   0 cxs454     (503) staff       (20)     1031 2023-06-24 15:21:40.000000 MCPoly-0.5.1/setup.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-27 14:13:38.944933 MCPoly-0.5.1/tests/
+-rw-r--r--   0 cxs454     (503) staff       (20)     9627 2023-06-18 17:38:10.000000 MCPoly-0.5.1/tests/test_lmpset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.5.1/tests/test_moldraw.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     3931 2023-06-24 15:32:23.000000 MCPoly-0.5.1/tests/test_orcaset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.5.1/tests/test_sscurve.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5241 2023-06-24 15:37:07.000000 MCPoly-0.5.1/tests/test_status.py
```

### Comparing `MCPoly-0.5.0/LICENSE` & `MCPoly-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/.DS_Store` & `MCPoly-0.5.1/MCPoly/.DS_Store`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/lmpset/DATAtoXYZ.py` & `MCPoly-0.5.1/MCPoly/lmpset/DATAtoXYZ.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/lmpset/DATAtomolTXT.py` & `MCPoly-0.5.1/MCPoly/lmpset/DATAtomolTXT.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/lmpset/chain.py` & `MCPoly-0.5.1/MCPoly/lmpset/chain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/lmpset/infchain.py` & `MCPoly-0.5.1/MCPoly/lmpset/infchain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/lmpset/mould.py` & `MCPoly-0.5.1/MCPoly/lmpset/mould.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/lmpset/rebuild.py` & `MCPoly-0.5.1/MCPoly/lmpset/rebuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
             xmin=num[1]
         if num[2]<ymin:
             ymin=num[2]
         if num[3]<zmin:
             zmin=num[3]
     atoms_number=len(pos)
     os.chdir(path)
-    print(os.getcwd())
     readfile = open(loc+'{0}.data'.format(file),'r')
     try:
         f = open(loc+'pre.data','x')
     except:
         f = open(loc+'pre.data','w')
     c=0
     i=0
```

### Comparing `MCPoly-0.5.0/MCPoly/moldraw/C_selection.py` & `MCPoly-0.5.1/MCPoly/moldraw/C_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/moldraw/bind_selection.py` & `MCPoly-0.5.1/MCPoly/moldraw/bind_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/moldraw/gui.py` & `MCPoly-0.5.1/MCPoly/moldraw/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/moldraw/molecule.py` & `MCPoly-0.5.1/MCPoly/moldraw/molecule.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/moldraw/sub_selection.py` & `MCPoly-0.5.1/MCPoly/moldraw/sub_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/orcaset/XYZtoINP.py` & `MCPoly-0.5.1/MCPoly/orcaset/XYZtoINP.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from ase.io import read
 import warnings
 
-def XYZtoINP(file,inpname='',fileloc='./',saveloc='./',method='B3LYP',basis_set='def2-SVP',opt=False,freq=False,scan=False,external_force=False,ts=False,aim=[0,0],stretch=-1,scanstep=10,strain=-1,maxiter=-1,maxcore=-1,corenum=1,electron=0,state=1):
+def XYZtoINP(file,inpname='',fileloc='./',saveloc='./',method='B3LYP',basis_set='def2-SVP',opt=False,freq=False,scan=False,external_force=False,ts=False,aim=[0,0],stretch=-1,scanstep=10,strain=-1,maxiter=-1,maxcore=-1,corenum=1,electron=0,state=1,MD=False,md_timestep=1.0,initvel=300, tsNHC=300, timecon=10.0, dumpcon=10,runstep=100,dumpname=''):
     """
     The method to convert .xyz file into .inp file.
     XYZtoINP(file,inpname='',loc='./',method='B3LYP',basis_set='def2-SVP',opt=False,freq=False,scan=False,external_force=False,ts=False,aim=[0,0],stretch=1,scanstep=10,strain=-1,maxiter=-1,maxcore=-1,corenum=1,electron=0,state=1)
     file: Your .xyz file name.
     inpname: The name of your saved .inp file.
     fileloc: File Location. The default is your current location.
     saveloc: Input File Save Location. The default is your current location.
@@ -93,28 +93,82 @@
             C         -7.11449        1.33604       -0.03969
             C         -5.87285        0.46952       -0.06689
             C         -4.65267        1.33725        0.06683
             C         -3.41103        0.47072        0.03973
             F         -7.23198        2.03119        1.11508
                 ...
             *
+    
+    Example 4:
+        Input:
+            from MCPoly.orcaset import XYZtoINP
+            XYZtoINP('Atom1',method='B3LYP D3BJ',basis_set='def2-TZVP',MD=True,\
+                     MD=True,freq=True,md_timestep=1.0,initvel=350,tsNHC=350,dumpcon=25,runstep=2500,maxcore=4096,corenum=8)
+        Output in Atom1.inp:
+            #Powered by MCPoly
+            
+            ! MD B3LYP D3BJ def2-TZVP 
+            %md
+            Timestep 1.0_fs
+            Initvel 350_K
+            Thermostat NHC 350_K Timecon 10.0_fs
+            Dump Position Stride 25 Filename "S4A_dump.xyz"
+            Run 2500
+            end
+            %maxcore 4096
+            %PAL NPROCS 8 END
+            
+            *xyz 0 1
+            C         -7.11449        1.33604       -0.03969
+            C         -5.87285        0.46952       -0.06689
+            C         -4.65267        1.33725        0.06683
+            C         -3.41103        0.47072        0.03973
+            F         -7.23198        2.03119        1.11508
+                ...
+            *
     """
     f=open(fileloc+file+'.xyz','r')
     if inpname=='':
         try:
             w=open(saveloc+file+'.inp','x')
         except:
             w=open(saveloc+file+'.inp','w')
     else:
         try:
             w=open(saveloc+inpname+'.inp','x')
         except:
             w=open(saveloc+inpname+'.inp','w')
     w.write('#Powered by MCPoly\n\n')
-    w.write('! {0} {1} '.format(method,basis_set))
+    w.write('! ')
+    if MD==True:
+        w.write('MD ')
+        sacn=False
+        opt=False
+        freq=False
+        external_force=False
+    
+    w.write('{0} {1} '.format(method,basis_set))
+        
+    if MD==True:
+        w.write('\n')
+        if initvel<0:
+            raise ValueError("Key word 'initvel' must be positive, for the unit is Kelvin.")
+        if tsNHC<0:
+            raise ValueError("Key word 'tsNHC' must be positive, for the unit is Kelvin.")
+        w.write('%md\n')
+        w.write('Timestep {0}_fs\n'.format(md_timestep))
+        w.write('Initvel {0}_K\n'.format(initvel))
+        w.write('Thermostat NHC {0}_K Timecon {1}_fs\n'.format(tsNHC,timecon))
+        if dumpname=='':
+            w.write('Dump Position Stride {0} Filename "{1}_dump.xyz"\n'.format(dumpcon,file))
+        else:
+            w.write('Dump Position Stride {0} Filename "{1}_dump.xyz"\n'.format(dumpcon,dumpname))
+        w.write('Run {0}\n'.format(runstep))
+        w.write('end\n')
+        
     if opt==True:
         if scan==True:
             pass
         if ts==True:
             w.write('OPTTS ')
         else:
             w.write('OPT ')
@@ -125,15 +179,15 @@
             warnings.warn('Your set the frequency calculation without geometry optimisation.')
         w.write('FREQ')
     w.write('\n')
     
     if maxiter!=-1:
         if maxiter<=0 or type(maxiter)==float:
             raise ValueError("Key word 'maxiter' must be a positive integar.")
-        w.write('%SCF\n    MAXITER {0}\n'.format(maxiter))
+        w.write('%geom\n    MAXITER {0}\nend\n'.format(maxiter))
     
     if maxcore!=-1:
         w.write('%maxcore {0}\n'.format(maxcore))
         if maxcore<=2048:
             warnings.warn('Your max core space is only {0:.3f} Å. You might delete this key words to get the same calculation speed, or try bigger one.'.format(maxcore))
 
     if corenum!=1:
```

### Comparing `MCPoly-0.5.0/MCPoly/orcaset/mgui.py` & `MCPoly-0.5.1/MCPoly/orcaset/mgui.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,24 +55,24 @@
     
     def intro_status3d(button):
         ii=0
         for file in files.value:
             ii=ii+1
             if roomox.value==False and coreox.value==False:
                 XYZtoINP(file,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,\
-                     maxcore=room.value*1024,corenum=corenum.value,electron=e.value,state=state.value)
+                     maxiter=maxiter.value,maxcore=room.value*1024,corenum=corenum.value,electron=e.value,state=state.value)
             elif roomox.value==False and coreox.value==True:
                 XYZtoINP(file,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,\
-                     maxcore=room.value*1024,electron=e.value,state=state.value)
+                     maxiter=maxiter.value,maxcore=room.value*1024,electron=e.value,state=state.value)
             elif roomox.value==True and coreox.value==False:
                 XYZtoINP(file,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,\
-                     corenum=corenum.value,electron=e.value,state=state.value)
+                     maxiter=maxiter.value,corenum=corenum.value,electron=e.value,state=state.value)
             elif roomox.value==True and coreox.value==True:
                 XYZtoINP(file,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,\
-                     electron=e.value,state=state.value)
+                     maxiter=maxiter.value,electron=e.value,state=state.value)
             with case:
                 display(widgets.HBox([widgets.Label(file), widgets.Label('  Processing...'), widgets.Label('[{0}]'.format(t.ctime(t.time())))]))
             orca(file,orcaloc.value,loc.value,loc.value)
             s=status(file,loc.value).status(statusonly=True)
             if s==4:
                 case.clear_output()
                 with case:
@@ -119,28 +119,29 @@
     coreox=widgets.ToggleButton(value=False,description='Default CoreNumber')
     e=widgets.IntText(description='Charge:',value=0,layout=widgets.Layout(width='50%'))
     state=widgets.IntText(description='State:',value=1,layout=widgets.Layout(width='47.5%'))
     geoox=widgets.ToggleButton(value=False,description='Structure Status',style=dict(font_weight='bold'),layout=widgets.Layout(width='98.5%'))
     startorca=widgets.Button(description='Start ORCA Calculation',layout=widgets.Layout(width='99%'),style=dict(font_weight='bold',text_decoration='underline'))
     geoout=widgets.interactive_output(geoshow, {'files': files, 'loc': loc, 'method': method, 'bs': bs})
     orcaloc=widgets.Text(value='./')
+    maxiter=widgets.IntText(description='MaxIteration:',value=200,layout=widgets.Layout(width='98.5%'))
     
     title1=widgets.Label('File Details',style=dict(font_weight='bold'))
     title2=widgets.Label('Calculation Methods',style=dict(font_weight='bold'))
     
     box_layout1 = widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
-                    align_items='stretch', border='solid', height='550px', width='31%')
+                    align_items='stretch', border='solid', height='650px', width='31%')
     box_layout2 = widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
-                    align_items='stretch', border='solid', height='550px', width='33%')
+                    align_items='stretch', border='solid', height='650px', width='33%')
     widgets.jslink((roomox,'value'),(room,'disabled'))
     widgets.jslink((coreox,'value'),(corenum,'disabled'))
     #introstatus=widgets.Button(description='See Current Calculation Status',style=dict(font_weight='bold',text_decoration='underline'),
     #                  layout=widgets.Layout(width='98.5%'))
 
     frame1=widgets.VBox([title1,loc,files,title2,widgets.HBox([opt,freq]),method,bs,widgets.HBox([corenum,coreox]),\
-                     widgets.HBox([room,roomox]),widgets.HBox([e,state])],layout=box_layout1)
+                     widgets.HBox([room,roomox]),maxiter,widgets.HBox([e,state])],layout=box_layout1)
     frame3=widgets.VBox([output2,case])
     output.layout=box_layout2
     frame3.layout=box_layout2
     startorca.on_click(intro_status3d)
 
     display(widgets.HBox([frame1,output,frame3]))
```

### Comparing `MCPoly-0.5.0/MCPoly/orcaset/multiorca.py` & `MCPoly-0.5.1/MCPoly/orcaset/multiorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/orcaset/orca.py` & `MCPoly-0.5.1/MCPoly/orcaset/orca.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,8 +39,14 @@
         os.chdir(orcaloc)
         if fileloc=='./':
             fileloc=path
         if saveloc=='./':
             saveloc=path
         os.system('./orca {0}{1}.inp > {2}{1}.out'.format(fileloc,file,saveloc))
         print('Program Completed.[{0}]\n'.format(t.ctime(t.time())))
-        os.chdir(path[:-1])
+        os.chdir(path[:-1])
+    f=open(file+'.inp','r')
+    for line in f:
+        md=re.search('%md',line)
+        if md:
+            os.system('cp {0}{1}_dump.xyz {1}_dump.xyz'.format(orcaloc,file))
+            os.system('rm {0}{1}_dump.xyz'.format(orcaloc,file))
```

### Comparing `MCPoly-0.5.0/MCPoly/orcaset/ssgui.py` & `MCPoly-0.5.1/MCPoly/orcaset/ssgui.py`

 * *Files 21% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def showfrom(fromshow,file,loc,aim1,aim2):
         fromoutput.clear_output()
         opath=os.getcwd()
         polymers0=[]
         for path in os.listdir(loc):
             if os.path.isfile(os.path.join(loc, path)):
-                a=re.search('{0}_'.format(file), path)
+                a=re.match('{0}_'.format(file), path)
                 if a:
                     b=re.search('_trj.xyz', path)
                     if b:
                         c=re.match('{0}_trj.xyz'.format(file), path)
                         if not c:
                             polymers0.append(path[:-8])
         polynums=[]
@@ -92,18 +92,22 @@
                 else:
                     view3dchoose(polymer,loc,choose=[aim1,aim2],width=450,height=400)
         os.chdir(opath)
 
     def curveshow(curve,file,loc):
         output2.clear_output()
         curveoutput.clear_output()
+        case.clear_output()
         with curveoutput:
             if curve==True:
                 single(file,loc).autocurve(savefig=False,savedata=False)
                 display(widgets.HBox([savechart,savedata]))
+    
+#    def aborting(button):
+#        
 
     def addshow1(addox1):
         addoutput1.clear_output()
         if addox1==True:
             addox2.disabled=False
             with addoutput1:
                 display(strain2,addforce2)
@@ -114,14 +118,15 @@
     def addshow2(addox2):
         addoutput2.clear_output()
         if addox2==True:
             with addoutput2:
                 display(strain3,addforce3)
 
     def geoshow(file,loc,aim1,aim2,method,bs):
+        aa.value=0
         atomsx=read(loc+file+'.xyz')
         num=len(atomsx)
         output.clear_output()
         with output:
             try:
                 if aim1==0 and aim2==0:
                     view3d(file,loc,width=450,height=400)
@@ -147,64 +152,110 @@
         single(file.value,loc.value).autocurve(savedata=False)
         
     def savedatax(button):
         single(file.value,loc.value).autocurve(savefig=False)
     
     def intro_status3d(button):
         atomsx=read(loc.value+file.value+'.xyz')
+        global forcestep
+        global key
         num=len(atomsx)
         if aim1.value>=num:
-            aim1.value=num-1
+            aim1.valu10e=num-1
         if aim2.value>=num:
             aim2.value=num-1
         output.clear_output()
-        with output2:
-            display(widgets.Label('File: {0}.xyz'.format(file.value),style=dict(font_weight='bold')))
-            if roomox.value==False and coreox.value==False:
-                XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
-                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,maxcore=room.value*1024,corenum=corenum.value)
-            elif roomox.value==True and coreox.value==True:
-                XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
-                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value)
-            elif roomox.value==False and coreox.value==True:
-                XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
-                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,maxcore=room.value*1024)
-            elif roomox.value==True and coreox.value==False:
-                XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
-                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,corenum=corenum.value)
-        os.system('cp {0}.inp {0}_0.000.inp'.format(file.value))
-        keys=[]
-        if addforce.value==0:
-            raise ValueError("You can't set the force add per step zero!")
-        forcestep={strain.value:addforce.value}
-        if addox1.value==True:
-            if addforce2.value==0:
+        case.clear_output()
+        output2.clear_output()
+        if aa.value==404:
+            with output2:
+                if roomox.value==False and coreox.value==False:
+                    XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
+                                 method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
+                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],\
+                                 maxiter=maxiter.value,maxcore=room.value*1024,corenum=corenum.value)
+                elif roomox.value==True and coreox.value==True:
+                    XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
+                                 method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
+                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],maxiter=maxiter.value)
+                elif roomox.value==False and coreox.value==True:
+                    XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
+                                 method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
+                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],maxiter=maxiter.value,maxcore=room.value*1024)
+                elif roomox.value==True and coreox.value==False:
+                    XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
+                                 method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
+                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],maxiter=maxiter.value,corenum=corenum.value)
+                    strain.value=strain.value+forcestep[key]
+            keys=[]
+            if addforce.value==0:
                 raise ValueError("You can't set the force add per step zero!")
-            forcestep={strain.value: addforce.value, strain2.value: addforce2.value}
-        elif addox1.value==True and addox2.value==True:
-            if addforce3.value==0:
+            forcestep={strain.value:addforce.value}
+            if addox1.value==True:
+                if addforce2.value==0:
+                    raise ValueError("You can't set the force add per step zero!")
+                forcestep={strain.value: addforce.value, strain2.value: addforce2.value}
+            elif addox1.value==True and addox2.value==True:
+                if addforce3.value==0:
+                    raise ValueError("You can't set the force add per step zero!")
+                forcestep={strain.value: addforce.value, strain2.value: addforce2.value, strain3.value: addforce3.value}
+            for key in forcestep:
+                keys.append(key)
+            keys.reverse()
+            key=keys[0]
+            ii=2
+        else:
+            with output2:
+                display(widgets.Label('File: {0}.xyz'.format(file.value),style=dict(font_weight='bold')))
+                if roomox.value==False and coreox.value==False:
+                    XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
+                     external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,maxiter=maxiter.value,maxcore=room.value*1024,corenum=corenum.value)
+                elif roomox.value==True and coreox.value==True:
+                    XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
+                     external_force=True,aim=[aim1.value,aim2.value],maxiter=maxiter.value,strain=strain.value)
+                elif roomox.value==False and coreox.value==True:
+                    XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
+                     external_force=True,aim=[aim1.value,aim2.value],maxiter=maxiter.value,strain=strain.value,maxcore=room.value*1024)
+                elif roomox.value==True and coreox.value==False:
+                    XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
+                     external_force=True,aim=[aim1.value,aim2.value],maxiter=maxiter.value,strain=strain.value,corenum=corenum.value)
+            if strain==0.000:
+                os.system('cp {0}.inp {0}_0.000.inp'.format(file.value))
+            keys=[]
+            if addforce.value==0:
                 raise ValueError("You can't set the force add per step zero!")
-            forcestep={strain.value: addforce.value, strain2.value: addforce2.value, strain3.value: addforce3.value}
-        for key in forcestep:
-            keys.append(key)
-        keys.reverse()
-        key=keys[0]
-        ii=-1
-        distances=[]
-        force=[]
+            forcestep={strain.value:addforce.value}
+            if addox1.value==True:
+                if addforce2.value==0:
+                    raise ValueError("You can't set the force add per step zero!")
+                forcestep={strain.value: addforce.value, strain2.value: addforce2.value}
+            elif addox1.value==True and addox2.value==True:
+                if addforce3.value==0:
+                    raise ValueError("You can't set the force add per step zero!")
+                forcestep={strain.value: addforce.value, strain2.value: addforce2.value, strain3.value: addforce3.value}
+            for key in forcestep:
+                keys.append(key)
+            keys.reverse()
+            key=keys[0]
+            ii=-1
+            global distances
+            distances=[]
+            global force
+            force=[]
         while 1:
-            ii=ii+1
             with case:
                 display(widgets.HBox([widgets.Label(file.value+'_{0:.3f}'.format(strain.value)), widgets.Label('  Processing...'), widgets.Label('[{0}]'.format(t.ctime(t.time())))]))
             orca(file.value+'_{0:.3f}'.format(strain.value),orcaloc.value,loc.value,loc.value)
+            ii=ii+1
             s=status(file.value+'_{0:.3f}'.format(strain.value),loc.value).status(statusonly=True)
             the_atoms=read(file.value+'_{0:.3f}.xyz'.format(strain.value))
             d=the_atoms.get_distance(aim1.value,aim2.value)
             case.clear_output()
             if s==4:
+                aa.value=0
                 distances.append(d)
                 force.append(strain.value)
                 xoy=checkbroken(distances,force)
                 if xoy==1:
                     with output2:
                         display(widgets.HBox([widgets.Valid(description=file.value+'_{0:.3f}'.format(strain.value),value=True),\
                                       widgets.Label('Broken.'), widgets.Label('[{0}]'.format(t.ctime(t.time())))]))
@@ -229,30 +280,45 @@
                         case.clear_output()
                         with case:
                             display(widgets.Valid(description=file.value+'_{0:.3f}'.format(strain.value),value=False,\
                                 readout='Error!'), widgets.Label('[{0}]'.format(t.ctime(t.time()))))
                     else:
                         distances[-1]=d
             elif s==2:
+                aa.value=0
                 with output2:
                     distances.append(d)
                     force.append(strain.value)
                     display(widgets.HBox([widgets.Valid(description=file.value+'_{0:.3f}'.format(strain.value),value=True),\
                                   widgets.Label('Completed.'), widgets.Label('[{0}]'.format(t.ctime(t.time())))]))
+            elif s==6:
+                aa.value=404
+                with output2:
+                    distances.append(d)
+                    force.append(strain.value)
+                    display(widgets.HBox([widgets.Valid(description=file.value+'_{0:.3f}'.format(strain.value),value=True),\
+                                  widgets.Label('Not Converged.'), widgets.Label('[{0}]'.format(t.ctime(t.time())))]))
+                    curve.layout=widgets.Layout(width='50%')
+                with case:
+                    display(widgets.Label("{0}_{1:.3f} is finished but it's not converged.\n Continue?".format(file.value,strain.value)))
+                    display(widgets.HBox([stop,curve]))
+                strain.value=strain.value+forcestep[key]
+                curve.layout=widgets.Layout(width='99%')
+                break
             if ii==0:
                 output.clear_output()
                 with output:
                     display(fromoutput)
             
             opath=os.getcwd()
             polys=[]
             try:
                 for path in os.listdir(loc.value):
                     if os.path.isfile(os.path.join(loc.value, path)):
-                        a=re.search('{0}_'.format(file.value), path)
+                        a=re.match('{0}_'.format(file.value), path)
                         if a:
                             b=re.search('_trj.xyz', path)
                             if b:
                                 c=re.search('{0}_trj.xyz'.format(file.value), path)
                                 if not c:
                                     polys.append(path[:-8])
                 polys.sort()
@@ -269,33 +335,35 @@
             os.chdir(opath)
             
             for key in keys:
                 if strain.value>=key:
                     if roomox.value==False and coreox.value==False:
                         XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
                                  method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
-                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],maxcore=room.value*1024,corenum=corenum.value)
+                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],\
+                                 maxiter=maxiter.value,maxcore=room.value*1024,corenum=corenum.value)
                     elif roomox.value==True and coreox.value==True:
                         XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
                                  method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
-                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key])
+                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],maxiter=maxiter.value)
                     elif roomox.value==False and coreox.value==True:
                         XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
                                  method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
-                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],maxcore=room.value*1024)
+                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],maxiter=maxiter.value,maxcore=room.value*1024)
                     elif roomox.value==True and coreox.value==False:
                         XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
                                  method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
-                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],corenum=corenum.value)
+                                 external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],maxiter=maxiter.value,corenum=corenum.value)
                     strain.value=strain.value+forcestep[key]
                     break
-        with output:
-            display(fromshow)
-        with output2:
-            display(curve)
+        if aa.value!=404:
+            with output:
+                display(fromshow)
+            with output2:
+                display(curve)
 
     def statusresult(button):
         statusoutput.clear_output()
         with statusoutput:
             while 1:
                 if s==1:
                     break
@@ -314,41 +382,46 @@
     for path in os.listdir(loc.value):
         if os.path.isfile(os.path.join(loc.value, path)):
             a=re.search('.xyz', path)
             if a:
                 b=re.search(file.value,path)
                 if b:
                     ssfiles.append(path[:-4])
+    
+    stop=widgets.Button(description='Continue!',layout=widgets.Layout(width='50%'))
+    aa=widgets.IntText(value=0)
     method=widgets.Text(description='Method:')
     bs=widgets.Text(description='Basis Set:')
     freq=widgets.ToggleButton(value=False,description='Frequency',layout=widgets.Layout(width='33.3%'))
     room=widgets.IntText(description='Space(GB):',value=4,min=1,layout=widgets.Layout(width='50%'))
     roomox=widgets.ToggleButton(value=False,description='Default Space')
     corenum=widgets.IntText(description='Core:',value=4,min=1,layout=widgets.Layout(width='50%'))
     coreox=widgets.ToggleButton(value=False,description='Default CoreNumber')
-    aim1=widgets.BoundedIntText(description='Atom 1:',value=0,min=0,max=200,layout=widgets.Layout(width='50%'))
-    aim2=widgets.BoundedIntText(description='Atom 2:',value=0,min=0,max=200,layout=widgets.Layout(width='47.5%'))
+    aim1=widgets.BoundedIntText(description='Atom 1:',value=0,min=0,max=300,layout=widgets.Layout(width='50%'))
+    aim2=widgets.BoundedIntText(description='Atom 2:',value=0,min=0,max=300,layout=widgets.Layout(width='47.5%'))
     strain=widgets.BoundedFloatText(description='Start Force(nN):',value=0.000,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addforce=widgets.BoundedFloatText(description='Force Add per Step(nN):',value=0.100,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addox1=widgets.ToggleButton(value=False,description='The Second Stage',style=dict(font_weight='bold'))
     strain2=widgets.BoundedFloatText(description='Till Force(nN):',value=0.000,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addforce2=widgets.BoundedFloatText(description='Force Add per Step(nN):',value=0.100,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addox2=widgets.ToggleButton(value=False,description='The Third Stage',style=dict(font_weight='bold'))
     strain3=widgets.BoundedFloatText(description='Till Force(nN):',value=0.000,min=0.000,step=0.100,style = {'description_width': 'initial'})
     addforce3=widgets.BoundedFloatText(description='Force Add per Step(nN):',value=0.100,min=0.000,step=0.100,style = {'description_width': 'initial'})
     startorca=widgets.Button(description='Start ORCA Calculation',layout=widgets.Layout(width='99%'),style=dict(font_weight='bold',text_decoration='underline'))
     orcaloc=widgets.Text(value='./')
     curve=widgets.ToggleButton(description='Stress-Strain Curve',layout=widgets.Layout(width='99%'),style=dict(font_weight='bold',text_decoration='underline'))
     fromshow=widgets.ToggleButton(description='Show the site of Force',value=True,layout=widgets.Layout(width='99%'),style=dict(font_weight='bold',text_decoration='underline'))
     savechart=widgets.Button(description='Save chart ( .png)',layout=widgets.Layout(width='50%'))
     savedata=widgets.Button(description='Save data (.txt)',layout=widgets.Layout(width='47.5%'))
+    maxiter=widgets.IntText(description='MaxIteration:',value=200,layout=widgets.Layout(width='98.5%'))
     
     startorca.on_click(intro_status3d)
     savechart.on_click(savechartx)
     savedata.on_click(savedatax)
+    stop.on_click(intro_status3d)
     
     title1=widgets.Label('File Details',style=dict(font_weight='bold'))
     title2=widgets.Label('Calculation Methods',style=dict(font_weight='bold'))
     title3=widgets.Label('Constant External Force Settings',style=dict(font_weight='bold'))
     
     addout1=widgets.interactive_output(addshow1, {'addox1': addox1})
     addout2=widgets.interactive_output(addshow2, {'addox2': addox2})
@@ -356,21 +429,21 @@
     ssout=widgets.interactive_output(curveshow, {'curve': curve, 'file': file, 'loc': loc})
     fromout=widgets.interactive_output(showfrom, {'fromshow': fromshow, 'file': file, 'loc': loc, 'aim1': aim1, 'aim2': aim2})
     
     widgets.jslink((roomox,'value'),(room,'disabled'))
     widgets.jslink((coreox,'value'),(corenum,'disabled'))
     
     box_layout1 = widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
-                    align_items='stretch', border='solid', height='550px', width='31%')
+                    align_items='stretch', border='solid', height='650px', width='31%')
     box_layout2 = widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
-                    align_items='stretch', border='solid', height='550px', width='33%')
+                    align_items='stretch', border='solid', height='650px', width='33%')
     
     frame1=widgets.VBox([title1,loc,file,widgets.HBox([title2,freq]),method,bs,widgets.HBox([corenum,coreox]),\
-                     widgets.HBox([room,roomox]),title3,widgets.HBox([aim1,aim2]),strain,addforce,addox1,addoutput1,addox2,addoutput2],layout=box_layout1)
+                     widgets.HBox([room,roomox]),maxiter,title3,widgets.HBox([aim1,aim2]),strain,addforce,addox1,addoutput1,addox2,addoutput2],layout=box_layout1)
     frame3=widgets.VBox([output2,case,curveoutput])
     output.layout=box_layout2
     frame3.layout=box_layout2
     curveoutput.layout=widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
-                    align_items='stretch', height='550px', width='100%')
+                    align_items='stretch', height='650px', width='100%')
     output2.layout=widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
                     align_items='stretch', width='100%')
     display(widgets.HBox([frame1,output,frame3]))
```

### Comparing `MCPoly-0.5.0/MCPoly/orcaset/ssorca.py` & `MCPoly-0.5.1/MCPoly/orcaset/ssorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/orcaset/view3dchoose.py` & `MCPoly-0.5.1/MCPoly/orcaset/view3dchoose.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/sscurve/YModulus.py` & `MCPoly-0.5.1/MCPoly/sscurve/YModulus.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/sscurve/gui.py` & `MCPoly-0.5.1/MCPoly/sscurve/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,17 +271,17 @@
     output=widgets.VBox([title1,loc,files,resultshow])
     
     resultshow.on_click(intro_result)
     save1.on_click(pngsave)
     save2.on_click(csvsave)
     
     box_layout1 = widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
-                align_items='stretch', border='solid', height='550px', width='26%')
+                align_items='stretch', border='solid', height='650px', width='26%')
     box_layout2 = widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
-                align_items='stretch', border='solid', height='550px', width='37%')
+                align_items='stretch', border='solid', height='650px', width='37%')
     judgeoutput.layout=widgets.Layout(display='flex', flew_flow='column', overflow='scroll hidden',\
                 align_items='stretch',height='325px', width='100%')
     
     filejudgeout=widgets.interactive_output(filejudge, {'files': files, 'loc': loc})
     geoout=widgets.interactive_output(geoshow, {'aim1': aim1, 'aim2': aim2, 'geoi': geoi, 'files': files})
     
     output=widgets.VBox([title1,loc,files,resultshow])
```

### Comparing `MCPoly-0.5.0/MCPoly/sscurve/multiple.py` & `MCPoly-0.5.1/MCPoly/sscurve/multiple.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/sscurve/single.py` & `MCPoly-0.5.1/MCPoly/sscurve/single.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/status/echart.py` & `MCPoly-0.5.1/MCPoly/status/echart.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/status/gui.py` & `MCPoly-0.5.1/MCPoly/status/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/status/status.py` & `MCPoly-0.5.1/MCPoly/status/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,42 @@
 import ipywidgets as iw
 import py3Dmol
 from rdkit import Chem
 from rdkit.Chem.Draw import IPythonConsole
 from rdkit.Chem import rdDetermineBonds
 
 def status_judge(s1,s2,converge):
-    if s1==0 or s1==4:
+    if s1==0 or s1==4 or s1==41:
         if s1==0:
             print('The Optimization is processing.')
         elif s1==4 and s2==0:
             print('The Optimization is aborted.')
+        elif s1==41:
+            print('The Optimization is aborted.\n The structure includes 180 or 0 degrees angles.')
         print('Last time:')
         print('Energy change: {0}'.format(converge[-5]))
         print('RMS gradient: {0}             MAX gradient: {0}'.format(converge[-4],converge[-3]))
         print('RMS step: {0}                 MAX step: {0}'.format(converge[-2],converge[-1]))
     if s1!=0 and s2<0:
         print('The Optimization was finished.')
-        if s1==4:
+        if s1==4 or s1>=40:
             print('The frequency calculation is aborted.')
+            if s1==41:
+                print('There are some 0 or 180 degrees angles.\n Try to rebuild the system.')
             return None
         if s2==-1:
             print('The CP-SCF equations are forming.')
         elif s2==-2:
             print('The CP-SCF equations are solving.')
         elif s2==-3:
             print('The Thermodynamics Calculation was processing.')
     if s2==1:
         print('The Thermodynamics Calculation was finished.')
+    if s2==9 and s1==6:
+        print('The Thermodynamics Calculation was finished, but the optimization did not converge but reached the maximum number of optimization cycles.')
         
 def statusfig(energy,choose,num=-1):
     t=range(len(energy))
     if choose==0:
         plt.plot(t,energy,'x-')
     else:
         plt.plot(t[-choose:],energy[-choose:],'x-')
@@ -68,19 +74,25 @@
     v = py3Dmol.view(width=width,height=height)
     IPythonConsole.addMolToView(mol,v)
     v.zoomTo()
     v.setStyle({'sphere':{'radius':0.4},'stick':{'radius':0.1}});
     v.show()
     return v
 
-def multicreatemol(filename,turn,width,height):
-    try:
-        ind = open('{0}_trj.xyz'.format(filename),'r+')
-    except:
-        raise FileNotFoundError('Perhaps your _trj.xyz file has some errors. Please check the location of your _trj.xyz file and then modify your file.')
+def multicreatemol(filename,turn,width,height,MD=False):
+    if MD==True:
+        try:
+            ind = open('{0}_dump.xyz'.format(filename),'r+')
+        except:
+            raise FileNotFoundError('Perhaps your _dump.xyz file has some errors. Please check the location of your _dump.xyz file and then modify your file.')
+    else:
+        try:
+            ind = open('{0}_trj.xyz'.format(filename),'r+')
+        except:
+            raise FileNotFoundError('Perhaps your _trj.xyz file has some errors. Please check the location of your _trj.xyz file and then modify your file.')
     mains = ind.readlines()
     num=eval(mains[0][:-1])
     term=len(mains)/(num+2)
     main=''
     partmain=mains[turn*(num+2):(turn+1)*(num+2)]
     for i,line in enumerate(partmain):
         if i==1:
@@ -90,122 +102,142 @@
     #print(main)
     raw_mol = Chem.MolFromXYZBlock(main)
     conn_mol = Chem.Mol(raw_mol)
     rdDetermineBonds.DetermineConnectivity(conn_mol)
     v=draw_with_spheres(conn_mol,width,height)
     return v
 
-def normalstatus(loc,file,choose=0,figureonly=False,statusonly=False):
+def normalstatus(loc,file,choose=0,figureonly=False,statusonly=False,MD=False):
     path = os.getcwd()
     os.chdir(loc)
     file=file+'.out'
     if figureonly==False and statusonly==False:
         print(file)
     s1=0
     s2=0
     term=0
     f=open(file,'r')
     x=0
     energy=[]
     converge=[]
-    for line in f:
-        a=re.search('FINAL SINGLE POINT ENERGY',line)
-        if a:
-            a2=re.search(r'-[0-9]+\.[0-9]+',line)
-            energy.append(eval(a2.group(0)))
-        x1=re.search('OPTIMIZATION RUN DONE',line)
-        if x1:
-            s1=1
-        if s1==1:
-            in1=re.search('Forming right-hand sides of CP-SCF equations',line)
-            if in1:
-                s2=-1
-            in2=re.search('Solving the CP-SCF equations',line)
-            if in2:
-                s2=-2
-            in3=re.search('VIBRATIONAL FREQUENCIES',line)
-            if in3:
-                s2=-3
-        x2=re.search('ORCA TERMINATED NORMALLY',line)
-        if x2:
-            s2=1
-        t=re.search('GEOMETRY OPTIMIZATION CYCLE',line)
-        if t:
-            t2=re.search(r'[0-9]+',line)
-            term=t2.group(0)
-        c=re.search('-|Geometry convergence|-',line)
-        if c:
-            x=1
-        if x==2:
-            yes=re.search('YES',line)
-            no=re.search('NO',line)
-            if yes:
-                converge.append('YES')
-            if no:
-                converge.append('NO')
-            u=re.search('-------------------------',line)
-            if u:
-                x=0
-        if x==1:
-            u=re.search('-------------------------',line)
-            if u:
-                x=2
-        x3=re.search('aborting the run',line)
-        if x3:
-            s1=4
+    if MD==False:
+        for line in f:
+            a=re.search('FINAL SINGLE POINT ENERGY',line)
+            if a:
+                a2=re.search(r'-[0-9]+\.[0-9]+',line)
+                energy.append(eval(a2.group(0)))
+            x1=re.search('OPTIMIZATION RUN DONE',line)
+            if x1:
+                s1=1
+            if s1==1:
+                in1=re.search('Forming right-hand sides of CP-SCF equations',line)
+                if in1:
+                    s2=-1
+                in2=re.search('Solving the CP-SCF equations',line)
+                if in2:
+                    s2=-2
+                in3=re.search('VIBRATIONAL FREQUENCIES',line)
+                if in3:
+                    s2=-3
+            x2=re.search('ORCA TERMINATED NORMALLY',line)
+            if x2:
+                if s1!=6:
+                    s2=9
+                else:
+                    s2=0
+            t=re.search('GEOMETRY OPTIMIZATION CYCLE',line)
+            if t:
+                t2=re.search(r'[0-9]+',line)
+                term=t2.group(0)
+            c=re.search('-|Geometry convergence|-',line)
+            if c:
+                x=1
+            if x==2:
+                yes=re.search('YES',line)
+                no=re.search('NO',line)
+                if yes:
+                    converge.append('YES')
+                if no:
+                    converge.append('NO')
+                u=re.search('-------------------------',line)
+                if u:
+                    x=0
+            if x==1:
+                u=re.search('-------------------------',line)
+                if u:
+                    x=2
+            x3=re.search('aborting the run',line)
+            if x3:
+                s1=4
+            x3=re.search('ANGLE IS APPROACHING 180',line)
+            if x3:
+                s1=41
+                break
+            x4=re.search('did not converge but reached',line)
+            if x4:
+                s1=6
+    else:
+        s2=1
+        ii=0
+        gap=0
+        for line in f:
+            x0=re.search('Dump Position Stride [0-9]+',line)
+            if x0:
+                y0=re.search(r'[0-9]+',x0.group(0))
+                gap=eval(y0.group(0))
+            x1=re.findall('\-\|',line)
+            if len(x1)>3:
+                if ii==0:
+                    ii=1
+                else:
+                    break
+            elif ii==1:
+                alls=re.findall(r'\-*[0-9]+\.*[0-9]*',line)
+                if alls[0]=='0':
+                    energy.append(eval(alls[-1]))
+                else:
+                    if eval(alls[0])%gap==0:
+                        energy.append(eval(alls[-3]))
+    f.close()
     if statusonly==True:
         if s2==1:
-            f.close()
-            os.chdir(path)
             return 2
         else:
-            f.close()
-            os.chdir(path)
             return s1
-    if figureonly==False:
+    if figureonly==False and MD==False:
         print('{0} turns have been calculated.'.format(term))
         status_judge(s1,s2,converge)
         statusfig(energy,choose)
-    f.close()
+    elif figureonly==False and MD==True:
+        print('{0} turns have been calculated.'.format(len(energy)))
+        statusfig(energy,choose)
     os.chdir(path)
     return energy
 
 def thermo(loc, file, keyword):
-    path = os.getcwd()
-    os.chdir(loc)
     f=open(file+'.out','r')
     for line in f:
         if keyword=='Gibbs':
             a=re.search('Final Gibbs free energy', line)
             if a:
                 b=re.search(r'-[0-9]+\.[0-9]+', line)
-                os.chdir(path)
-                f.close()
                 return '{0:.6f}'.format(eval(b.group(0)))
         if keyword=='Enthalpy':
             a=re.search('Total enthalpy', line)
             if a:
                 b=re.search(r'-[0-9]+\.[0-9]+', line)
-                os.chdir(path)
-                f.close()
                 return '{0:.6f}'.format(eval(b.group(0)))
         if keyword=='Entropy':
             a=re.search('Total entropy correction', line)
             if a:
                 b=re.findall(r'-[0-9]+\.[0-9]+', line)
-                os.chdir(path)
-                f.close()
                 return '{0:.6f}'.format(eval(b[0]))
-    os.chdir(path)
-    f.close()
     raise Exception("'{0}.out' may not have keyword freq, or it's aborted. Please check your input file and recalculate it.".format(file))
 
 def charge(loc, file, num, keyword):
-    path = os.getcwd()
-    os.chdir(loc)
     f=open(file+'.out','r')
     i=0
     ac=[None]*200
     for line in f:
         if keyword=='Mulliken':
             d=re.search('Sum of atomic charges',line)
             if d:
@@ -226,20 +258,17 @@
                 b=re.search(r'-?[0-9]+\.[0-9]+', line)
                 if b:
                     n=re.findall(r'[0-9]+', line)
                     ac[eval(n[0])]=eval(b.group(0))
             d=re.search('LOEWDIN REDUCED ORBITAL CHARGES',line)
             if d:
                 i=0
-    os.chdir(path)
     return ac[num]
 
 def atoms_all(loc, file):
-    path = os.getcwd()
-    os.chdir(loc)
     f=open(file+'.out','r')
     i=0
     n=0
     atoms=[['NOT','99999','99999','99999']]*200
     elements=['NOT']*200
     xyzs=[['99999','99999','99999']]*200
     for line in f:
@@ -271,21 +300,17 @@
         try:
             atoms.remove(['NOT','99999','99999','99999'])
             elements.remove('NOT')
             xyzs.remove(['99999','99999','99999'])
         except:
             break
     f.close()
-    os.chdir(path)
     return atoms
 
-def atoms_all_xyz(loc, file,transfer=False):
-    path = os.getcwd()
-    if transfer==False:
-        os.chdir(loc)
+def atoms_all_xyz(loc, file):
     f=open(file+'.xyz','r')
     atoms=[['NOT','99999','99999','99999']]*200
     elements=['NOT']*200
     xyzs=[['99999','99999','99999']]*200
     i=0
     for line in f:
         b=re.findall(r'-?[0-9]+\.[0-9]+', line)
@@ -300,15 +325,14 @@
         try:
             atoms.remove(['NOT','99999','99999','99999'])
             elements.remove('NOT')
             xyzs.remove(['99999','99999','99999'])
         except:
             break
     f.close()
-    os.chdir(path)
     return atoms
 
 class status:
     """
     A method to see the current process of the ORCA optimisation, including convergence situation and relevant energy chart.
     status(file, loc='./')
     file: File Name.
@@ -457,15 +481,15 @@
     TIPS: In the following list, a piece of atom information is like that:
         ['C', 4.11199532065866, 1.93907233706568, -1.49149364116961]
         The first one is the element type, the following three numbers are location in x,y,z-axis.
         """
         try:
             return atoms_all(self.loc,self.file)
         except:
-            return atoms_all_xyz(self.loc,self.file,transfer=True)
+            return atoms_all_xyz(self.loc,self.file)
     
     def mass(self):
         """
     A method to find out the mass of all particles in system.
     mass()
         """
         M=0
@@ -538,34 +562,36 @@
                 M=M+192.22
             elif i[0]=='Pt':
                 M=M+195.08
             elif i[0]=='Au':
                 M=M+196.97
             elif i[0]=='Hg':
                 M=M+200.59
-        return eval('{0:.3f}'.format(M))
+        return M
     
     def atom_num(self):
         """
     A method to find out the atom number of the system.
     atom_num()
         """
         return len(atoms_all(self.loc,self.file))
     
-    def figure(self,num=0,width=300,height=300):
+    def figure(self,num=0,width=300,height=300,MD=False,save=''):
         """
     A method to see the current geometry structure of the ORCA optimisation, powered by py3Dmol and rdkit.
     TIPS: Make sure your _trj.xyz file is in the document with .out file, or there will be NoFileFoundError!!!
     
-    figure(num=0, width=300, height=300)
+    figure(num=0, width=300, height=300,MD=False,save='')
     num: The step of your convergence.
     width, height: The size of your 3D geometry molecule strcuture. Default: 300x300.
+    MD: See the single status of Molecular Dynamics (MD). The default is False.
+    save: The name of the single status XYZ file you want to save. The default is not saving the single status.
         """
             
-        figure=normalstatus(self.loc,self.file,figureonly=True)
+        figure=normalstatus(self.loc,self.file,figureonly=True,MD=MD)
         file=self.file
         try:
             path = os.getcwd()
             os.chdir(self.loc)
             multicreatemol(file, num, width, height)
             os.chdir(path)
         except:
@@ -591,14 +617,38 @@
                 multicreatemol(file, num, width, height)
                 os.chdir(path)
             except:
                 if num==len(figure)-1:
                     print("The last step hasn't been optimised yet.")
         interact(turn,num=iw.IntSlider(min=0,max=len(figure)-1,step=1,value=num))
     
+    def figuremd(self,num=0,width=300,height=300):
+        """
+    A method to see the current geometry structure and optimization trajectory of the ORCA Molecular Dynamics, powered by py3Dmol and ipywidgets package.
+    TIPS: Make sure your _dump.xyz file is in the document with .out file, or there will be FileNotFoundError!!!
+    
+    figuremd(num=0, width=300, height=300)
+    num: The step of your convergence. The default is the origin structure.
+    width, height: The size of your 3D geometry molecule strcuture. Default: 300x300.
+    After forming the 3D geometry molecule strcuture, you can scroll to see other structures of relevant molecules.
+        """
+            
+        figure=normalstatus(self.loc,self.file,figureonly=True,MD=True)
+        file=self.file
+        def turn(num):
+            try:
+                path = os.getcwd()
+                os.chdir(self.loc)
+                multicreatemol(file, num, width, height, MD=True)
+                os.chdir(path)
+            except:
+                if num==len(figure)-1:
+                    print("The last step hasn't been optimised yet.")
+        interact(turn,num=iw.IntSlider(min=0,max=len(figure),step=1,value=num))
+    
     def figurecharge(self,width=300,height=300):
         """
     A method to see the Mulliken Charge of each atom base on 3D geometry structure of the system.
     TIPS: Make sure your .xyz file is in the document with .out file, or there will be FileNotFoundError!!!
     
     width, height: The size of your 3D geometry molecule strcuture. Default: 300x300.
     After forming the 3D geometry molecule strcuture, you can scroll to see the charge of the relevant atom.
```

### Comparing `MCPoly-0.5.0/MCPoly/view3d/view3d.py` & `MCPoly-0.5.1/MCPoly/view3d/view3d.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/MCPoly/vis/vis.py` & `MCPoly-0.5.1/MCPoly/vis/vis.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 mydir = os.path.dirname( __file__ )
 orcadir = os.path.join(mydir, '..')#, 'orcaset')
 sys.path.append(orcadir)
 from orcaset.gui import gui as gui1
 from sscurve.gui import gui as gui2
 from moldraw.gui import gui as gui4
+from sscurve.gui2 import gui2 as gui5
 
 mydir = os.path.dirname( __file__ )
 orcadir = os.path.join(mydir, '..', 'orcaset')
 sys.path.append(orcadir)
 from ssgui import ssgui
 
 mydir = os.path.dirname( __file__ )
@@ -29,37 +30,40 @@
 #ssdir = os.path.join(mydir, '..', 'sscurve')
 #sys.path.append(ssdir)
 #from gui import gui as gui2
 
 def vis():
     """
         The method to summon all four GUI functions.
-        You can see how to use by input 'MCPoly.orcaset.gui?'(Normal ORCA), 'MCPoly.orcaset.ssgui?' (Mechanical ORCA), 'MCPoly.orcaset.mgui?' (Multiple ORCA), 'MCPoly.sscurve.gui?' (Stress-Strain Curve), 'MCPoly.status.gui?' (Energy Diagram) and 'MCPoly.moldraw.gui?' (Molecule Designer)..
+        You can see how to use by input 'MCPoly.orcaset.gui?'(Normal ORCA), 'MCPoly.orcaset.ssgui?' (Mechanical ORCA), 'MCPoly.orcaset.mgui?' (Multiple ORCA) and 'MCPoly.sscurve.gui?' (Stress-Strain Curve)
     """
     screen1=widgets.Output()
     screen2=widgets.Output()
     screen3=widgets.Output()
     screen4=widgets.Output()
     screen5=widgets.Output()
     screen6=widgets.Output()
+    screen7=widgets.Output()
     
     with screen1:
         gui1()
     with screen2:
         ssgui()
     with screen3:
         mgui()
     with screen4:
         gui2()
     with screen5:
-        gui3()
+        gui5()
     with screen6:
+        gui3()
+    with screen7:
         gui4()
     
-    tab_contents = ['Normal ORCA','Mechanical ORCA','Multiple ORCA','Stress-Strain Curve','Energy Diagram','Molecule Designer']
+    tab_contents = ['Normal ORCA','Mechanical ORCA','Multiple ORCA','Stress-Strain Curve','Distance Curve','Energy Diagram','Molecule Designer']
     tab = widgets.Tab(style=dict(font_weight='bold'))
     #children = [widgets.Label(name,style=dict(font_weight='bold')) for name in tab_contents]
-    children = [screen1,screen2,screen3,screen4,screen5,screen6]
+    children = [screen1,screen2,screen3,screen4,screen5,screen6,screen7]
     tab.children=children
     tab.titles = tab_contents
     tab.layout = widgets.Layout(layout=widgets.Layout(width='50%'))
     display(tab)
```

### Comparing `MCPoly-0.5.0/MCPoly.egg-info/PKG-INFO` & `MCPoly-0.5.1/MCPoly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.5.0
+Version: 0.5.1
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
```

### Comparing `MCPoly-0.5.0/MCPoly.egg-info/SOURCES.txt` & `MCPoly-0.5.1/MCPoly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/PKG-INFO` & `MCPoly-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.5.0
+Version: 0.5.1
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
```

### Comparing `MCPoly-0.5.0/README.md` & `MCPoly-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/setup.py` & `MCPoly-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='MCPoly',
-    version='0.5.0',
+    version='0.5.1',
     description='Useful tools for Computational Chemistry for polymers',
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=['MCPoly','MCPoly.lmpset','MCPoly.moldraw','MCPoly.orcaset','MCPoly.sscurve','MCPoly.status','MCPoly.view3d','MCPoly.version','MCPoly.vis'],
     author='Omicron Fluor',
     author_email='cxs454@student.bham.ac.uk',
```

### Comparing `MCPoly-0.5.0/tests/test_lmpset.py` & `MCPoly-0.5.1/tests/test_lmpset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/tests/test_moldraw.py` & `MCPoly-0.5.1/tests/test_moldraw.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/tests/test_orcaset.py` & `MCPoly-0.5.1/tests/test_orcaset.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,14 +70,51 @@
         if d2:
             i5=1
             break
     f.close()
     os.chdir(opath)
     assert i1*i2*i3*i4*i5!=0
 
+def test_XYZtoINP4():
+    opath=os.getcwd()
+    os.chdir('./MCPoly/tests')
+    file='Atoms1'
+    loc='./data_orcaset/'
+    XYZtoINP(file,fileloc=loc,saveloc=loc,method='B3LYP D3BJ',basis_set='def2-TZVP',MD=True,\
+                     MD=True,freq=True,md_timestep=1.0,initvel=350,tsNHC=350,dumpcon=25,runstep=2500,maxcore=4096,corenum=8)
+    i1=0
+    i2=0
+    i3=0
+    i4=0
+    i5=0
+    i6=0
+    f=open(loc+file+'.inp','r')
+    for line in f:
+        a=re.search(r'MD B3LYP def2-TZVP',line)
+        if a:
+            i1=1
+        b=re.search(r'maxcore 4096',line)
+        if b:
+            i2=1
+        c=re.search('%PAL NPROCS 8 END',line)
+        if c:
+            i3=1
+        d1=re.search(r'Timestep 1.0_fs',line)
+        if d1:
+            i4=1
+        d2=re.search('Dump Position Stride 25 Filename "Atoms1_dump.xyz"',line)
+        if d2:
+            i5=1
+        d3=re.search('Run 2500',line)
+        if d3:
+            i6=1
+    f.close()
+    os.chdir(opath)
+    assert i1*i2*i3*i4*i5*i6!=0
+
 def test_XYZtoINP1():
     opath=os.getcwd()
     os.chdir('./MCPoly/tests')
     file='Atoms1'
     loc='./data_orcaset/'
     XYZtoINP(file,fileloc=loc,saveloc=loc)
     i=0
```

### Comparing `MCPoly-0.5.0/tests/test_sscurve.py` & `MCPoly-0.5.1/tests/test_sscurve.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.0/tests/test_status.py` & `MCPoly-0.5.1/tests/test_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,9 +202,8 @@
     assert num==14
 
 def test_status_mass(current1):
     opath=os.getcwd()
     os.chdir('./MCPoly/tests')
     num=current1.mass()
     os.chdir(opath)
-    assert num==238.024
-    
+    assert num==238.024
```

