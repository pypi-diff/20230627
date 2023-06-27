# Comparing `tmp/robologs_ros_utils-0.1.1a26.tar.gz` & `tmp/robologs_ros_utils-0.1.1a27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robologs_ros_utils-0.1.1a26.tar", max compression
+gzip compressed data, was "robologs_ros_utils-0.1.1a27.tar", max compression
```

## Comparing `robologs_ros_utils-0.1.1a26.tar` & `robologs_ros_utils-0.1.1a27.tar`

### file list

```diff
@@ -1,48 +1,26 @@
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a26/README.md
--rw-r--r--   0        0        0     1608 2023-06-26 15:49:41.390848 robologs_ros_utils-0.1.1a26/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/__initi__.py
--rw-r--r--   0        0        0      948 2023-06-26 15:49:22.442716 robologs_ros_utils-0.1.1a26/robologs_ros_utils/cli.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/connectors/__init__.py
--rw-r--r--   0        0        0      154 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/connectors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      417 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/connectors/__pycache__/commands.cpython-38.pyc
--rw-r--r--   0        0        0      750 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/connectors/__pycache__/s3_upload.cpython-38.pyc
--rw-r--r--   0        0        0      766 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/connectors/classes.py
--rw-r--r--   0        0        0      184 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/connectors/commands.py
--rw-r--r--   0        0        0       61 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/connectors/rosbag_to_s3.py
--rw-r--r--   0        0        0      583 2023-06-26 13:26:47.560525 robologs_ros_utils-0.1.1a26/robologs_ros_utils/connectors/s3_upload.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/aws/athena/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/aws/dynamodb/__init__.py
--rw-r--r--   0        0        0     7186 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/aws/dynamodb/dynamodb_utils.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/aws/lambdas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/aws/s3/__init__.py
--rw-r--r--   0        0        0      163 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/aws/s3/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1467 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/aws/s3/__pycache__/s3_utils.cpython-38.pyc
--rw-r--r--   0        0        0     1228 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/aws/s3/s3_utils.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/azure/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/destinations/google_cloud/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.786728 robologs_ros_utils-0.1.1a26/robologs_ros_utils/functions/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/__init__.py
--rw-r--r--   0        0        0      171 2023-06-26 14:13:16.767932 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/__init__.py
--rw-r--r--   0        0        0      176 2023-06-26 14:13:16.767932 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2595 2023-06-26 14:13:17.695938 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/__pycache__/ros_img_tools.cpython-38.pyc
--rw-r--r--   0        0        0    11444 2023-06-26 14:13:16.771932 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/__pycache__/ros_utils.cpython-38.pyc
--rw-r--r--   0        0        0      523 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/argument_parsers.py
--rw-r--r--   0        0        0     2589 2023-06-26 13:24:22.807675 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/clip_rosbag.py
--rw-r--r--   0        0        0      399 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/commands.py
--rw-r--r--   0        0        0     2709 2023-06-26 13:24:22.803675 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/get_images_from_bag.py
--rw-r--r--   0        0        0     1063 2023-06-26 13:24:22.811675 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/get_summary_from_bag.py
--rw-r--r--   0        0        0     3040 2023-06-26 13:24:22.811675 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/get_videos_from_bag.py
--rw-r--r--   0        0        0     2669 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/ros_img_tools.py
--rw-r--r--   0        0        0    15662 2023-06-26 13:23:43.759458 robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/ros_utils.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/file_utils/__init__.py
--rw-r--r--   0        0        0      180 2023-06-26 14:13:17.695938 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/file_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5223 2023-06-26 14:13:17.695938 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/file_utils/__pycache__/file_utils.cpython-38.pyc
--rw-r--r--   0        0        0     4615 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/file_utils/file_utils.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/img_utils/__init__.py
--rw-r--r--   0        0        0      179 2023-06-26 14:13:17.695938 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/img_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1386 2023-06-26 14:13:17.695938 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/img_utils/__pycache__/img_utils.cpython-38.pyc
--rw-r--r--   0        0        0     1147 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/img_utils/img_utils.py
--rw-r--r--   0        0        0        0 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/video_utils/__init__.py
--rw-r--r--   0        0        0     1766 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a26/setup.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a26/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a27/README.md
+-rw-r--r--   0        0        0     1608 2023-06-27 14:28:19.042780 robologs_ros_utils-0.1.1a27/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.586726 robologs_ros_utils-0.1.1a27/robologs_ros_utils/__init__.py
+-rw-r--r--   0        0        0      949 2023-06-27 08:15:43.054590 robologs_ros_utils-0.1.1a27/robologs_ros_utils/cli.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/__init__.py
+-rw-r--r--   0        0        0      171 2023-06-26 14:13:16.767932 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/__init__.py
+-rw-r--r--   0        0        0      176 2023-06-26 14:13:16.767932 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2595 2023-06-26 14:13:17.695938 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/__pycache__/ros_img_tools.cpython-38.pyc
+-rw-r--r--   0        0        0    11396 2023-06-27 13:51:54.362193 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/__pycache__/ros_utils.cpython-38.pyc
+-rw-r--r--   0        0        0      523 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/argument_parsers.py
+-rw-r--r--   0        0        0     2578 2023-06-27 11:55:49.889627 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/clip_rosbag.py
+-rw-r--r--   0        0        0      399 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/commands.py
+-rw-r--r--   0        0        0     2698 2023-06-27 11:55:58.437675 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/get_images_from_bag.py
+-rw-r--r--   0        0        0     1052 2023-06-27 11:55:36.549553 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/get_summary_from_bag.py
+-rw-r--r--   0        0        0     3029 2023-06-27 11:56:05.773716 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/get_videos_from_bag.py
+-rw-r--r--   0        0        0     2669 2023-06-26 13:09:39.590726 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/ros_img_tools.py
+-rw-r--r--   0        0        0    15655 2023-06-27 13:51:44.266140 robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/ros_utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:36:54.527450 robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-27 11:37:14.987556 robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5212 2023-06-27 11:59:04.658716 robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/__pycache__/file_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     1376 2023-06-27 11:59:04.774716 robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/__pycache__/img_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     4615 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/file_utils.py
+-rw-r--r--   0        0        0     1147 2023-06-26 13:09:39.682727 robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/img_utils.py
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a27/setup.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 robologs_ros_utils-0.1.1a27/PKG-INFO
```

### Comparing `robologs_ros_utils-0.1.1a26/pyproject.toml` & `robologs_ros_utils-0.1.1a27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robologs-ros-utils"
-version = "0.1.1a26"
+version = "0.1.1a27"
 description = "robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities"
 authors = ["roboto.ai <info@roboto.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.2"
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/cli.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from inspect import getmembers
 
 import click
 
 from robologs_ros_utils.connectors.commands import connectors
 from robologs_ros_utils.sources.ros1.commands import ros
 
+
 @click.group(invoke_without_command=True)
 @click.pass_context
 def cli(ctx):
     if ctx.invoked_subcommand is None:
         click.echo(
             """
                __          __
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/__pycache__/ros_img_tools.cpython-38.pyc` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/__pycache__/ros_img_tools.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/__pycache__/ros_utils.cpython-38.pyc` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/__pycache__/ros_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 13:23:43 2023 UTC, .py size: 15662 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-00000000: 550d 0d0a 0000 0000 5f91 9964 2e3d 0000  U......._..d.=..
+00000000: 550d 0d0a 0000 0000 70e9 9a64 273d 0000  U.......p..d'=..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 4002 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6402 6c08 5a08 6401 6402 6c09 5a0a 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0b 6d0c 5a0c 0100 6401 6405 6c0d  d.l.m.Z...d.d.l.
 00000080: 6d0e 5a0e 0100 6401 6406 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
 00000090: 0100 6401 6407 6c11 6d12 5a12 0100 6401  ..d.d.l.m.Z...d.
 000000a0: 6408 6c13 6d14 5a14 6d15 5a15 0100 6401  d.l.m.Z.m.Z...d.
 000000b0: 6409 6c16 6d16 5a16 0100 6401 640a 6c17  d.l.m.Z...d.d.l.
 000000c0: 6d18 5a18 0100 6401 640b 6c19 6d1a 5a1a  m.Z...d.d.l.m.Z.
-000000d0: 0100 6401 640c 6c1b 6d1c 5a1c 0100 651d  ..d.d.l.m.Z...e.
-000000e0: 651e 640d 9c02 640e 640f 8404 5a1f 651e  e.d...d.d...Z.e.
-000000f0: 651e 6410 9c02 6411 6412 8404 5a20 651d  e.d...d.d...Z e.
-00000100: 651e 6413 9c02 6414 6415 8404 5a21 6522  e.d...d.d...Z!e"
-00000110: 6522 651d 6522 651e 6416 9c05 6417 6418  e"e.e"e.d...d.d.
-00000120: 8404 5a23 6419 641a 8400 5a24 6525 6525  ..Z#d.d...Z$e%e%
-00000130: 6525 641b 9c03 641c 641d 8404 5a26 6445  e%d...d.d...Z&dE
-00000140: 6522 651d 651d 641f 9c03 6420 6421 8405  e"e.e.d...d d!..
-00000150: 5a27 6446 6522 651d 6522 651d 6423 9c04  Z'dFe"e.e"e.d#..
-00000160: 6424 6425 8405 5a28 6447 651d 651d 651d  d$d%..Z(dGe.e.e.
-00000170: 6427 9c03 6428 6429 8405 5a29 6505 652a  d'..d(d)..Z)e.e*
-00000180: 1900 6505 652a 1900 652a 652a 642a 9c04  ..e.e*..e*e*d*..
-00000190: 642b 642c 8404 5a2b 652a 652a 652a 652c  d+d,..Z+e*e*e*e,
-000001a0: 642d 9c04 642e 642f 8404 5a2d 6430 6431  d-..d.d/..Z-d0d1
-000001b0: 8400 5a2e 6448 651d 652c 6402 6433 9c03  ..Z.dHe.e,d.d3..
-000001c0: 6434 6435 8405 5a2f 6449 651d 651d 651d  d4d5..Z/dIe.e.e.
-000001d0: 6505 6525 1900 652c 651d 6505 6525 1900  e.e%..e,e.e.e%..
-000001e0: 6505 6522 1900 6505 652a 1900 6505 652a  e.e"..e.e*..e.e*
-000001f0: 1900 6438 9c0a 6439 643a 8405 5a30 6522  ..d8..d9d:..Z0e"
-00000200: 6522 643b 9c02 643c 643d 8404 5a31 644a  e"d;..d<d=..Z1dJ
-00000210: 6522 6505 6522 1900 6505 6522 1900 6507  e"e.e"..e.e"..e.
-00000220: 652c 652c 6602 1900 643e 9c04 643f 6440  e,e,f...d>..d?d@
-00000230: 8405 5a32 644b 651d 651d 6505 6525 1900  ..Z2dKe.e.e.e%..
-00000240: 6505 6506 652a 6522 6602 1900 1900 6505  e.e.e*e"f.....e.
-00000250: 6506 652a 6522 6602 1900 1900 651d 6442  e.e*e"f.....e.dB
-00000260: 9c06 6443 6444 8405 5a33 6402 5300 294c  ..dCdD..Z3d.S.)L
+000000d0: 0100 6401 640c 6c19 6d1b 5a1b 0100 651c  ..d.d.l.m.Z...e.
+000000e0: 651d 640d 9c02 640e 640f 8404 5a1e 651d  e.d...d.d...Z.e.
+000000f0: 651d 6410 9c02 6411 6412 8404 5a1f 651c  e.d...d.d...Z.e.
+00000100: 651d 6413 9c02 6414 6415 8404 5a20 6521  e.d...d.d...Z e!
+00000110: 6521 651c 6521 651d 6416 9c05 6417 6418  e!e.e!e.d...d.d.
+00000120: 8404 5a22 6419 641a 8400 5a23 6524 6524  ..Z"d.d...Z#e$e$
+00000130: 6524 641b 9c03 641c 641d 8404 5a25 6444  e$d...d.d...Z%dD
+00000140: 6521 651c 651c 641f 9c03 6420 6421 8405  e!e.e.d...d d!..
+00000150: 5a26 6445 6521 651c 6521 651c 6423 9c04  Z&dEe!e.e!e.d#..
+00000160: 6424 6425 8405 5a27 6446 651c 651c 651c  d$d%..Z'dFe.e.e.
+00000170: 6427 9c03 6428 6429 8405 5a28 6505 6529  d'..d(d)..Z(e.e)
+00000180: 1900 6505 6529 1900 6529 6529 642a 9c04  ..e.e)..e)e)d*..
+00000190: 642b 642c 8404 5a2a 6529 6529 6529 652b  d+d,..Z*e)e)e)e+
+000001a0: 642d 9c04 642e 642f 8404 5a2c 6430 6431  d-..d.d/..Z,d0d1
+000001b0: 8400 5a2d 6447 651c 652b 6402 6433 9c03  ..Z-dGe.e+d.d3..
+000001c0: 6434 6435 8405 5a2e 6448 651c 651c 651c  d4d5..Z.dHe.e.e.
+000001d0: 6505 6524 1900 652b 651c 6505 6524 1900  e.e$..e+e.e.e$..
+000001e0: 6505 6521 1900 6505 6529 1900 6505 6529  e.e!..e.e)..e.e)
+000001f0: 1900 6437 9c0a 6438 6439 8405 5a2f 6521  ..d7..d8d9..Z/e!
+00000200: 6521 643a 9c02 643b 643c 8404 5a30 6449  e!d:..d;d<..Z0dI
+00000210: 6521 6505 6521 1900 6505 6521 1900 6507  e!e.e!..e.e!..e.
+00000220: 652b 652b 6602 1900 643d 9c04 643e 643f  e+e+f...d=..d>d?
+00000230: 8405 5a31 644a 651c 651c 6505 6524 1900  ..Z1dJe.e.e.e$..
+00000240: 6505 6506 6529 6521 6602 1900 1900 6505  e.e.e)e!f.....e.
+00000250: 6506 6529 6521 6602 1900 1900 651c 6441  e.e)e!f.....e.dA
+00000260: 9c06 6442 6443 8405 5a32 6402 5300 294b  ..dBdC..Z2d.S.)K
 00000270: 7a50 526f 7362 6167 2075 7469 6c69 7469  zPRosbag utiliti
 00000280: 6573 0a0a 5468 6973 206d 6f64 756c 6520  es..This module 
 00000290: 636f 6e74 6169 6e73 2066 756e 6374 696f  contains functio
 000002a0: 6e73 2074 6f20 6578 7472 6163 7420 6461  ns to extract da
 000002b0: 7461 2066 726f 6d20 726f 7362 6167 732e  ta from rosbags.
 000002c0: 0a0a e900 0000 004e 2903 da08 4f70 7469  .......N)...Opti
 000002d0: 6f6e 616c da05 556e 696f 6eda 0554 7570  onal..Union..Tup
@@ -83,42 +83,42 @@
 00000520: 7469 6d65 da08 6475 7261 7469 6f6e 6900  time..durationi.
 00000530: 0010 005a 0c66 696c 655f 7369 7a65 5f6d  ...Z.file_size_m
 00000540: 62da 0772 6563 6f72 6473 da06 746f 7069  b..records..topi
 00000550: 6373 290d da02 6f73 da04 7061 7468 da06  cs)...os..path..
 00000560: 6578 6973 7473 da09 4578 6365 7074 696f  exists..Exceptio
 00000570: 6eda 0865 6e64 7377 6974 6872 0500 0000  n..endswithr....
 00000580: da04 6469 6374 da04 7374 6174 7212 0000  ..dict..statr...
-00000590: 0072 1300 0000 da07 7374 5f73 697a 655a  .r......st_sizeZ
-000005a0: 0b74 6f70 6963 5f74 6162 6c65 5a07 746f  .topic_tableZ.to
-000005b0: 5f64 6963 7429 0472 0f00 0000 5a03 6261  _dict).r....Z.ba
-000005c0: 675a 0a66 696c 655f 7374 6174 73da 0c73  gZ.file_stats..s
-000005d0: 756d 6d61 7279 5f64 6963 74a9 0072 2000  ummary_dict..r .
+00000590: 0072 1300 0000 da07 7374 5f73 697a 65da  .r......st_size.
+000005a0: 0b74 6f70 6963 5f74 6162 6c65 da07 746f  .topic_table..to
+000005b0: 5f64 6963 7429 0472 0f00 0000 da03 6261  _dict).r......ba
+000005c0: 67da 0a66 696c 655f 7374 6174 735a 0c73  g..file_statsZ.s
+000005d0: 756d 6d61 7279 5f64 6963 74a9 0072 2300  ummary_dict..r#.
 000005e0: 0000 fa56 2f68 6f6d 652f 7976 6573 2f43  ...V/home/yves/C
 000005f0: 6f64 652f 726f 626f 6c6f 6773 2d72 6f73  ode/robologs-ros
 00000600: 2d75 7469 6c73 2f70 7974 686f 6e2f 726f  -utils/python/ro
 00000610: 626f 6c6f 6773 5f72 6f73 5f75 7469 6c73  bologs_ros_utils
 00000620: 2f73 6f75 7263 6573 2f72 6f73 312f 726f  /sources/ros1/ro
 00000630: 735f 7574 696c 732e 7079 da16 6765 745f  s_utils.py..get_
 00000640: 6261 675f 696e 666f 5f66 726f 6d5f 6669  bag_info_from_fi
 00000650: 6c65 1900 0000 7322 0000 0000 0a0c 010e  le....s"........
 00000660: 020a 010e 0202 010c 0206 0104 010c 020a  ................
-00000670: 0206 010a 010a 0110 010e 0110 0272 2200  .............r".
+00000670: 0206 010a 010a 0110 010e 0110 0272 2500  .............r%.
 00000680: 0000 2902 da14 726f 7362 6167 5f6d 6574  ..)...rosbag_met
 00000690: 6164 6174 615f 6469 6374 7210 0000 0063  adata_dictr....c
 000006a0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
 000006b0: 0500 0000 4300 0000 732c 0000 0074 0083  ....C...s,...t..
 000006c0: 007d 0164 017c 006b 0672 287c 0064 0119  .}.d.|.k.r(|.d..
 000006d0: 0044 005d 107d 027c 027c 017c 0264 0219  .D.].}.|.|.|.d..
 000006e0: 003c 0071 167c 0153 0029 034e 7216 0000  .<.q.|.S.).Nr...
 000006f0: 00da 0654 6f70 6963 7329 0172 1c00 0000  ...Topics).r....
-00000700: 2903 7223 0000 00da 0a74 6f70 6963 5f64  ).r#.....topic_d
-00000710: 6963 74da 0565 6e74 7279 7220 0000 0072  ict..entryr ...r
-00000720: 2000 0000 7221 0000 00da 0e67 6574 5f74   ...r!.....get_t
+00000700: 2903 7226 0000 00da 0a74 6f70 6963 5f64  ).r&.....topic_d
+00000710: 6963 74da 0565 6e74 7279 7223 0000 0072  ict..entryr#...r
+00000720: 2300 0000 7224 0000 00da 0e67 6574 5f74  #...r$.....get_t
 00000730: 6f70 6963 5f64 6963 743c 0000 0073 0a00  opic_dict<...s..
-00000740: 0000 0001 0602 0801 0c01 0e02 7227 0000  ............r'..
+00000740: 0000 0001 0602 0801 0c01 0e02 722a 0000  ............r*..
 00000750: 0029 02da 0a69 6e70 7574 5f70 6174 6872  .)...input_pathr
 00000760: 1000 0000 6301 0000 0000 0000 0000 0000  ....c...........
 00000770: 0003 0000 0007 0000 0043 0000 0073 5c00  .........C...s\.
 00000780: 0000 7400 8300 7d01 7c00 a001 6401 a101  ..t...}.|...d...
 00000790: 7226 7402 7c00 8301 7c01 7403 6a04 a005  r&t.|...|.t.j...
 000007a0: 7c00 a101 3c00 6e32 7406 7407 a007 7403  |...<.n2t.t...t.
 000007b0: 6a04 a008 7c00 6402 a102 a101 8301 4400  j...|.d.......D.
@@ -136,24 +136,24 @@
 00000870: 2072 6f73 6261 6720 6d65 7461 6461 7461   rosbag metadata
 00000880: 2066 6f72 2065 6163 6820 726f 7362 6167   for each rosbag
 00000890: 2e20 5468 6520 6b65 7920 6f66 2074 6865  . The key of the
 000008a0: 2064 6963 7469 6f6e 6172 7920 6973 2074   dictionary is t
 000008b0: 6865 2072 6f73 6261 6720 6669 6c65 2070  he rosbag file p
 000008c0: 6174 682e 0a0a 2020 2020 7211 0000 007a  ath...    r....z
 000008d0: 072e 2f2a 2e62 6167 2909 721c 0000 0072  ../*.bag).r....r
-000008e0: 1b00 0000 7222 0000 0072 1700 0000 7218  ....r"...r....r.
+000008e0: 1b00 0000 7225 0000 0072 1700 0000 7218  ....r%...r....r.
 000008f0: 0000 00da 0761 6273 7061 7468 da06 736f  .....abspath..so
 00000900: 7274 6564 da04 676c 6f62 da04 6a6f 696e  rted..glob..join
-00000910: 2903 7228 0000 005a 1072 6f73 6261 675f  ).r(...Z.rosbag_
+00000910: 2903 722b 0000 005a 1072 6f73 6261 675f  ).r+...Z.rosbag_
 00000920: 696e 666f 5f64 6963 74da 0866 696c 656e  info_dict..filen
-00000930: 616d 6572 2000 0000 7220 0000 0072 2100  amer ...r ...r!.
+00000930: 616d 6572 2300 0000 7223 0000 0072 2400  amer#...r#...r$.
 00000940: 0000 da20 6765 745f 6261 675f 696e 666f  ... get_bag_info
 00000950: 5f66 726f 6d5f 6669 6c65 5f6f 725f 666f  _from_file_or_fo
 00000960: 6c64 6572 4600 0000 730c 0000 0000 0a06  lderF...s.......
-00000970: 020a 0116 021c 0116 0272 2e00 0000 2905  .........r....).
+00000970: 020a 0116 021c 0116 0272 3100 0000 2905  .........r1...).
 00000980: da0d 6d73 675f 7469 6d65 7374 616d 70da  ..msg_timestamp.
 00000990: 1072 6f73 6261 675f 7469 6d65 7374 616d  .rosbag_timestam
 000009a0: 70da 0966 696c 655f 7061 7468 da05 696e  p..file_path..in
 000009b0: 6465 7872 1000 0000 6304 0000 0000 0000  dexr....c.......
 000009c0: 0000 0000 0006 0000 0006 0000 0043 0000  .............C..
 000009d0: 0073 2000 0000 7400 6a01 a002 7c02 a101  .s ...t.j...|...
 000009e0: 5c02 7d04 7d05 7c00 7c01 7c02 7c03 7c05  \.}.}.|.|.|.|.|.
@@ -162,35 +162,35 @@
 00000a10: 5f74 696d 6573 7461 6d70 2028 696e 7429  _timestamp (int)
 00000a20: 3a0a 2020 2020 2020 2020 726f 7362 6167  :.        rosbag
 00000a30: 5f74 696d 6573 7461 6d70 2028 696e 7429  _timestamp (int)
 00000a40: 3a0a 2020 2020 2020 2020 6669 6c65 5f70  :.        file_p
 00000a50: 6174 6820 2873 7472 293a 0a20 2020 2020  ath (str):.     
 00000a60: 2020 2069 6e64 6578 2028 696e 7429 3a0a     index (int):.
 00000a70: 0a20 2020 2052 6574 7572 6e73 3a20 6469  .    Returns: di
-00000a80: 6374 0a0a 2020 2020 2905 722f 0000 0072  ct..    ).r/...r
-00000a90: 3000 0000 7218 0000 005a 096d 7367 5f69  0...r....Z.msg_i
+00000a80: 6374 0a0a 2020 2020 2905 7232 0000 0072  ct..    ).r2...r
+00000a90: 3300 0000 7218 0000 005a 096d 7367 5f69  3...r....Z.msg_i
 00000aa0: 6e64 6578 da08 696d 675f 6e61 6d65 2903  ndex..img_name).
 00000ab0: 7217 0000 0072 1800 0000 da05 7370 6c69  r....r......spli
-00000ac0: 7429 0672 2f00 0000 7230 0000 0072 3100  t).r/...r0...r1.
-00000ad0: 0000 7232 0000 00da 015f 7233 0000 0072  ..r2....._r3...r
-00000ae0: 2000 0000 7220 0000 0072 2100 0000 da1a   ...r ...r!.....
+00000ac0: 7429 0672 3200 0000 7233 0000 0072 3400  t).r2...r3...r4.
+00000ad0: 0000 7235 0000 00da 015f 7236 0000 0072  ..r5....._r6...r
+00000ae0: 2300 0000 7223 0000 0072 2400 0000 da1a  #...r#...r$.....
 00000af0: 6372 6561 7465 5f6d 616e 6966 6573 745f  create_manifest_
 00000b00: 656e 7472 795f 6469 6374 5b00 0000 730e  entry_dict[...s.
 00000b10: 0000 0000 0b10 0202 0102 0102 0102 0102  ................
-00000b20: fb72 3600 0000 6300 0000 0000 0000 0000  .r6...c.........
+00000b20: fb72 3900 0000 6300 0000 0000 0000 0000  .r9...c.........
 00000b30: 0000 0000 0000 0002 0000 0043 0000 0073  ...........C...s
 00000b40: 0800 0000 6401 6402 6702 5300 2903 fa13  ....d.d.g.S.)...
 00000b50: 0a20 2020 2052 6574 7572 6e73 3a0a 0a20  .    Returns:.. 
 00000b60: 2020 207a 1b73 656e 736f 725f 6d73 6773     z.sensor_msgs
 00000b70: 2f43 6f6d 7072 6573 7365 6449 6d61 6765  /CompressedImage
 00000b80: 7a11 7365 6e73 6f72 5f6d 7367 732f 496d  z.sensor_msgs/Im
-00000b90: 6167 6572 2000 0000 7220 0000 0072 2000  ager ...r ...r .
-00000ba0: 0000 7220 0000 0072 2100 0000 da15 6765  ..r ...r!.....ge
+00000b90: 6167 6572 2300 0000 7223 0000 0072 2300  ager#...r#...r#.
+00000ba0: 0000 7223 0000 0072 2400 0000 da15 6765  ..r#...r$.....ge
 00000bb0: 745f 696d 6167 655f 746f 7069 635f 7479  t_image_topic_ty
-00000bc0: 7065 7370 0000 0073 0200 0000 0005 7238  pesp...s......r8
+00000bc0: 7065 7370 0000 0073 0200 0000 0005 723b  pesp...s......r;
 00000bd0: 0000 0029 03da 0a61 6c6c 5f74 6f70 6963  ...)...all_topic
 00000be0: 73da 1266 696c 7465 725f 746f 7069 635f  s..filter_topic_
 00000bf0: 7479 7065 7372 1000 0000 6302 0000 0000  typesr....c.....
 00000c00: 0000 0000 0000 0002 0000 0003 0000 0003  ................
 00000c10: 0000 0073 1200 0000 8700 6601 6401 6402  ...s......f.d.d.
 00000c20: 8408 7c00 4400 8301 5300 2903 7a5c 0a20  ..|.D...S.).z\. 
 00000c30: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
@@ -198,78 +198,78 @@
 00000c50: 7429 3a0a 2020 2020 2020 2020 6669 6c74  t):.        filt
 00000c60: 6572 5f74 6f70 6963 5f74 7970 6573 2028  er_topic_types (
 00000c70: 6c69 7374 293a 0a0a 2020 2020 5265 7475  list):..    Retu
 00000c80: 726e 733a 0a0a 2020 2020 6301 0000 0000  rns:..    c.....
 00000c90: 0000 0000 0000 0002 0000 0004 0000 0013  ................
 00000ca0: 0000 0073 2000 0000 6700 7c00 5d18 7d01  ...s ...g.|.].}.
 00000cb0: 7c01 6400 1900 8800 6b06 7204 7c01 6401  |.d.....k.r.|.d.
-00000cc0: 1900 9102 7104 5300 2902 5a05 5479 7065  ....q.S.).Z.Type
-00000cd0: 7372 2400 0000 7220 0000 00a9 02da 022e  sr$...r ........
-00000ce0: 30da 0178 a901 723a 0000 0072 2000 0000  0..x..r:...r ...
-00000cf0: 7221 0000 00da 0a3c 6c69 7374 636f 6d70  r!.....<listcomp
+00000cc0: 1900 9102 7104 5300 2902 da05 5479 7065  ....q.S.)...Type
+00000cd0: 7372 2700 0000 7223 0000 00a9 02da 022e  sr'...r#........
+00000ce0: 30da 0178 a901 723d 0000 0072 2300 0000  0..x..r=...r#...
+00000cf0: 7224 0000 00da 0a3c 6c69 7374 636f 6d70  r$.....<listcomp
 00000d00: 3e81 0000 0073 0600 0000 0600 0200 0c00  >....s..........
 00000d10: 7a2b 6765 745f 746f 7069 635f 6e61 6d65  z+get_topic_name
 00000d20: 735f 6f66 5f74 7970 652e 3c6c 6f63 616c  s_of_type.<local
-00000d30: 733e 2e3c 6c69 7374 636f 6d70 3e72 2000  s>.<listcomp>r .
-00000d40: 0000 a902 7239 0000 0072 3a00 0000 7220  ....r9...r:...r 
-00000d50: 0000 0072 3e00 0000 7221 0000 00da 1767  ...r>...r!.....g
+00000d30: 733e 2e3c 6c69 7374 636f 6d70 3e72 2300  s>.<listcomp>r#.
+00000d40: 0000 a902 723c 0000 0072 3d00 0000 7223  ....r<...r=...r#
+00000d50: 0000 0072 4200 0000 7224 0000 00da 1767  ...rB...r$.....g
 00000d60: 6574 5f74 6f70 6963 5f6e 616d 6573 5f6f  et_topic_names_o
 00000d70: 665f 7479 7065 7800 0000 7302 0000 0000  f_typex...s.....
-00000d80: 0972 4100 0000 da03 6a70 6729 03da 0974  .rA.....jpg)...t
+00000d80: 0972 4500 0000 da03 6a70 6729 03da 0974  .rE.....jpg)...t
 00000d90: 696d 6573 7461 6d70 da0b 6669 6c65 5f66  imestamp..file_f
 00000da0: 6f72 6d61 7472 1000 0000 6302 0000 0000  ormatr....c.....
 00000db0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
 00000dc0: 0000 0073 1600 0000 7400 7c00 8301 9b00  ...s....t.|.....
 00000dd0: 6401 7c01 9b00 9d03 7d02 7c02 5300 2902  d.|.....}.|.S.).
 00000de0: 7a52 0a20 2020 2041 7267 733a 0a20 2020  zR.    Args:.   
 00000df0: 2020 2020 2074 696d 6573 7461 6d70 2028       timestamp (
 00000e00: 696e 7429 3a0a 2020 2020 2020 2020 6669  int):.        fi
 00000e10: 6c65 5f66 6f72 6d61 7420 2873 7472 293a  le_format (str):
 00000e20: 0a0a 2020 2020 5265 7475 726e 733a 0a0a  ..    Returns:..
 00000e30: 2020 2020 da01 2e29 01da 0373 7472 2903      ...)...str).
-00000e40: 7243 0000 0072 4400 0000 7233 0000 0072  rC...rD...r3...r
-00000e50: 2000 0000 7220 0000 0072 2100 0000 da1d   ...r ...r!.....
+00000e40: 7247 0000 0072 4800 0000 7236 0000 0072  rG...rH...r6...r
+00000e50: 2300 0000 7223 0000 0072 2400 0000 da1d  #...r#...r$.....
 00000e60: 6765 745f 696d 6167 655f 6e61 6d65 5f66  get_image_name_f
 00000e70: 726f 6d5f 7469 6d65 7374 616d 7084 0000  rom_timestamp...
-00000e80: 0073 0400 0000 0009 1201 7247 0000 00e9  .s........rG....
-00000e90: 0600 0000 2904 7232 0000 0072 4400 0000  ....).r2...rD...
+00000e80: 0073 0400 0000 0009 1201 724b 0000 00e9  .s........rK....
+00000e90: 0600 0000 2904 7235 0000 0072 4800 0000  ....).r5...rH...
 00000ea0: da0c 7a65 726f 5f70 6164 6469 6e67 7210  ..zero_paddingr.
 00000eb0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
 00000ec0: 0400 0000 0300 0000 4300 0000 731c 0000  ........C...s...
 00000ed0: 0074 007c 0083 01a0 017c 02a1 019b 0064  .t.|.....|.....d
 00000ee0: 017c 019b 009d 037d 037c 0353 0029 027a  .|.....}.|.S.).z
 00000ef0: 610a 2020 2020 4172 6773 3a0a 2020 2020  a.    Args:.    
 00000f00: 2020 2020 696e 6465 7820 2829 3a0a 2020      index ():.  
 00000f10: 2020 2020 2020 6669 6c65 5f66 6f72 6d61        file_forma
 00000f20: 7420 2829 3a0a 2020 2020 2020 2020 7a65  t ():.        ze
 00000f30: 726f 5f70 6164 6469 6e67 2028 293a 0a0a  ro_padding ():..
 00000f40: 2020 2020 5265 7475 726e 733a 0a0a 2020      Returns:..  
-00000f50: 2020 7245 0000 0029 0272 4600 0000 da05    rE...).rF.....
-00000f60: 7a66 696c 6c29 0472 3200 0000 7244 0000  zfill).r2...rD..
-00000f70: 0072 4900 0000 7233 0000 0072 2000 0000  .rI...r3...r ...
-00000f80: 7220 0000 0072 2100 0000 da19 6765 745f  r ...r!.....get_
+00000f50: 2020 7249 0000 0029 0272 4a00 0000 da05    rI...).rJ.....
+00000f60: 7a66 696c 6c29 0472 3500 0000 7248 0000  zfill).r5...rH..
+00000f70: 0072 4d00 0000 7236 0000 0072 2300 0000  .rM...r6...r#...
+00000f80: 7223 0000 0072 2400 0000 da19 6765 745f  r#...r$.....get_
 00000f90: 696d 6167 655f 6e61 6d65 5f66 726f 6d5f  image_name_from_
 00000fa0: 696e 6465 7891 0000 0073 0400 0000 000a  index....s......
-00000fb0: 1801 724b 0000 0072 3500 0000 2903 da0a  ..rK...r5...)...
+00000fb0: 1801 724f 0000 0072 3800 0000 2903 da0a  ..rO...r8...)...
 00000fc0: 746f 7069 635f 6e61 6d65 da11 7265 706c  topic_name..repl
 00000fd0: 6163 655f 6368 6172 6163 7465 7272 1000  ace_characterr..
 00000fe0: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
 00000ff0: 0000 0004 0000 0043 0000 0073 1400 0000  .......C...s....
 00001000: 7c00 a000 6401 7c01 a102 6402 6403 8502  |...d.|...d.d...
 00001010: 1900 5300 2904 7a53 0a20 2020 2041 7267  ..S.).zS.    Arg
 00001020: 733a 0a20 2020 2020 2020 2074 6f70 6963  s:.        topic
 00001030: 5f6e 616d 6520 2829 3a0a 2020 2020 2020  _name ():.      
 00001040: 2020 7265 706c 6163 655f 6368 6172 6163    replace_charac
 00001050: 7465 7220 2829 3a0a 0a20 2020 2052 6574  ter ():..    Ret
 00001060: 7572 6e73 3a0a 0a20 2020 20fa 012f e901  urns:..    ../..
 00001070: 0000 004e 2901 da07 7265 706c 6163 6529  ...N)...replace)
-00001080: 0272 4c00 0000 724d 0000 0072 2000 0000  .rL...rM...r ...
-00001090: 7220 0000 0072 2100 0000 da16 7265 706c  r ...r!.....repl
+00001080: 0272 5000 0000 7251 0000 0072 2300 0000  .rP...rQ...r#...
+00001090: 7223 0000 0072 2400 0000 da16 7265 706c  r#...r$.....repl
 000010a0: 6163 655f 726f 735f 746f 7069 635f 6e61  ace_ros_topic_na
-000010b0: 6d65 9f00 0000 7302 0000 0000 0972 5100  me....s......rQ.
+000010b0: 6d65 9f00 0000 7302 0000 0000 0972 5500  me....s......rU.
 000010c0: 0000 a904 7212 0000 0072 1300 0000 da0c  ....r....r......
 000010d0: 7374 6172 745f 726f 7362 6167 da0a 656e  start_rosbag..en
 000010e0: 645f 726f 7362 6167 6304 0000 0000 0000  d_rosbagc.......
 000010f0: 0000 0000 0005 0000 0003 0000 0043 0000  .............C..
 00001100: 0073 6c00 0000 7c03 7c02 1800 7d04 7c04  .sl...|.|...}.|.
 00001110: 6401 6b01 7214 6402 5300 7c00 722c 7c01  d.k.r.d.S.|.r,|.
 00001120: 722c 7400 7c01 7c00 1800 7c04 1b00 8301  r,t.|.|...|.....
@@ -283,23 +283,23 @@
 000011a0: 6e65 293a 0a20 2020 2020 2020 2065 6e64  ne):.        end
 000011b0: 5f74 696d 6520 2866 6c6f 6174 206f 7220  _time (float or 
 000011c0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
 000011d0: 7461 7274 5f72 6f73 6261 6720 2866 6c6f  tart_rosbag (flo
 000011e0: 6174 293a 0a20 2020 2020 2020 2065 6e64  at):.        end
 000011f0: 5f72 6f73 6261 6720 2866 6c6f 6174 293a  _rosbag (float):
 00001200: 0a0a 2020 2020 5265 7475 726e 733a 0a0a  ..    Returns:..
-00001210: 2020 2020 7201 0000 004e 724f 0000 0029      r....NrO...)
+00001210: 2020 2020 7201 0000 004e 7253 0000 0029      r....NrS...)
 00001220: 01da 0566 6c6f 6174 2905 7212 0000 0072  ...float).r....r
-00001230: 1300 0000 7253 0000 0072 5400 0000 5a0f  ....rS...rT...Z.
+00001230: 1300 0000 7257 0000 0072 5800 0000 5a0f  ....rW...rX...Z.
 00001240: 726f 7362 6167 5f64 7572 6174 696f 6e72  rosbag_durationr
-00001250: 2000 0000 7220 0000 0072 2100 0000 da13   ...r ...r!.....
+00001250: 2300 0000 7223 0000 0072 2400 0000 da13  #...r#...r$.....
 00001260: 6765 745f 6669 6c74 6572 5f66 7261 6374  get_filter_fract
 00001270: 696f 6eab 0000 0073 1600 0000 000b 0802  ion....s........
 00001280: 0801 0402 0801 1002 0801 1002 0801 1002  ................
-00001290: 0801 7256 0000 0029 04da 0174 7212 0000  ..rV...)...tr...
+00001290: 0801 725a 0000 0029 04da 0174 7212 0000  ..rZ...)...tr...
 000012a0: 0072 1300 0000 7210 0000 0063 0300 0000  .r....r....c....
 000012b0: 0000 0000 0000 0000 0300 0000 0200 0000  ................
 000012c0: 4300 0000 7360 0000 007c 0172 207c 0272  C...s`...|.r |.r
 000012d0: 207c 007c 016b 0572 1c7c 007c 026b 0172   |.|.k.r.|.|.k.r
 000012e0: 1c64 0153 0064 0253 007c 0173 387c 0272  .d.S.d.S.|.s8|.r
 000012f0: 387c 007c 026b 0172 3464 0153 0064 0253  8|.|.k.r4d.S.d.S
 00001300: 007c 0172 507c 0273 507c 007c 016b 0572  .|.rP|.sP|.|.k.r
@@ -307,410 +307,407 @@
 00001320: 5c64 0153 0064 0353 0029 047a 670a 2020  \d.S.d.S.).zg.  
 00001330: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
 00001340: 7420 2866 6c6f 6174 293a 0a20 2020 2020  t (float):.     
 00001350: 2020 2073 7461 7274 5f74 696d 6520 2866     start_time (f
 00001360: 6c6f 6174 293a 0a20 2020 2020 2020 2065  loat):.        e
 00001370: 6e64 5f74 696d 6520 2866 6c6f 6174 293a  nd_time (float):
 00001380: 0a0a 2020 2020 5265 7475 726e 733a 0a0a  ..    Returns:..
-00001390: 2020 2020 5446 4e72 2000 0000 2903 7257      TFNr ...).rW
-000013a0: 0000 0072 1200 0000 7213 0000 0072 2000  ...r....r....r .
-000013b0: 0000 7220 0000 0072 2100 0000 da16 6368  ..r ...r!.....ch
+00001390: 2020 2020 5446 4e72 2300 0000 2903 725b      TFNr#...).r[
+000013a0: 0000 0072 1200 0000 7213 0000 0072 2300  ...r....r....r#.
+000013b0: 0000 7223 0000 0072 2400 0000 da16 6368  ..r#...r$.....ch
 000013c0: 6563 6b5f 6966 5f69 6e5f 7469 6d65 5f72  eck_if_in_time_r
 000013d0: 616e 6765 c800 0000 731c 0000 0000 0b08  ange....s.......
 000013e0: 0110 0104 0204 0208 0108 0104 0204 0208  ................
-000013f0: 0108 0104 0204 0208 0172 5800 0000 6300  .........rX...c.
+000013f0: 0108 0104 0204 0208 0172 5c00 0000 6300  .........r\...c.
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
-00001420: 2902 7237 0000 007a 1169 6d67 5f6d 616e  ).r7...z.img_man
-00001430: 6966 6573 742e 6a73 6f6e 7220 0000 0072  ifest.jsonr ...r
-00001440: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
+00001420: 2902 723a 0000 007a 1169 6d67 5f6d 616e  ).r:...z.img_man
+00001430: 6966 6573 742e 6a73 6f6e 7223 0000 0072  ifest.jsonr#...r
+00001440: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
 00001450: 0000 00da 1567 6574 5f6e 616d 655f 696d  .....get_name_im
 00001460: 675f 6d61 6e69 6665 7374 e900 0000 7302  g_manifest....s.
-00001470: 0000 0000 0572 5900 0000 5429 03da 0666  .....rY...T)...f
+00001470: 0000 0000 0572 5d00 0000 5429 03da 0666  .....r]...T)...f
 00001480: 6f6c 6465 72da 0973 6176 655f 696d 6773  older..save_imgs
 00001490: 7210 0000 0063 0200 0000 0000 0000 0000  r....c..........
 000014a0: 0000 0400 0000 0600 0000 4300 0000 734a  ..........C...sJ
 000014b0: 0000 0074 00a0 0174 026a 03a0 047c 0074  ...t...t.j...|.t
 000014c0: 0583 00a1 02a1 017d 0274 067c 0264 0119  .......}.t.|.d..
 000014d0: 0064 0219 0064 0383 027d 0374 076a 087c  .d...d...}.t.j.|
 000014e0: 007c 007c 0364 048d 0301 007c 0173 4674  .|.|.d.....|.sFt
 000014f0: 00a0 097c 00a1 0101 0064 0553 0029 067a  ...|.....d.S.).z
 00001500: 500a 2020 2020 4172 6773 3a0a 2020 2020  P.    Args:.    
 00001510: 2020 2020 666f 6c64 6572 2028 7374 7229      folder (str)
 00001520: 3a0a 2020 2020 2020 2020 6465 6c65 7465  :.        delete
 00001530: 5f69 6d67 7320 2862 6f6f 6c29 3a0a 0a20  _imgs (bool):.. 
 00001540: 2020 2052 6574 7572 6e73 3a0a 0a20 2020     Returns:..   
-00001550: 20da 0574 6f70 6963 5a09 4672 6571 7565   ..topicZ.Freque
-00001560: 6e63 79e9 0200 0000 2903 7228 0000 00da  ncy.....).r(....
+00001550: 20da 0574 6f70 6963 da09 4672 6571 7565   ..topic..Freque
+00001560: 6e63 79e9 0200 0000 2903 722b 0000 00da  ncy.....).r+....
 00001570: 0b6f 7574 7075 745f 7061 7468 da0a 6672  .output_path..fr
 00001580: 616d 655f 7261 7465 4e29 0a72 0d00 0000  ame_rateN).r....
-00001590: 5a09 7265 6164 5f6a 736f 6e72 1700 0000  Z.read_jsonr....
-000015a0: 7218 0000 0072 2c00 0000 7259 0000 00da  r....r,...rY....
+00001590: da09 7265 6164 5f6a 736f 6e72 1700 0000  ..read_jsonr....
+000015a0: 7218 0000 0072 2f00 0000 725d 0000 00da  r....r/...r]....
 000015b0: 0572 6f75 6e64 720c 0000 005a 1863 7265  .roundr....Z.cre
 000015c0: 6174 655f 7669 6465 6f5f 6672 6f6d 5f69  ate_video_from_i
-000015d0: 6d61 6765 735a 1464 656c 6574 655f 6669  magesZ.delete_fi
-000015e0: 6c65 735f 6f66 5f74 7970 6529 0472 5a00  les_of_type).rZ.
-000015f0: 0000 725b 0000 005a 0c69 6d67 5f6d 616e  ..r[...Z.img_man
-00001600: 6966 6573 7472 5f00 0000 7220 0000 0072  ifestr_...r ...r
-00001610: 2000 0000 7221 0000 00da 1b67 6574 5f76   ...r!.....get_v
+000015d0: 6d61 6765 73da 1464 656c 6574 655f 6669  mages..delete_fi
+000015e0: 6c65 735f 6f66 5f74 7970 6529 0472 5e00  les_of_type).r^.
+000015f0: 0000 725f 0000 005a 0c69 6d67 5f6d 616e  ..r_...Z.img_man
+00001600: 6966 6573 7472 6400 0000 7223 0000 0072  ifestrd...r#...r
+00001610: 2300 0000 7224 0000 00da 1b67 6574 5f76  #...r$.....get_v
 00001620: 6964 656f 5f66 726f 6d5f 696d 6167 655f  ideo_from_image_
 00001630: 666f 6c64 6572 f100 0000 730c 0000 0000  folder....s.....
-00001640: 0916 0112 0110 0204 010a 0272 6100 0000  ...........ra...
-00001650: 46da 0a73 6571 7565 6e74 6961 6c29 0a72  F..sequential).r
-00001660: 0f00 0000 da0d 6f75 7470 7574 5f66 6f6c  ......output_fol
-00001670: 6465 7272 4400 0000 7216 0000 00da 0f63  derrD...r......c
-00001680: 7265 6174 655f 6d61 6e69 6665 7374 da06  reate_manifest..
-00001690: 6e61 6d69 6e67 da06 7265 7369 7a65 da06  naming..resize..
-000016a0: 7361 6d70 6c65 7212 0000 0072 1300 0000  sampler....r....
-000016b0: 630a 0000 0000 0000 0000 0000 0028 0000  c............(..
-000016c0: 000a 0000 0003 0000 0073 5204 0000 7400  .........sR...t.
-000016d0: 7c00 6401 8d01 7d0a 7401 7c0a 6402 8d01  |.d...}.t.|.d...
-000016e0: 7d0b 7c0a 731c 6403 5300 8800 733a 7c0a  }.|.s.d.S...s:|.
-000016f0: 6404 1900 7d0c 7402 8300 7d0d 7403 7c0c  d...}.t...}.t.|.
-00001700: 7c0d 6405 8d02 8900 7404 8300 7d0e 6406  |.d.....t...}.d.
-00001710: 7d0f 7404 8300 7d10 8800 4400 5d46 7d11  }.t...}...D.]F}.
-00001720: 7c11 7c0b a005 a100 6b07 7272 7406 a007  |.|.....k.rrt...
-00001730: 6407 7c11 9b00 6408 9d03 a101 0100 714e  d.|...d.......qN
-00001740: 6406 7c0e 7c11 3c00 7c0f 7c0b 7c11 1900  d.|.|.<.|.|.|...
-00001750: 6409 1900 3700 7d0f 7404 8300 7c10 7c11  d...7.}.t...|.|.
-00001760: 3c00 714e 7c0f 7d12 7c08 73a2 7c09 72d6  <.qN|.}.|.s.|.r.
-00001770: 7408 7c08 7c09 7c0a 640a 1900 7c0a 640b  t.|.|.|.d...|.d.
-00001780: 1900 640c 8d04 7d13 7c13 6406 6b00 72c6  ..d...}.|.d.k.r.
-00001790: 6406 6e02 7c13 7d13 7409 7c0f 7c13 1400  d.n.|.}.t.|.|...
-000017a0: 8301 7d12 7c07 72e2 7c12 7c07 1d00 7d12  ..}.|.r.|.|...}.
-000017b0: 8800 73fc 7406 a007 640d 7c00 9b00 640e  ..s.t...d.|...d.
-000017c0: 9d03 a101 0100 6403 5300 7406 a00a 640f  ......d.S.t...d.
-000017d0: a101 0100 740b 6410 7c0f 9b00 6411 7c12  ....t.d.|...d.|.
-000017e0: 9b00 6412 9d05 8301 0100 740c 7c00 8301  ..d.......t.|...
-000017f0: 9003 8f22 7d14 8700 6601 6413 6414 8408  ..."}...f.d.d...
-00001800: 7c14 6a0d 4400 8301 7d15 7c15 9001 735a  |.j.D...}.|...sZ
-00001810: 7406 a007 6415 a101 0100 5700 3500 5100  t...d.....W.5.Q.
-00001820: 5200 a300 6403 5300 740e 7c0f 6416 8d01  R...d.S.t.|.d...
-00001830: 9002 8f40 7d16 740f 7c14 6a10 7c15 6417  ...@}.t.|.j.|.d.
-00001840: 8d01 8301 4400 9002 5d26 5c02 7d17 5c03  ....D...]&\.}.\.
-00001850: 7d18 7d19 7d1a 7c18 6a11 7d11 7412 7413  }.}.}.|.j.}.t.t.
-00001860: 7c1a 7c18 6a14 8302 7c18 6a14 8302 7d1b  |.|.j...|.j...}.
-00001870: 7c19 6418 1400 7d1c 7415 7c1c 7c08 7c09  |.d...}.t.|.|.|.
-00001880: 8303 9001 73cc 7c0e 7c11 0500 1900 6419  ....s.|.|.....d.
-00001890: 3700 0300 3c00 9001 7178 7c07 9001 72f8  7...<...qx|...r.
-000018a0: 7c0e 7c11 1900 7c07 1600 6406 6b02 9001  |.|...|...d.k...
-000018b0: 73f8 7c0e 7c11 0500 1900 6419 3700 0300  s.|.|.....d.7...
-000018c0: 3c00 9001 7178 7416 7c11 8301 7d1d 7409  <...qxt.|...}.t.
-000018d0: 7417 7c1b 6a18 6a19 6a1a 8301 7417 7c1b  t.|.j.j.j...t.|.
-000018e0: 6a18 6a19 6a1b 8301 1700 8301 7d1e 741c  j.j.j.......}.t.
-000018f0: 6a1d a01e 7c01 7c1d a102 7d1f 741c 6a1d  j...|.|...}.t.j.
-00001900: a01f 7c1f a101 9002 7346 741c a020 7c1f  ..|.....sFt.. |.
-00001910: a101 0100 7c1b 6a21 641a 6b02 9002 72a0  ....|.j!d.k...r.
-00001920: 641b 641c 641d 641b 641c 641e 9c05 7d20  d.d.d.d.d.d...} 
-00001930: 7422 a023 7424 a025 7c20 7c1b 6a26 1900  t".#t$.%| |.j&..
-00001940: 7c1b 6a27 7c1b 6a28 6602 7c1b 6a29 a103  |.j'|.j(f.|.j)..
-00001950: a101 7d21 7c1b 6a26 641f 6b02 9002 72a0  ..}!|.j&d.k...r.
-00001960: 742a a02b 7c21 742a 6a2c a102 7d21 7c1b  t*.+|!t*j,..}!|.
-00001970: 6a21 6420 6b02 9002 72ce 6421 7c1b 6a2d  j!d k...r.d!|.j-
-00001980: 6b06 9002 72c4 742e a02f 7c1b a101 7d21  k...r.t../|...}!
-00001990: 6e0a 742e a030 7c1b a101 7d21 7c05 6422  n.t..0|...}!|.d"
-000019a0: 6b02 9002 72e6 7431 7c19 7c02 6423 8d02  k...r.t1|.|.d#..
-000019b0: 7d22 6e28 7c05 6424 6b02 9002 72fe 7431  }"n(|.d$k...r.t1
-000019c0: 7c1e 7c02 6423 8d02 7d22 6e10 7432 7c0e  |.|.d#..}"n.t2|.
-000019d0: 7c11 1900 7c02 6425 8d02 7d22 7c1d 9b00  |...|.d%..}"|...
-000019e0: 6426 7c22 9b00 9d03 7d22 741c 6a1d a01e  d&|"....}"t.j...
-000019f0: 7c1f 7c22 a102 7d23 7c06 9003 7248 7433  |.|"..}#|...rHt3
-00001a00: 6a34 7c21 7c06 6406 1900 7c06 6419 1900  j4|!|.d...|.d...
-00001a10: 6427 8d03 7d21 742a a035 7c23 7c21 a102  d'..}!t*.5|#|!..
-00001a20: 0100 7c04 9003 7276 7436 7c1e 7c19 7c23  ..|...rvt6|.|.|#
-00001a30: 7c0e 7c11 1900 6428 8d04 7c10 7c11 1900  |.|...d(..|.|...
-00001a40: 7c22 3c00 7c11 7c0e a005 a100 6b06 9003  |"<.|.|.....k...
-00001a50: 7294 7c0e 7c11 0500 1900 6419 3700 0300  r.|.|.....d.7...
-00001a60: 3c00 7c16 a037 6419 a101 0100 9001 7178  <.|..7d.......qx
-00001a70: 5700 3500 5100 5200 5800 7438 8300 7d24  W.5.Q.R.X.t8..}$
-00001a80: 7c04 9004 7244 7c10 a005 a100 4400 5d82  |...rD|.....D.].
-00001a90: 7d25 741c 6a1d a01e 7c01 7416 7c25 8301  }%t.j...|.t.|%..
-00001aa0: a102 7d1f 7c24 a039 7c1f a101 0100 741c  ..}.|$.9|.....t.
-00001ab0: 6a1d a01f 7c1f a101 9003 73f8 741c a020  j...|.....s.t.. 
-00001ac0: 7c1f a101 0100 7404 8300 7d26 7c10 7c25  |.....t...}&|.|%
-00001ad0: 1900 7c26 6429 3c00 7c0b 7c25 1900 7c26  ..|&d)<.|.|%..|&
-00001ae0: 642a 3c00 741c 6a1d a01e 7c1f 743a 8300  d*<.t.j...|.t:..
-00001af0: a102 7d27 741c 6a1d a01f 7c27 a101 9003  ..}'t.j...|'....
-00001b00: 73c0 743b a03c 7c26 7c27 a102 0100 9003  s.t;.<|&|'......
-00001b10: 71c0 5700 3500 5100 5200 5800 7c24 5300  q.W.5.Q.R.X.|$S.
-00001b20: 292b 6126 0100 000a 2020 2020 4172 6773  )+a&....    Args
-00001b30: 3a0a 2020 2020 2020 2020 726f 7362 6167  :.        rosbag
-00001b40: 5f70 6174 6820 2873 7472 293a 0a20 2020  _path (str):.   
-00001b50: 2020 2020 206f 7574 7075 745f 666f 6c64       output_fold
-00001b60: 6572 2028 7374 7229 3a0a 2020 2020 2020  er (str):.      
-00001b70: 2020 6669 6c65 5f66 6f72 6d61 7420 2873    file_format (s
-00001b80: 7472 293a 0a20 2020 2020 2020 2074 6f70  tr):.        top
-00001b90: 6963 7320 286c 6973 7429 3a0a 2020 2020  ics (list):.    
-00001ba0: 2020 2020 6372 6561 7465 5f6d 616e 6966      create_manif
-00001bb0: 6573 7420 2862 6f6f 6c29 3a0a 2020 2020  est (bool):.    
-00001bc0: 2020 2020 6e61 6d69 6e67 2028 7374 7229      naming (str)
-00001bd0: 3a0a 2020 2020 2020 2020 7265 7369 7a65  :.        resize
-00001be0: 2028 6c69 7374 293a 0a20 2020 2020 2020   (list):.       
-00001bf0: 2073 616d 706c 6520 2869 6e74 293a 0a20   sample (int):. 
-00001c00: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
-00001c10: 6520 2866 6c6f 6174 293a 0a20 2020 2020  e (float):.     
-00001c20: 2020 2065 6e64 5f74 696d 6520 2866 6c6f     end_time (flo
-00001c30: 6174 293a 0a0a 2020 2020 5265 7475 726e  at):..    Return
-00001c40: 733a 204e 6f6e 650a 0a20 2020 2029 0172  s: None..    ).r
-00001c50: 0f00 0000 2901 7223 0000 004e 7216 0000  ....).r#...Nr...
-00001c60: 0072 4000 0000 7201 0000 007a 0a52 6f62  .r@...r....z.Rob
-00001c70: 6f6c 6f67 733a 207a 1920 6e6f 7420 696e  ologs: z. not in
-00001c80: 2052 4f53 4261 672e 2e73 6b69 7070 696e   ROSBag..skippin
-00001c90: 672e 7a0d 4d65 7373 6167 6520 436f 756e  g.z.Message Coun
-00001ca0: 7472 1200 0000 7213 0000 0072 5200 0000  tr....r....rR...
-00001cb0: 7a28 526f 626f 6c6f 6773 3a20 6e6f 2069  z(Robologs: no i
-00001cc0: 6d61 6765 2074 6f70 6963 7320 746f 2065  mage topics to e
-00001cd0: 7874 7261 6374 2069 6e20 7a03 2e2e 2e7a  xtract in z....z
-00001ce0: 1e52 6f62 6f6c 6f67 733a 2065 7874 7261  .Robologs: extra
-00001cf0: 6374 696e 6720 696d 6167 6573 2e2e 2e7a  cting images...z
-00001d00: 1952 6f62 6f6c 6f67 733a 2069 7465 7261  .Robologs: itera
-00001d10: 7469 6e67 206f 7665 7220 7a14 2069 6d61  ting over z. ima
-00001d20: 6765 7320 746f 2065 7874 7261 6374 3a20  ges to extract: 
-00001d30: 7a07 2069 6d61 6765 7363 0100 0000 0000  z. imagesc......
-00001d40: 0000 0000 0000 0200 0000 0400 0000 1300  ................
-00001d50: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
-00001d60: 016a 0088 006b 0672 047c 0191 0271 0453  .j...k.r.|...q.S
-00001d70: 0072 2000 0000 2901 725c 0000 0072 3b00  .r ...).r\...r;.
-00001d80: 0000 a901 7216 0000 0072 2000 0000 7221  ....r....r ...r!
-00001d90: 0000 0072 3f00 0000 5101 0000 7306 0000  ...r?...Q...s...
-00001da0: 0006 0002 000a 007a 2767 6574 5f69 6d61  .......z'get_ima
-00001db0: 6765 735f 6672 6f6d 5f62 6167 2e3c 6c6f  ges_from_bag.<lo
-00001dc0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00001dd0: 7a38 526f 626f 6c6f 6773 3a20 6e6f 6e65  z8Robologs: none
-00001de0: 206f 6620 7468 6520 7365 6c65 6374 6564   of the selected
-00001df0: 2074 6f70 6963 7320 6172 6520 696e 2074   topics are in t
-00001e00: 6865 2052 4f53 4261 672e 2901 da05 746f  he ROSBag.)...to
-00001e10: 7461 6c29 01da 0b63 6f6e 6e65 6374 696f  tal)...connectio
-00001e20: 6e73 6795 d626 e80b 2e11 3e72 4f00 0000  nsg..&....>rO...
-00001e30: 7a15 7365 6e73 6f72 5f6d 7367 732f 6d73  z.sensor_msgs/ms
-00001e40: 672f 496d 6167 65da 0352 4742 da04 5247  g/Image..RGB..RG
-00001e50: 4241 da01 4c29 055a 0472 6762 385a 0572  BA..L).Z.rgb8Z.r
-00001e60: 6762 6138 5a05 6d6f 6e6f 385a 0438 5543  gba8Z.mono8Z.8UC
-00001e70: 33da 0562 6772 6138 726e 0000 007a 1f73  3..bgra8rn...z.s
-00001e80: 656e 736f 725f 6d73 6773 2f6d 7367 2f43  ensor_msgs/msg/C
-00001e90: 6f6d 7072 6573 7365 6449 6d61 6765 5a0f  ompressedImageZ.
-00001ea0: 636f 6d70 7265 7373 6564 4465 7074 6872  compressedDepthr
-00001eb0: 3000 0000 2902 7243 0000 0072 4400 0000  0...).rC...rD...
-00001ec0: 722f 0000 0029 0272 3200 0000 7244 0000  r/...).r2...rD..
-00001ed0: 0072 3500 0000 2903 da03 696d 675a 096e  .r5...)...imgZ.n
-00001ee0: 6577 5f77 6964 7468 5a0a 6e65 775f 6865  ew_widthZ.new_he
-00001ef0: 6967 6874 2904 722f 0000 0072 3000 0000  ight).r/...r0...
-00001f00: 7231 0000 0072 3200 0000 5a06 696d 6167  r1...r2...Z.imag
-00001f10: 6573 725c 0000 0029 3d72 2200 0000 7227  esr\...)=r"...r'
-00001f20: 0000 0072 3800 0000 7241 0000 0072 1c00  ...r8...rA...r..
-00001f30: 0000 da04 6b65 7973 da07 6c6f 6767 696e  ....keys..loggin
-00001f40: 67da 0777 6172 6e69 6e67 7256 0000 00da  g..warningrV....
-00001f50: 0369 6e74 da05 6465 6275 67da 0570 7269  .int..debug..pri
-00001f60: 6e74 7208 0000 0072 6a00 0000 720b 0000  ntr....rj...r...
-00001f70: 00da 0965 6e75 6d65 7261 7465 da08 6d65  ...enumerate..me
-00001f80: 7373 6167 6573 725c 0000 0072 0900 0000  ssagesr\...r....
-00001f90: 720a 0000 005a 076d 7367 7479 7065 7258  r....Z.msgtyperX
-00001fa0: 0000 0072 5100 0000 7246 0000 00da 0668  ...rQ...rF.....h
-00001fb0: 6561 6465 725a 0573 7461 6d70 da03 7365  eaderZ.stamp..se
-00001fc0: 635a 076e 616e 6f73 6563 7217 0000 0072  cZ.nanosecr....r
-00001fd0: 1800 0000 722c 0000 0072 1900 0000 da08  ....r,...r......
-00001fe0: 6d61 6b65 6469 7273 5a0b 5f5f 6d73 6774  makedirsZ.__msgt
-00001ff0: 7970 655f 5fda 026e 70da 0561 7272 6179  ype__..np..array
-00002000: 7206 0000 00da 0966 726f 6d62 7974 6573  r......frombytes
-00002010: da08 656e 636f 6469 6e67 da05 7769 6474  ..encoding..widt
-00002020: 68da 0668 6569 6768 74da 0464 6174 61da  h..height..data.
-00002030: 0363 7632 5a08 6376 7443 6f6c 6f72 5a0f  .cv2Z.cvtColorZ.
-00002040: 434f 4c4f 525f 4247 5241 3252 4742 41da  COLOR_BGRA2RGBA.
-00002050: 0666 6f72 6d61 7472 0c00 0000 5a1f 636f  .formatr....Z.co
-00002060: 6e76 6572 745f 636f 6d70 7265 7373 6564  nvert_compressed
-00002070: 5f64 6570 7468 5f74 6f5f 6376 325a 1463  _depth_to_cv2Z.c
-00002080: 6f6e 7665 7274 5f69 6d61 6765 5f74 6f5f  onvert_image_to_
-00002090: 6376 3272 4700 0000 724b 0000 0072 0e00  cv2rG...rK...r..
-000020a0: 0000 5a0c 7265 7369 7a65 5f69 6d61 6765  ..Z.resize_image
-000020b0: 5a07 696d 7772 6974 6572 3600 0000 da06  Z.imwriter6.....
-000020c0: 7570 6461 7465 da04 6c69 7374 da06 6170  update..list..ap
-000020d0: 7065 6e64 7259 0000 0072 0d00 0000 5a09  pendrY...r....Z.
-000020e0: 7361 7665 5f6a 736f 6e29 2872 0f00 0000  save_json)(r....
-000020f0: 7263 0000 0072 4400 0000 7216 0000 0072  rc...rD...r....r
-00002100: 6400 0000 7265 0000 0072 6600 0000 7267  d...re...rf...rg
-00002110: 0000 0072 1200 0000 7213 0000 0072 2300  ...r....r....r#.
-00002120: 0000 7225 0000 005a 0f61 6c6c 5f74 6f70  ..r%...Z.all_top
-00002130: 6963 735f 6469 6374 5a0f 696d 675f 746f  ics_dictZ.img_to
-00002140: 7069 635f 7479 7065 735a 1674 6f70 6963  pic_typesZ.topic
-00002150: 5f6d 7367 5f63 6f75 6e74 6572 5f64 6963  _msg_counter_dic
-00002160: 745a 1674 6f74 616c 5f6e 756d 6265 725f  tZ.total_number_
-00002170: 6f66 5f69 6d61 6765 735a 0d6d 616e 6966  of_imagesZ.manif
-00002180: 6573 745f 6469 6374 725c 0000 005a 126e  est_dictr\...Z.n
-00002190: 725f 696d 6773 5f74 6f5f 6578 7472 6163  r_imgs_to_extrac
-000021a0: 745a 0f66 696c 7465 725f 6475 7261 7469  tZ.filter_durati
-000021b0: 6f6e da06 7265 6164 6572 726a 0000 005a  on..readerrj...Z
-000021c0: 0470 6261 72da 0269 74da 0a63 6f6e 6e65  .pbar..it..conne
-000021d0: 6374 696f 6e72 5700 0000 5a07 7261 7764  ctionrW...Z.rawd
-000021e0: 6174 61da 036d 7367 5a0d 726f 7362 6167  ata..msgZ.rosbag
-000021f0: 5f74 696d 655f 735a 1574 6f70 6963 5f6e  _time_sZ.topic_n
-00002200: 616d 655f 756e 6465 7273 636f 7265 722f  ame_underscorer/
-00002210: 0000 005a 206f 7574 7075 745f 696d 6167  ...Z output_imag
-00002220: 6573 5f66 6f6c 6465 725f 666f 6c64 6572  es_folder_folder
-00002230: 5f70 6174 685a 0d69 6d67 5f65 6e63 6f64  _pathZ.img_encod
-00002240: 696e 6773 5a08 6376 5f69 6d61 6765 5a0a  ingsZ.cv_imageZ.
-00002250: 696d 6167 655f 6e61 6d65 5a0a 696d 6167  image_nameZ.imag
-00002260: 655f 7061 7468 5a17 6f75 7470 7574 5f69  e_pathZ.output_i
-00002270: 6d67 735f 666f 6c64 6572 5f6c 6973 74da  mgs_folder_list.
-00002280: 036b 6579 5a0b 6f75 7470 7574 5f64 6963  .keyZ.output_dic
-00002290: 745a 196f 7574 7075 745f 7061 7468 5f6d  tZ.output_path_m
-000022a0: 616e 6966 6573 745f 6a73 6f6e 7220 0000  anifest_jsonr ..
-000022b0: 0072 6800 0000 7221 0000 00da 1367 6574  .rh...r!.....get
-000022c0: 5f69 6d61 6765 735f 6672 6f6d 5f62 6167  _images_from_bag
-000022d0: 0401 0000 73c6 0000 0000 1d0a 010a 0104  ....s...........
-000022e0: 0104 0204 0108 0106 010c 0206 0104 0106  ................
-000022f0: 0208 010c 0112 0102 0208 0110 010c 0204  ................
-00002300: 0208 0102 0102 0102 0106 0106 fc06 0610  ................
-00002310: 020c 0204 0108 0204 0112 0204 020a 0116  ................
-00002320: 020c 0114 0206 010a 010e 020e 0120 0106  ............. ..
-00002330: 0114 0108 010e 0110 0104 0218 0110 0104  ................
-00002340: 0208 0220 020e 020e 010a 020c 0110 0124  ... ...........$
-00002350: 010c 010e 020c 010c 010c 020a 020a 010e  ................
-00002360: 020a 010e 0310 020e 020e 0206 0118 020c  ................
-00002370: 0206 0102 0102 0102 0102 0106 fc0e 070e  ................
-00002380: 0110 0218 0206 0206 010c 0112 010a 010e  ................
-00002390: 010a 0206 010c 010c 0210 030e 011a 0272  ...............r
-000023a0: 8c00 0000 a902 da08 6f66 6673 6574 5f73  ........offset_s
-000023b0: da14 6669 7273 745f 726f 7362 6167 5f74  ..first_rosbag_t
-000023c0: 696d 655f 6e73 6302 0000 0000 0000 0000  ime_nsc.........
-000023d0: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-000023e0: 1400 0000 7400 7c00 6401 1400 8301 7d02  ....t.|.d.....}.
-000023f0: 7c02 7c01 1700 5300 2902 4e67 0000 0000  |.|...S.).Ng....
-00002400: 65cd cd41 2901 7273 0000 0029 0372 8e00  e..A).rs...).r..
-00002410: 0000 728f 0000 005a 096f 6666 7365 745f  ..r....Z.offset_
-00002420: 6e73 7220 0000 0072 2000 0000 7221 0000  nsr ...r ...r!..
-00002430: 00da 1d63 6f6e 7665 7274 5f6f 6666 7365  ...convert_offse
-00002440: 745f 735f 746f 5f72 6f73 6261 675f 6e73  t_s_to_rosbag_ns
-00002450: ae01 0000 7304 0000 0000 020c 0172 9000  ....s........r..
-00002460: 0000 2904 da07 7469 6d65 5f6e 73da 1473  ..)...time_ns..s
-00002470: 7461 7274 5f74 696d 655f 726f 7362 6167  tart_time_rosbag
-00002480: 5f6e 73da 1265 6e64 5f74 696d 655f 726f  _ns..end_time_ro
-00002490: 7362 6167 5f6e 7372 1000 0000 6303 0000  sbag_nsr....c...
-000024a0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-000024b0: 0043 0000 0073 2400 0000 7c01 7210 7c00  .C...s$...|.r.|.
-000024c0: 7c01 6b00 7210 6401 5300 7c02 7220 7c00  |.k.r.d.S.|.r |.
-000024d0: 7c02 6b04 7220 6402 5300 6403 5300 2904  |.k.r d.S.d.S.).
-000024e0: 617b 0100 000a 2020 2020 5468 6973 2066  a{....    This f
-000024f0: 756e 6374 696f 6e20 6368 6563 6b73 2069  unction checks i
-00002500: 6620 6120 7469 6d65 7374 616d 7020 6973  f a timestamp is
-00002510: 2077 6974 6869 6e67 2061 2073 7065 6369   withing a speci
-00002520: 6669 6564 2074 696d 6572 616e 6765 2061  fied timerange a
-00002530: 6e64 2072 6574 7572 6e73 2054 7275 6520  nd returns True 
-00002540: 6f72 2046 616c 7365 2069 6620 7765 2061  or False if we a
-00002550: 7265 2e20 4974 2061 6c73 6f0a 2020 2020  re. It also.    
-00002560: 7265 7475 726e 7320 6120 7365 636f 6e64  returns a second
-00002570: 2062 6f6f 6c65 616e 2074 6f20 696e 6469   boolean to indi
-00002580: 6361 7465 2069 6620 7765 2061 7265 2070  cate if we are p
-00002590: 6173 7420 7468 6520 656e 6420 7469 6d65  ast the end time
-000025a0: 2e20 5468 6973 2063 616e 2062 6520 7573  . This can be us
-000025b0: 6564 2074 6f20 6272 6561 6b20 6f75 7420  ed to break out 
-000025c0: 6f66 2074 6865 206c 6f6f 7020 6561 726c  of the loop earl
-000025d0: 792e 0a20 2020 2041 7267 733a 0a20 2020  y..    Args:.   
-000025e0: 2020 2020 2074 696d 655f 6e73 2028 696e       time_ns (in
-000025f0: 7429 3a0a 2020 2020 2020 2020 7374 6172  t):.        star
-00002600: 745f 7469 6d65 5f72 6f73 6261 675f 6e73  t_time_rosbag_ns
-00002610: 2028 696e 7429 3a0a 2020 2020 2020 2020   (int):.        
-00002620: 656e 645f 7469 6d65 5f72 6f73 6261 675f  end_time_rosbag_
-00002630: 6e73 2028 696e 7429 3a0a 0a20 2020 2052  ns (int):..    R
-00002640: 6574 7572 6e73 3a20 5475 7270 6c65 206f  eturns: Turple o
-00002650: 6620 626f 6f6c 6561 6e73 0a0a 2020 2020  f booleans..    
-00002660: 2902 4646 2902 4654 2902 5446 7220 0000  ).FF).FT).TFr ..
-00002670: 00a9 0372 9100 0000 7292 0000 0072 9300  ...r....r....r..
-00002680: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
-00002690: 00da 1c69 735f 6d65 7373 6167 655f 7769  ...is_message_wi
-000026a0: 7468 696e 5f74 696d 655f 7261 6e67 65b4  thin_time_range.
-000026b0: 0100 0073 0e00 0000 000f 0401 0801 0402  ...s............
-000026c0: 0401 0801 0402 7295 0000 00da 0972 6f73  ......r......ros
-000026d0: 6261 675f 6e73 2906 da0e 696e 7075 745f  bag_ns)...input_
-000026e0: 6261 675f 7061 7468 da0f 6f75 7470 7574  bag_path..output
-000026f0: 5f62 6167 5f70 6174 68da 0a74 6f70 6963  _bag_path..topic
-00002700: 5f6c 6973 7472 1200 0000 7213 0000 00da  _listr....r.....
-00002710: 0e74 696d 6573 7461 6d70 5f74 7970 6563  .timestamp_typec
-00002720: 0600 0000 0000 0000 0000 0000 0e00 0000  ................
-00002730: 0900 0000 4300 0000 73d0 0000 007c 0564  ....C...s....|.d
-00002740: 016b 0772 1674 0064 027c 059b 009d 0283  .k.r.t.d.|......
-00002750: 0182 0174 017c 0164 0383 028f a67d 0664  ...t.|.d.....}.d
-00002760: 047d 0764 057d 0874 017c 0083 01a0 02a1  .}.d.}.t.|......
-00002770: 0044 005d 8a5c 037d 097d 0a7d 0b7c 0864  .D.].\.}.}.}.|.d
-00002780: 046b 0072 787c 0ba0 03a1 007d 087c 0564  .k.rx|.....}.|.d
-00002790: 066b 0272 787c 0372 6874 047c 037c 0864  .k.rx|.rht.|.|.d
-000027a0: 078d 027d 037c 0472 7874 047c 047c 0864  ...}.|.rxt.|.|.d
-000027b0: 078d 027d 047c 0272 867c 097c 026b 0772  ...}.|.r.|.|.k.r
-000027c0: 8671 3674 057c 0ba0 03a1 007c 037c 0464  .q6t.|.....|.|.d
-000027d0: 088d 035c 027d 0c7d 0d7c 0d72 a401 0071  ...\.}.}.|.r...q
-000027e0: c27c 0c73 aa71 367c 0764 0937 007d 077c  .|.s.q6|.d.7.}.|
-000027f0: 06a0 067c 097c 0a7c 0ba1 0301 0071 3657  ...|.|.|.....q6W
-00002800: 0035 0051 0052 0058 0064 0a53 0029 0b7a  .5.Q.R.X.d.S.).z
-00002810: b30a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00002820: 2020 2020 696e 7075 745f 6261 675f 7061      input_bag_pa
-00002830: 7468 2028 293a 0a20 2020 2020 2020 206f  th ():.        o
-00002840: 7574 7075 745f 6261 675f 7061 7468 2028  utput_bag_path (
-00002850: 293a 0a20 2020 2020 2020 2074 6f70 6963  ):.        topic
-00002860: 5f6c 6973 7420 2829 3a0a 2020 2020 2020  _list ():.      
-00002870: 2020 7374 6172 745f 7469 6d65 2028 293a    start_time ():
-00002880: 0a20 2020 2020 2020 2065 6e64 5f74 696d  .        end_tim
-00002890: 6520 2829 3a0a 2020 2020 2020 2020 7469  e ():.        ti
-000028a0: 6d65 7374 616d 705f 7479 7065 2028 293a  mestamp_type ():
-000028b0: 0a0a 2020 2020 5265 7475 726e 733a 0a0a  ..    Returns:..
-000028c0: 2020 2020 2902 7296 0000 0072 8e00 0000      ).r....r....
-000028d0: 7a2c 526f 626f 6c6f 6773 3a20 696e 7661  z,Robologs: inva
-000028e0: 6c69 6420 7469 6d65 7374 616d 705f 7479  lid timestamp_ty
-000028f0: 7065 2070 6172 616d 6574 6572 3a20 da01  pe parameter: ..
-00002900: 7772 0100 0000 e9ff ffff ff72 8e00 0000  wr.........r....
-00002910: 728d 0000 0072 9400 0000 724f 0000 004e  r....r....rO...N
-00002920: 2907 721a 0000 0072 0700 0000 5a0d 7265  ).r....r....Z.re
-00002930: 6164 5f6d 6573 7361 6765 735a 0774 6f5f  ad_messagesZ.to_
-00002940: 6e73 6563 7290 0000 0072 9500 0000 da05  nsecr....r......
-00002950: 7772 6974 6529 0e72 9700 0000 7298 0000  write).r....r...
-00002960: 0072 9900 0000 7212 0000 0072 1300 0000  .r....r....r....
-00002970: 729a 0000 005a 066f 7574 6261 675a 0b6d  r....Z.outbagZ.m
-00002980: 7367 5f63 6f75 6e74 6572 5a10 6669 7273  sg_counterZ.firs
-00002990: 745f 7469 6d65 5f73 7461 6d70 725c 0000  t_time_stampr\..
-000029a0: 0072 8a00 0000 7257 0000 00da 0d69 6e5f  .r....rW.....in_
-000029b0: 7469 6d65 5f72 616e 6765 da0d 7061 7374  time_range..past
-000029c0: 5f65 6e64 5f74 696d 6572 2000 0000 7220  _end_timer ...r 
-000029d0: 0000 0072 2100 0000 da14 6765 745f 636c  ...r!.....get_cl
-000029e0: 6970 7065 645f 6261 675f 6669 6c65 ce01  ipped_bag_file..
-000029f0: 0000 7342 0000 0000 1508 010e 020c 0104  ..sB............
-00002a00: 0104 0116 0208 0108 0108 0104 0102 0102  ................
-00002a10: 0002 ff06 0304 0102 0102 0002 ff06 0404  ................
-00002a20: 0108 0102 0208 0102 0102 fe0a 0504 0104  ................
-00002a30: 0204 0102 0208 011a 0272 a000 0000 2901  .........r....).
-00002a40: 7242 0000 0029 0272 4200 0000 7248 0000  rB...).rB...rH..
-00002a50: 0029 0172 3500 0000 2901 5429 0872 4200  .).r5...).T).rB.
-00002a60: 0000 4e46 7262 0000 004e 4e4e 4e29 024e  ..NFrb...NNNN).N
-00002a70: 4e29 044e 4e4e 7296 0000 0029 34da 075f  N).NNNr....)4.._
-00002a80: 5f64 6f63 5f5f 722b 0000 0072 7100 0000  _doc__r+...rq...
-00002a90: 7217 0000 00da 0674 7970 696e 6772 0200  r......typingr..
-00002aa0: 0000 7203 0000 0072 0400 0000 7282 0000  ..r....r....r...
-00002ab0: 00da 056e 756d 7079 727b 0000 005a 0562  ...numpyr{...Z.b
-00002ac0: 6167 7079 7205 0000 00da 0350 494c 7206  agpyr......PILr.
-00002ad0: 0000 005a 0672 6f73 6261 6772 0700 0000  ...Z.rosbagr....
-00002ae0: 5a0f 726f 7362 6167 732e 726f 7362 6167  Z.rosbags.rosbag
-00002af0: 3172 0800 0000 5a0d 726f 7362 6167 732e  1r....Z.rosbags.
-00002b00: 7365 7264 6572 0900 0000 720a 0000 0072  serder....r....r
-00002b10: 0b00 0000 da1f 726f 626f 6c6f 6773 5f72  ......robologs_r
-00002b20: 6f73 5f75 7469 6c73 2e73 6f75 7263 6573  os_utils.sources
-00002b30: 2e72 6f73 3172 0c00 0000 da23 726f 626f  .ros1r.....#robo
-00002b40: 6c6f 6773 5f72 6f73 5f75 7469 6c73 2e75  logs_ros_utils.u
-00002b50: 7469 6c73 2e66 696c 655f 7574 696c 7372  tils.file_utilsr
-00002b60: 0d00 0000 5a22 726f 626f 6c6f 6773 5f72  ....Z"robologs_r
-00002b70: 6f73 5f75 7469 6c73 2e75 7469 6c73 2e69  os_utils.utils.i
-00002b80: 6d67 5f75 7469 6c73 720e 0000 0072 4600  mg_utilsr....rF.
-00002b90: 0000 721c 0000 0072 2200 0000 7227 0000  ..r....r"...r'..
-00002ba0: 0072 2e00 0000 7273 0000 0072 3600 0000  .r....rs...r6...
-00002bb0: 7238 0000 0072 8500 0000 7241 0000 0072  r8...r....rA...r
-00002bc0: 4700 0000 724b 0000 0072 5100 0000 7255  G...rK...rQ...rU
-00002bd0: 0000 0072 5600 0000 da04 626f 6f6c 7258  ...rV.....boolrX
-00002be0: 0000 0072 5900 0000 7261 0000 0072 8c00  ...rY...ra...r..
-00002bf0: 0000 7290 0000 0072 9500 0000 72a0 0000  ..r....r....r...
-00002c00: 0072 2000 0000 7220 0000 0072 2000 0000  .r ...r ...r ...
-00002c10: 7221 0000 00da 083c 6d6f 6475 6c65 3e01  r!.....<module>.
-00002c20: 0000 0073 8c00 0000 0405 0801 0801 0801  ...s............
-00002c30: 1402 0801 0801 0c01 0c01 0c01 0c01 1001  ................
-00002c40: 0c02 0c01 0c01 0c03 1023 100a 1015 1615  .........#......
-00002c50: 0808 120c 140d 160e 140c 1c1d 1421 0808  .............!..
-00002c60: 1416 0001 0001 0001 0001 0001 0001 0001  ................
-00002c70: 00f6 0201 0201 0201 0201 0601 0201 0201  ................
-00002c80: 0601 0601 0601 06f6 0c7f 002b 1007 0000  ...........+....
-00002c90: 00ff 0201 0200 0600 0601 0afe 0c1d 0001  ................
-00002ca0: 0001 0001 00fa 0201 0201 0201 0601 0e01  ................
-00002cb0: 0e01 02fa                                ....
+00001640: 0916 0112 0110 0204 010a 0272 6800 0000  ...........rh...
+00001650: da0a 7365 7175 656e 7469 616c 290a 720f  ..sequential).r.
+00001660: 0000 00da 0d6f 7574 7075 745f 666f 6c64  .....output_fold
+00001670: 6572 7248 0000 0072 1600 0000 da0f 6372  errH...r......cr
+00001680: 6561 7465 5f6d 616e 6966 6573 74da 066e  eate_manifest..n
+00001690: 616d 696e 67da 0672 6573 697a 65da 0673  aming..resize..s
+000016a0: 616d 706c 6572 1200 0000 7213 0000 0063  ampler....r....c
+000016b0: 0a00 0000 0000 0000 0000 0000 2800 0000  ............(...
+000016c0: 0a00 0000 0300 0000 7352 0400 0074 007c  ........sR...t.|
+000016d0: 0064 018d 017d 0a74 017c 0a64 028d 017d  .d...}.t.|.d...}
+000016e0: 0b7c 0a73 1c64 0353 0088 0073 3a7c 0a64  .|.s.d.S...s:|.d
+000016f0: 0419 007d 0c74 0283 007d 0d74 037c 0c7c  ...}.t...}.t.|.|
+00001700: 0d64 058d 0289 0074 0483 007d 0e64 067d  .d.....t...}.d.}
+00001710: 0f74 0483 007d 1088 0044 005d 467d 117c  .t...}...D.]F}.|
+00001720: 117c 0ba0 05a1 006b 0772 7274 06a0 0764  .|.....k.rrt...d
+00001730: 077c 119b 0064 089d 03a1 0101 0071 4e64  .|...d.......qNd
+00001740: 067c 0e7c 113c 007c 0f7c 0b7c 1119 0064  .|.|.<.|.|.|...d
+00001750: 0919 0037 007d 0f74 0483 007c 107c 113c  ...7.}.t...|.|.<
+00001760: 0071 4e7c 0f7d 127c 0873 a27c 0972 d674  .qN|.}.|.s.|.r.t
+00001770: 087c 087c 097c 0a64 0a19 007c 0a64 0b19  .|.|.|.d...|.d..
+00001780: 0064 0c8d 047d 137c 1364 066b 0072 c664  .d...}.|.d.k.r.d
+00001790: 066e 027c 137d 1374 097c 0f7c 1314 0083  .n.|.}.t.|.|....
+000017a0: 017d 127c 0772 e27c 127c 071d 007d 1288  .}.|.r.|.|...}..
+000017b0: 0073 fc74 06a0 0764 0d7c 009b 0064 0e9d  .s.t...d.|...d..
+000017c0: 03a1 0101 0064 0353 0074 06a0 0a64 0fa1  .....d.S.t...d..
+000017d0: 0101 0074 0b64 107c 0f9b 0064 117c 129b  ...t.d.|...d.|..
+000017e0: 0064 129d 0583 0101 0074 0c7c 0083 0190  .d.......t.|....
+000017f0: 038f 227d 1487 0066 0164 1364 1484 087c  .."}...f.d.d...|
+00001800: 146a 0d44 0083 017d 157c 1590 0173 5a74  .j.D...}.|...sZt
+00001810: 06a0 0764 15a1 0101 0057 0035 0051 0052  ...d.....W.5.Q.R
+00001820: 00a3 0064 0353 0074 0e7c 0f64 168d 0190  ...d.S.t.|.d....
+00001830: 028f 407d 1674 0f7c 146a 107c 1564 178d  ..@}.t.|.j.|.d..
+00001840: 0183 0144 0090 025d 265c 027d 175c 037d  ...D...]&\.}.\.}
+00001850: 187d 197d 1a7c 186a 117d 1174 1274 137c  .}.}.|.j.}.t.t.|
+00001860: 1a7c 186a 1483 027c 186a 1483 027d 1b7c  .|.j...|.j...}.|
+00001870: 1964 1814 007d 1c74 157c 1c7c 087c 0983  .d...}.t.|.|.|..
+00001880: 0390 0173 cc7c 0e7c 1105 0019 0064 1937  ...s.|.|.....d.7
+00001890: 0003 003c 0090 0171 787c 0790 0172 f87c  ...<...qx|...r.|
+000018a0: 0e7c 1119 007c 0716 0064 066b 0290 0173  .|...|...d.k...s
+000018b0: f87c 0e7c 1105 0019 0064 1937 0003 003c  .|.|.....d.7...<
+000018c0: 0090 0171 7874 167c 1183 017d 1d74 0974  ...qxt.|...}.t.t
+000018d0: 177c 1b6a 186a 196a 1a83 0174 177c 1b6a  .|.j.j.j...t.|.j
+000018e0: 186a 196a 1b83 0117 0083 017d 1e74 1c6a  .j.j.......}.t.j
+000018f0: 1da0 1e7c 017c 1da1 027d 1f74 1c6a 1da0  ...|.|...}.t.j..
+00001900: 1f7c 1fa1 0190 0273 4674 1ca0 207c 1fa1  .|.....sFt.. |..
+00001910: 0101 007c 1b6a 2164 1a6b 0290 0272 a064  ...|.j!d.k...r.d
+00001920: 1b64 1c64 1d64 1b64 1c64 1e9c 057d 2074  .d.d.d.d.d...} t
+00001930: 22a0 2374 24a0 257c 207c 1b6a 2619 007c  ".#t$.%| |.j&..|
+00001940: 1b6a 277c 1b6a 2866 027c 1b6a 29a1 03a1  .j'|.j(f.|.j)...
+00001950: 017d 217c 1b6a 2664 1f6b 0290 0272 a074  .}!|.j&d.k...r.t
+00001960: 2aa0 2b7c 2174 2a6a 2ca1 027d 217c 1b6a  *.+|!t*j,..}!|.j
+00001970: 2164 206b 0290 0272 ce64 217c 1b6a 2d6b  !d k...r.d!|.j-k
+00001980: 0690 0272 c474 2ea0 2f7c 1ba1 017d 216e  ...r.t../|...}!n
+00001990: 0a74 2ea0 307c 1ba1 017d 217c 0564 226b  .t..0|...}!|.d"k
+000019a0: 0290 0272 e674 317c 197c 0264 238d 027d  ...r.t1|.|.d#..}
+000019b0: 226e 287c 0564 246b 0290 0272 fe74 317c  "n(|.d$k...r.t1|
+000019c0: 1e7c 0264 238d 027d 226e 1074 327c 0e7c  .|.d#..}"n.t2|.|
+000019d0: 1119 007c 0264 258d 027d 227c 1d9b 0064  ...|.d%..}"|...d
+000019e0: 267c 229b 009d 037d 2274 1c6a 1da0 1e7c  &|"....}"t.j...|
+000019f0: 1f7c 22a1 027d 237c 0690 0372 4874 336a  .|"..}#|...rHt3j
+00001a00: 347c 217c 0664 0619 007c 0664 1919 0064  4|!|.d...|.d...d
+00001a10: 278d 037d 2174 2aa0 357c 237c 21a1 0201  '..}!t*.5|#|!...
+00001a20: 007c 0490 0372 7674 367c 1e7c 197c 237c  .|...rvt6|.|.|#|
+00001a30: 0e7c 1119 0064 288d 047c 107c 1119 007c  .|...d(..|.|...|
+00001a40: 223c 007c 117c 0ea0 05a1 006b 0690 0372  "<.|.|.....k...r
+00001a50: 947c 0e7c 1105 0019 0064 1937 0003 003c  .|.|.....d.7...<
+00001a60: 007c 16a0 3764 19a1 0101 0090 0171 7857  .|..7d.......qxW
+00001a70: 0035 0051 0052 0058 0074 3883 007d 247c  .5.Q.R.X.t8..}$|
+00001a80: 0490 0472 447c 10a0 05a1 0044 005d 827d  ...rD|.....D.].}
+00001a90: 2574 1c6a 1da0 1e7c 0174 167c 2583 01a1  %t.j...|.t.|%...
+00001aa0: 027d 1f7c 24a0 397c 1fa1 0101 0074 1c6a  .}.|$.9|.....t.j
+00001ab0: 1da0 1f7c 1fa1 0190 0373 f874 1ca0 207c  ...|.....s.t.. |
+00001ac0: 1fa1 0101 0074 0483 007d 267c 107c 2519  .....t...}&|.|%.
+00001ad0: 007c 2664 293c 007c 0b7c 2519 007c 2664  .|&d)<.|.|%..|&d
+00001ae0: 2a3c 0074 1c6a 1da0 1e7c 1f74 3a83 00a1  *<.t.j...|.t:...
+00001af0: 027d 2774 1c6a 1da0 1f7c 27a1 0190 0373  .}'t.j...|'....s
+00001b00: c074 3ba0 3c7c 267c 27a1 0201 0090 0371  .t;.<|&|'......q
+00001b10: c057 0035 0051 0052 0058 007c 2453 0029  .W.5.Q.R.X.|$S.)
+00001b20: 2b61 2601 0000 0a20 2020 2041 7267 733a  +a&....    Args:
+00001b30: 0a20 2020 2020 2020 2072 6f73 6261 675f  .        rosbag_
+00001b40: 7061 7468 2028 7374 7229 3a0a 2020 2020  path (str):.    
+00001b50: 2020 2020 6f75 7470 7574 5f66 6f6c 6465      output_folde
+00001b60: 7220 2873 7472 293a 0a20 2020 2020 2020  r (str):.       
+00001b70: 2066 696c 655f 666f 726d 6174 2028 7374   file_format (st
+00001b80: 7229 3a0a 2020 2020 2020 2020 746f 7069  r):.        topi
+00001b90: 6373 2028 6c69 7374 293a 0a20 2020 2020  cs (list):.     
+00001ba0: 2020 2063 7265 6174 655f 6d61 6e69 6665     create_manife
+00001bb0: 7374 2028 626f 6f6c 293a 0a20 2020 2020  st (bool):.     
+00001bc0: 2020 206e 616d 696e 6720 2873 7472 293a     naming (str):
+00001bd0: 0a20 2020 2020 2020 2072 6573 697a 6520  .        resize 
+00001be0: 286c 6973 7429 3a0a 2020 2020 2020 2020  (list):.        
+00001bf0: 7361 6d70 6c65 2028 696e 7429 3a0a 2020  sample (int):.  
+00001c00: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
+00001c10: 2028 666c 6f61 7429 3a0a 2020 2020 2020   (float):.      
+00001c20: 2020 656e 645f 7469 6d65 2028 666c 6f61    end_time (floa
+00001c30: 7429 3a0a 0a20 2020 2052 6574 7572 6e73  t):..    Returns
+00001c40: 3a20 4e6f 6e65 0a0a 2020 2020 2901 720f  : None..    ).r.
+00001c50: 0000 0029 0172 2600 0000 4e72 1600 0000  ...).r&...Nr....
+00001c60: 7244 0000 0072 0100 0000 7a0a 526f 626f  rD...r....z.Robo
+00001c70: 6c6f 6773 3a20 7a19 206e 6f74 2069 6e20  logs: z. not in 
+00001c80: 524f 5342 6167 2e2e 736b 6970 7069 6e67  ROSBag..skipping
+00001c90: 2e7a 0d4d 6573 7361 6765 2043 6f75 6e74  .z.Message Count
+00001ca0: 7212 0000 0072 1300 0000 7256 0000 007a  r....r....rV...z
+00001cb0: 2852 6f62 6f6c 6f67 733a 206e 6f20 696d  (Robologs: no im
+00001cc0: 6167 6520 746f 7069 6373 2074 6f20 6578  age topics to ex
+00001cd0: 7472 6163 7420 696e 207a 032e 2e2e 7a1e  tract in z....z.
+00001ce0: 526f 626f 6c6f 6773 3a20 6578 7472 6163  Robologs: extrac
+00001cf0: 7469 6e67 2069 6d61 6765 732e 2e2e 7a19  ting images...z.
+00001d00: 526f 626f 6c6f 6773 3a20 6974 6572 6174  Robologs: iterat
+00001d10: 696e 6720 6f76 6572 207a 1420 696d 6167  ing over z. imag
+00001d20: 6573 2074 6f20 6578 7472 6163 743a 207a  es to extract: z
+00001d30: 0720 696d 6167 6573 6301 0000 0000 0000  . imagesc.......
+00001d40: 0000 0000 0002 0000 0004 0000 0013 0000  ................
+00001d50: 0073 1a00 0000 6700 7c00 5d12 7d01 7c01  .s....g.|.].}.|.
+00001d60: 6a00 8800 6b06 7204 7c01 9102 7104 5300  j...k.r.|...q.S.
+00001d70: 7223 0000 0029 0172 6000 0000 723f 0000  r#...).r`...r?..
+00001d80: 00a9 0172 1600 0000 7223 0000 0072 2400  ...r....r#...r$.
+00001d90: 0000 7243 0000 0050 0100 0073 0600 0000  ..rC...P...s....
+00001da0: 0600 0200 0a00 7a27 6765 745f 696d 6167  ......z'get_imag
+00001db0: 6573 5f66 726f 6d5f 6261 672e 3c6c 6f63  es_from_bag.<loc
+00001dc0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
+00001dd0: 3852 6f62 6f6c 6f67 733a 206e 6f6e 6520  8Robologs: none 
+00001de0: 6f66 2074 6865 2073 656c 6563 7465 6420  of the selected 
+00001df0: 746f 7069 6373 2061 7265 2069 6e20 7468  topics are in th
+00001e00: 6520 524f 5342 6167 2e29 01da 0574 6f74  e ROSBag.)...tot
+00001e10: 616c 2901 da0b 636f 6e6e 6563 7469 6f6e  al)...connection
+00001e20: 7367 95d6 26e8 0b2e 113e 7253 0000 007a  sg..&....>rS...z
+00001e30: 1573 656e 736f 725f 6d73 6773 2f6d 7367  .sensor_msgs/msg
+00001e40: 2f49 6d61 6765 da03 5247 42da 0452 4742  /Image..RGB..RGB
+00001e50: 41da 014c 2905 5a04 7267 6238 5a05 7267  A..L).Z.rgb8Z.rg
+00001e60: 6261 385a 056d 6f6e 6f38 5a04 3855 4333  ba8Z.mono8Z.8UC3
+00001e70: da05 6267 7261 3872 7500 0000 7a1f 7365  ..bgra8ru...z.se
+00001e80: 6e73 6f72 5f6d 7367 732f 6d73 672f 436f  nsor_msgs/msg/Co
+00001e90: 6d70 7265 7373 6564 496d 6167 655a 0f63  mpressedImageZ.c
+00001ea0: 6f6d 7072 6573 7365 6444 6570 7468 7233  ompressedDepthr3
+00001eb0: 0000 0029 0272 4700 0000 7248 0000 0072  ...).rG...rH...r
+00001ec0: 3200 0000 2902 7235 0000 0072 4800 0000  2...).r5...rH...
+00001ed0: 7238 0000 0029 03da 0369 6d67 5a09 6e65  r8...)...imgZ.ne
+00001ee0: 775f 7769 6474 685a 0a6e 6577 5f68 6569  w_widthZ.new_hei
+00001ef0: 6768 7429 0472 3200 0000 7233 0000 0072  ght).r2...r3...r
+00001f00: 3400 0000 7235 0000 00da 0669 6d61 6765  4...r5.....image
+00001f10: 7372 6000 0000 293d 7225 0000 0072 2a00  sr`...)=r%...r*.
+00001f20: 0000 723b 0000 0072 4500 0000 721c 0000  ..r;...rE...r...
+00001f30: 00da 046b 6579 73da 076c 6f67 6769 6e67  ...keys..logging
+00001f40: da07 7761 726e 696e 6772 5a00 0000 da03  ..warningrZ.....
+00001f50: 696e 74da 0564 6562 7567 da05 7072 696e  int..debug..prin
+00001f60: 7472 0800 0000 7271 0000 0072 0b00 0000  tr....rq...r....
+00001f70: da09 656e 756d 6572 6174 65da 086d 6573  ..enumerate..mes
+00001f80: 7361 6765 7372 6000 0000 7209 0000 0072  sagesr`...r....r
+00001f90: 0a00 0000 5a07 6d73 6774 7970 6572 5c00  ....Z.msgtyper\.
+00001fa0: 0000 7255 0000 0072 4a00 0000 da06 6865  ..rU...rJ.....he
+00001fb0: 6164 6572 da05 7374 616d 70da 0373 6563  ader..stamp..sec
+00001fc0: 5a07 6e61 6e6f 7365 6372 1700 0000 7218  Z.nanosecr....r.
+00001fd0: 0000 0072 2f00 0000 7219 0000 00da 086d  ...r/...r......m
+00001fe0: 616b 6564 6972 735a 0b5f 5f6d 7367 7479  akedirsZ.__msgty
+00001ff0: 7065 5f5f da02 6e70 da05 6172 7261 7972  pe__..np..arrayr
+00002000: 0600 0000 da09 6672 6f6d 6279 7465 73da  ......frombytes.
+00002010: 0865 6e63 6f64 696e 67da 0577 6964 7468  .encoding..width
+00002020: da06 6865 6967 6874 da04 6461 7461 da03  ..height..data..
+00002030: 6376 325a 0863 7674 436f 6c6f 725a 0f43  cv2Z.cvtColorZ.C
+00002040: 4f4c 4f52 5f42 4752 4132 5247 4241 da06  OLOR_BGRA2RGBA..
+00002050: 666f 726d 6174 720c 0000 005a 1f63 6f6e  formatr....Z.con
+00002060: 7665 7274 5f63 6f6d 7072 6573 7365 645f  vert_compressed_
+00002070: 6465 7074 685f 746f 5f63 7632 5a14 636f  depth_to_cv2Z.co
+00002080: 6e76 6572 745f 696d 6167 655f 746f 5f63  nvert_image_to_c
+00002090: 7632 724b 0000 0072 4f00 0000 720e 0000  v2rK...rO...r...
+000020a0: 005a 0c72 6573 697a 655f 696d 6167 655a  .Z.resize_imageZ
+000020b0: 0769 6d77 7269 7465 7239 0000 00da 0675  .imwriter9.....u
+000020c0: 7064 6174 65da 046c 6973 74da 0661 7070  pdate..list..app
+000020d0: 656e 6472 5d00 0000 720d 0000 00da 0973  endr]...r......s
+000020e0: 6176 655f 6a73 6f6e 2928 720f 0000 0072  ave_json)(r....r
+000020f0: 6a00 0000 7248 0000 0072 1600 0000 726b  j...rH...r....rk
+00002100: 0000 0072 6c00 0000 726d 0000 0072 6e00  ...rl...rm...rn.
+00002110: 0000 7212 0000 0072 1300 0000 7226 0000  ..r....r....r&..
+00002120: 0072 2800 0000 5a0f 616c 6c5f 746f 7069  .r(...Z.all_topi
+00002130: 6373 5f64 6963 745a 0f69 6d67 5f74 6f70  cs_dictZ.img_top
+00002140: 6963 5f74 7970 6573 5a16 746f 7069 635f  ic_typesZ.topic_
+00002150: 6d73 675f 636f 756e 7465 725f 6469 6374  msg_counter_dict
+00002160: 5a16 746f 7461 6c5f 6e75 6d62 6572 5f6f  Z.total_number_o
+00002170: 665f 696d 6167 6573 5a0d 6d61 6e69 6665  f_imagesZ.manife
+00002180: 7374 5f64 6963 7472 6000 0000 5a12 6e72  st_dictr`...Z.nr
+00002190: 5f69 6d67 735f 746f 5f65 7874 7261 6374  _imgs_to_extract
+000021a0: 5a0f 6669 6c74 6572 5f64 7572 6174 696f  Z.filter_duratio
+000021b0: 6eda 0672 6561 6465 7272 7100 0000 5a04  n..readerrq...Z.
+000021c0: 7062 6172 da02 6974 da0a 636f 6e6e 6563  pbar..it..connec
+000021d0: 7469 6f6e 725b 0000 00da 0772 6177 6461  tionr[.....rawda
+000021e0: 7461 da03 6d73 675a 0d72 6f73 6261 675f  ta..msgZ.rosbag_
+000021f0: 7469 6d65 5f73 5a15 746f 7069 635f 6e61  time_sZ.topic_na
+00002200: 6d65 5f75 6e64 6572 7363 6f72 6572 3200  me_underscorer2.
+00002210: 0000 5a20 6f75 7470 7574 5f69 6d61 6765  ..Z output_image
+00002220: 735f 666f 6c64 6572 5f66 6f6c 6465 725f  s_folder_folder_
+00002230: 7061 7468 5a0d 696d 675f 656e 636f 6469  pathZ.img_encodi
+00002240: 6e67 735a 0863 765f 696d 6167 655a 0a69  ngsZ.cv_imageZ.i
+00002250: 6d61 6765 5f6e 616d 655a 0a69 6d61 6765  mage_nameZ.image
+00002260: 5f70 6174 685a 176f 7574 7075 745f 696d  _pathZ.output_im
+00002270: 6773 5f66 6f6c 6465 725f 6c69 7374 da03  gs_folder_list..
+00002280: 6b65 795a 0b6f 7574 7075 745f 6469 6374  keyZ.output_dict
+00002290: 5a19 6f75 7470 7574 5f70 6174 685f 6d61  Z.output_path_ma
+000022a0: 6e69 6665 7374 5f6a 736f 6e72 2300 0000  nifest_jsonr#...
+000022b0: 726f 0000 0072 2400 0000 da13 6765 745f  ro...r$.....get_
+000022c0: 696d 6167 6573 5f66 726f 6d5f 6261 6704  images_from_bag.
+000022d0: 0100 0073 c600 0000 001d 0a01 0a01 0401  ...s............
+000022e0: 0402 0401 0801 0601 0c01 0601 0401 0602  ................
+000022f0: 0801 0c01 1201 0202 0801 1001 0c02 0402  ................
+00002300: 0801 0201 0201 0201 0601 06fc 0606 1002  ................
+00002310: 0c02 0401 0802 0401 1202 0402 0a01 1602  ................
+00002320: 0c01 1402 0601 0a01 0e02 0e01 2001 0601  ............ ...
+00002330: 1401 0801 0e01 1001 0402 1801 1001 0402  ................
+00002340: 0802 2002 0e02 0e01 0a02 0c01 1001 2401  .. ...........$.
+00002350: 0c01 0e02 0c01 0c01 0c02 0a02 0a01 0e02  ................
+00002360: 0a01 0e03 1002 0e02 0e02 0601 1802 0c02  ................
+00002370: 0601 0201 0201 0201 0201 06fc 0e07 0e01  ................
+00002380: 1002 1802 0602 0601 0c01 1201 0a01 0e01  ................
+00002390: 0a02 0601 0c01 0c02 1003 0e01 1a02 7297  ..............r.
+000023a0: 0000 00a9 02da 086f 6666 7365 745f 73da  .......offset_s.
+000023b0: 1466 6972 7374 5f72 6f73 6261 675f 7469  .first_rosbag_ti
+000023c0: 6d65 5f6e 7363 0200 0000 0000 0000 0000  me_nsc..........
+000023d0: 0000 0300 0000 0300 0000 4300 0000 7314  ..........C...s.
+000023e0: 0000 0074 007c 0064 0114 0083 017d 027c  ...t.|.d.....}.|
+000023f0: 027c 0117 0053 0029 024e 6700 0000 0065  .|...S.).Ng....e
+00002400: cdcd 4129 0172 7b00 0000 2903 7299 0000  ..A).r{...).r...
+00002410: 0072 9a00 0000 5a09 6f66 6673 6574 5f6e  .r....Z.offset_n
+00002420: 7372 2300 0000 7223 0000 0072 2400 0000  sr#...r#...r$...
+00002430: da1d 636f 6e76 6572 745f 6f66 6673 6574  ..convert_offset
+00002440: 5f73 5f74 6f5f 726f 7362 6167 5f6e 73ad  _s_to_rosbag_ns.
+00002450: 0100 0073 0400 0000 0002 0c01 729b 0000  ...s........r...
+00002460: 0029 04da 0774 696d 655f 6e73 da14 7374  .)...time_ns..st
+00002470: 6172 745f 7469 6d65 5f72 6f73 6261 675f  art_time_rosbag_
+00002480: 6e73 da12 656e 645f 7469 6d65 5f72 6f73  ns..end_time_ros
+00002490: 6261 675f 6e73 7210 0000 0063 0300 0000  bag_nsr....c....
+000024a0: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+000024b0: 4300 0000 7324 0000 007c 0172 107c 007c  C...s$...|.r.|.|
+000024c0: 016b 0072 1064 0153 007c 0272 207c 007c  .k.r.d.S.|.r |.|
+000024d0: 026b 0472 2064 0253 0064 0353 0029 0461  .k.r d.S.d.S.).a
+000024e0: 7b01 0000 0a20 2020 2054 6869 7320 6675  {....    This fu
+000024f0: 6e63 7469 6f6e 2063 6865 636b 7320 6966  nction checks if
+00002500: 2061 2074 696d 6573 7461 6d70 2069 7320   a timestamp is 
+00002510: 7769 7468 696e 6720 6120 7370 6563 6966  withing a specif
+00002520: 6965 6420 7469 6d65 7261 6e67 6520 616e  ied timerange an
+00002530: 6420 7265 7475 726e 7320 5472 7565 206f  d returns True o
+00002540: 7220 4661 6c73 6520 6966 2077 6520 6172  r False if we ar
+00002550: 652e 2049 7420 616c 736f 0a20 2020 2072  e. It also.    r
+00002560: 6574 7572 6e73 2061 2073 6563 6f6e 6420  eturns a second 
+00002570: 626f 6f6c 6561 6e20 746f 2069 6e64 6963  boolean to indic
+00002580: 6174 6520 6966 2077 6520 6172 6520 7061  ate if we are pa
+00002590: 7374 2074 6865 2065 6e64 2074 696d 652e  st the end time.
+000025a0: 2054 6869 7320 6361 6e20 6265 2075 7365   This can be use
+000025b0: 6420 746f 2062 7265 616b 206f 7574 206f  d to break out o
+000025c0: 6620 7468 6520 6c6f 6f70 2065 6172 6c79  f the loop early
+000025d0: 2e0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000025e0: 2020 2020 7469 6d65 5f6e 7320 2869 6e74      time_ns (int
+000025f0: 293a 0a20 2020 2020 2020 2073 7461 7274  ):.        start
+00002600: 5f74 696d 655f 726f 7362 6167 5f6e 7320  _time_rosbag_ns 
+00002610: 2869 6e74 293a 0a20 2020 2020 2020 2065  (int):.        e
+00002620: 6e64 5f74 696d 655f 726f 7362 6167 5f6e  nd_time_rosbag_n
+00002630: 7320 2869 6e74 293a 0a0a 2020 2020 5265  s (int):..    Re
+00002640: 7475 726e 733a 2054 7572 706c 6520 6f66  turns: Turple of
+00002650: 2062 6f6f 6c65 616e 730a 0a20 2020 2029   booleans..    )
+00002660: 0246 4629 0246 5429 0254 4672 2300 0000  .FF).FT).TFr#...
+00002670: a903 729c 0000 0072 9d00 0000 729e 0000  ..r....r....r...
+00002680: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00002690: da1c 6973 5f6d 6573 7361 6765 5f77 6974  ..is_message_wit
+000026a0: 6869 6e5f 7469 6d65 5f72 616e 6765 b301  hin_time_range..
+000026b0: 0000 730e 0000 0000 0f04 0108 0104 0204  ..s.............
+000026c0: 0108 0104 0272 a000 0000 da09 726f 7362  .....r......rosb
+000026d0: 6167 5f6e 7329 06da 0e69 6e70 7574 5f62  ag_ns)...input_b
+000026e0: 6167 5f70 6174 68da 0f6f 7574 7075 745f  ag_path..output_
+000026f0: 6261 675f 7061 7468 da0a 746f 7069 635f  bag_path..topic_
+00002700: 6c69 7374 7212 0000 0072 1300 0000 da0e  listr....r......
+00002710: 7469 6d65 7374 616d 705f 7479 7065 6306  timestamp_typec.
+00002720: 0000 0000 0000 0000 0000 000e 0000 0009  ................
+00002730: 0000 0043 0000 0073 d000 0000 7c05 6401  ...C...s....|.d.
+00002740: 6b07 7216 7400 6402 7c05 9b00 9d02 8301  k.r.t.d.|.......
+00002750: 8201 7401 7c01 6403 8302 8fa6 7d06 6404  ..t.|.d.....}.d.
+00002760: 7d07 6405 7d08 7401 7c00 8301 a002 a100  }.d.}.t.|.......
+00002770: 4400 5d8a 5c03 7d09 7d0a 7d0b 7c08 6404  D.].\.}.}.}.|.d.
+00002780: 6b00 7278 7c0b a003 a100 7d08 7c05 6406  k.rx|.....}.|.d.
+00002790: 6b02 7278 7c03 7268 7404 7c03 7c08 6407  k.rx|.rht.|.|.d.
+000027a0: 8d02 7d03 7c04 7278 7404 7c04 7c08 6407  ..}.|.rxt.|.|.d.
+000027b0: 8d02 7d04 7c02 7286 7c09 7c02 6b07 7286  ..}.|.r.|.|.k.r.
+000027c0: 7136 7405 7c0b a003 a100 7c03 7c04 6408  q6t.|.....|.|.d.
+000027d0: 8d03 5c02 7d0c 7d0d 7c0d 72a4 0100 71c2  ..\.}.}.|.r...q.
+000027e0: 7c0c 73aa 7136 7c07 6409 3700 7d07 7c06  |.s.q6|.d.7.}.|.
+000027f0: a006 7c09 7c0a 7c0b a103 0100 7136 5700  ..|.|.|.....q6W.
+00002800: 3500 5100 5200 5800 640a 5300 290b 7ab3  5.Q.R.X.d.S.).z.
+00002810: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+00002820: 2020 2069 6e70 7574 5f62 6167 5f70 6174     input_bag_pat
+00002830: 6820 2829 3a0a 2020 2020 2020 2020 6f75  h ():.        ou
+00002840: 7470 7574 5f62 6167 5f70 6174 6820 2829  tput_bag_path ()
+00002850: 3a0a 2020 2020 2020 2020 746f 7069 635f  :.        topic_
+00002860: 6c69 7374 2028 293a 0a20 2020 2020 2020  list ():.       
+00002870: 2073 7461 7274 5f74 696d 6520 2829 3a0a   start_time ():.
+00002880: 2020 2020 2020 2020 656e 645f 7469 6d65          end_time
+00002890: 2028 293a 0a20 2020 2020 2020 2074 696d   ():.        tim
+000028a0: 6573 7461 6d70 5f74 7970 6520 2829 3a0a  estamp_type ():.
+000028b0: 0a20 2020 2052 6574 7572 6e73 3a0a 0a20  .    Returns:.. 
+000028c0: 2020 2029 0272 a100 0000 7299 0000 007a     ).r....r....z
+000028d0: 2c52 6f62 6f6c 6f67 733a 2069 6e76 616c  ,Robologs: inval
+000028e0: 6964 2074 696d 6573 7461 6d70 5f74 7970  id timestamp_typ
+000028f0: 6520 7061 7261 6d65 7465 723a 20da 0177  e parameter: ..w
+00002900: 7201 0000 00e9 ffff ffff 7299 0000 0072  r.........r....r
+00002910: 9800 0000 729f 0000 0072 5300 0000 4e29  ....r....rS...N)
+00002920: 0772 1a00 0000 7207 0000 00da 0d72 6561  .r....r......rea
+00002930: 645f 6d65 7373 6167 6573 da07 746f 5f6e  d_messages..to_n
+00002940: 7365 6372 9b00 0000 72a0 0000 00da 0577  secr....r......w
+00002950: 7269 7465 290e 72a2 0000 0072 a300 0000  rite).r....r....
+00002960: 72a4 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00002970: a500 0000 da06 6f75 7462 6167 5a0b 6d73  ......outbagZ.ms
+00002980: 675f 636f 756e 7465 725a 1066 6972 7374  g_counterZ.first
+00002990: 5f74 696d 655f 7374 616d 7072 6000 0000  _time_stampr`...
+000029a0: 7295 0000 0072 5b00 0000 5a0d 696e 5f74  r....r[...Z.in_t
+000029b0: 696d 655f 7261 6e67 655a 0d70 6173 745f  ime_rangeZ.past_
+000029c0: 656e 645f 7469 6d65 7223 0000 0072 2300  end_timer#...r#.
+000029d0: 0000 7224 0000 00da 1467 6574 5f63 6c69  ..r$.....get_cli
+000029e0: 7070 6564 5f62 6167 5f66 696c 65cd 0100  pped_bag_file...
+000029f0: 0073 4200 0000 0015 0801 0e02 0c01 0401  .sB.............
+00002a00: 0401 1602 0801 0801 0801 0401 0201 0200  ................
+00002a10: 02ff 0603 0401 0201 0200 02ff 0604 0401  ................
+00002a20: 0801 0202 0801 0201 02fe 0a05 0401 0402  ................
+00002a30: 0401 0202 0801 1a02 72ac 0000 0029 0172  ........r....).r
+00002a40: 4600 0000 2902 7246 0000 0072 4c00 0000  F...).rF...rL...
+00002a50: 2901 7238 0000 0029 0154 2908 7246 0000  ).r8...).T).rF..
+00002a60: 004e 5472 6900 0000 4e4e 4e4e 2902 4e4e  .NTri...NNNN).NN
+00002a70: 2904 4e4e 4e72 a100 0000 2933 da07 5f5f  ).NNNr....)3..__
+00002a80: 646f 635f 5f72 2e00 0000 7279 0000 0072  doc__r....ry...r
+00002a90: 1700 0000 da06 7479 7069 6e67 7202 0000  ......typingr...
+00002aa0: 0072 0300 0000 7204 0000 0072 8b00 0000  .r....r....r....
+00002ab0: da05 6e75 6d70 7972 8400 0000 da05 6261  ..numpyr......ba
+00002ac0: 6770 7972 0500 0000 da03 5049 4c72 0600  gpyr......PILr..
+00002ad0: 0000 da06 726f 7362 6167 7207 0000 005a  ....rosbagr....Z
+00002ae0: 0f72 6f73 6261 6773 2e72 6f73 6261 6731  .rosbags.rosbag1
+00002af0: 7208 0000 005a 0d72 6f73 6261 6773 2e73  r....Z.rosbags.s
+00002b00: 6572 6465 7209 0000 0072 0a00 0000 720b  erder....r....r.
+00002b10: 0000 00da 1f72 6f62 6f6c 6f67 735f 726f  .....robologs_ro
+00002b20: 735f 7574 696c 732e 736f 7572 6365 732e  s_utils.sources.
+00002b30: 726f 7331 720c 0000 00da 1872 6f62 6f6c  ros1r......robol
+00002b40: 6f67 735f 726f 735f 7574 696c 732e 7574  ogs_ros_utils.ut
+00002b50: 696c 7372 0d00 0000 720e 0000 0072 4a00  ilsr....r....rJ.
+00002b60: 0000 721c 0000 0072 2500 0000 722a 0000  ..r....r%...r*..
+00002b70: 0072 3100 0000 727b 0000 0072 3900 0000  .r1...r{...r9...
+00002b80: 723b 0000 0072 8e00 0000 7245 0000 0072  r;...r....rE...r
+00002b90: 4b00 0000 724f 0000 0072 5500 0000 7259  K...rO...rU...rY
+00002ba0: 0000 0072 5a00 0000 da04 626f 6f6c 725c  ...rZ.....boolr\
+00002bb0: 0000 0072 5d00 0000 7268 0000 0072 9700  ...r]...rh...r..
+00002bc0: 0000 729b 0000 0072 a000 0000 72ac 0000  ..r....r....r...
+00002bd0: 0072 2300 0000 7223 0000 0072 2300 0000  .r#...r#...r#...
+00002be0: 7224 0000 00da 083c 6d6f 6475 6c65 3e01  r$.....<module>.
+00002bf0: 0000 0073 8c00 0000 0405 0801 0801 0801  ...s............
+00002c00: 1402 0801 0801 0c01 0c01 0c01 0c01 1001  ................
+00002c10: 0c02 0c01 0c01 0c03 1023 100a 1015 1615  .........#......
+00002c20: 0808 120c 140d 160e 140c 1c1d 1421 0808  .............!..
+00002c30: 1416 0001 0001 0001 0001 0001 0001 0001  ................
+00002c40: 00f6 0201 0201 0201 0201 0601 0201 0201  ................
+00002c50: 0601 0601 0601 06f6 0c7f 002a 1007 0000  ...........*....
+00002c60: 00ff 0201 0200 0600 0601 0afe 0c1d 0001  ................
+00002c70: 0001 0001 00fa 0201 0201 0201 0601 0e01  ................
+00002c80: 0e01 02fa                                ....
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/argument_parsers.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/argument_parsers.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/clip_rosbag.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/clip_rosbag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 
 import click
 
 from robologs_ros_utils.sources.ros1 import ros_utils
-from robologs_ros_utils.utils.file_utils import file_utils
+from robologs_ros_utils.utils import file_utils
 
 
 @click.command()
 @click.option("--input", "-i", type=str, required=True, help="A single rosbag or folder with rosbags")
 @click.option("--output", "-o", type=str, required=True, help="Output directory")
 @click.option("--topics", type=str, help="Topic names used for extraction, comma-separated list")
 @click.option("--start-time", type=float, help="Only extract from start time")
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/get_images_from_bag.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/get_images_from_bag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 
 import click
 
 from robologs_ros_utils.sources.ros1 import argument_parsers, ros_utils
-from robologs_ros_utils.utils.file_utils import file_utils
+from robologs_ros_utils.utils import file_utils
 
 
 @click.command()
 @click.option("--input", "-i", type=str, required=True, help="A single rosbag, or folder with rosbags")
 @click.option("--output", "-o", type=str, required=True, help="Output directory")
 @click.option("--format", "-f", type=str, default="jpg", help="Output image format")
 @click.option("--manifest", "-m", is_flag=True, help="Save manifest.json with timestamps and metadata")
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/get_summary_from_bag.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/get_summary_from_bag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 
 import click
 
 from robologs_ros_utils.sources.ros1 import ros_utils
-from robologs_ros_utils.utils.file_utils import file_utils
+from robologs_ros_utils.utils import file_utils
 
 
 @click.command()
 @click.option("--input", "-i", type=str, required=True, help="A single rosbag, or folder with rosbags")
 @click.option("--output", "-o", type=str, required=True, help="Output directory, or json path")
 @click.option("--file-name", "-f", type=str, default="rosbag_metadata.json", help="Output file name")
 def get_summary(input, output, file_name):
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/get_videos_from_bag.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/get_videos_from_bag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 
 import click
 
 from robologs_ros_utils.sources.ros1 import argument_parsers, ros_utils
-from robologs_ros_utils.utils.file_utils import file_utils
+from robologs_ros_utils.utils import file_utils
 
 
 @click.command()
 @click.option("--input", "-i", type=str, required=True, help="A single rosbag, or folder with rosbags")
 @click.option("--output", "-o", type=str, required=True, help="Output directory")
 @click.option("--format", "-f", type=str, default="jpg", help="Output image format")
 @click.option("--manifest", "-m", type=str, help="Save manifest.json with timestamps and metadata")
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/ros_img_tools.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/ros_img_tools.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/sources/ros1/ros_utils.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/sources/ros1/ros_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from PIL import Image
 from rosbag import Bag
 from rosbags.rosbag1 import Reader
 from rosbags.serde import deserialize_cdr, ros1_to_cdr
 from tqdm import tqdm
 
 from robologs_ros_utils.sources.ros1 import ros_img_tools
-from robologs_ros_utils.utils.file_utils import file_utils
-from robologs_ros_utils.utils.img_utils import img_utils
+from robologs_ros_utils.utils import file_utils
+from robologs_ros_utils.utils import img_utils
 
 
 def get_bag_info_from_file(rosbag_path: str) -> dict:
     """
     Args:
         rosbag_path (str): Input file path rosbag.
 
@@ -258,15 +258,15 @@
 
 
 def get_images_from_bag(
     rosbag_path: str,
     output_folder: str,
     file_format: str = "jpg",
     topics: Optional[list] = None,
-    create_manifest: bool = False,
+    create_manifest: bool = True,
     naming: str = "sequential",
     resize: Optional[list] = None,
     sample: Optional[int] = None,
     start_time: Optional[float] = None,
     end_time: Optional[float] = None,
 ):
     """
@@ -291,15 +291,14 @@
     if not rosbag_metadata_dict:
         return
 
     if not topics:
         all_topics_dict = rosbag_metadata_dict["topics"]
         img_topic_types = get_image_topic_types()
         topics = get_topic_names_of_type(all_topics=all_topics_dict, filter_topic_types=img_topic_types)
-
     topic_msg_counter_dict = dict()
     total_number_of_images = 0
     manifest_dict = dict()
 
     for topic in topics:
         if topic not in topic_dict.keys():
             logging.warning(f"Robologs: {topic} not in ROSBag..skipping.")
@@ -385,15 +384,15 @@
 
                 image_name = f"{topic_name_underscore}_{image_name}"
 
                 image_path = os.path.join(output_images_folder_folder_path, image_name)
 
                 if resize:
                     cv_image = img_utils.resize_image(img=cv_image, new_width=resize[0], new_height=resize[1])
-
+                
                 cv2.imwrite(image_path, cv_image)
 
                 if create_manifest:
                     manifest_dict[topic][image_name] = create_manifest_entry_dict(
                         msg_timestamp=msg_timestamp,
                         rosbag_timestamp=t,
                         file_path=image_path,
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/file_utils/__pycache__/file_utils.cpython-38.pyc` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/__pycache__/file_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 13:09:39 2023 UTC, .py size: 4615 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -33,295 +33,294 @@
 00000200: 7468 2028 7374 7229 3a20 6669 6c65 2070  th (str): file p
 00000210: 6174 680a 0a20 2020 2052 6574 7572 6e73  ath..    Returns
 00000220: 3a20 4120 6c69 7374 2077 6974 6820 7061  : A list with pa
 00000230: 7468 2063 6f6d 706f 6e65 6e74 730a 2020  th components.  
 00000240: 2020 2905 da02 6f73 7204 0000 00da 086e    )...osr......n
 00000250: 6f72 6d70 6174 68da 0573 706c 6974 da03  ormpath..split..
 00000260: 7365 70a9 0172 0400 0000 a900 720b 0000  sep..r......r...
-00000270: 00fa 5b2f 686f 6d65 2f79 7665 732f 436f  ..[/home/yves/Co
+00000270: 00fa 502f 686f 6d65 2f79 7665 732f 436f  ..P/home/yves/Co
 00000280: 6465 2f72 6f62 6f6c 6f67 732d 726f 732d  de/robologs-ros-
 00000290: 7574 696c 732f 7079 7468 6f6e 2f72 6f62  utils/python/rob
 000002a0: 6f6c 6f67 735f 726f 735f 7574 696c 732f  ologs_ros_utils/
 000002b0: 7574 696c 732f 6669 6c65 5f75 7469 6c73  utils/file_utils
-000002c0: 2f66 696c 655f 7574 696c 732e 7079 da19  /file_utils.py..
-000002d0: 7370 6c69 745f 666f 6c64 6572 5f70 6174  split_folder_pat
-000002e0: 685f 746f 5f6c 6973 740b 0000 0073 0400  h_to_list....s..
-000002f0: 0000 0008 0c01 720d 0000 0046 2903 7204  ......r....F).r.
-00000300: 0000 00da 1064 656c 6574 655f 6966 5f65  .....delete_if_e
-00000310: 7869 7374 7372 0500 0000 6302 0000 0000  xistsr....c.....
-00000320: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000330: 0000 0073 3400 0000 7c01 721a 7400 6a01  ...s4...|.r.t.j.
-00000340: a002 7c00 a101 721a 7403 a004 7c00 a101  ..|...r.t...|...
-00000350: 0100 7400 6a01 a002 7c00 a101 7330 7400  ..t.j...|...s0t.
-00000360: a005 7c00 a101 0100 6401 5300 2902 7ab9  ..|.....d.S.).z.
-00000370: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
-00000380: 6f6e 2063 7265 6174 6573 2061 2064 6972  on creates a dir
-00000390: 6563 746f 7279 2e0a 2020 2020 4172 6773  ectory..    Args
-000003a0: 3a0a 2020 2020 2020 2020 7061 7468 2028  :.        path (
-000003b0: 7374 7229 3a20 6469 7265 6374 6f72 7920  str): directory 
-000003c0: 7061 7468 0a20 2020 2020 2020 2064 656c  path.        del
-000003d0: 6574 655f 6966 5f65 7869 7374 7320 2862  ete_if_exists (b
-000003e0: 6f6f 6c29 3a20 6966 2054 7275 652c 2065  ool): if True, e
-000003f0: 7869 7374 696e 6720 6469 7265 6374 6f72  xisting director
-00000400: 7920 7769 6c6c 2062 6520 6465 6c65 7465  y will be delete
-00000410: 640a 0a20 2020 2052 6574 7572 6e73 3a20  d..    Returns: 
-00000420: 4e6f 6e65 0a20 2020 204e 2906 7206 0000  None.    N).r...
-00000430: 0072 0400 0000 da06 6578 6973 7473 da06  .r......exists..
-00000440: 7368 7574 696c da06 726d 7472 6565 da08  shutil..rmtree..
-00000450: 6d61 6b65 6469 7273 2902 7204 0000 0072  makedirs).r....r
-00000460: 0e00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-00000470: 0000 00da 1063 7265 6174 655f 6469 7265  .....create_dire
-00000480: 6374 6f72 7917 0000 0073 0c00 0000 0009  ctory....s......
-00000490: 0401 0c01 0a02 0c01 0a01 7213 0000 0063  ..........r....c
-000004a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000004b0: 0300 0000 4300 0000 731e 0000 0074 006a  ....C...s....t.j
-000004c0: 01a0 027c 00a1 0173 1a74 037c 009b 0064  ...|...s.t.|...d
-000004d0: 019d 0283 0182 0164 0253 0029 037a 940a  .......d.S.).z..
-000004e0: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-000004f0: 6e20 6368 6563 6b73 2069 6620 6120 6669  n checks if a fi
-00000500: 6c65 2065 7869 7374 732c 2061 6e64 0a20  le exists, and. 
-00000510: 2020 2072 6169 7365 7320 616e 2065 7863     raises an exc
-00000520: 6570 7469 6f6e 2069 6620 6e6f 740a 2020  eption if not.  
-00000530: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00000540: 7061 7468 2028 7374 7229 3a20 696e 7075  path (str): inpu
-00000550: 7420 6669 6c65 2070 6174 680a 0a20 2020  t file path..   
-00000560: 2052 6574 7572 6e73 3a20 4e6f 6e65 0a20   Returns: None. 
-00000570: 2020 207a 1020 646f 6573 206e 6f74 2065     z. does not e
-00000580: 7869 7374 2e4e 2904 7206 0000 0072 0400  xist.N).r....r..
-00000590: 0000 720f 0000 00da 0945 7863 6570 7469  ..r......Excepti
-000005a0: 6f6e 720a 0000 0072 0b00 0000 720b 0000  onr....r....r...
-000005b0: 0072 0c00 0000 da11 6368 6563 6b5f 6669  .r......check_fi
-000005c0: 6c65 5f65 7869 7374 7329 0000 0073 0600  le_exists)...s..
-000005d0: 0000 0009 0c01 0e01 7215 0000 0029 03da  ........r....)..
-000005e0: 0464 6174 6172 0400 0000 7205 0000 0063  .datar....r....c
-000005f0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000600: 0900 0000 4300 0000 732c 0000 0074 007c  ....C...s,...t.|
-00000610: 0164 0183 028f 187d 0274 016a 027c 007c  .d.....}.t.j.|.|
-00000620: 0264 0264 0364 048d 0401 0057 0035 0051  .d.d.d.....W.5.Q
-00000630: 0052 0058 0064 0553 0029 067a 700a 2020  .R.X.d.S.).zp.  
-00000640: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00000650: 7361 7665 7320 6120 6c69 7374 206f 720a  saves a list or.
-00000660: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00000670: 2020 6461 7461 2028 6469 6374 206f 7220    data (dict or 
-00000680: 6c69 7374 293a 0a20 2020 2020 2020 2070  list):.        p
-00000690: 6174 6820 2873 7472 293a 0a0a 2020 2020  ath (str):..    
-000006a0: 5265 7475 726e 733a 0a20 2020 20da 0177  Returns:.    ..w
-000006b0: e904 0000 0054 2902 da06 696e 6465 6e74  .....T)...indent
-000006c0: da09 736f 7274 5f6b 6579 734e 2903 da04  ..sort_keysN)...
-000006d0: 6f70 656e da04 6a73 6f6e da04 6475 6d70  open..json..dump
-000006e0: 2903 7216 0000 0072 0400 0000 5a06 665f  ).r....r....Z.f_
-000006f0: 6a73 6f6e 720b 0000 0072 0b00 0000 720c  jsonr....r....r.
-00000700: 0000 00da 0973 6176 655f 6a73 6f6e 3700  .....save_json7.
-00000710: 0000 7306 0000 0000 090c 011c 0272 1e00  ..s..........r..
-00000720: 0000 2901 da09 6a73 6f6e 5f70 6174 6863  ..)...json_pathc
-00000730: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000740: 0900 0000 4300 0000 7322 0000 0074 007c  ....C...s"...t.|
-00000750: 0083 018f 107d 0174 01a0 027c 01a1 017d  .....}.t...|...}
-00000760: 0257 0035 0051 0052 0058 007c 0253 0029  .W.5.Q.R.X.|.S.)
-00000770: 017a 8e0a 2020 2020 5468 6973 2066 756e  .z..    This fun
-00000780: 6374 696f 6e20 7265 6164 7320 6120 6a73  ction reads a js
-00000790: 6f6e 2066 696c 6520 616e 6420 7265 7475  on file and retu
-000007a0: 726e 2061 204a 534f 4e20 6f62 6a65 6374  rn a JSON object
-000007b0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-000007c0: 2020 206a 736f 6e5f 7061 7468 2028 7374     json_path (st
-000007d0: 7229 3a20 4a53 4f4e 2066 696c 6520 7061  r): JSON file pa
-000007e0: 7468 0a0a 2020 2020 5265 7475 726e 733a  th..    Returns:
-000007f0: 204a 534f 4e20 6f62 6a65 6374 0a20 2020   JSON object.   
-00000800: 2029 0372 1b00 0000 721c 0000 00da 046c   ).r....r......l
-00000810: 6f61 6429 0372 1f00 0000 da09 6a73 6f6e  oad).r......json
-00000820: 5f66 696c 6572 1600 0000 720b 0000 0072  _filer....r....r
-00000830: 0b00 0000 720c 0000 00da 0972 6561 645f  ....r......read_
-00000840: 6a73 6f6e 4600 0000 7306 0000 0000 080a  jsonF...s.......
-00000850: 0114 0172 2200 0000 2901 7205 0000 0063  ...r"...).r....c
-00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000870: 0300 0000 4300 0000 730c 0000 0074 0074  ....C...s....t.t
-00000880: 01a0 02a1 0083 0153 0029 017a 380a 2020  .......S.).z8.  
-00000890: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-000008a0: 7265 7475 726e 7320 6120 5555 4944 0a20  returns a UUID. 
-000008b0: 2020 2052 6574 7572 6e73 3a20 5555 4944     Returns: UUID
-000008c0: 0a20 2020 2029 03da 0373 7472 da04 7575  .    )...str..uu
-000008d0: 6964 da05 7575 6964 3472 0b00 0000 720b  id..uuid4r....r.
-000008e0: 0000 0072 0b00 0000 720c 0000 00da 0b63  ...r....r......c
-000008f0: 7265 6174 655f 7575 6964 5300 0000 7302  reate_uuidS...s.
-00000900: 0000 0000 0572 2600 0000 2903 da0f 7375  .....r&...)...su
-00000910: 625f 666f 6c64 6572 5f6e 616d 65da 0b73  b_folder_name..s
-00000920: 6561 7263 685f 7061 7468 7205 0000 0063  earch_pathr....c
-00000930: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00000940: 0600 0000 4300 0000 7348 0000 0067 007d  ....C...sH...g.}
-00000950: 0274 00a0 017c 01a1 0144 005d 345c 037d  .t...|...D.]4\.}
-00000960: 037d 047d 0574 027c 0383 0101 0074 027c  .}.}.t.|.....t.|
-00000970: 0483 0101 007c 007c 046b 0672 0e7c 02a0  .....|.|.k.r.|..
-00000980: 0374 006a 04a0 057c 03a1 01a1 0101 0071  .t.j...|.......q
-00000990: 0e7c 0253 0029 017a d00a 2020 2020 5468  .|.S.).z..    Th
-000009a0: 6973 2066 756e 6374 696f 6e20 6669 6e64  is function find
-000009b0: 7320 6120 6669 6c65 6e61 6d65 2069 6e20  s a filename in 
-000009c0: 6120 7375 6266 6f6c 6465 722e 0a20 2020  a subfolder..   
-000009d0: 2041 7267 733a 0a20 2020 2020 2020 2073   Args:.        s
-000009e0: 7562 5f66 6f6c 6465 725f 6e61 6d65 2028  ub_folder_name (
-000009f0: 7374 7229 3a20 6e61 6d65 206f 6620 7375  str): name of su
-00000a00: 6266 6f6c 6465 720a 2020 2020 2020 2020  bfolder.        
-00000a10: 7365 6172 6368 5f70 6174 6820 2873 7472  search_path (str
-00000a20: 293a 2070 6174 6820 6f66 2066 6f6c 6465  ): path of folde
-00000a30: 7220 746f 2062 6520 7365 6172 6368 6564  r to be searched
-00000a40: 0a0a 2020 2020 5265 7475 726e 733a 2041  ..    Returns: A
-00000a50: 206c 6973 7420 7769 7468 2066 696c 656e   list with filen
-00000a60: 616d 6573 0a20 2020 2029 0672 0600 0000  ames.    ).r....
-00000a70: da04 7761 6c6b da05 7072 696e 74da 0661  ..walk..print..a
-00000a80: 7070 656e 6472 0400 0000 da04 6a6f 696e  ppendr......join
-00000a90: 2906 7227 0000 0072 2800 0000 da06 7265  ).r'...r(.....re
-00000aa0: 7375 6c74 da04 726f 6f74 da03 6469 72da  sult..root..dir.
-00000ab0: 0566 696c 6573 720b 0000 0072 0b00 0000  .filesr....r....
-00000ac0: 720c 0000 00da 0f66 696e 645f 7375 625f  r......find_sub_
-00000ad0: 666f 6c64 6572 5b00 0000 730e 0000 0000  folder[...s.....
-00000ae0: 0a04 0114 0108 0108 0108 0114 0172 3100  .............r1.
-00000af0: 0000 2903 da0d 7061 7468 5f7a 6970 5f66  ..)...path_zip_f
-00000b00: 696c 65da 0d6f 7574 7075 745f 666f 6c64  ile..output_fold
-00000b10: 6572 7205 0000 0063 0200 0000 0000 0000  err....c........
-00000b20: 0000 0000 0300 0000 0900 0000 4300 0000  ............C...
-00000b30: 7324 0000 0074 007c 0064 0183 028f 107d  s$...t.|.d.....}
-00000b40: 027c 02a0 017c 01a1 0101 0057 0035 0051  .|...|.....W.5.Q
-00000b50: 0052 0058 0064 0253 0029 037a d50a 2020  .R.X.d.S.).z..  
-00000b60: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00000b70: 756e 7a69 7073 2061 2066 696c 6520 746f  unzips a file to
-00000b80: 2061 2073 7065 6369 6669 6320 666f 6c64   a specific fold
-00000b90: 6572 206c 6f63 6174 696f 6e2e 0a20 2020  er location..   
-00000ba0: 2041 7267 733a 0a20 2020 2020 2020 2070   Args:.        p
-00000bb0: 6174 685f 7a69 705f 6669 6c65 2028 7374  ath_zip_file (st
-00000bc0: 7229 3a20 6162 736f 6c75 7465 2070 6174  r): absolute pat
-00000bd0: 6820 6f66 202e 7a69 7020 6669 6c65 0a20  h of .zip file. 
-00000be0: 2020 2020 2020 206f 7574 7075 745f 666f         output_fo
-00000bf0: 6c64 6572 2028 7374 7229 3a20 6162 736f  lder (str): abso
-00000c00: 6c75 7465 2070 6174 6820 6f66 206f 7574  lute path of out
-00000c10: 7075 7420 666f 6c64 6572 0a0a 2020 2020  put folder..    
-00000c20: 5265 7475 726e 733a 204e 6f6e 650a 2020  Returns: None.  
-00000c30: 2020 da01 724e 2902 7203 0000 00da 0a65    ..rN).r......e
-00000c40: 7874 7261 6374 616c 6c29 0372 3200 0000  xtractall).r2...
-00000c50: 7233 0000 005a 067a 6970 4f62 6a72 0b00  r3...Z.zipObjr..
-00000c60: 0000 720b 0000 0072 0c00 0000 da14 756e  ..r....r......un
-00000c70: 7a69 705f 6669 6c65 5f74 6f5f 666f 6c64  zip_file_to_fold
-00000c80: 6572 6e00 0000 7306 0000 0000 090c 0114  ern...s.........
-00000c90: 0172 3600 0000 2903 da0d 7061 7468 5f74  .r6...)...path_t
-00000ca0: 6172 5f66 696c 6572 3300 0000 7205 0000  ar_filer3...r...
-00000cb0: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
-00000cc0: 0000 0300 0000 4300 0000 7320 0000 0074  ......C...s ...t
-00000cd0: 00a0 017c 00a1 017d 027c 02a0 027c 01a1  ...|...}.|...|..
-00000ce0: 0101 007c 02a0 03a1 0001 0064 0153 0029  ...|.......d.S.)
-00000cf0: 027a d60a 2020 2020 5468 6973 2066 756e  .z..    This fun
-00000d00: 6374 696f 6e20 756e 7461 7273 2061 2066  ction untars a f
-00000d10: 696c 6520 746f 2061 2073 7065 6369 6669  ile to a specifi
-00000d20: 6320 666f 6c64 6572 206c 6f63 6174 696f  c folder locatio
-00000d30: 6e2e 0a0a 2020 2020 4172 6773 3a0a 2020  n...    Args:.  
-00000d40: 2020 2020 2020 7061 7468 5f74 6172 5f66        path_tar_f
-00000d50: 696c 6520 2873 7472 293a 2061 6273 6f6c  ile (str): absol
-00000d60: 7574 6520 7061 7468 206f 6620 2e74 6172  ute path of .tar
-00000d70: 2066 696c 650a 2020 2020 2020 2020 6f75   file.        ou
-00000d80: 7470 7574 5f66 6f6c 6465 7220 2873 7472  tput_folder (str
-00000d90: 293a 2061 6273 6f6c 7574 6520 7061 7468  ): absolute path
-00000da0: 206f 6620 6f75 7470 7574 2066 6f6c 6465   of output folde
-00000db0: 720a 0a20 2020 2052 6574 7572 6e73 3a20  r..    Returns: 
-00000dc0: 4e6f 6e65 0a20 2020 204e 2904 da07 7461  None.    N)...ta
-00000dd0: 7266 696c 6572 1b00 0000 7235 0000 00da  rfiler....r5....
-00000de0: 0563 6c6f 7365 2903 7237 0000 0072 3300  .close).r7...r3.
-00000df0: 0000 5a08 7461 725f 6669 6c65 720b 0000  ..Z.tar_filer...
-00000e00: 0072 0b00 0000 720c 0000 00da 1475 6e74  .r....r......unt
-00000e10: 6172 5f66 696c 655f 746f 5f66 6f6c 6465  ar_file_to_folde
-00000e20: 727c 0000 0073 0800 0000 000a 0a01 0a01  r|...s..........
-00000e30: 0801 723a 0000 0029 03da 0c69 6e70 7574  ..r:...)...input
-00000e40: 5f66 6f6c 6465 72da 0b66 696c 655f 666f  _folder..file_fo
-00000e50: 726d 6174 7205 0000 0063 0200 0000 0000  rmatr....c......
-00000e60: 0000 0000 0000 0600 0000 0b00 0000 4300  ..............C.
-00000e70: 0000 7376 0000 0074 00a0 007c 009b 0064  ..sv...t...|...d
-00000e80: 019d 02a1 017d 0264 027c 019b 009d 027d  .....}.d.|.....}
-00000e90: 0374 0183 007d 047c 0244 005d 287d 057c  .t...}.|.D.](}.|
-00000ea0: 0474 0274 00a0 0074 036a 04a0 0574 036a  .t.t...t.j...t.j
-00000eb0: 04a0 067c 057c 03a1 02a1 01a1 0183 0117  ...|.|..........
-00000ec0: 007d 0471 247c 0474 0274 00a0 0074 036a  .}.q$|.t.t...t.j
-00000ed0: 04a0 0574 036a 04a0 067c 007c 03a1 02a1  ...t.j...|.|....
-00000ee0: 01a1 0183 0117 007d 047c 0453 0029 037a  .......}.|.S.).z
-00000ef0: b10a 2020 2020 5468 6973 2066 756e 6374  ..    This funct
-00000f00: 696f 6e20 6765 7473 2061 206c 6973 7420  ion gets a list 
-00000f10: 6f66 2061 6c6c 2066 696c 6573 206f 6620  of all files of 
-00000f20: 7479 7065 2022 6669 6c65 5f66 6f72 6d61  type "file_forma
-00000f30: 7422 2069 6e20 6120 6469 7265 6374 6f72  t" in a director
-00000f40: 790a 2020 2020 4172 6773 3a0a 2020 2020  y.    Args:.    
-00000f50: 2020 2020 696e 7075 745f 666f 6c64 6572      input_folder
-00000f60: 2028 7374 7229 3a20 696e 7075 7420 666f   (str): input fo
-00000f70: 6c64 6572 2070 6174 680a 0a20 2020 2052  lder path..    R
-00000f80: 6574 7572 6e73 3a20 6c69 7374 2077 6974  eturns: list wit
-00000f90: 6820 2e70 6466 2066 696c 6573 0a0a 2020  h .pdf files..  
-00000fa0: 2020 7a03 2f2a 2f7a 042e 2f2a 2e29 07da    z./*/z../*.)..
-00000fb0: 0467 6c6f 62da 046c 6973 74da 0673 6f72  .glob..list..sor
-00000fc0: 7465 6472 0600 0000 7204 0000 00da 0761  tedr....r......a
-00000fd0: 6273 7061 7468 722c 0000 0029 0672 3b00  bspathr,...).r;.
-00000fe0: 0000 723c 0000 005a 0e73 7562 666f 6c64  ..r<...Z.subfold
-00000ff0: 6572 5f6c 6973 745a 0b66 696c 655f 7374  er_listZ.file_st
-00001000: 7269 6e67 da02 6c6c da05 656e 7472 7972  ring..ll..entryr
-00001010: 0b00 0000 720b 0000 0072 0c00 0000 da22  ....r....r....."
-00001020: 6765 745f 616c 6c5f 6669 6c65 735f 6f66  get_all_files_of
-00001030: 5f74 7970 655f 696e 5f64 6972 6563 746f  _type_in_directo
-00001040: 7279 8c00 0000 730e 0000 0000 0a10 010a  ry....s.........
-00001050: 0106 0208 0126 0324 0172 4300 0000 2903  .....&.$.rC...).
-00001060: 723b 0000 00da 0973 7562 7374 7269 6e67  r;.....substring
-00001070: 7205 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00001080: 0000 0300 0000 0400 0000 4300 0000 731a  ..........C...s.
-00001090: 0000 007c 009b 0064 017c 019b 0064 019d  ...|...d.|...d..
-000010a0: 047d 0274 00a0 007c 02a1 0153 0029 027a  .}.t...|...S.).z
-000010b0: b40a 2020 2020 5468 6973 2066 756e 6374  ..    This funct
-000010c0: 696f 6e20 7265 7475 726e 7320 6669 6c65  ion returns file
-000010d0: 7320 7768 6963 6820 636f 6e74 6169 6e61  s which containa
-000010e0: 2063 6572 7461 696e 2073 7562 7374 7269   certain substri
-000010f0: 6e67 0a20 2020 2041 7267 733a 0a20 2020  ng.    Args:.   
-00001100: 2020 2020 2069 6e70 7574 5f66 6f6c 6465       input_folde
-00001110: 7220 2873 7472 293a 2069 6e70 7574 2066  r (str): input f
-00001120: 6f6c 6465 720a 2020 2020 2020 2020 7375  older.        su
-00001130: 6273 7472 696e 6720 2873 7472 293a 2073  bstring (str): s
-00001140: 7562 7374 7269 6e67 0a0a 2020 2020 5265  ubstring..    Re
-00001150: 7475 726e 733a 2066 696c 6520 7061 7468  turns: file path
-00001160: 0a20 2020 20da 012a 2901 723d 0000 0029  .    ..*).r=...)
-00001170: 0372 3b00 0000 7244 0000 005a 0867 6c6f  .r;...rD...Z.glo
-00001180: 625f 7374 7272 0b00 0000 720b 0000 0072  b_strr....r....r
-00001190: 0c00 0000 da13 6669 6e64 5f73 7562 7374  ......find_subst
-000011a0: 7269 6e67 5f70 6174 68a2 0000 0073 0400  ring_path....s..
-000011b0: 0000 0009 1001 7246 0000 007a 042e 6a70  ......rF...z..jp
-000011c0: 677a 042e 706e 6729 0372 3b00 0000 da10  gz..png).r;.....
-000011d0: 6669 6c65 5f66 6f72 6d61 745f 6c69 7374  file_format_list
-000011e0: 7205 0000 0063 0200 0000 0000 0000 0000  r....c..........
-000011f0: 0000 0400 0000 0900 0000 4300 0000 733c  ..........C...s<
-00001200: 0000 007c 0144 005d 327d 0274 0074 01a0  ...|.D.]2}.t.t..
-00001210: 0174 026a 03a0 047c 0064 017c 029b 009d  .t.j...|.d.|....
-00001220: 02a1 02a1 0183 0144 005d 0e7d 0374 02a0  .......D.].}.t..
-00001230: 057c 03a1 0101 0071 2671 0464 0253 0029  .|.....q&q.d.S.)
-00001240: 037a c80a 2020 2020 5468 6973 2066 756e  .z..    This fun
-00001250: 6374 696f 6e20 6465 6c65 7465 7320 616c  ction deletes al
-00001260: 6c20 6669 6c65 7320 6f66 2074 7970 650a  l files of type.
-00001270: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00001280: 2020 696e 7075 745f 666f 6c64 6572 2028    input_folder (
-00001290: 7374 7229 3a20 696e 7075 7420 666f 6c64  str): input fold
-000012a0: 6572 0a20 2020 2020 2020 2066 696c 655f  er.        file_
-000012b0: 666f 726d 6174 5f6c 6973 7420 286c 6973  format_list (lis
-000012c0: 7429 3a20 6c69 7374 206f 6620 6669 6c65  t): list of file
-000012d0: 2074 7970 6573 2074 6f20 6265 2064 656c   types to be del
-000012e0: 6574 6564 2e20 452e 672e 205b 2e6a 7067  eted. E.g. [.jpg
-000012f0: 2c20 2e70 6e67 5d0a 0a20 2020 2052 6574  , .png]..    Ret
-00001300: 7572 6e73 3a0a 0a20 2020 207a 032e 2f2a  urns:..    z../*
-00001310: 4e29 0672 3f00 0000 723d 0000 0072 0600  N).r?...r=...r..
-00001320: 0000 7204 0000 0072 2c00 0000 da06 7265  ..r....r,.....re
-00001330: 6d6f 7665 2904 723b 0000 0072 4700 0000  move).r;...rG...
-00001340: 723c 0000 00da 0866 696c 656e 616d 6572  r<.....filenamer
-00001350: 0b00 0000 720b 0000 0072 0c00 0000 da14  ....r....r......
-00001360: 6465 6c65 7465 5f66 696c 6573 5f6f 665f  delete_files_of_
-00001370: 7479 7065 af00 0000 7308 0000 0000 0a08  type....s.......
-00001380: 0122 010e 0172 4a00 0000 2901 4629 1a72  ."...rJ...).F).r
-00001390: 3d00 0000 721c 0000 0072 0600 0000 7210  =...r....r....r.
-000013a0: 0000 0072 3800 0000 7224 0000 00da 0674  ...r8...r$.....t
-000013b0: 7970 696e 6772 0200 0000 da07 7a69 7066  ypingr......zipf
-000013c0: 696c 6572 0300 0000 7223 0000 0072 3e00  iler....r#...r>.
-000013d0: 0000 720d 0000 00da 0462 6f6f 6c72 1300  ..r......boolr..
-000013e0: 0000 7215 0000 00da 0464 6963 7472 1e00  ..r......dictr..
-000013f0: 0000 7222 0000 0072 2600 0000 7231 0000  ..r"...r&...r1..
-00001400: 0072 3600 0000 723a 0000 0072 4300 0000  .r6...r:...rC...
-00001410: 7246 0000 0072 4a00 0000 720b 0000 0072  rF...rJ...r....r
-00001420: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
-00001430: 3c6d 6f64 756c 653e 0100 0000 7326 0000  <module>....s&..
-00001440: 0008 0108 0108 0108 0108 0108 010c 010c  ................
-00001450: 0310 0c14 1210 0e1a 0f0e 0d0e 0812 1312  ................
-00001460: 0e12 1012 1612 0d                        .......
+000002c0: 2e70 79da 1973 706c 6974 5f66 6f6c 6465  .py..split_folde
+000002d0: 725f 7061 7468 5f74 6f5f 6c69 7374 0b00  r_path_to_list..
+000002e0: 0000 7304 0000 0000 080c 0172 0d00 0000  ..s........r....
+000002f0: 4629 0372 0400 0000 da10 6465 6c65 7465  F).r......delete
+00000300: 5f69 665f 6578 6973 7473 7205 0000 0063  _if_existsr....c
+00000310: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000320: 0300 0000 4300 0000 7334 0000 007c 0172  ....C...s4...|.r
+00000330: 1a74 006a 01a0 027c 00a1 0172 1a74 03a0  .t.j...|...r.t..
+00000340: 047c 00a1 0101 0074 006a 01a0 027c 00a1  .|.....t.j...|..
+00000350: 0173 3074 00a0 057c 00a1 0101 0064 0153  .s0t...|.....d.S
+00000360: 0029 027a b90a 2020 2020 5468 6973 2066  .).z..    This f
+00000370: 756e 6374 696f 6e20 6372 6561 7465 7320  unction creates 
+00000380: 6120 6469 7265 6374 6f72 792e 0a20 2020  a directory..   
+00000390: 2041 7267 733a 0a20 2020 2020 2020 2070   Args:.        p
+000003a0: 6174 6820 2873 7472 293a 2064 6972 6563  ath (str): direc
+000003b0: 746f 7279 2070 6174 680a 2020 2020 2020  tory path.      
+000003c0: 2020 6465 6c65 7465 5f69 665f 6578 6973    delete_if_exis
+000003d0: 7473 2028 626f 6f6c 293a 2069 6620 5472  ts (bool): if Tr
+000003e0: 7565 2c20 6578 6973 7469 6e67 2064 6972  ue, existing dir
+000003f0: 6563 746f 7279 2077 696c 6c20 6265 2064  ectory will be d
+00000400: 656c 6574 6564 0a0a 2020 2020 5265 7475  eleted..    Retu
+00000410: 726e 733a 204e 6f6e 650a 2020 2020 4e29  rns: None.    N)
+00000420: 0672 0600 0000 7204 0000 00da 0665 7869  .r....r......exi
+00000430: 7374 73da 0673 6875 7469 6cda 0672 6d74  sts..shutil..rmt
+00000440: 7265 65da 086d 616b 6564 6972 7329 0272  ree..makedirs).r
+00000450: 0400 0000 720e 0000 0072 0b00 0000 720b  ....r....r....r.
+00000460: 0000 0072 0c00 0000 da10 6372 6561 7465  ...r......create
+00000470: 5f64 6972 6563 746f 7279 1700 0000 730c  _directory....s.
+00000480: 0000 0000 0904 010c 010a 020c 010a 0172  ...............r
+00000490: 1300 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000004a0: 0001 0000 0003 0000 0043 0000 0073 1e00  .........C...s..
+000004b0: 0000 7400 6a01 a002 7c00 a101 731a 7403  ..t.j...|...s.t.
+000004c0: 7c00 9b00 6401 9d02 8301 8201 6402 5300  |...d.......d.S.
+000004d0: 2903 7a94 0a20 2020 2054 6869 7320 6675  ).z..    This fu
+000004e0: 6e63 7469 6f6e 2063 6865 636b 7320 6966  nction checks if
+000004f0: 2061 2066 696c 6520 6578 6973 7473 2c20   a file exists, 
+00000500: 616e 640a 2020 2020 7261 6973 6573 2061  and.    raises a
+00000510: 6e20 6578 6365 7074 696f 6e20 6966 206e  n exception if n
+00000520: 6f74 0a20 2020 2041 7267 733a 0a20 2020  ot.    Args:.   
+00000530: 2020 2020 2070 6174 6820 2873 7472 293a       path (str):
+00000540: 2069 6e70 7574 2066 696c 6520 7061 7468   input file path
+00000550: 0a0a 2020 2020 5265 7475 726e 733a 204e  ..    Returns: N
+00000560: 6f6e 650a 2020 2020 7a10 2064 6f65 7320  one.    z. does 
+00000570: 6e6f 7420 6578 6973 742e 4e29 0472 0600  not exist.N).r..
+00000580: 0000 7204 0000 0072 0f00 0000 da09 4578  ..r....r......Ex
+00000590: 6365 7074 696f 6e72 0a00 0000 720b 0000  ceptionr....r...
+000005a0: 0072 0b00 0000 720c 0000 00da 1163 6865  .r....r......che
+000005b0: 636b 5f66 696c 655f 6578 6973 7473 2900  ck_file_exists).
+000005c0: 0000 7306 0000 0000 090c 010e 0172 1500  ..s..........r..
+000005d0: 0000 2903 da04 6461 7461 7204 0000 0072  ..)...datar....r
+000005e0: 0500 0000 6302 0000 0000 0000 0000 0000  ....c...........
+000005f0: 0003 0000 0009 0000 0043 0000 0073 2c00  .........C...s,.
+00000600: 0000 7400 7c01 6401 8302 8f18 7d02 7401  ..t.|.d.....}.t.
+00000610: 6a02 7c00 7c02 6402 6403 6404 8d04 0100  j.|.|.d.d.d.....
+00000620: 5700 3500 5100 5200 5800 6405 5300 2906  W.5.Q.R.X.d.S.).
+00000630: 7a70 0a20 2020 2054 6869 7320 6675 6e63  zp.    This func
+00000640: 7469 6f6e 2073 6176 6573 2061 206c 6973  tion saves a lis
+00000650: 7420 6f72 0a20 2020 2041 7267 733a 0a20  t or.    Args:. 
+00000660: 2020 2020 2020 2064 6174 6120 2864 6963         data (dic
+00000670: 7420 6f72 206c 6973 7429 3a0a 2020 2020  t or list):.    
+00000680: 2020 2020 7061 7468 2028 7374 7229 3a0a      path (str):.
+00000690: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+000006a0: 2020 da01 77e9 0400 0000 5429 02da 0669    ..w.....T)...i
+000006b0: 6e64 656e 74da 0973 6f72 745f 6b65 7973  ndent..sort_keys
+000006c0: 4e29 03da 046f 7065 6eda 046a 736f 6eda  N)...open..json.
+000006d0: 0464 756d 7029 0372 1600 0000 7204 0000  .dump).r....r...
+000006e0: 005a 0666 5f6a 736f 6e72 0b00 0000 720b  .Z.f_jsonr....r.
+000006f0: 0000 0072 0c00 0000 da09 7361 7665 5f6a  ...r......save_j
+00000700: 736f 6e37 0000 0073 0600 0000 0009 0c01  son7...s........
+00000710: 1c02 721e 0000 0029 01da 096a 736f 6e5f  ..r....)...json_
+00000720: 7061 7468 6301 0000 0000 0000 0000 0000  pathc...........
+00000730: 0003 0000 0009 0000 0043 0000 0073 2200  .........C...s".
+00000740: 0000 7400 7c00 8301 8f10 7d01 7401 a002  ..t.|.....}.t...
+00000750: 7c01 a101 7d02 5700 3500 5100 5200 5800  |...}.W.5.Q.R.X.
+00000760: 7c02 5300 2901 7a8e 0a20 2020 2054 6869  |.S.).z..    Thi
+00000770: 7320 6675 6e63 7469 6f6e 2072 6561 6473  s function reads
+00000780: 2061 206a 736f 6e20 6669 6c65 2061 6e64   a json file and
+00000790: 2072 6574 7572 6e20 6120 4a53 4f4e 206f   return a JSON o
+000007a0: 626a 6563 740a 2020 2020 4172 6773 3a0a  bject.    Args:.
+000007b0: 2020 2020 2020 2020 6a73 6f6e 5f70 6174          json_pat
+000007c0: 6820 2873 7472 293a 204a 534f 4e20 6669  h (str): JSON fi
+000007d0: 6c65 2070 6174 680a 0a20 2020 2052 6574  le path..    Ret
+000007e0: 7572 6e73 3a20 4a53 4f4e 206f 626a 6563  urns: JSON objec
+000007f0: 740a 2020 2020 2903 721b 0000 0072 1c00  t.    ).r....r..
+00000800: 0000 da04 6c6f 6164 2903 721f 0000 005a  ....load).r....Z
+00000810: 096a 736f 6e5f 6669 6c65 7216 0000 0072  .json_filer....r
+00000820: 0b00 0000 720b 0000 0072 0c00 0000 da09  ....r....r......
+00000830: 7265 6164 5f6a 736f 6e46 0000 0073 0600  read_jsonF...s..
+00000840: 0000 0008 0a01 1401 7221 0000 0029 0172  ........r!...).r
+00000850: 0500 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000860: 0000 0000 0003 0000 0043 0000 0073 0c00  .........C...s..
+00000870: 0000 7400 7401 a002 a100 8301 5300 2901  ..t.t.......S.).
+00000880: 7a38 0a20 2020 2054 6869 7320 6675 6e63  z8.    This func
+00000890: 7469 6f6e 2072 6574 7572 6e73 2061 2055  tion returns a U
+000008a0: 5549 440a 2020 2020 5265 7475 726e 733a  UID.    Returns:
+000008b0: 2055 5549 440a 2020 2020 2903 da03 7374   UUID.    )...st
+000008c0: 72da 0475 7569 64da 0575 7569 6434 720b  r..uuid..uuid4r.
+000008d0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+000008e0: 0000 da0b 6372 6561 7465 5f75 7569 6453  ....create_uuidS
+000008f0: 0000 0073 0200 0000 0005 7225 0000 0029  ...s......r%...)
+00000900: 03da 0f73 7562 5f66 6f6c 6465 725f 6e61  ...sub_folder_na
+00000910: 6d65 da0b 7365 6172 6368 5f70 6174 6872  me..search_pathr
+00000920: 0500 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000930: 0006 0000 0006 0000 0043 0000 0073 4800  .........C...sH.
+00000940: 0000 6700 7d02 7400 a001 7c01 a101 4400  ..g.}.t...|...D.
+00000950: 5d34 5c03 7d03 7d04 7d05 7402 7c03 8301  ]4\.}.}.}.t.|...
+00000960: 0100 7402 7c04 8301 0100 7c00 7c04 6b06  ..t.|.....|.|.k.
+00000970: 720e 7c02 a003 7400 6a04 a005 7c03 a101  r.|...t.j...|...
+00000980: a101 0100 710e 7c02 5300 2901 7ad0 0a20  ....q.|.S.).z.. 
+00000990: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+000009a0: 2066 696e 6473 2061 2066 696c 656e 616d   finds a filenam
+000009b0: 6520 696e 2061 2073 7562 666f 6c64 6572  e in a subfolder
+000009c0: 2e0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000009d0: 2020 2020 7375 625f 666f 6c64 6572 5f6e      sub_folder_n
+000009e0: 616d 6520 2873 7472 293a 206e 616d 6520  ame (str): name 
+000009f0: 6f66 2073 7562 666f 6c64 6572 0a20 2020  of subfolder.   
+00000a00: 2020 2020 2073 6561 7263 685f 7061 7468       search_path
+00000a10: 2028 7374 7229 3a20 7061 7468 206f 6620   (str): path of 
+00000a20: 666f 6c64 6572 2074 6f20 6265 2073 6561  folder to be sea
+00000a30: 7263 6865 640a 0a20 2020 2052 6574 7572  rched..    Retur
+00000a40: 6e73 3a20 4120 6c69 7374 2077 6974 6820  ns: A list with 
+00000a50: 6669 6c65 6e61 6d65 730a 2020 2020 2906  filenames.    ).
+00000a60: 7206 0000 00da 0477 616c 6bda 0570 7269  r......walk..pri
+00000a70: 6e74 da06 6170 7065 6e64 7204 0000 00da  nt..appendr.....
+00000a80: 046a 6f69 6e29 0672 2600 0000 7227 0000  .join).r&...r'..
+00000a90: 00da 0672 6573 756c 74da 0472 6f6f 74da  ...result..root.
+00000aa0: 0364 6972 da05 6669 6c65 7372 0b00 0000  .dir..filesr....
+00000ab0: 720b 0000 0072 0c00 0000 da0f 6669 6e64  r....r......find
+00000ac0: 5f73 7562 5f66 6f6c 6465 725b 0000 0073  _sub_folder[...s
+00000ad0: 0e00 0000 000a 0401 1401 0801 0801 0801  ................
+00000ae0: 1401 7230 0000 0029 03da 0d70 6174 685f  ..r0...)...path_
+00000af0: 7a69 705f 6669 6c65 da0d 6f75 7470 7574  zip_file..output
+00000b00: 5f66 6f6c 6465 7272 0500 0000 6302 0000  _folderr....c...
+00000b10: 0000 0000 0000 0000 0003 0000 0009 0000  ................
+00000b20: 0043 0000 0073 2400 0000 7400 7c00 6401  .C...s$...t.|.d.
+00000b30: 8302 8f10 7d02 7c02 a001 7c01 a101 0100  ....}.|...|.....
+00000b40: 5700 3500 5100 5200 5800 6402 5300 2903  W.5.Q.R.X.d.S.).
+00000b50: 7ad5 0a20 2020 2054 6869 7320 6675 6e63  z..    This func
+00000b60: 7469 6f6e 2075 6e7a 6970 7320 6120 6669  tion unzips a fi
+00000b70: 6c65 2074 6f20 6120 7370 6563 6966 6963  le to a specific
+00000b80: 2066 6f6c 6465 7220 6c6f 6361 7469 6f6e   folder location
+00000b90: 2e0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00000ba0: 2020 2020 7061 7468 5f7a 6970 5f66 696c      path_zip_fil
+00000bb0: 6520 2873 7472 293a 2061 6273 6f6c 7574  e (str): absolut
+00000bc0: 6520 7061 7468 206f 6620 2e7a 6970 2066  e path of .zip f
+00000bd0: 696c 650a 2020 2020 2020 2020 6f75 7470  ile.        outp
+00000be0: 7574 5f66 6f6c 6465 7220 2873 7472 293a  ut_folder (str):
+00000bf0: 2061 6273 6f6c 7574 6520 7061 7468 206f   absolute path o
+00000c00: 6620 6f75 7470 7574 2066 6f6c 6465 720a  f output folder.
+00000c10: 0a20 2020 2052 6574 7572 6e73 3a20 4e6f  .    Returns: No
+00000c20: 6e65 0a20 2020 20da 0172 4e29 0272 0300  ne.    ..rN).r..
+00000c30: 0000 da0a 6578 7472 6163 7461 6c6c 2903  ....extractall).
+00000c40: 7231 0000 0072 3200 0000 5a06 7a69 704f  r1...r2...Z.zipO
+00000c50: 626a 720b 0000 0072 0b00 0000 720c 0000  bjr....r....r...
+00000c60: 00da 1475 6e7a 6970 5f66 696c 655f 746f  ...unzip_file_to
+00000c70: 5f66 6f6c 6465 726e 0000 0073 0600 0000  _foldern...s....
+00000c80: 0009 0c01 1401 7235 0000 0029 03da 0d70  ......r5...)...p
+00000c90: 6174 685f 7461 725f 6669 6c65 7232 0000  ath_tar_filer2..
+00000ca0: 0072 0500 0000 6302 0000 0000 0000 0000  .r....c.........
+00000cb0: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
+00000cc0: 2000 0000 7400 a001 7c00 a101 7d02 7c02   ...t...|...}.|.
+00000cd0: a002 7c01 a101 0100 7c02 a003 a100 0100  ..|.....|.......
+00000ce0: 6401 5300 2902 7ad6 0a20 2020 2054 6869  d.S.).z..    Thi
+00000cf0: 7320 6675 6e63 7469 6f6e 2075 6e74 6172  s function untar
+00000d00: 7320 6120 6669 6c65 2074 6f20 6120 7370  s a file to a sp
+00000d10: 6563 6966 6963 2066 6f6c 6465 7220 6c6f  ecific folder lo
+00000d20: 6361 7469 6f6e 2e0a 0a20 2020 2041 7267  cation...    Arg
+00000d30: 733a 0a20 2020 2020 2020 2070 6174 685f  s:.        path_
+00000d40: 7461 725f 6669 6c65 2028 7374 7229 3a20  tar_file (str): 
+00000d50: 6162 736f 6c75 7465 2070 6174 6820 6f66  absolute path of
+00000d60: 202e 7461 7220 6669 6c65 0a20 2020 2020   .tar file.     
+00000d70: 2020 206f 7574 7075 745f 666f 6c64 6572     output_folder
+00000d80: 2028 7374 7229 3a20 6162 736f 6c75 7465   (str): absolute
+00000d90: 2070 6174 6820 6f66 206f 7574 7075 7420   path of output 
+00000da0: 666f 6c64 6572 0a0a 2020 2020 5265 7475  folder..    Retu
+00000db0: 726e 733a 204e 6f6e 650a 2020 2020 4e29  rns: None.    N)
+00000dc0: 04da 0774 6172 6669 6c65 721b 0000 0072  ...tarfiler....r
+00000dd0: 3400 0000 da05 636c 6f73 6529 0372 3600  4.....close).r6.
+00000de0: 0000 7232 0000 005a 0874 6172 5f66 696c  ..r2...Z.tar_fil
+00000df0: 6572 0b00 0000 720b 0000 0072 0c00 0000  er....r....r....
+00000e00: da14 756e 7461 725f 6669 6c65 5f74 6f5f  ..untar_file_to_
+00000e10: 666f 6c64 6572 7c00 0000 7308 0000 0000  folder|...s.....
+00000e20: 0a0a 010a 0108 0172 3900 0000 2903 da0c  .......r9...)...
+00000e30: 696e 7075 745f 666f 6c64 6572 da0b 6669  input_folder..fi
+00000e40: 6c65 5f66 6f72 6d61 7472 0500 0000 6302  le_formatr....c.
+00000e50: 0000 0000 0000 0000 0000 0006 0000 000b  ................
+00000e60: 0000 0043 0000 0073 7600 0000 7400 a000  ...C...sv...t...
+00000e70: 7c00 9b00 6401 9d02 a101 7d02 6402 7c01  |...d.....}.d.|.
+00000e80: 9b00 9d02 7d03 7401 8300 7d04 7c02 4400  ....}.t...}.|.D.
+00000e90: 5d28 7d05 7c04 7402 7400 a000 7403 6a04  ](}.|.t.t...t.j.
+00000ea0: a005 7403 6a04 a006 7c05 7c03 a102 a101  ..t.j...|.|.....
+00000eb0: a101 8301 1700 7d04 7124 7c04 7402 7400  ......}.q$|.t.t.
+00000ec0: a000 7403 6a04 a005 7403 6a04 a006 7c00  ..t.j...t.j...|.
+00000ed0: 7c03 a102 a101 a101 8301 1700 7d04 7c04  |...........}.|.
+00000ee0: 5300 2903 7ab1 0a20 2020 2054 6869 7320  S.).z..    This 
+00000ef0: 6675 6e63 7469 6f6e 2067 6574 7320 6120  function gets a 
+00000f00: 6c69 7374 206f 6620 616c 6c20 6669 6c65  list of all file
+00000f10: 7320 6f66 2074 7970 6520 2266 696c 655f  s of type "file_
+00000f20: 666f 726d 6174 2220 696e 2061 2064 6972  format" in a dir
+00000f30: 6563 746f 7279 0a20 2020 2041 7267 733a  ectory.    Args:
+00000f40: 0a20 2020 2020 2020 2069 6e70 7574 5f66  .        input_f
+00000f50: 6f6c 6465 7220 2873 7472 293a 2069 6e70  older (str): inp
+00000f60: 7574 2066 6f6c 6465 7220 7061 7468 0a0a  ut folder path..
+00000f70: 2020 2020 5265 7475 726e 733a 206c 6973      Returns: lis
+00000f80: 7420 7769 7468 202e 7064 6620 6669 6c65  t with .pdf file
+00000f90: 730a 0a20 2020 207a 032f 2a2f 7a04 2e2f  s..    z./*/z../
+00000fa0: 2a2e 2907 da04 676c 6f62 da04 6c69 7374  *.)...glob..list
+00000fb0: da06 736f 7274 6564 7206 0000 0072 0400  ..sortedr....r..
+00000fc0: 0000 da07 6162 7370 6174 6872 2b00 0000  ....abspathr+...
+00000fd0: 2906 723a 0000 0072 3b00 0000 da0e 7375  ).r:...r;.....su
+00000fe0: 6266 6f6c 6465 725f 6c69 7374 da0b 6669  bfolder_list..fi
+00000ff0: 6c65 5f73 7472 696e 67da 026c 6cda 0565  le_string..ll..e
+00001000: 6e74 7279 720b 0000 0072 0b00 0000 720c  ntryr....r....r.
+00001010: 0000 00da 2267 6574 5f61 6c6c 5f66 696c  ...."get_all_fil
+00001020: 6573 5f6f 665f 7479 7065 5f69 6e5f 6469  es_of_type_in_di
+00001030: 7265 6374 6f72 798c 0000 0073 0e00 0000  rectory....s....
+00001040: 000a 1001 0a01 0602 0801 2603 2401 7244  ..........&.$.rD
+00001050: 0000 0029 0372 3a00 0000 da09 7375 6273  ...).r:.....subs
+00001060: 7472 696e 6772 0500 0000 6302 0000 0000  tringr....c.....
+00001070: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00001080: 0000 0073 1a00 0000 7c00 9b00 6401 7c01  ...s....|...d.|.
+00001090: 9b00 6401 9d04 7d02 7400 a000 7c02 a101  ..d...}.t...|...
+000010a0: 5300 2902 7ab4 0a20 2020 2054 6869 7320  S.).z..    This 
+000010b0: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
+000010c0: 2066 696c 6573 2077 6869 6368 2063 6f6e   files which con
+000010d0: 7461 696e 6120 6365 7274 6169 6e20 7375  taina certain su
+000010e0: 6273 7472 696e 670a 2020 2020 4172 6773  bstring.    Args
+000010f0: 3a0a 2020 2020 2020 2020 696e 7075 745f  :.        input_
+00001100: 666f 6c64 6572 2028 7374 7229 3a20 696e  folder (str): in
+00001110: 7075 7420 666f 6c64 6572 0a20 2020 2020  put folder.     
+00001120: 2020 2073 7562 7374 7269 6e67 2028 7374     substring (st
+00001130: 7229 3a20 7375 6273 7472 696e 670a 0a20  r): substring.. 
+00001140: 2020 2052 6574 7572 6e73 3a20 6669 6c65     Returns: file
+00001150: 2070 6174 680a 2020 2020 da01 2a29 0172   path.    ..*).r
+00001160: 3c00 0000 2903 723a 0000 0072 4500 0000  <...).r:...rE...
+00001170: 5a08 676c 6f62 5f73 7472 720b 0000 0072  Z.glob_strr....r
+00001180: 0b00 0000 720c 0000 00da 1366 696e 645f  ....r......find_
+00001190: 7375 6273 7472 696e 675f 7061 7468 a200  substring_path..
+000011a0: 0000 7304 0000 0000 0910 0172 4700 0000  ..s........rG...
+000011b0: 7a04 2e6a 7067 7a04 2e70 6e67 2903 723a  z..jpgz..png).r:
+000011c0: 0000 00da 1066 696c 655f 666f 726d 6174  .....file_format
+000011d0: 5f6c 6973 7472 0500 0000 6302 0000 0000  _listr....c.....
+000011e0: 0000 0000 0000 0004 0000 0009 0000 0043  ...............C
+000011f0: 0000 0073 3c00 0000 7c01 4400 5d32 7d02  ...s<...|.D.]2}.
+00001200: 7400 7401 a001 7402 6a03 a004 7c00 6401  t.t...t.j...|.d.
+00001210: 7c02 9b00 9d02 a102 a101 8301 4400 5d0e  |...........D.].
+00001220: 7d03 7402 a005 7c03 a101 0100 7126 7104  }.t...|.....q&q.
+00001230: 6402 5300 2903 7ac8 0a20 2020 2054 6869  d.S.).z..    Thi
+00001240: 7320 6675 6e63 7469 6f6e 2064 656c 6574  s function delet
+00001250: 6573 2061 6c6c 2066 696c 6573 206f 6620  es all files of 
+00001260: 7479 7065 0a20 2020 2041 7267 733a 0a20  type.    Args:. 
+00001270: 2020 2020 2020 2069 6e70 7574 5f66 6f6c         input_fol
+00001280: 6465 7220 2873 7472 293a 2069 6e70 7574  der (str): input
+00001290: 2066 6f6c 6465 720a 2020 2020 2020 2020   folder.        
+000012a0: 6669 6c65 5f66 6f72 6d61 745f 6c69 7374  file_format_list
+000012b0: 2028 6c69 7374 293a 206c 6973 7420 6f66   (list): list of
+000012c0: 2066 696c 6520 7479 7065 7320 746f 2062   file types to b
+000012d0: 6520 6465 6c65 7465 642e 2045 2e67 2e20  e deleted. E.g. 
+000012e0: 5b2e 6a70 672c 202e 706e 675d 0a0a 2020  [.jpg, .png]..  
+000012f0: 2020 5265 7475 726e 733a 0a0a 2020 2020    Returns:..    
+00001300: 7a03 2e2f 2a4e 2906 723e 0000 0072 3c00  z../*N).r>...r<.
+00001310: 0000 7206 0000 0072 0400 0000 722b 0000  ..r....r....r+..
+00001320: 00da 0672 656d 6f76 6529 0472 3a00 0000  ...remove).r:...
+00001330: 7248 0000 0072 3b00 0000 da08 6669 6c65  rH...r;.....file
+00001340: 6e61 6d65 720b 0000 0072 0b00 0000 720c  namer....r....r.
+00001350: 0000 00da 1464 656c 6574 655f 6669 6c65  .....delete_file
+00001360: 735f 6f66 5f74 7970 65af 0000 0073 0800  s_of_type....s..
+00001370: 0000 000a 0801 2201 0e01 724b 0000 0029  ......"...rK...)
+00001380: 0146 291a 723c 0000 0072 1c00 0000 7206  .F).r<...r....r.
+00001390: 0000 0072 1000 0000 7237 0000 0072 2300  ...r....r7...r#.
+000013a0: 0000 da06 7479 7069 6e67 7202 0000 00da  ....typingr.....
+000013b0: 077a 6970 6669 6c65 7203 0000 0072 2200  .zipfiler....r".
+000013c0: 0000 723d 0000 0072 0d00 0000 da04 626f  ..r=...r......bo
+000013d0: 6f6c 7213 0000 0072 1500 0000 da04 6469  olr....r......di
+000013e0: 6374 721e 0000 0072 2100 0000 7225 0000  ctr....r!...r%..
+000013f0: 0072 3000 0000 7235 0000 0072 3900 0000  .r0...r5...r9...
+00001400: 7244 0000 0072 4700 0000 724b 0000 0072  rD...rG...rK...r
+00001410: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
+00001420: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001430: 0073 2600 0000 0801 0801 0801 0801 0801  .s&.............
+00001440: 0801 0c01 0c03 100c 1412 100e 1a0f 0e0d  ................
+00001450: 0e08 1213 120e 1210 1216 120d            ............
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/file_utils/file_utils.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/img_utils/__pycache__/img_utils.cpython-38.pyc` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/__pycache__/img_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 13:09:39 2023 UTC, .py size: 1147 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -11,77 +11,76 @@
 000000a0: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
 000000b0: 7314 0000 0074 006a 017c 007c 017c 0266  s....t.j.|.|.|.f
 000000c0: 027c 0364 018d 0353 0029 024e 2903 da03  .|.d...S.).N)...
 000000d0: 7372 635a 0564 7369 7a65 da0d 696e 7465  srcZ.dsize..inte
 000000e0: 7270 6f6c 6174 696f 6e29 02da 0363 7632  rpolation)...cv2
 000000f0: da06 7265 7369 7a65 2904 da03 696d 6772  ..resize)...imgr
 00000100: 0200 0000 7203 0000 0072 0500 0000 a900  ....r....r......
-00000110: 7209 0000 00fa 592f 686f 6d65 2f79 7665  r.....Y/home/yve
+00000110: 7209 0000 00fa 4f2f 686f 6d65 2f79 7665  r.....O/home/yve
 00000120: 732f 436f 6465 2f72 6f62 6f6c 6f67 732d  s/Code/robologs-
 00000130: 726f 732d 7574 696c 732f 7079 7468 6f6e  ros-utils/python
 00000140: 2f72 6f62 6f6c 6f67 735f 726f 735f 7574  /robologs_ros_ut
 00000150: 696c 732f 7574 696c 732f 696d 675f 7574  ils/utils/img_ut
-00000160: 696c 732f 696d 675f 7574 696c 732e 7079  ils/img_utils.py
-00000170: da0c 7265 7369 7a65 5f69 6d61 6765 0700  ..resize_image..
-00000180: 0000 7302 0000 0000 0172 0b00 0000 e700  ..s......r......
-00000190: 0000 0000 00f0 3fe9 e803 0000 fa04 2e70  ......?........p
-000001a0: 6e67 2904 da0c 696e 7075 745f 666f 6c64  ng)...input_fold
-000001b0: 6572 da0d 6f75 7470 7574 5f66 6f6c 6465  er..output_folde
-000001c0: 7272 0700 0000 da08 6d61 785f 7369 7a65  rr......max_size
-000001d0: 6305 0000 0000 0000 0000 0000 000c 0000  c...............
-000001e0: 0008 0000 0043 0000 0073 8600 0000 7400  .....C...s....t.
-000001f0: 7401 a001 7402 6a03 a004 7c00 6401 7c04  t...t.j...|.d.|.
-00000200: 9b00 9d02 a102 a101 8301 4400 5d62 7d05  ..........D.]b}.
-00000210: 7405 a006 7c05 a101 7d06 7c06 6a07 5c03  t...|...}.|.j.\.
-00000220: 7d07 7d08 7d09 7c08 7c03 6b04 7256 7405  }.}.}.|.|.k.rVt.
-00000230: 6a08 7c06 6402 7c02 7c02 7405 6a09 6403  j.|.d.|.|.t.j.d.
-00000240: 8d05 7d06 7402 6a03 a00a 7c05 a101 5c02  ..}.t.j...|...\.
-00000250: 7d09 7d0a 7402 6a03 a004 7c01 7c0a a102  }.}.t.j...|.|...
-00000260: 7d0b 7405 a00b 7c0b 7c06 a102 0100 711e  }.t...|.|.....q.
-00000270: 6404 5300 2905 614a 0100 000a 2020 2020  d.S.).aJ....    
-00000280: 5468 6973 2066 756e 6374 696f 6e20 6372  This function cr
-00000290: 6561 7465 7320 7468 756d 626e 6169 6c73  eates thumbnails
-000002a0: 2066 726f 6d20 696d 6167 6573 2069 6e20   from images in 
-000002b0: 6120 666f 6c64 6572 0a20 2020 2041 7267  a folder.    Arg
-000002c0: 733a 0a20 2020 2020 2020 2069 6e70 7574  s:.        input
-000002d0: 5f66 6f6c 6465 723a 2069 6e70 7574 2066  _folder: input f
-000002e0: 6f6c 6465 7220 7769 7468 2069 6d67 730a  older with imgs.
-000002f0: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
-00000300: 6f6c 6465 723a 206f 7574 7075 7420 666f  older: output fo
-00000310: 6c64 6572 2077 6865 7265 2074 6875 6d62  lder where thumb
-00000320: 6e61 696c 7320 6172 6520 7361 7665 640a  nails are saved.
-00000330: 2020 2020 2020 2020 7265 7369 7a65 3a20          resize: 
-00000340: 7065 7263 656e 7461 6765 2074 6f20 7768  percentage to wh
-00000350: 6963 6820 7468 6520 696d 6167 6520 7769  ich the image wi
-00000360: 6c6c 2072 6520 7265 7369 7a65 640a 2020  ll re resized.  
-00000370: 2020 2020 2020 6d61 785f 7369 7a65 3a20        max_size: 
-00000380: 6f6e 6c79 2072 6573 697a 6520 696d 6167  only resize imag
-00000390: 6573 2077 6869 6368 2061 7265 2062 6967  es which are big
-000003a0: 6765 7220 7468 616e 206d 6178 5f73 697a  ger than max_siz
-000003b0: 650a 0a20 2020 2052 6574 7572 6e73 3a0a  e..    Returns:.
-000003c0: 0a20 2020 207a 032e 2f2a 2902 7201 0000  .    z../*).r...
-000003d0: 0072 0100 0000 2903 da02 6678 da02 6679  .r....)...fx..fy
-000003e0: 7205 0000 004e 290c da06 736f 7274 6564  r....N)...sorted
-000003f0: da04 676c 6f62 da02 6f73 da04 7061 7468  ..glob..os..path
-00000400: da04 6a6f 696e 7206 0000 00da 0669 6d72  ..joinr......imr
-00000410: 6561 64da 0573 6861 7065 7207 0000 00da  ead..shaper.....
-00000420: 0a49 4e54 4552 5f41 5245 41da 0573 706c  .INTER_AREA..spl
-00000430: 6974 da07 696d 7772 6974 6529 0c72 0f00  it..imwrite).r..
-00000440: 0000 7210 0000 0072 0700 0000 7211 0000  ..r....r....r...
-00000450: 005a 0e66 696c 655f 6578 7465 6e73 696f  .Z.file_extensio
-00000460: 6eda 0866 696c 656e 616d 6572 0800 0000  n..filenamer....
-00000470: da06 6865 6967 6874 da05 7769 6474 68da  ..height..width.
-00000480: 015f da0a 696d 6167 655f 6e61 6d65 da0b  ._..image_name..
-00000490: 6f75 7470 7574 5f70 6174 6872 0900 0000  output_pathr....
-000004a0: 7209 0000 0072 0a00 0000 da1d 6372 6561  r....r......crea
-000004b0: 7465 5f74 6875 6d62 6e61 696c 735f 6672  te_thumbnails_fr
-000004c0: 6f6d 5f66 6f6c 6465 720b 0000 0073 1200  om_folder....s..
-000004d0: 0000 000e 2201 0a01 0c01 0801 1601 1001  ...."...........
-000004e0: 0e01 0e01 7224 0000 0029 0372 0c00 0000  ....r$...).r....
-000004f0: 720d 0000 0072 0e00 0000 2909 7215 0000  r....r....).r...
-00000500: 0072 1600 0000 7206 0000 0072 1b00 0000  .r....r....r....
-00000510: da03 696e 7472 0b00 0000 da03 7374 72da  ..intr......str.
-00000520: 0566 6c6f 6174 7224 0000 0072 0900 0000  .floatr$...r....
-00000530: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
-00000540: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
-00000550: 0000 0801 0802 0803 1605 0000 0000 00ff  ................
-00000560: 0201 0200 0200 0200 02ff                 ..........
+00000160: 696c 732e 7079 da0c 7265 7369 7a65 5f69  ils.py..resize_i
+00000170: 6d61 6765 0700 0000 7302 0000 0000 0172  mage....s......r
+00000180: 0b00 0000 e700 0000 0000 00f0 3fe9 e803  ............?...
+00000190: 0000 fa04 2e70 6e67 2904 da0c 696e 7075  .....png)...inpu
+000001a0: 745f 666f 6c64 6572 da0d 6f75 7470 7574  t_folder..output
+000001b0: 5f66 6f6c 6465 7272 0700 0000 da08 6d61  _folderr......ma
+000001c0: 785f 7369 7a65 6305 0000 0000 0000 0000  x_sizec.........
+000001d0: 0000 000c 0000 0008 0000 0043 0000 0073  ...........C...s
+000001e0: 8600 0000 7400 7401 a001 7402 6a03 a004  ....t.t...t.j...
+000001f0: 7c00 6401 7c04 9b00 9d02 a102 a101 8301  |.d.|...........
+00000200: 4400 5d62 7d05 7405 a006 7c05 a101 7d06  D.]b}.t...|...}.
+00000210: 7c06 6a07 5c03 7d07 7d08 7d09 7c08 7c03  |.j.\.}.}.}.|.|.
+00000220: 6b04 7256 7405 6a08 7c06 6402 7c02 7c02  k.rVt.j.|.d.|.|.
+00000230: 7405 6a09 6403 8d05 7d06 7402 6a03 a00a  t.j.d...}.t.j...
+00000240: 7c05 a101 5c02 7d09 7d0a 7402 6a03 a004  |...\.}.}.t.j...
+00000250: 7c01 7c0a a102 7d0b 7405 a00b 7c0b 7c06  |.|...}.t...|.|.
+00000260: a102 0100 711e 6404 5300 2905 614a 0100  ....q.d.S.).aJ..
+00000270: 000a 2020 2020 5468 6973 2066 756e 6374  ..    This funct
+00000280: 696f 6e20 6372 6561 7465 7320 7468 756d  ion creates thum
+00000290: 626e 6169 6c73 2066 726f 6d20 696d 6167  bnails from imag
+000002a0: 6573 2069 6e20 6120 666f 6c64 6572 0a20  es in a folder. 
+000002b0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000002c0: 2069 6e70 7574 5f66 6f6c 6465 723a 2069   input_folder: i
+000002d0: 6e70 7574 2066 6f6c 6465 7220 7769 7468  nput folder with
+000002e0: 2069 6d67 730a 2020 2020 2020 2020 6f75   imgs.        ou
+000002f0: 7470 7574 5f66 6f6c 6465 723a 206f 7574  tput_folder: out
+00000300: 7075 7420 666f 6c64 6572 2077 6865 7265  put folder where
+00000310: 2074 6875 6d62 6e61 696c 7320 6172 6520   thumbnails are 
+00000320: 7361 7665 640a 2020 2020 2020 2020 7265  saved.        re
+00000330: 7369 7a65 3a20 7065 7263 656e 7461 6765  size: percentage
+00000340: 2074 6f20 7768 6963 6820 7468 6520 696d   to which the im
+00000350: 6167 6520 7769 6c6c 2072 6520 7265 7369  age will re resi
+00000360: 7a65 640a 2020 2020 2020 2020 6d61 785f  zed.        max_
+00000370: 7369 7a65 3a20 6f6e 6c79 2072 6573 697a  size: only resiz
+00000380: 6520 696d 6167 6573 2077 6869 6368 2061  e images which a
+00000390: 7265 2062 6967 6765 7220 7468 616e 206d  re bigger than m
+000003a0: 6178 5f73 697a 650a 0a20 2020 2052 6574  ax_size..    Ret
+000003b0: 7572 6e73 3a0a 0a20 2020 207a 032e 2f2a  urns:..    z../*
+000003c0: 2902 7201 0000 0072 0100 0000 2903 da02  ).r....r....)...
+000003d0: 6678 da02 6679 7205 0000 004e 290c da06  fx..fyr....N)...
+000003e0: 736f 7274 6564 da04 676c 6f62 da02 6f73  sorted..glob..os
+000003f0: da04 7061 7468 da04 6a6f 696e 7206 0000  ..path..joinr...
+00000400: 00da 0669 6d72 6561 64da 0573 6861 7065  ...imread..shape
+00000410: 7207 0000 00da 0a49 4e54 4552 5f41 5245  r......INTER_ARE
+00000420: 41da 0573 706c 6974 da07 696d 7772 6974  A..split..imwrit
+00000430: 6529 0c72 0f00 0000 7210 0000 0072 0700  e).r....r....r..
+00000440: 0000 7211 0000 005a 0e66 696c 655f 6578  ..r....Z.file_ex
+00000450: 7465 6e73 696f 6eda 0866 696c 656e 616d  tension..filenam
+00000460: 6572 0800 0000 da06 6865 6967 6874 da05  er......height..
+00000470: 7769 6474 68da 015f da0a 696d 6167 655f  width.._..image_
+00000480: 6e61 6d65 da0b 6f75 7470 7574 5f70 6174  name..output_pat
+00000490: 6872 0900 0000 7209 0000 0072 0a00 0000  hr....r....r....
+000004a0: da1d 6372 6561 7465 5f74 6875 6d62 6e61  ..create_thumbna
+000004b0: 696c 735f 6672 6f6d 5f66 6f6c 6465 720b  ils_from_folder.
+000004c0: 0000 0073 1200 0000 000e 2201 0a01 0c01  ...s......".....
+000004d0: 0801 1601 1001 0e01 0e01 7224 0000 0029  ..........r$...)
+000004e0: 0372 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+000004f0: 2909 7215 0000 0072 1600 0000 7206 0000  ).r....r....r...
+00000500: 0072 1b00 0000 da03 696e 7472 0b00 0000  .r......intr....
+00000510: da03 7374 72da 0566 6c6f 6174 7224 0000  ..str..floatr$..
+00000520: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000530: 720a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000540: 0000 0073 1800 0000 0801 0802 0803 1605  ...s............
+00000550: 0000 0000 00ff 0201 0200 0200 0200 02ff  ................
```

### Comparing `robologs_ros_utils-0.1.1a26/robologs_ros_utils/utils/img_utils/img_utils.py` & `robologs_ros_utils-0.1.1a27/robologs_ros_utils/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `robologs_ros_utils-0.1.1a26/setup.py` & `robologs_ros_utils-0.1.1a27/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['robologs_ros_utils',
- 'robologs_ros_utils.connectors',
- 'robologs_ros_utils.destinations.aws.athena',
- 'robologs_ros_utils.destinations.aws.dynamodb',
- 'robologs_ros_utils.destinations.aws.lambdas',
- 'robologs_ros_utils.destinations.aws.s3',
- 'robologs_ros_utils.destinations.azure',
- 'robologs_ros_utils.destinations.google_cloud',
- 'robologs_ros_utils.functions',
  'robologs_ros_utils.sources',
  'robologs_ros_utils.sources.ros1',
- 'robologs_ros_utils.utils.file_utils',
- 'robologs_ros_utils.utils.img_utils',
- 'robologs_ros_utils.utils.video_utils']
+ 'robologs_ros_utils.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bagpy>=0.5,<0.6',
  'black[d]>=22.12.0,<23.0.0',
@@ -38,15 +28,15 @@
  'types-tqdm>=4.64.7.9,<5.0.0.0']
 
 entry_points = \
 {'console_scripts': ['robologs-ros-utils = robologs_ros_utils.cli:main']}
 
 setup_kwargs = {
     'name': 'robologs-ros-utils',
-    'version': '0.1.1a26',
+    'version': '0.1.1a27',
     'description': 'robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities',
     'long_description': '',
     'author': 'roboto.ai',
     'author_email': 'info@roboto.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `robologs_ros_utils-0.1.1a26/PKG-INFO` & `robologs_ros_utils-0.1.1a27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robologs-ros-utils
-Version: 0.1.1a26
+Version: 0.1.1a27
 Summary: robologs-ros-utils is an open source library of containerized data transformations for the robotics and drone communities
 License: Apache-2.0
 Author: roboto.ai
 Author-email: info@roboto.ai
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

