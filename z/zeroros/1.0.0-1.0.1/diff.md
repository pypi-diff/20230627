# Comparing `tmp/zeroros-1.0.0.tar.gz` & `tmp/zeroros-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroros-1.0.0.tar", last modified: Fri Jun 23 13:10:02 2023, max compression
+gzip compressed data, was "zeroros-1.0.1.tar", last modified: Tue Jun 27 15:25:04 2023, max compression
```

## Comparing `zeroros-1.0.0.tar` & `zeroros-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:10:02.015514 zeroros-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-23 13:09:52.000000 zeroros-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-23 13:10:02.011514 zeroros-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-23 13:09:52.000000 zeroros-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:10:02.015514 zeroros-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-23 13:09:52.000000 zeroros-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:10:02.011514 zeroros-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:10:02.011514 zeroros-1.0.0/src/zeroros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/datalogger.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:10:02.011514 zeroros-1.0.0/src/zeroros/messages/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/messages/geometry_msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/messages/nav_msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/messages/sensor_msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/messages/std_msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-23 13:09:52.000000 zeroros-1.0.0/src/zeroros/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:10:02.011514 zeroros-1.0.0/src/zeroros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-23 13:10:02.000000 zeroros-1.0.0/src/zeroros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-23 13:10:02.000000 zeroros-1.0.0/src/zeroros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:10:02.000000 zeroros-1.0.0/src/zeroros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 13:10:02.000000 zeroros-1.0.0/src/zeroros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 13:10:02.000000 zeroros-1.0.0/src/zeroros.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.802597 zeroros-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-27 15:24:54.000000 zeroros-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-27 15:25:04.802597 zeroros-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-27 15:24:54.000000 zeroros-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:25:04.802597 zeroros-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-27 15:24:54.000000 zeroros-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.798597 zeroros-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.798597 zeroros-1.0.1/src/zeroros/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/datalogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.802597 zeroros-1.0.1/src/zeroros/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/geometry_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/nav_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/sensor_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/std_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.802597 zeroros-1.0.1/src/zeroros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/top_level.txt
```

### Comparing `zeroros-1.0.0/LICENSE` & `zeroros-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.0/PKG-INFO` & `zeroros-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-Metadata-Version: 2.1
-Name: zeroros
-Version: 1.0.0
-Summary: ZeroROS middleware
-Home-page: https://github.com/miquelmassot/zeroros
-Author: Miquel Massot
-Author-email: miquel.massot@gmail.com
-Maintainer: Miquel Massot
-Maintainer-email: miquel.massot@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Reports, https://github.com/miquelmassot/zeroros/issues
-Project-URL: Source, https://github.com/miquelmassot/zeroros
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ZeroROS
-Python-only, dependency-free middleware that resembles ROS using ZeroMQ.
+<p align="center">
+<img src="imgs/logo.png?raw=true)" width="600"/>
+</p>
 
+# Zero-dependency ROS-like middleware for Python
 This library is intended to be used for small projects that require a simple middleware
 for communication between processes. It is not intended to be a replacement for ROS.
 
+<p align="center">
+    <a href="https://pypi.org/project/zeroros/">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/zeroros">
+    </a>
+    <a href="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml">
+        <img alt="Wheels" src="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml/badge.svg">
+    </a>
+    <a href="https://github.com/miquelmassot/zeroros/blob/main/LICENSE">
+        <img alt="License" src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg">
+    </a>
+    <br/>
+</p>
+
 ## Installation
 Use pip to install the library:
 
 ```bash
 pip install zeroros
 ```
 
@@ -100,7 +92,8 @@
 * `geometry_msgs.PoseStamped`
 * `geometry_msgs.PoseWithCovariance`
 * `geometry_msgs.TwistWithCovariance`
 * `nav_msgs.Odometry`
 * `nav_msgs.Path`
 * `sensors_msgs.LaserScan`
 * More to come...
+
```

### Comparing `zeroros-1.0.0/setup.py` & `zeroros-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # read the contents of README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="zeroros",
-    version="1.0.0",
+    version="1.0.1",
     description="ZeroROS middleware",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Miquel Massot",
     author_email="miquel.massot@gmail.com",
     maintainer="Miquel Massot",
     maintainer_email="miquel.massot@gmail.com",
```

### Comparing `zeroros-1.0.0/src/zeroros/datalogger.py` & `zeroros-1.0.1/src/zeroros/datalogger.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.0/src/zeroros/message_broker.py` & `zeroros-1.0.1/src/zeroros/message_broker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import threading
 
 import zmq
 
 
+
+
 class MessageBroker:
     def __init__(self):
         # gather list of topics from pub/subs
         self.topics = {}
+        self.context = None
         # run broker in seperate thread
         self.broker_thread = threading.Thread(target=self.config_broker)
         self.broker_thread.start()
 
     def config_broker(self):
         """connects, binds, and configure sockets"""
         # https://zguide.zeromq.org/docs/chapter2/#The-Dynamic-Discovery-Problem
         self.context = zmq.Context()
         frontend = self.context.socket(zmq.XSUB)
-        frontend.bind("tcp://127.0.0.1:5559")
+        frontend.bind("tcp://127.0.0.1:5555")
         backend = self.context.socket(zmq.XPUB)
-        backend.bind("tcp://127.0.0.1:5560")
+        backend.bind("tcp://127.0.0.1:5556")
 
         # built-in pub/sub fowarder
         zmq.proxy(frontend, backend)
 
         # Shouldn't get here
         frontend.close()
         backend.close()
```

### Comparing `zeroros-1.0.0/src/zeroros/messages/geometry_msgs.py` & `zeroros-1.0.1/src/zeroros/messages/geometry_msgs.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,14 +67,33 @@
         self.w = w  # type: float
 
     def __str__(self):
         return "Quaternion(x={}, y={}, z={}, w={})".format(
             self.x, self.y, self.z, self.w
         )
 
+    def from_euler(self, roll: float, pitch: float, yaw: float):
+        cy = np.cos(yaw * 0.5)
+        sy = np.sin(yaw * 0.5)
+        cp = np.cos(pitch * 0.5)
+        sp = np.sin(pitch * 0.5)
+        cr = np.cos(roll * 0.5)
+        sr = np.sin(roll * 0.5)
+
+        self.w = cy * cp * cr + sy * sp * sr
+        self.x = cy * cp * sr - sy * sp * cr
+        self.y = sy * cp * sr + cy * sp * cr
+        self.z = sy * cp * cr - cy * sp * sr
+
+    def to_euler(self):
+        roll = np.arctan2(2.0 * (self.w * self.x + self.y * self.z), 1.0 - 2.0 * (self.x * self.x + self.y * self.y))
+        pitch = np.arcsin(2.0 * (self.w * self.y - self.z * self.x))
+        yaw = np.arctan2(2.0 * (self.w * self.z + self.x * self.y), 1.0 - 2.0 * (self.y * self.y + self.z * self.z))
+        return roll, pitch, yaw
+
     def to_json(self):
         return {"x": self.x, "y": self.y, "z": self.z, "w": self.w}
 
     def from_json(self, json):
         self.x = json["x"]
         self.y = json["y"]
         self.z = json["z"]
```

### Comparing `zeroros-1.0.0/src/zeroros/messages/nav_msgs.py` & `zeroros-1.0.1/src/zeroros/messages/nav_msgs.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.0/src/zeroros/messages/sensor_msgs.py` & `zeroros-1.0.1/src/zeroros/messages/sensor_msgs.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.0/src/zeroros/messages/std_msgs.py` & `zeroros-1.0.1/src/zeroros/messages/std_msgs.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.0/src/zeroros/publisher.py` & `zeroros-1.0.1/src/zeroros/publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class Publisher:
     def __init__(
         self,
         topic: str,
         message_class: type[Message],
         ip: str = "127.0.0.1",
-        port: int = 5559,
+        port: int = 5555,
     ):
         print("Creating publisher for topic: ", topic)
         self.topic = validate_topic(topic)
         self.message_class = message_class
         self.ip = ip
         self.port = port
         self.context = zmq.Context()
```

### Comparing `zeroros-1.0.0/src/zeroros/subscriber.py` & `zeroros-1.0.1/src/zeroros/subscriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class Subscriber:
     def __init__(
         self,
         topic: str,
         message_class: type[Message],
         callback_handle: callable,
         ip: str = "127.0.0.1",
-        port: int = 5560,
+        port: int = 5556,
     ):
         self.ip = ip
         self.port = port
         print("Subscribing to topic: ", topic)
         self.topic = validate_topic(topic)
         self.message_class = message_class
         self.url = "tcp://" + str(self.ip) + ":" + str(self.port)
```

### Comparing `zeroros-1.0.0/src/zeroros.egg-info/PKG-INFO` & `zeroros-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroros
-Version: 1.0.0
+Version: 1.0.1
 Summary: ZeroROS middleware
 Home-page: https://github.com/miquelmassot/zeroros
 Author: Miquel Massot
 Author-email: miquel.massot@gmail.com
 Maintainer: Miquel Massot
 Maintainer-email: miquel.massot@gmail.com
 License: BSD-3-Clause
@@ -17,20 +17,35 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ZeroROS
-Python-only, dependency-free middleware that resembles ROS using ZeroMQ.
+<p align="center">
+<img src="imgs/logo.png?raw=true)" width="600"/>
+</p>
 
+# Zero-dependency ROS-like middleware for Python
 This library is intended to be used for small projects that require a simple middleware
 for communication between processes. It is not intended to be a replacement for ROS.
 
+<p align="center">
+    <a href="https://pypi.org/project/zeroros/">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/zeroros">
+    </a>
+    <a href="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml">
+        <img alt="Wheels" src="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml/badge.svg">
+    </a>
+    <a href="https://github.com/miquelmassot/zeroros/blob/main/LICENSE">
+        <img alt="License" src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg">
+    </a>
+    <br/>
+</p>
+
 ## Installation
 Use pip to install the library:
 
 ```bash
 pip install zeroros
 ```
 
@@ -100,7 +115,8 @@
 * `geometry_msgs.PoseStamped`
 * `geometry_msgs.PoseWithCovariance`
 * `geometry_msgs.TwistWithCovariance`
 * `nav_msgs.Odometry`
 * `nav_msgs.Path`
 * `sensors_msgs.LaserScan`
 * More to come...
+
```

### Comparing `zeroros-1.0.0/src/zeroros.egg-info/SOURCES.txt` & `zeroros-1.0.1/src/zeroros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

