# Comparing `tmp/vivintpy-2023.3.4.tar.gz` & `tmp/vivintpy-2023.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivintpy-2023.3.4.tar", max compression
+gzip compressed data, was "vivintpy-2023.3.5.tar", max compression
```

## Comparing `vivintpy-2023.3.4.tar` & `vivintpy-2023.3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1076 2023-06-26 22:21:54.390737 vivintpy-2023.3.4/LICENSE
--rw-r--r--   0        0        0     2658 2023-06-26 22:21:54.390737 vivintpy-2023.3.4/README.md
--rw-r--r--   0        0        0     1108 2023-06-26 22:22:17.543220 vivintpy-2023.3.4/pyproject.toml
--rw-r--r--   0        0        0       63 2023-06-26 22:22:17.543220 vivintpy-2023.3.4/vivintpy/__init__.py
--rw-r--r--   0        0        0     7673 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/account.py
--rw-r--r--   0        0        0     4371 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/const.py
--rw-r--r--   0        0        0     8165 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/__init__.py
--rw-r--r--   0        0        0    12054 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/alarm_panel.py
--rw-r--r--   0        0        0     9255 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/camera.py
--rw-r--r--   0        0        0     1279 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/door_lock.py
--rw-r--r--   0        0        0     2068 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/garage_door.py
--rw-r--r--   0        0        0     1798 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/switch.py
--rw-r--r--   0        0        0     3325 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/thermostat.py
--rw-r--r--   0        0        0     3274 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/wireless_sensor.py
--rw-r--r--   0        0        0     1657 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/entity.py
--rw-r--r--   0        0        0    11826 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/enums.py
--rw-r--r--   0        0        0      705 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/exceptions.py
--rw-r--r--   0        0        0    81878 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/proto/beam_pb2.py
--rw-r--r--   0        0        0   102437 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/proto/beam_pb2.pyi
--rw-r--r--   0        0        0   168580 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/proto/beam_pb2_grpc.py
--rw-r--r--   0        0        0     4657 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/pubnub.py
--rw-r--r--   0        0        0        0 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/py.typed
--rw-r--r--   0        0        0     3664 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/system.py
--rw-r--r--   0        0        0     1288 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/utils.py
--rw-r--r--   0        0        0    19437 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/vivintskyapi.py
--rw-r--r--   0        0        0   411296 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/zjs_device_config_db.json
--rw-r--r--   0        0        0     1036 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/zjs_device_config_db.py
--rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 vivintpy-2023.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-27 05:44:52.658873 vivintpy-2023.3.5/LICENSE
+-rw-r--r--   0        0        0     2658 2023-06-27 05:44:52.658873 vivintpy-2023.3.5/README.md
+-rw-r--r--   0        0        0     1120 2023-06-27 05:45:10.838946 vivintpy-2023.3.5/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-06-27 05:45:10.838946 vivintpy-2023.3.5/vivintpy/__init__.py
+-rw-r--r--   0        0        0     7673 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/account.py
+-rw-r--r--   0        0        0     4371 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/const.py
+-rw-r--r--   0        0        0     8165 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/devices/__init__.py
+-rw-r--r--   0        0        0    12054 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/devices/alarm_panel.py
+-rw-r--r--   0        0        0     9255 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/devices/camera.py
+-rw-r--r--   0        0        0     1279 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/devices/door_lock.py
+-rw-r--r--   0        0        0     2068 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/devices/garage_door.py
+-rw-r--r--   0        0        0     1798 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/devices/switch.py
+-rw-r--r--   0        0        0     3325 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/devices/thermostat.py
+-rw-r--r--   0        0        0     3274 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/devices/wireless_sensor.py
+-rw-r--r--   0        0        0     1657 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/entity.py
+-rw-r--r--   0        0        0    11826 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/enums.py
+-rw-r--r--   0        0        0      705 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/exceptions.py
+-rw-r--r--   0        0        0    81878 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/proto/beam_pb2.py
+-rw-r--r--   0        0        0   102437 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/proto/beam_pb2.pyi
+-rw-r--r--   0        0        0   168580 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/proto/beam_pb2_grpc.py
+-rw-r--r--   0        0        0     4657 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/pubnub.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/py.typed
+-rw-r--r--   0        0        0     3664 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/system.py
+-rw-r--r--   0        0        0     1288 2023-06-27 05:44:52.662873 vivintpy-2023.3.5/vivintpy/utils.py
+-rw-r--r--   0        0        0    19437 2023-06-27 05:44:52.666873 vivintpy-2023.3.5/vivintpy/vivintskyapi.py
+-rw-r--r--   0        0        0   411296 2023-06-27 05:44:52.666873 vivintpy-2023.3.5/vivintpy/zjs_device_config_db.json
+-rw-r--r--   0        0        0     1036 2023-06-27 05:44:52.666873 vivintpy-2023.3.5/vivintpy/zjs_device_config_db.py
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 vivintpy-2023.3.5/PKG-INFO
```

### Comparing `vivintpy-2023.3.4/LICENSE` & `vivintpy-2023.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/README.md` & `vivintpy-2023.3.5/README.md`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/pyproject.toml` & `vivintpy-2023.3.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "vivintpy"
-version = "2023.3.4"
+version = "2023.3.5"
 description = "Python library for interacting with a Vivint security and smart home system."
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/natekspencer/vivintpy"
 repository = "https://github.com/natekspencer/vivintpy"
 keywords = ["Vivint", "alarm system", "security", "smart home", "home automation", "asynchronous"]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8.1"
 aiohttp = "^3.8.4"
-certifi = "^2022.9.24"
+certifi = ">=2022.9.24,<2024.0.0"
 pubnub = "^7.0"
-grpcio = "1.56.0"
-protobuf = "^4.22.1"
+grpcio = "^1.51.1"
+protobuf = "^4.23.1"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^3.28.0"
 pytest = "^7.2.2"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 pytest-timeout = "^2.1.0"
```

### Comparing `vivintpy-2023.3.4/vivintpy/account.py` & `vivintpy-2023.3.5/vivintpy/account.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/const.py` & `vivintpy-2023.3.5/vivintpy/const.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/devices/__init__.py` & `vivintpy-2023.3.5/vivintpy/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/devices/alarm_panel.py` & `vivintpy-2023.3.5/vivintpy/devices/alarm_panel.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/devices/camera.py` & `vivintpy-2023.3.5/vivintpy/devices/camera.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/devices/door_lock.py` & `vivintpy-2023.3.5/vivintpy/devices/door_lock.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/devices/garage_door.py` & `vivintpy-2023.3.5/vivintpy/devices/garage_door.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/devices/switch.py` & `vivintpy-2023.3.5/vivintpy/devices/switch.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/devices/thermostat.py` & `vivintpy-2023.3.5/vivintpy/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/devices/wireless_sensor.py` & `vivintpy-2023.3.5/vivintpy/devices/wireless_sensor.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/entity.py` & `vivintpy-2023.3.5/vivintpy/entity.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/enums.py` & `vivintpy-2023.3.5/vivintpy/enums.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/exceptions.py` & `vivintpy-2023.3.5/vivintpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/proto/beam_pb2.py` & `vivintpy-2023.3.5/vivintpy/proto/beam_pb2.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/proto/beam_pb2.pyi` & `vivintpy-2023.3.5/vivintpy/proto/beam_pb2.pyi`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/proto/beam_pb2_grpc.py` & `vivintpy-2023.3.5/vivintpy/proto/beam_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/pubnub.py` & `vivintpy-2023.3.5/vivintpy/pubnub.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/system.py` & `vivintpy-2023.3.5/vivintpy/system.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/utils.py` & `vivintpy-2023.3.5/vivintpy/utils.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/vivintskyapi.py` & `vivintpy-2023.3.5/vivintpy/vivintskyapi.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/zjs_device_config_db.json` & `vivintpy-2023.3.5/vivintpy/zjs_device_config_db.json`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/vivintpy/zjs_device_config_db.py` & `vivintpy-2023.3.5/vivintpy/zjs_device_config_db.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.4/PKG-INFO` & `vivintpy-2023.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: vivintpy
-Version: 2023.3.4
+Version: 2023.3.5
 Summary: Python library for interacting with a Vivint security and smart home system.
 Home-page: https://github.com/natekspencer/vivintpy
 License: MIT
 Keywords: Vivint,alarm system,security,smart home,home automation,asynchronous
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: certifi (>=2022.9.24,<2023.0.0)
-Requires-Dist: grpcio (==1.56.0)
-Requires-Dist: protobuf (>=4.22.1,<5.0.0)
+Requires-Dist: certifi (>=2022.9.24,<2024.0.0)
+Requires-Dist: grpcio (>=1.51.1,<2.0.0)
+Requires-Dist: protobuf (>=4.23.1,<5.0.0)
 Requires-Dist: pubnub (>=7.0,<8.0)
 Project-URL: Repository, https://github.com/natekspencer/vivintpy
 Description-Content-Type: text/markdown
 
 [![pypi](https://img.shields.io/pypi/v/vivintpy?style=for-the-badge)](https://pypi.org/project/vivintpy)
 [![downloads](https://img.shields.io/pypi/dm/vivintpy?style=for-the-badge)](https://pypi.org/project/vivintpy)
 [![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1 Name: vivintpy Version: 2023.3.4 Summary: Python library
+Metadata-Version: 2.1 Name: vivintpy Version: 2023.3.5 Summary: Python library
 for interacting with a Vivint security and smart home system. Home-page: https:
 //github.com/natekspencer/vivintpy License: MIT Keywords: Vivint,alarm
 system,security,smart home,home automation,asynchronous Author: Nathan Spencer
-Author-email: natekspencer@gmail.com Requires-Python: >=3.7.2,<4.0.0
+Author-email: natekspencer@gmail.com Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: certifi
-(>=2022.9.24,<2023.0.0) Requires-Dist: grpcio (==1.56.0) Requires-Dist:
-protobuf (>=4.22.1,<5.0.0) Requires-Dist: pubnub (>=7.0,<8.0) Project-URL:
-Repository, https://github.com/natekspencer/vivintpy Description-Content-Type:
-text/markdown [![pypi](https://img.shields.io/pypi/v/vivintpy?style=for-the-
-badge)](https://pypi.org/project/vivintpy) [![downloads](https://
-img.shields.io/pypi/dm/vivintpy?style=for-the-badge)](https://pypi.org/project/
-vivintpy) [![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_â/
-ðº-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)]
-(https://ko-fi.com/natekspencer) # vivintpy Python library for interacting with
-a Vivint security and smart home system. This was built to support the `Vivint`
-integration in [Home-Assistant](https://www.home-assistant.io/) but _should_
-work outside of it too. Currently, it can be utilized via [HACS](https://
-hacs.xyz/) by adding the [hacs-vivint](https://github.com/natekspencer/hacs-
-vivint) custom repository. ## Credit This was inspired by the great work done
-by [Mike Reibard](https://github.com/Riebart/vivint.py) to reverse engineer the
-Vivint Sky API and [Ovidiu Stateina](https://github.com/ovirs/pyvivint) for the
-repository from which this is forked and expanded on. ## Features It currently
-has support for the following device types: - alarm panels - cameras - door
-locks - garage doors - switches - binary - multilevel - thermostats - wireless
-sensors - carbon monoxide - door/window - flood - glass break - motion - smoke/
-fire - etc In addition, it integrates with PubNub to receive real-time updates
-for devices. This subscription stops receiving notifications around 15-20
-minutes unless a call is made to the Vivint Sky API periodically. This
-**might** be related to the cookie expiration since it expires 20 minutes after
-the last API call was received. If another client connects, however, the
-notifications start to stream again for all currently connected clients. ##
-Usage See demo.py for a demonstration on how to use this library. ## TODO: -
-write a better readme - write some documentation - add advanced support for: -
-thermostats - add tests --- ## Support Me I'm not employed by Vivint, and
-provide this python package as-is. If you don't already own a Vivint system,
-please consider using [my referal code (kaf164)](https://www.vivint.com/
-get?refCode=kaf164&exid=165211vivint.com/get?refCode=kaf164&exid=165211) to get
-$50 off your bill (as well as a tip to me in appreciation)! If you already own
-a Vivint system and still want to donate, consider buying me a coffee â (or
-beer ðº) instead by using the link below: [Buy_Me_a_Coffee_at_ko-fi.com]_
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.4,<4.0.0) Requires-
+Dist: certifi (>=2022.9.24,<2024.0.0) Requires-Dist: grpcio (>=1.51.1,<2.0.0)
+Requires-Dist: protobuf (>=4.23.1,<5.0.0) Requires-Dist: pubnub (>=7.0,<8.0)
+Project-URL: Repository, https://github.com/natekspencer/vivintpy Description-
+Content-Type: text/markdown [![pypi](https://img.shields.io/pypi/v/
+vivintpy?style=for-the-badge)](https://pypi.org/project/vivintpy) [![downloads]
+(https://img.shields.io/pypi/dm/vivintpy?style=for-the-badge)](https://
+pypi.org/project/vivintpy) [![Buy Me A Coffee/Beer](https://img.shields.io/
+badge/Buy_Me_A_â/ðº-F16061?style=for-the-badge&logo=ko-
+fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer) # vivintpy
+Python library for interacting with a Vivint security and smart home system.
+This was built to support the `Vivint` integration in [Home-Assistant](https://
+www.home-assistant.io/) but _should_ work outside of it too. Currently, it can
+be utilized via [HACS](https://hacs.xyz/) by adding the [hacs-vivint](https://
+github.com/natekspencer/hacs-vivint) custom repository. ## Credit This was
+inspired by the great work done by [Mike Reibard](https://github.com/Riebart/
+vivint.py) to reverse engineer the Vivint Sky API and [Ovidiu Stateina](https:/
+/github.com/ovirs/pyvivint) for the repository from which this is forked and
+expanded on. ## Features It currently has support for the following device
+types: - alarm panels - cameras - door locks - garage doors - switches - binary
+- multilevel - thermostats - wireless sensors - carbon monoxide - door/window -
+flood - glass break - motion - smoke/fire - etc In addition, it integrates with
+PubNub to receive real-time updates for devices. This subscription stops
+receiving notifications around 15-20 minutes unless a call is made to the
+Vivint Sky API periodically. This **might** be related to the cookie expiration
+since it expires 20 minutes after the last API call was received. If another
+client connects, however, the notifications start to stream again for all
+currently connected clients. ## Usage See demo.py for a demonstration on how to
+use this library. ## TODO: - write a better readme - write some documentation -
+add advanced support for: - thermostats - add tests --- ## Support Me I'm not
+employed by Vivint, and provide this python package as-is. If you don't already
+own a Vivint system, please consider using [my referal code (kaf164)](https://
+www.vivint.com/get?refCode=kaf164&exid=165211vivint.com/
+get?refCode=kaf164&exid=165211) to get $50 off your bill (as well as a tip to
+me in appreciation)! If you already own a Vivint system and still want to
+donate, consider buying me a coffee â (or beer ðº) instead by using the
+link below: [Buy_Me_a_Coffee_at_ko-fi.com]_
```

