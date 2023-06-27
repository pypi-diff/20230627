# Comparing `tmp/mini-cheetah-motor-driver-socketcan-0.4.1.tar.gz` & `tmp/mini-cheetah-motor-driver-socketcan-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini-cheetah-motor-driver-socketcan-0.4.1.tar", last modified: Thu Feb 23 16:47:07 2023, max compression
+gzip compressed data, was "mini-cheetah-motor-driver-socketcan-0.4.2.tar", last modified: Tue Jun 27 13:46:45 2023, max compression
```

## Comparing `mini-cheetah-motor-driver-socketcan-0.4.1.tar` & `mini-cheetah-motor-driver-socketcan-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 16:47:07.465743 mini-cheetah-motor-driver-socketcan-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-02-23 16:46:54.000000 mini-cheetah-motor-driver-socketcan-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-02-23 16:47:07.465743 mini-cheetah-motor-driver-socketcan-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7355 2023-02-23 16:46:54.000000 mini-cheetah-motor-driver-socketcan-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-02-23 16:46:54.000000 mini-cheetah-motor-driver-socketcan-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-02-23 16:47:07.465743 mini-cheetah-motor-driver-socketcan-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 16:47:07.465743 mini-cheetah-motor-driver-socketcan-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 16:47:07.465743 mini-cheetah-motor-driver-socketcan-0.4.1/src/mini_cheetah_motor_driver_socketcan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-02-23 16:47:07.000000 mini-cheetah-motor-driver-socketcan-0.4.1/src/mini_cheetah_motor_driver_socketcan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-02-23 16:47:07.000000 mini-cheetah-motor-driver-socketcan-0.4.1/src/mini_cheetah_motor_driver_socketcan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-23 16:47:07.000000 mini-cheetah-motor-driver-socketcan-0.4.1/src/mini_cheetah_motor_driver_socketcan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-02-23 16:47:07.000000 mini-cheetah-motor-driver-socketcan-0.4.1/src/mini_cheetah_motor_driver_socketcan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-02-23 16:47:07.000000 mini-cheetah-motor-driver-socketcan-0.4.1/src/mini_cheetah_motor_driver_socketcan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 16:47:07.465743 mini-cheetah-motor-driver-socketcan-0.4.1/src/motor_driver/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-23 16:46:54.000000 mini-cheetah-motor-driver-socketcan-0.4.1/src/motor_driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21079 2023-02-23 16:46:54.000000 mini-cheetah-motor-driver-socketcan-0.4.1/src/motor_driver/canmotorlib.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 13:46:45.840307 mini-cheetah-motor-driver-socketcan-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-06-27 13:46:37.000000 mini-cheetah-motor-driver-socketcan-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-06-27 13:46:45.840307 mini-cheetah-motor-driver-socketcan-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7355 2023-06-27 13:46:37.000000 mini-cheetah-motor-driver-socketcan-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-27 13:46:37.000000 mini-cheetah-motor-driver-socketcan-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-27 13:46:45.840307 mini-cheetah-motor-driver-socketcan-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 13:46:45.840307 mini-cheetah-motor-driver-socketcan-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 13:46:45.840307 mini-cheetah-motor-driver-socketcan-0.4.2/src/mini_cheetah_motor_driver_socketcan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-06-27 13:46:45.000000 mini-cheetah-motor-driver-socketcan-0.4.2/src/mini_cheetah_motor_driver_socketcan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-27 13:46:45.000000 mini-cheetah-motor-driver-socketcan-0.4.2/src/mini_cheetah_motor_driver_socketcan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 13:46:45.000000 mini-cheetah-motor-driver-socketcan-0.4.2/src/mini_cheetah_motor_driver_socketcan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-27 13:46:45.000000 mini-cheetah-motor-driver-socketcan-0.4.2/src/mini_cheetah_motor_driver_socketcan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-27 13:46:45.000000 mini-cheetah-motor-driver-socketcan-0.4.2/src/mini_cheetah_motor_driver_socketcan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 13:46:45.840307 mini-cheetah-motor-driver-socketcan-0.4.2/src/motor_driver/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 13:46:37.000000 mini-cheetah-motor-driver-socketcan-0.4.2/src/motor_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21168 2023-06-27 13:46:37.000000 mini-cheetah-motor-driver-socketcan-0.4.2/src/motor_driver/canmotorlib.py
```

### Comparing `mini-cheetah-motor-driver-socketcan-0.4.1/LICENSE` & `mini-cheetah-motor-driver-socketcan-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mini-cheetah-motor-driver-socketcan-0.4.1/PKG-INFO` & `mini-cheetah-motor-driver-socketcan-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-cheetah-motor-driver-socketcan
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python Driver for MIT Mini-Cheetah Actuator which uses SocketCAN for communication.
 Home-page: https://github.com/dfki-ric-underactuated-lab/mini-cheetah-tmotor-python-can
 Author: Shubham Vyas
 Author-email: Shubham.Vyas@dfki.de
 Project-URL: Bug Tracker, https://github.com/dfki-ric-underactuated-lab/mini-cheetah-tmotor-python-can/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mini-cheetah-motor-driver-socketcan-0.4.1/README.md` & `mini-cheetah-motor-driver-socketcan-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mini-cheetah-motor-driver-socketcan-0.4.1/setup.cfg` & `mini-cheetah-motor-driver-socketcan-0.4.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mini-cheetah-motor-driver-socketcan
-version = 0.4.1
+version = 0.4.2
 author = Shubham Vyas
 author_email = Shubham.Vyas@dfki.de
 description = A Python Driver for MIT Mini-Cheetah Actuator which uses SocketCAN for communication.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dfki-ric-underactuated-lab/mini-cheetah-tmotor-python-can
 project_urls =
```

### Comparing `mini-cheetah-motor-driver-socketcan-0.4.1/src/mini_cheetah_motor_driver_socketcan.egg-info/PKG-INFO` & `mini-cheetah-motor-driver-socketcan-0.4.2/src/mini_cheetah_motor_driver_socketcan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-cheetah-motor-driver-socketcan
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python Driver for MIT Mini-Cheetah Actuator which uses SocketCAN for communication.
 Home-page: https://github.com/dfki-ric-underactuated-lab/mini-cheetah-tmotor-python-can
 Author: Shubham Vyas
 Author-email: Shubham.Vyas@dfki.de
 Project-URL: Bug Tracker, https://github.com/dfki-ric-underactuated-lab/mini-cheetah-tmotor-python-can/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mini-cheetah-motor-driver-socketcan-0.4.1/src/motor_driver/canmotorlib.py` & `mini-cheetah-motor-driver-socketcan-0.4.2/src/motor_driver/canmotorlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
             self.motorParams = AK70_10_V1p1_params
 
         can_socket = (can_socket,)
         self.motor_id = motor_id
         # create a raw socket and bind it to the given CAN interface
         try:
             self.motor_socket = socket.socket(socket.AF_CAN, socket.SOCK_RAW, socket.CAN_RAW)
+            self.motor_socket.setsockopt(socket.SOL_CAN_RAW, socket.CAN_RAW_LOOPBACK, 0)
             self.motor_socket.bind(can_socket)
             self.motor_socket.settimeout(socket_timeout)
             print("Bound to: ", can_socket)
         except Exception as e:
             print("Unable to Connect to Socket Specified: ", can_socket)
             print("Error:", e)
```

