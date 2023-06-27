# Comparing `tmp/pymacnet-0.0.2.tar.gz` & `tmp/pymacnet-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymacnet-0.0.2.tar", last modified: Tue Apr 18 17:05:53 2023, max compression
+gzip compressed data, was "pymacnet-1.0.0.tar", last modified: Mon Jun 26 23:50:47 2023, max compression
```

## Comparing `pymacnet-0.0.2.tar` & `pymacnet-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 17:05:53.441067 pymacnet-0.0.2/
--rw-rw-rw-   0        0        0     1093 2023-02-28 19:02:47.000000 pymacnet-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    14464 2023-04-18 17:05:53.440069 pymacnet-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13939 2023-04-17 21:40:45.000000 pymacnet-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 17:05:53.426070 pymacnet-0.0.2/pymacnet/
--rw-rw-rw-   0        0        0    21281 2023-04-17 21:40:45.000000 pymacnet-0.0.2/pymacnet/MaccorInterface.py
--rw-rw-rw-   0        0        0       44 2023-02-28 19:02:47.000000 pymacnet-0.0.2/pymacnet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:05:53.435068 pymacnet-0.0.2/pymacnet/maccorspoofer/
--rw-rw-rw-   0        0        0    14777 2023-02-28 19:02:47.000000 pymacnet-0.0.2/pymacnet/maccorspoofer/MaccorSpoofer.py
--rw-rw-rw-   0        0        0       40 2023-02-28 19:02:47.000000 pymacnet-0.0.2/pymacnet/maccorspoofer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:05:53.439068 pymacnet-0.0.2/pymacnet/messages/
--rw-rw-rw-   0        0        0       57 2023-01-12 22:21:43.000000 pymacnet-0.0.2/pymacnet/messages/__init__.py
--rw-rw-rw-   0        0        0    10492 2023-01-17 17:08:00.000000 pymacnet-0.0.2/pymacnet/messages/messages.py
--rw-rw-rw-   0        0        0      450 2023-01-17 17:08:00.000000 pymacnet-0.0.2/pymacnet/messages/status_dictionary.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:05:53.433068 pymacnet-0.0.2/pymacnet.egg-info/
--rw-rw-rw-   0        0        0    14464 2023-04-18 17:05:53.000000 pymacnet-0.0.2/pymacnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-04-18 17:05:53.000000 pymacnet-0.0.2/pymacnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 17:05:53.000000 pymacnet-0.0.2/pymacnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 17:05:53.000000 pymacnet-0.0.2/pymacnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 17:05:53.441067 pymacnet-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1110 2023-04-18 17:05:12.000000 pymacnet-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:50:47.346696 pymacnet-1.0.0/
+-rw-rw-rw-   0        0        0     1093 2023-05-09 20:21:34.000000 pymacnet-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    16836 2023-06-26 23:50:47.337553 pymacnet-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16311 2023-06-24 03:56:53.000000 pymacnet-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 23:50:47.241369 pymacnet-1.0.0/pymacnet/
+-rw-rw-rw-   0        0        0       94 2023-06-24 03:56:53.000000 pymacnet-1.0.0/pymacnet/__init__.py
+-rw-rw-rw-   0        0        0    18025 2023-06-26 23:07:13.000000 pymacnet-1.0.0/pymacnet/channel_interface.py
+-rw-rw-rw-   0        0        0    10253 2023-06-26 23:07:13.000000 pymacnet-1.0.0/pymacnet/cycler_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:50:47.266550 pymacnet-1.0.0/pymacnet/maccorspoofer/
+-rw-rw-rw-   0        0        0    15588 2023-06-24 03:56:53.000000 pymacnet-1.0.0/pymacnet/maccorspoofer/MaccorSpoofer.py
+-rw-rw-rw-   0        0        0       40 2023-05-09 20:21:34.000000 pymacnet-1.0.0/pymacnet/maccorspoofer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:50:47.288998 pymacnet-1.0.0/pymacnet/messages/
+-rw-rw-rw-   0        0        0       57 2023-05-09 20:21:34.000000 pymacnet-1.0.0/pymacnet/messages/__init__.py
+-rw-rw-rw-   0        0        0    13055 2023-06-24 03:56:53.000000 pymacnet-1.0.0/pymacnet/messages/messages.py
+-rw-rw-rw-   0        0        0      450 2023-05-09 20:21:34.000000 pymacnet-1.0.0/pymacnet/messages/status_dictionary.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:50:47.258513 pymacnet-1.0.0/pymacnet.egg-info/
+-rw-rw-rw-   0        0        0    16836 2023-06-26 23:50:46.000000 pymacnet-1.0.0/pymacnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-06-26 23:50:46.000000 pymacnet-1.0.0/pymacnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 23:50:46.000000 pymacnet-1.0.0/pymacnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 23:50:46.000000 pymacnet-1.0.0/pymacnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 23:50:47.347696 pymacnet-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      870 2023-06-24 03:56:53.000000 pymacnet-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:50:47.335545 pymacnet-1.0.0/tests/
+-rw-rw-rw-   0        0        0     3434 2023-06-26 23:07:13.000000 pymacnet-1.0.0/tests/test_channel_interface.py
+-rw-rw-rw-   0        0        0     1336 2023-06-24 03:56:53.000000 pymacnet-1.0.0/tests/test_cycler_interface.py
+-rw-rw-rw-   0        0        0     4384 2023-06-24 03:56:53.000000 pymacnet-1.0.0/tests/test_maccor_spoofer.py
```

### Comparing `pymacnet-0.0.2/LICENSE` & `pymacnet-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymacnet-0.0.2/README.md` & `pymacnet-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,295 +1,381 @@
+Metadata-Version: 2.1
+Name: pymacnet
+Version: 1.0.0
+Summary: A class based python interface for communication and control of Maccor cyclers over Macnet.
+Home-page: https://github.com/BattGenie/pymacnet.git
+Author: Zander Nevitt
+Author-email: zandern@battgenie.life
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pymacnet
 
-`pymacnet` is a Python module that provides a channel level interface for communication and control of [Maccor cyclers](http://www.maccor.com/) via MacNet. MacNet is an interface provided by Maccor that allows for controlling their cyclers via UDP/IP and TCP/IP. `pymacnet` provides a hassle-free way to utilize MacNet with a simple python class.
+`pymacnet` is a Python module that provides cycler and channel level interfaces for communication and control of [Maccor cyclers](http://www.maccor.com/) via MacNet. MacNet is an interface provided by Maccor that allows for controlling their cyclers via UDP/IP and TCP/IP. `pymacnet` provides a hassle-free way to utilize MacNet with a simple python class.
 
-### Overview
+## Overview
 
-- [Motivation](#Motivation)
-- [Installation](#Installation)
-    - [Requirements](#Requirements)
-    - [Source Installation](#source-installation)
-- [Examples](#Examples)
+- [Motivation](#motivation)
+- [Installation](#installation)
+  - [Requirements](#requirements)
+  - [Installation Instructions](#installation-instructions)
+- [Examples](#examples)
   - [Getting Started](#getting-started)
-    - [Configuration](#Configuration)
-  - [Getting Channel Readings](#getting-channel-readings) 
+    - [CyclerInterface Configuration](#cyclerinterface-configuration)
+    - [ChannelInterface Configuration](#channelinterface-configuration)
+  - [Getting Cycler Level Information](#getting-cycler-level-information)
+  - [Getting Channel Readings](#getting-channel-readings)
   - [Starting a Test](#starting-a-test)
   - [Setting Variables](#setting-variables)
   - [Direct Control](#direct-control)
-- [Development](#Dev)
-  - [Contributing](#Contributing)
-  - [Testing](#Testing)
-    - [MaccorSpoofer](#MaccorSpoofer)
-  - [Documentation](#Documentation)
-- [License](#License)
+- [Development](#development)
+  - [Contributing](#contributing)
+  - [Testing](#testing)
+    - [MaccorSpoofer](#maccorspoofer)
+  - [Documentation](#documentation)
+- [License](#license)
 
-# <a name="Motivation"></a>Motivation
+## Motivation
 
 Why did we create `pymacnet`? This package enables a wide variety of applications such as:
 
 - Real-time data logging, monitoring and alerting
 
-`pymacnet` can be used to passively monitor running tests and log readings directly to a database, bypassing the need to manually export data. Moreover, it's possible to create automated alerts based on incoming real-time data. For example, if a test were to fault or temperature were to exceed a set threshold. While Maccor already has a built-in notification system with MacNotify, `pymacnet` provides a more flexible and customizable solution without having to directly modify test procedures. 
+`pymacnet` can be used to passively monitor running tests and log readings directly to a database, bypassing the need to manually export data. Moreover, it's possible to create automated alerts based on incoming real-time data. For example, if a test were to fault or temperature were to exceed a set threshold. While Maccor already has a built-in notification system with MacNotify, `pymacnet` provides a more flexible and customizable solution without having to directly modify test procedures.
 
 - Automated test management
 
 The GUI provided by Maccor for test management is straight-forward and easy to use, but requires significant manual work. With `pymacnet` it is possible to write programs to automatically start tests simultaneously across many channels (or even many cyclers) at once.
 
 - Testing of next generation closed-loop charging methods
 
 While conventional constant-current followed by constant-voltage (CCCV) charging has been the industry standard for many years and is well supported by cyclers, there is movement towards advanced [closed-loop control charging techniques that provide improved battery life and decreased charge times](https://battgenie.life/technology/). `pymacnet` enables testing of closed-loop battery charging methods by providing an interface between software hosting battery charging algorithms and active Maccor tests, allowing the charge current to be dynamically set.
 
-- Well tested, easy to use, community supported interface in the most popular programming language. 
+- Well tested, easy to use, community supported interface in the most popular programming language.
 
-It is entirely possible to write one's own MacNet wrapper, but `pymacnet` provides a well-tested ready to use package that takes care of lower level communication, providing a simple yet powerful interface in the most popular programming language. 
+It is entirely possible to write one's own MacNet wrapper, but `pymacnet` provides a well-tested ready to use package that takes care of lower level communication, providing a simple yet powerful interface in the most popular programming language.
 
-# <a name="Installation"></a>Installation
+## Installation
 
-## <a name="Requirements"></a>Requirements
+### Requirements
 
 `pymacnet` requires only Python 3 and packages from the standard library. It has been tested on on Windows, Mac, and Debian operating systems.
 
-## <a name="Source Installation"></a>Source Installation
+### Installation Instructions
 
-To install from source clone [this repository](https://github.com/BattGenie/pymacnet), navigate into the directory, and type the following into the command line:
+Install pymacnet using pip:
 
+```sh
+pip install pymacnet
 ```
+
+Install pymacnet from source code:
+
+```sh
+git clone https://github.com/BattGenie/pymacnet.git
+cd pymacnet
+pip install -r requirements.txt
 pip install .
 ```
 
-# <a name="Examples"></a>Examples
+## Examples
+
+This section goes over various examples of how to use `pymacnet` to do such tasks as getting channel readings, starting a test, and even controlling a channel directly without a test procedure. For interactive examples see the `demo.ipynb` notebook in the repository.
+
+### Getting Started
+
+`pymacnet` provides two classes for interacting with a Maccor cycler:
 
-This section goes over various of examples of how to use `pymacnet` to do such tasks as getting channel readings, starting a test, and even controlling a channel directly without a test procedure. For interactive examples see the `demo.ipynb` notebook in the repository. 
+- `CyclerInterface` Provides a cycler level interface. The class instance allows for reading cycler level information, such as system software and configuration information, and statuses of all channels.
 
-## <a name="Getting Started"></a>Getting Started
+- `ChannelInterface` Provides a channel level interface for a specific channel on the cycler. `ChannelInterface` is a child class of `CyclerInterface` so all the same cycler level methods are available, but with `ChannelInterface` it's possible to read more detailed information about a channel and even even control it. Each class instance targets a specific channel of the cycler.
 
-`pymacnet` provides a class `MaccorInterface` that communicates with the Maccor cycler via MacNet. Each class instance targets a specific channel of the cycler and requires a configuration dictionary with the following fields:
+#### CyclerInterface Configuration
 
-### <a name="Configuration"></a>Configuration
+The fields required in a `CyclerInterface` configuration dictionary are as follows:
 
+- `server_ip` - The IP address of the Maccor server. Use 127.0.0.1 if running on the same machine as the server.
+- `json_msg_port` - The port to communicate through with JSON messages. Default set to 57570.
+- `bin_msg_port` - The port to communicate through with binary messages. Default set to 57560.
+- `msg_buffer_size_bytes` - How big of a message buffer to use for sending/receiving messages. A minimum of 1024 bytes is recommended. 
+
+#### ChannelInterface Configuration
+
+The fields required in a `ChannelInterface` configuration dictionary are as follows:
+
+- `server_ip` - The IP address of the Maccor server. Use 127.0.0.1 if running on the same machine as the server.
+- `json_msg_port` - The port to communicate through with JSON messages. Default set to 57570.
+- `bin_msg_port` - The port to communicate through with binary messages. Default set to 57560.
+- `msg_buffer_size_bytes` - How big of a message buffer to use for sending/receiving messages. A minimum of 1024 bytes is recommended. 
 - `channel` - The channel to be targeted for all operations.
 - `test_name` - The test name to be used for any tests started. If left blank, Maccor will generate a unique random name for any started tests. Note that Maccor requires unique test names for each test.
 - `test_procedure` - The test procedure to be used, if starting a test with a procedure. Not needed with direct control.
 - `c_rate_ah` - The capacity value to be referenced when setting "C" values within the Maccor schedule. Units of amp-hours. Ignored if not used anywhere in the test.
 - `v_max_safety_limit_v` - Upper voltage safety limit for the channel. Units of volts.
 - `v_min_safety_limit_v` - Lower voltage safety limit for the channel. Units of volts.
 - `i_max_safety_limit_a` - Upper current safety limit for the channel. Units of amps.
 - `i_min_safety_limit_a` - Lower current safety limit for the channel. Units of amps.
 - `v_max_v` - Upper voltage limit used for charge/CV limits. Units of volts. Only used with direct control.
 - `v_min_v` - Lower voltage limit used for discharge limit. Units of volts. Only used with direct control.
 - `data_record_time_s` - How often data points are taken during direct control tests. Zero turns off. Used only for direct control.
 - `data_record_voltage_delta_vbys` - The dV/dt at which data points are taken during direct control tests. Zero disables. Used only for direct control.
 - `data_record_current_delta_abys` - The dI/dt at which data points are taken during direct control tests. Zero disables. Used only for direct control.
-- `server_ip` - The IP address of the Maccor server. Use 127.0.0.1 if running on the same machine as the server.
-- `json_server_port` - The port to communicate through with JSON commands. Default set to 57570.
-- `tcp_server_port` - The port to communicate through with TCP commands. Default set to 57560.
 
-## <a name="Readings"></a>Getting Channel Readings
+### Getting Cycler Level Information
+
+Here is some example code for getting cycler level readings with the `CyclerInterface` class. 
+
+```python
+import time
+import sys
+import pymacnet 
+
+config = {
+    "server_ip": "127.0.0.1",
+    "json_msg_port": 57570,
+    "bin_msg_port": 57560,
+    "msg_buffer_size_bytes": 1024
+}
+    
+cycler_interface = pymacnet.CyclerInterface(config)
+if not channel_interface.start():
+    sys.exit("failed to create connection!")
+
+system_info = cycler_interface.read_system_info()
+print(system_info)
+
+general_info = cycler_interface.read_general_info()
+print(general_info)
+
+channel_statuses = cycler_interface.read_all_channel_statuses()
+print(channel_statuses)
+```
+
+Example output:
+
+```text
+{'FClass': 1, 'FNum': 1, 'APIVersion': 1, 'MacTest32EXEversionMajor': 3, 'MacTest32EXEversionMinor': 2, 'MacTest32EXEversionBuild': 18 'MacTest32DLLversionMajor': 3, 'MacTest32DLLversionMsinor': 2, 'MacTest32DLLversionBuild': 18, 'MacTest32ExeDT': '2016-11-08T15:02:58', 'MacTest32DLLDT': '2016-11-13T11:29:48'}
+```
+
+```text
+{'FClass': 1, 'FNum': 2, 'SystemID': 'Win10', 'SystemType': 0, 'ControllerBoards': 3, 'TestChannels': 12, 'AuxBoards': 1, 'AuxChannels': 128, 'SMB1Pos': 0, 'SMB3Pos': 1}
+```
+
+```text
+[{'RF1': 0, 'RF2': 0, 'Stat': 0}, {'RF1': 0, 'RF2': 0, 'Stat': 0}]
+```
+
+### Getting Channel Readings
 
-Below is example code for reading channel status (which includes voltage, current, etc.) from channel 75 on a Maccor cycler with IP address `3.3.31.83`.
+Below is example code for reading channel status (which includes voltage, current, etc.) from channel 75.
 
 ```python
 import time
 import sys
 import pymacnet 
 
 config = {
+    "server_ip": "127.0.0.1",
+    "json_msg_port": 57570,
+    "bin_msg_port": 57560,
+    "msg_buffer_size_bytes": 1024
     "channel": 75,
     "test_name": "",
     "c_rate_ah": 1,
     "v_max_v": 4.2,
     "v_min_v": 3.0,
     "v_max_safety_limit_v": 4.25,
     "v_min_safety_limit_v": 2.9,
     "i_max_safety_limit_a": 3.0,
     "i_min_safety_limit_a": 3.0,
     "data_record_time_s": 0.05,
     "data_record_voltage_delta_vbys": 0.0,
     "data_record_current_delta_abys": 0.0,
     "test_procedure": "test_procedure_1",
-    "server_ip": "3.3.31.83",
-    "json_server_port": 57570,
-    "tcp_server_port": 57560,
-    "msg_buffer_size_bytes": 1024
 }
     
-maccor_interface = pymacnet.MaccorInterface(config)
-if not maccor_interface.start():
+channel_interface = pymacnet.ChannelInterface(config)
+if not channel_interface.start():
     sys.exit("failed to create connection!")
 
-status_reading = maccor_interface.read_status()
+status_reading = channel_interface.read_status()
 print(status_reading)
 ```
 
 Example output:
 
-```
+```text
 {'FClass': 4, 'FNum': 7, 'Chan': 1, 'RF1': 0, 'RF2': 192, 'Stat': 0, 'LastRecNum': 4225, 'Cycle': 0, 'Step': 5, 'TestTime': 2.0, 'StepTime': 1.0, 'Capacity': 0, 'Energy': 0, 'Current': 0, 'Voltage': 3.85, 'TesterTime': '2022-10-13T12:32:56'}
 ```
 
-## <a name="Test"></a>Starting a Test
+### Starting a Test
 
-Here is in example of how to start a test named "simple_test_1" on channel 75 with an existing test procedure named "test_procedure_1". Note the safety limits defined in the config will be set on the channel before starting the test. Also, test names must be unique. If a non-unique test name is provided then the test will not start. If no test name is provided then a unique random test name is generated. 
+Here is in example of how to start a test named "simple_test_1" on channel 75 with an existing test procedure named "test_procedure_1". Note the safety limits defined in the config will be set on the channel before starting the test. Also, test names must be unique. If a non-unique test name is provided then the test will not start. If no test name is provided then a unique random test name is generated.
 
 ```python
 import pymacnet
 import sys
 
 config = {
+    "server_ip": "127.0.0.1",
+    "json_msg_port": 57570,
+    "bin_msg_port": 57560,
+    "msg_buffer_size_bytes": 1024
     "channel": 75,
     "test_name": "simple_test_1",
     "c_rate_ah": 1,
     "v_max_v": 4.2,
     "v_min_v": 3.0,
     "v_max_safety_limit_v": 4.25,
     "v_min_safety_limit_v": 2.9,
     "i_max_safety_limit_a": 3.0,
     "i_min_safety_limit_a": 3.0,
     "data_record_time_s": 0.05,
     "data_record_voltage_delta_vbys": 0.0,
     "data_record_current_delta_abys": 0.0,
     "test_procedure": "test_procedure_1",
-    "server_ip": "3.3.31.83",
-    "json_server_port": 57570,
-    "tcp_server_port": 57560,
-    "msg_buffer_size_bytes": 1024
 }
-maccor_interface = pymacnet.MaccorInterface(config_dict)
-if not maccor_interface.start():
+channel_interface = pymacnet.ChannelInterface(config_dict)
+if not channel_interface.start():
     sys.exit("failed to create connection!")
 
-if maccor_interface.start_test_with_procedure():
+if channel_interface.start_test_with_procedure():
     print("Test started!")
 ```
 
-## <a name="Variables"></a>Setting Variables
+### Setting Variables
 
 Here is an example of how to set VAR1 to 0.01 on a test running on channel 75.
 
 ```python
 import pymacnet
 import sys
 
 config = {
+    "server_ip": "127.0.0.1",
+    "json_msg_port": 57570,
+    "bin_msg_port": 57560,
+    "msg_buffer_size_bytes": 1024
     "channel": 75,
     "test_name": "",
     "c_rate_ah": 1,
     "v_max_v": 4.2,
     "v_min_v": 3.0,
     "v_max_safety_limit_v": 4.25,
     "v_min_safety_limit_v": 2.9,
     "i_max_safety_limit_a": 3.0,
     "i_min_safety_limit_a": 3.0,
     "data_record_time_s": 0.05,
     "data_record_voltage_delta_vbys": 0.0,
     "data_record_current_delta_abys": 0.0,
     "test_procedure": "test_procedure_1",
-    "server_ip": "3.3.31.83",
-    "json_server_port": 57570,
-    "tcp_server_port": 57560,
-    "msg_buffer_size_bytes": 1024
 }
 
-maccor_interface = pymacnet.MaccorInterface(config_dict)
-if not maccor_interface.start():
+channel_interface = pymacnet.ChannelInterface(config_dict)
+if not channel_interface.start():
     sys.exit("failed to create connection!")
 
-maccor_interface.set_channel_variable(var_num = 1, var_value = 0.01)
+channel_interface.set_channel_variable(var_num = 1, var_value = 0.01)
 ```
 
-## <a name="Direct"></a>Direct Control
+### Direct Control
 
 Here is an example of how to bypass using a test procedure all together and control the channel directly using direct control.  Note the channel safety limits will be set before the test is started. **WARNING DIRECT CONTROL IS POTENTIALLY DANGEROUS. BE CAREFUL AND MAKE SURE YOU UNDERSTAND EXACTLY WHAT YOUR CODE IS DOING.**
 
 ```python
 import pymacnet
 import sys
 
 config = {
+    "server_ip": "127.0.0.1",
+    "json_msg_port": 57570,
+    "bin_msg_port": 57560,
+    "msg_buffer_size_bytes": 1024
     "channel": 75,
     "test_name": "",
     "c_rate_ah": 1,
     "v_max_v": 4.2,
     "v_min_v": 3.0,
     "v_max_safety_limit_v": 4.25,
     "v_min_safety_limit_v": 2.9,
     "i_max_safety_limit_a": 3.0,
     "i_min_safety_limit_a": 3.0,
     "data_record_time_s": 0.05,
     "data_record_voltage_delta_vbys": 0.0,
     "data_record_current_delta_abys": 0.0,
     "test_procedure": "test_procedure_1",
-    "server_ip": "3.3.31.83",
-    "json_server_port": 57570,
-    "tcp_server_port": 57560,
-    "msg_buffer_size_bytes": 1024
 }
 
-maccor_interface = pymacnet.MaccorInterface(config_dict)
-if not maccor_interface.start():
+channel_interface = pymacnet.ChannelInterface(config_dict)
+if not channel_interface.start():
     sys.exit("failed to create connection!")
 
-if maccor_interface.start_test_with_direct_control():
+if channel_interface.start_test_with_direct_control():
     print("Test started!")
 else:
     sys.exit("Failed to start test!")
 
-time.sleep(1) # Must wait at least 100 ms between trying to set contro
+time.sleep(1) # Must wait at least 100 ms between trying to set control
 
 # Discharge at 200 mA for 5 seconds. 
-maccor_interface.set_direct_mode_output(current_a = -0.200)
+channel_interface.set_direct_mode_output(current_a = -0.200)
 time.sleep(5)
 
 # Rest for 5 seconds
-maccor_interface.set_direct_mode_output(current_a = 0)
+channel_interface.set_direct_mode_output(current_a = 0)
 time.sleep(5) 
 
 # Charge at 200 mA for 5 seconds
-maccor_interface.set_direct_mode_output(current_a = 0.200)
+channel_interface.set_direct_mode_output(current_a = 0.200)
 time.sleep(5)
 
-maccor_interface.set_direct_mode_output(current_a = 0.0)
+channel_interface.set_direct_mode_output(current_a = 0.0)
 time.sleep(1)
 ```
 
-# <a name="Dev"></a>Development
+## Development
 
 This section contains various information to help developers further extend and test `pymacnet`
 
-## <a name="Contributing"></a>Contributing
+### Contributing
 
 As it exists now, `pymacnet` only implements a fraction of the messages supported by MacNet. Further work can be done to expand `pymacnet` to include more of the messages detailed in the MacNet documentation `docs/macnet_from_maccor_help.pdf`.
 
-We welcome your help in expanding `pymacnet`! Please see the [CONTRIBUTING.md](https://github.com/BattGenie/pymacnet/blob/main/CONTRIBUTING.md) file in this repository for contribution guideliens. 
+We welcome your help in expanding `pymacnet`! Please see the [CONTRIBUTING.md](https://github.com/BattGenie/pymacnet/blob/main/CONTRIBUTING.md) file in this repository for contribution guidelines.
 
-## <a name="Testing"></a>Testing
+### Testing
 
 To run the tests navigate to the "tests" directory and type the following:
 
-```
+```sh
 pytest .
 ```
 
-### <a name="MaccorSpoofer"></a>MaccorSpoofer
+#### MaccorSpoofer
 
-Testing software on a real cycler is dangerous so we've created a submodule `maccorspoofer` to emulate some of the behavior of the Maccor software with a class `MaccorSpoofer`. This class creates TCP and UDP servers and accepts connections from n number of clients. The `MaccorSpoofer` does not perfectly emulate a Maccor cycler (for example, it does not track if a test is already running on a channel) and merely checks that the message format is correct and responds with standard message. 
+Testing software on a real cycler is dangerous so we've created a submodule `maccorspoofer` to emulate some of the behavior of the Maccor software with a class `MaccorSpoofer`. This class creates TCP and UDP servers and accepts connections from n number of clients. The `MaccorSpoofer` does not perfectly emulate a Maccor cycler (for example, it does not track if a test is already running on a channel) and merely checks that the message format is correct and responds with standard message.
 
-## <a name="Documentation"></a>Documentation
+### Documentation
 
 All documentation was generated with [pydoc](https://docs.python.org/3/library/pydoc.html). To re-generate the documentation type the following command from the top level directory of the repository:
 
-```
+```sh
 pdoc --html .
 ```
 
-# <a name="License"></a>License
+## License
 
 MIT License
 
-Copyright (c) 2023 BattGenie Inc. 
+Copyright (c) 2023 BattGenie Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymacnet-0.0.2/pymacnet/MaccorInterface.py` & `pymacnet-1.0.0/pymacnet/channel_interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,291 +1,121 @@
-import socket
 import logging
-import json
-import struct
 import copy
 import pymacnet.messages
 from datetime import datetime
+from .cycler_interface import CyclerInterface
 
-log = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
-class MaccorInterface:
+class ChannelInterface(CyclerInterface):
     """
     Class for controlling Maccor Cycler using MacNet.
     """
 
-    __msg_buffer_size_bytes = 1024
-
     def __init__(self, config: dict):
         """
-        Creates a class instance. The `start()` method still needs to be run to create the connection.
+        Creates a ChannelInterface class instance.
 
         Parameters
         ----------
         config : dict
-            A configuration dictionary. See the README.md for a detailed breakdown of all parameters 
-            that must be included.
-        """
-
-        # Channels are zero indexed within Macnet so we must subtract one here.
-        self.channel = config['channel'] - 1
-        self.config = config
-        self.__json_sock = None
-        self.__tcp_sock = None
-
-    def start(self) -> bool:
-        """
-        Verifies that the config passed during construction is valid and creates connections to 
-        the Maccor server.
-
-        Returns
-        -------
-        success : bool
-            True or False based on whether the config passed at construction is valid.
-        """
-        if not self.__verify_config():
-            return False
-        elif not self.__create_connection():
-            return False
-        else:
-            return True
-
-    def __verify_config(self) -> bool:
-        """
-        Verifies that the config passed on construction is valid.
-
-        Returns
-        --------------------------
-        success : bool
-            True or False based on whether the config passed at construction is valid.
-        """
-
-        required_config_keys = ['channel',
-                                'test_name',
-                                'test_procedure',
-                                'v_max_safety_limit_v',
-                                'v_min_safety_limit_v',
-                                'i_max_safety_limit_a',
-                                'i_min_safety_limit_a',
-                                'v_max_v',
-                                'v_min_v',
-                                'c_rate_ah',
-                                'data_record_time_s',
-                                'data_record_voltage_delta_vbys',
-                                'data_record_current_delta_abys',
-                                'server_ip',
-                                'json_server_port',
-                                'tcp_server_port']
-
-        for key in required_config_keys:
-            if key not in self.config:
-                log.error("Missing key from config! Missing : " + key)
-                return False
-        return True
-
-    def __create_connection(self) -> bool:
-        """
-        Creates a connection with Maccor server to send/receive JSON and binary messages.
-
-        Returns
-       ----------
-        success : bool
-            True or False based on whether the connection was created successfully
-        """
-        try:
-            self.__json_sock = socket.socket(
-                socket.AF_INET, socket.SOCK_STREAM
-            )
-            self.__json_sock.connect(
-                (self.config['server_ip'], self.config['json_server_port'])
-            )
-        except:
-            log.error(
-                "Failed to create JSON TCP connection with Maccor server!", exc_info=True)
-            return False
-        try:
-            self.__tcp_sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            self.__tcp_sock.connect(
-                (self.config['server_ip'], self.config['tcp_server_port'])
-            )
-        except:
-            log.error(
-                "Failed to create TCP connection with Maccor server!", exc_info=True)
-            return False
-
-        return True
-
-    def __send_receive_msg(self, outgoing_msg_dict) -> dict:
-        """
-        Takes in a message dictionary, packs it, sends it to the Maccor server, and unpacks the response.
-
-        Parameters
-        ----------
-        msg_outgoing_dict : dict
-            A dictionary containing the message to be sent.
-
-        Returns
-        ----------
-        msg_incoming_dict : dict
-            A dictionary containing the message response. Returns None if there is an issue.
-        """
-
-        # Make Sure this is json_socket connection exists first.
-        if self.__json_sock:
-            pass
-        else:
-            log.error("json_socket connection does not exist!", exc_info=True)
-            return None
-        # Pack message
-        try:
-            msg_outgoing_packed = json.dumps(outgoing_msg_dict, indent=4)
-            msg_outgoing_packed = msg_outgoing_packed.encode()
-        except:
-            log.error("Error packing outgoing message!", exc_info=True)
-            return None
-        # Send message
-        try:
-            self.__json_sock.send(msg_outgoing_packed)
-        except:
-            log.error("Error sending message!", exc_info=True)
-            return None
-        # Receive response
-        try:
-            msg_incoming_packed = self.__json_sock.recv(
-                self.__msg_buffer_size_bytes
-            )
-        except:
-            log.error("Error receiving message!", exc_info=True)
-            return None
-        # Unpack response
-        try:
-            msg_incoming_dict = json.loads(msg_incoming_packed.decode('utf-8'))
-        except:
-            log.error("Error unpacking incoming message!", exc_info=True)
-            log.error("Message: " + str(msg_incoming_packed))
-            return None
-
-        # If the response messages has the channel in it add 1 so things look correct to user.
-        if 'result' in msg_incoming_dict.keys():
-            if 'Chan' in msg_incoming_dict['result'].keys():
-                msg_incoming_dict['result']['Chan'] += 1
+            A configuration dictionary. Must contain the following keys:
+            - `server_ip` - The IP address of the Maccor server. Use 127.0.0.1 if running on the same machine as the server.
+            - `json_msg_port` - The port to communicate through with JSON messages. Default set to 57570.
+            - `bin_msg_port` - The port to communicate through with binary messages. Default set to 57560.
+            - `msg_buffer_size_bytes` - How big of a message buffer to use for sending/receiving messages. A minimum of 1024 bytes is recommended. 
+            - `channel` - The channel to be targeted for all operations.
+            - `test_name` - The test name to be used for any tests started. If left blank, Maccor will generate a unique random name for any started tests. Note that Maccor requires unique test names for each test.
+            - `test_procedure` - The test procedure to be used, if starting a test with a procedure. Not needed with direct control.
+            - `c_rate_ah` - The capacity value to be referenced when setting "C" values within the Maccor schedule. Units of amp-hours. Ignored if not used anywhere in the test.
+            - `v_max_safety_limit_v` - Upper voltage safety limit for the channel. Units of volts.
+            - `v_min_safety_limit_v` - Lower voltage safety limit for the channel. Units of volts.
+            - `i_max_safety_limit_a` - Upper current safety limit for the channel. Units of amps.
+            - `i_min_safety_limit_a` - Lower current safety limit for the channel. Units of amps.
+            - `v_max_v` - Upper voltage limit used for charge/CV limits. Units of volts. Only used with direct control.
+            - `v_min_v` - Lower voltage limit used for discharge limit. Units of volts. Only used with direct control.
+            - `data_record_time_s` - How often data points are taken during direct control tests. Zero turns off. Used only for direct control.
+            - `data_record_voltage_delta_vbys` - The dV/dt at which data points are taken during direct control tests. Zero disables. Used only for direct control.
+            - `data_record_current_delta_abys` - The dI/dt at which data points are taken during direct control tests. Zero disables. Used only for direct control.
+        """
+
+        # Channels are zero indexed within MacNet so we must subtract one here.
+        self.__channel = config['channel'] - 1
+        self.__config = config
+
+        assert (self.__verify_config())
+        super().__init__(config=config)
+
+    def get_channel_number(self):
+        '''
+        Returns the channel number for the class instance.
+        '''
+        return self.__channel
 
-        return msg_incoming_dict
-
-    def read_status(self) -> dict:
+    def read_channel_status(self) -> dict:
         """
         Method to read the status of the channel defined in the config.
 
         Returns
         -------
         status : dict
             A dictionary detailing the status of the channel. Returns None if there is an issue.
         """
-
-        msg_outging_dict = copy.deepcopy(pymacnet.messages.tx_read_status_msg)
-        msg_outging_dict['params']['Chan'] = self.channel
-
-        status = self.__send_receive_msg(msg_outging_dict)
-
-        if status:
-            return status['result']
-        else:
-            log.error("Failed to read channel status")
-            return None
+        
+        # Add 1 to channel index since 1 is subtracted as part of init.
+        return super().read_channel_status(channel=(self.__channel+1))
 
     def read_aux(self) -> list:
         """
         Reads the auxiliary readings for the channel specified in the config.
 
         Returns
         -------
         aux_readings : list
             A list of the auxiliary readings.
         """
 
-        msg_outging_dict = copy.deepcopy(pymacnet.messages.tx_read_aux_msg)
-        msg_outging_dict['params']['Chan'] = self.channel
+        msg_outgoing_dict = copy.deepcopy(pymacnet.messages.tx_read_aux_msg)
+        msg_outgoing_dict['params']['Chan'] = self.__channel
 
-        aux_readings = self.__send_receive_msg(msg_outging_dict)
+        aux_readings = self._send_receive_json_msg(msg_outgoing_dict)
         if aux_readings:
             return aux_readings['result']['AuxValues']
         else:
-            log.error("Failed to read channel aux values!")
+            logger.error("Failed to read channel aux values!")
             return None
 
     def reset_channel(self) -> bool:
         """
         Resets the channel. Note this will stop any actively running test on the target channel.
 
         Returns
         -------
         success : bool
             True of False based on whether the test was started or not.
         """
-        msg_outging_dict = copy.deepcopy(
+        msg_outgoing_dict = copy.deepcopy(
             pymacnet.messages.tx_reset_channel_msg
         )
-        msg_outging_dict['params']['Chan'] = self.channel
+        msg_outgoing_dict['params']['Chan'] = self.__channel
 
-        reply = self.__send_receive_msg(msg_outging_dict)
+        reply = self._send_receive_json_msg(msg_outgoing_dict)
         if reply:
             if reply['result']['Result'] == 'OK':
                 success = True
             else:
-                log.error("Failed reset channel! Channel did not reset!")
+                logger.error("Failed reset channel! Channel did not reset!")
                 success = False
         else:
-            log.error("Failed reset channel! Did not receive reply!")
+            logger.error("Failed reset channel! Did not receive reply!")
             success = False
 
         return success
 
-    def __set_channel_safety_limits(self) -> bool:
-        """
-        Sets channel safety limits on the channel specified in the config. 
-
-        Returns
-        -------
-        success : bool
-            Returns True/False based on whether the safety limits were set correctly.
-        """
-        msg_outging_dict = copy.deepcopy(
-            pymacnet.messages.tx_set_safety_limits_msg
-        )
-        msg_outging_dict['params']['Chan'] = self.channel
-        msg_outging_dict['params']['VSafeMax'] = self.config['v_max_safety_limit_v']
-        msg_outging_dict['params']['VSafeMin'] = self.config['v_min_safety_limit_v']
-        msg_outging_dict['params']['ISafeChg'] = self.config['i_max_safety_limit_a']
-        msg_outging_dict['params']['ISafeDis'] = self.config['i_min_safety_limit_a']
-
-        # Check to make sure all safety limits were set correctly
-        reply = self.__send_receive_msg(msg_outging_dict)
-        if reply:
-            try:
-                assert ((reply['result']['Chan']) == self.config['channel'])
-                assert (abs(reply['result']['VSafeMax'] -
-                        self.config['v_max_safety_limit_v']) < 0.001)
-                assert (abs(reply['result']['VSafeMin'] -
-                        self.config['v_min_safety_limit_v']) < 0.001)
-                assert (abs(reply['result']['ISafeChg'] -
-                        self.config['i_max_safety_limit_a']) < 0.001)
-                assert (abs(reply['result']['ISafeDis'] -
-                        self.config['i_min_safety_limit_a']) < 0.001)
-            except:
-                log.error(
-                    "Set safety limits to not match sent safety limits! Message response: " + str(reply))
-                return False
-        else:
-            log.error(
-                "Failed to receive reply message when trying to set safety limits!")
-            return False
-
-        return True
-
     def set_channel_variable(self, var_num=1, var_value=0) -> bool:
         """
         Sets test variables on the target channel. See the "Variables" section in the 
         Maccor manual for more details about how to use these in tests.
 
         Parameters
         ----------
@@ -295,30 +125,31 @@
             Value to set the variable to.
 
         Returns
         -------
         success : bool
             True of False based on whether or not the variable value was set.
         """
-        msg_outging_dict = copy.deepcopy(pymacnet.messages.tx_set_variable_msg)
-        msg_outging_dict['params']['Chan'] = self.channel
-        msg_outging_dict['params']['VarNum'] = var_num
-        msg_outging_dict['params']['Value'] = var_value
+        msg_outgoing_dict = copy.deepcopy(
+            pymacnet.messages.tx_set_variable_msg)
+        msg_outgoing_dict['params']['Chan'] = self.__channel
+        msg_outgoing_dict['params']['VarNum'] = var_num
+        msg_outgoing_dict['params']['Value'] = var_value
 
         # Check to make variable was set
-        reply = self.__send_receive_msg(msg_outging_dict)
+        reply = self._send_receive_json_msg(msg_outgoing_dict)
         if reply:
             try:
-                assert ((reply['result']['Chan']) == self.config['channel'])
+                assert ((reply['result']['Chan']) == self.__config['channel'])
                 assert (reply['result']['Result'] == 'OK')
             except:
-                log.error("Variable not set!")
+                logger.error("Variable not set!")
                 return False
         else:
-            log.error(
+            logger.error(
                 "Failed to receive reply message when trying to set variable!")
             return False
 
         return True
 
     def start_test_with_procedure(self) -> bool:
         """
@@ -326,109 +157,111 @@
         Note that it will not start a test if the channel is current running a test.
 
         Returns
         -------
         success : bool
             True of False based on whether the test was started or not
         """
-        msg_outging_dict = copy.deepcopy(
+        msg_outgoing_dict = copy.deepcopy(
             pymacnet.messages.tx_start_test_with_procedure_msg)
-        msg_outging_dict['params']['Chan'] = self.channel
-        msg_outging_dict['params']['ProcName'] = self.config['test_procedure']
-        msg_outging_dict['params']['Crate'] = self.config['c_rate_ah']
-        msg_outging_dict['params']['Comment'] = "Started with pymacnet at " + \
+        msg_outgoing_dict['params']['Chan'] = self.__channel
+        msg_outgoing_dict['params']['ProcName'] = self.__config['test_procedure']
+        msg_outgoing_dict['params']['Crate'] = self.__config['c_rate_ah']
+        msg_outgoing_dict['params']['Comment'] = "Started with pymacnet at " + \
             str(datetime.timestamp(datetime.now()))
 
         # If test name is not specified then start test with a random test
-        if not self.config['test_name']:
-            msg_outging_dict['params']['TestName'] = 'Random'
+        if not self.__config['test_name']:
+            msg_outgoing_dict['params']['TestName'] = 'Random'
         else:
-            msg_outging_dict['params']['TestName'] = self.config['test_name']
+            msg_outgoing_dict['params']['TestName'] = self.__config['test_name']
 
         # Check the status of the channel before we try to start the test.]
-        status = self.read_status()
+        status = self.read_channel_status()
         if status:
             if pymacnet.messages.status_dictionary[status['Stat']] == 'Completed':
                 self.reset_channel()
         else:
-            log.error("Cannot read channel status!")
+            logger.error("Cannot read channel status!")
             return False
 
         # Set the safety limits.
         if not self.__set_channel_safety_limits():
-            log.error("Failed to set channel safety limits!")
+            logger.error("Failed to set channel safety limits!")
             return False
 
         # Start the test.
-        response = self.__send_receive_msg(msg_outging_dict)
+        response = self._send_receive_json_msg(msg_outgoing_dict)
         if response:
             if response['result']['Result'] != 'OK':
-                log.error("Error starting test! Comment from Maccor: " +
-                          response['result']['Result'])
+                logger.error("Error starting test! Comment from Maccor: " +
+                             response['result']['Result'])
                 return False
             else:
                 return True
         else:
-            log.error("Failed to get message response when trying to start test!")
+            logger.error(
+                "Failed to get message response when trying to start test!")
             return False
 
     def start_test_with_direct_control(self) -> bool:
         """
         Starts a test to be manually controlled with direct output on the channel specified in the config.
 
         Returns
         -------
         success : bool
             True of False based on whether the test was started or not.
         """
 
-        msg_outging_dict = copy.deepcopy(
+        msg_outgoing_dict = copy.deepcopy(
             pymacnet.messages.tx_start_test_with_direct_control_msg)
-        msg_outging_dict['params']['Chan'] = self.channel
-        msg_outging_dict['params']['DataTime'] = self.config['data_record_time_s']
-        msg_outging_dict['params']['DataV'] = self.config['data_record_voltage_delta_vbys']
-        msg_outging_dict['params']['DataI'] = self.config['data_record_current_delta_abys']
+        msg_outgoing_dict['params']['Chan'] = self.__channel
+        msg_outgoing_dict['params']['DataTime'] = self.__config['data_record_time_s']
+        msg_outgoing_dict['params']['DataV'] = self.__config['data_record_voltage_delta_vbys']
+        msg_outgoing_dict['params']['DataI'] = self.__config['data_record_current_delta_abys']
         # Make sure the start current is always zero.
-        msg_outging_dict['params']['Current'] = 0
+        msg_outgoing_dict['params']['Current'] = 0
         # Set to something within range so it's not disabled.
-        msg_outging_dict['params']['Voltage'] = self.config['v_max_v']
+        msg_outgoing_dict['params']['Voltage'] = self.__config['v_max_v']
         # TODO: FIX having a weird issue where I can't set the mode to rest.
-        msg_outging_dict['params']['ChMode'] = "C"
+        msg_outgoing_dict['params']['ChMode'] = "C"
 
         # If test name is not specified then start test with a random test
-        if not self.config['test_name']:
-            msg_outging_dict['params']['TestName'] = "Random"
+        if not self.__config['test_name']:
+            msg_outgoing_dict['params']['TestName'] = "Random"
         else:
-            msg_outging_dict['params']['TestName'] = self.config['test_name']
+            msg_outgoing_dict['params']['TestName'] = self.__config['test_name']
 
         # Check the status of the channel before we try to start the test.
-        status = self.read_status()
+        status = self.read_channel_status()
         if status:
             if pymacnet.messages.status_dictionary[status['Stat']] == 'Completed':
                 self.reset_channel()
         else:
-            log.error("Cannot read channel status!")
+            logger.error("Cannot read channel status!")
             return False
 
         # Set the safety limits.
         if not self.__set_channel_safety_limits():
-            log.error("Failed to set channel safety limits!")
+            logger.error("Failed to set channel safety limits!")
             return False
 
         # Start the test
-        response = self.__send_receive_msg(msg_outging_dict)
+        response = self._send_receive_json_msg(msg_outgoing_dict)
         if response:
             if response['result']['Result'] != 'OK':
-                log.error("Error starting test! Comment from Maccor: " +
-                          response['result']['Result'])
+                logger.error("Error starting test! Comment from Maccor: " +
+                             response['result']['Result'])
                 return False
             else:
                 return True
         else:
-            log.error("Failed to get message response when trying to start test!")
+            logger.error(
+                "Failed to get message response when trying to start test!")
             return False
 
     def set_direct_mode_output(self, current_a, voltage_v=4900) -> bool:
         """
         Sets the current/voltage output on the channel specified on in the config. Note that the
         test must have been started with the start_test_direct_control method for this to work.
 
@@ -453,18 +286,18 @@
             mode = "R"
         elif current_a > 0:
             set_current_a = current_a
             set_voltage_v = voltage_v
             mode = "C"
         elif current_a < 0:
             set_current_a = abs(current_a)
-            set_voltage_v = self.config['v_min_v']
+            set_voltage_v = self.__config['v_min_v']
             mode = "D"
         else:
-            log.error("Undefined state is set direct control output!")
+            logger.error("Undefined state is set direct control output!")
             return False
 
         # Determine range based on the magnitude of the current
         if set_current_a == 0:
             # Don't bother changing current range if we're just setting to zero.
             current_range = 4
         elif set_current_a < 0.000150:
@@ -472,86 +305,113 @@
         elif set_current_a < 0.005:
             current_range = 2
         elif set_current_a < 0.150:
             current_range = 3
         else:
             current_range = 4
 
-        msg_outging_dict = copy.deepcopy(
+        msg_outgoing_dict = copy.deepcopy(
             pymacnet.messages.tx_set_direct_output_msg)
-        msg_outging_dict['params']['Chan'] = self.channel
-        msg_outging_dict['params']['Current'] = set_current_a
-        msg_outging_dict['params']['Voltage'] = set_voltage_v
-        msg_outging_dict['params']['ChMode'] = mode
-        msg_outging_dict['params']['CurrentRange'] = current_range
+        msg_outgoing_dict['params']['Chan'] = self.__channel
+        msg_outgoing_dict['params']['Current'] = set_current_a
+        msg_outgoing_dict['params']['Voltage'] = set_voltage_v
+        msg_outgoing_dict['params']['ChMode'] = mode
+        msg_outgoing_dict['params']['CurrentRange'] = current_range
 
         # Send the rest command using the caveman method as JSON cannot set rest currently (10/4/2022)
         if mode == "R":
-            return self.__send_rest_cmd_msg(msg_outging_dict)
-
-        # Send message and make sure response indicates values were accepted.
-        response = self.__send_receive_msg(msg_outging_dict)
-        if response:
-            if response['result']['Result'] == "OK":
-                return True
+            return self._send_direct_output_rest_bin_msg(msg_outgoing_dict)
+        else:
+            # Send message and make sure response indicates values were accepted.
+            response = self._send_receive_json_msg(msg_outgoing_dict)
+            if response:
+                if response['result']['Result'] == "OK":
+                    return True
+                else:
+                    logger.error(
+                        "Error Setting output! Message : " + str(response))
+                    return False
             else:
-                log.error("Error Setting output! Message : " + str(response))
+                logger.error(
+                    "Failed to get message response when trying to set output!")
                 return False
-        else:
-            log.error("Failed to get message response when trying to set output!")
-            return False
 
-    def __send_rest_cmd_msg(self, msg_outging_dict) -> bool:
+    def __set_channel_safety_limits(self) -> bool:
         """
-        Commands rest step using caveman MacNet UDP/TCP method.
-
-        Parameters
-        ----------
-        msg_outgoing_dict : dict
-            A dictionary containing the message to be sent.
+        Sets channel safety limits on the channel specified in the config. 
 
         Returns
         -------
         success : bool
-            True of False based on whether or not rest was set
+            Returns True/False based on whether the safety limits were set correctly.
         """
+        msg_outgoing_dict = copy.deepcopy(
+            pymacnet.messages.tx_set_safety_limits_msg
+        )
+        msg_outgoing_dict['params']['Chan'] = self.__channel
+        msg_outgoing_dict['params']['VSafeMax'] = self.__config['v_max_safety_limit_v']
+        msg_outgoing_dict['params']['VSafeMin'] = self.__config['v_min_safety_limit_v']
+        msg_outgoing_dict['params']['ISafeChg'] = self.__config['i_max_safety_limit_a']
+        msg_outgoing_dict['params']['ISafeDis'] = self.__config['i_min_safety_limit_a']
 
-        msg_outgoing_bytes = struct.pack('<HHHHffffBB',
-                                         msg_outging_dict["params"]['FClass'],
-                                         msg_outging_dict["params"]['FNum'],
-                                         msg_outging_dict["params"]['Chan'],
-                                         18,
-                                         msg_outging_dict["params"]['Current'],
-                                         msg_outging_dict["params"]['Voltage'],
-                                         msg_outging_dict["params"]['Power'],
-                                         msg_outging_dict["params"]['Resistance'],
-                                         msg_outging_dict["params"]['CurrentRange'],
-                                         ord('R'))
-
-        try:
-            self.__tcp_sock.send(msg_outgoing_bytes)
-        except:
-            log.error("Error sending rest message!", exc_info=True)
-            return False
-        try:
-            response = self.__tcp_sock.recv(self.__msg_buffer_size_bytes)
-        except:
-            log.error("Error receiving rest message response!", exc_info=True)
-            return False
-        if response:
-            # TODO: Should check something related to the response.
-            pass
+        # Check to make sure all safety limits were set correctly
+        reply = self._send_receive_json_msg(msg_outgoing_dict)
+        if reply:
+            try:
+                assert ((reply['result']['Chan']) == self.__config['channel'])
+                assert (abs(reply['result']['VSafeMax'] -
+                        self.__config['v_max_safety_limit_v']) < 0.001)
+                assert (abs(reply['result']['VSafeMin'] -
+                        self.__config['v_min_safety_limit_v']) < 0.001)
+                assert (abs(reply['result']['ISafeChg'] -
+                        self.__config['i_max_safety_limit_a']) < 0.001)
+                assert (abs(reply['result']['ISafeDis'] -
+                        self.__config['i_min_safety_limit_a']) < 0.001)
+            except:
+                logger.error(
+                    "Set safety limits to not match sent safety limits! Message response: " + str(reply))
+                return False
         else:
-            log.error("No response for setting rest!")
+            logger.error(
+                "Failed to receive reply message when trying to set safety limits!")
             return False
 
         return True
 
-    def __del__(self):
+    def __verify_config(self) -> bool:
         """
-        Kills cycler connections on death.
+        Verifies that the config passed on construction is valid.
+
+        Returns
+        --------------------------
+        success : bool
+            True or False based on whether the config passed at construction is valid.
         """
-        if self.__json_sock:
-            self.__json_sock.close()
+        success = False
 
-        if self.__tcp_sock:
-            self.__tcp_sock.close()
+        required_config_keys = ['channel',
+                                'test_name',
+                                'test_procedure',
+                                'v_max_safety_limit_v',
+                                'v_min_safety_limit_v',
+                                'i_max_safety_limit_a',
+                                'i_min_safety_limit_a',
+                                'v_max_v',
+                                'v_min_v',
+                                'c_rate_ah',
+                                'data_record_time_s',
+                                'data_record_voltage_delta_vbys',
+                                'data_record_current_delta_abys',
+                                'server_ip',
+                                'json_msg_port',
+                                'bin_msg_port']
+
+        missing_keyes = False
+        for key in required_config_keys:
+            if key not in self.__config:
+                logger.error("Missing key from config! Missing : " + key)
+                missing_keyes = True
+
+        if not missing_keyes:
+            success = True
+
+        return success
```

### Comparing `pymacnet-0.0.2/pymacnet/maccorspoofer/MaccorSpoofer.py` & `pymacnet-1.0.0/pymacnet/maccorspoofer/MaccorSpoofer.py`

 * *Files 3% similar despite different names*

```diff
@@ -324,17 +324,14 @@
         Returns
         -------
         tx_msg : PyBytesObject
             The client response.
         """
 
         rx_msg = json.loads(rx_msg)
-        if rx_msg['params']['Chan'] > self.__channel_data.num_channels:
-            # TODO: Should respond with some sort of error message if request is out of range
-            pass
 
         if (pymacnet.messages.tx_read_status_msg['params']['FClass'] == rx_msg['params']['FClass'] and
                 pymacnet.messages.tx_read_status_msg['params']['FNum'] == rx_msg['params']['FNum']):
             tx_msg = copy.deepcopy(
                 self.__channel_data.fetch_channel_status(
                     rx_msg['params']['Chan'])
             )
@@ -368,18 +365,29 @@
             tx_msg['result']['Chan'] = rx_msg['params']['Chan']
             tx_msg['result']['VSafeMax'] = rx_msg['params']['VSafeMax']
             tx_msg['result']['VSafeMin'] = rx_msg['params']['VSafeMin']
             tx_msg['result']['ISafeChg'] = rx_msg['params']['ISafeChg']
             tx_msg['result']['ISafeDis'] = rx_msg['params']['ISafeDis']
             tx_msg['result']['PBatSafeChg'] = rx_msg['params']['PBatSafeChg']
             tx_msg['result']['PBatSafeDis'] = rx_msg['params']['PBatSafeDis']
+        elif (pymacnet.messages.tx_system_info_msg['params']['FClass'] == rx_msg['params']['FClass'] and
+                pymacnet.messages.tx_system_info_msg['params']['FNum'] == rx_msg['params']['FNum']):
+            tx_msg = pymacnet.messages.rx_system_info_msg
+        elif (pymacnet.messages.tx_general_info_msg['params']['FClass'] == rx_msg['params']['FClass'] and
+                pymacnet.messages.tx_general_info_msg['params']['FNum'] == rx_msg['params']['FNum']):
+            tx_msg = pymacnet.messages.rx_general_info_msg
+        elif (pymacnet.messages.tx_channel_status_multiple_channels['params']['FClass'] == rx_msg['params']['FClass'] and
+                pymacnet.messages.tx_channel_status_multiple_channels['params']['FNum'] == rx_msg['params']['FNum']):
+            tx_msg = pymacnet.messages.rx_channel_status_multiple_channels
         else:
             tx_msg = {'err': 1}
 
         tx_msg = json.dumps(tx_msg, indent=4)
+        # Needs to be included as it's included in messages from Maccor server as indicator of message termination
+        tx_msg += '\r\n'
         tx_msg = tx_msg.encode('utf-8')
 
         return tx_msg
 
 
 class _TcpWorker(_SocketWorker):
```

### Comparing `pymacnet-0.0.2/pymacnet/messages/messages.py` & `pymacnet-1.0.0/pymacnet/messages/messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,21 +71,21 @@
 Start test with direct control
 
 Selects the test channel to be started. The test name and procedure name can be up to 250 characters long.
 Also, do not select the channel in advance of starting the test. The JSON Start test command will both select and 
 start the channel. If, however, multiple channels should be started with the same test, do first select the channels,
 then start the test using 65535, meaning "all selected".
 
-Paramters as follows:
+Parameters as follows:
 
 `TestName` Up to 25 ascii characters for the data file name. “Random” will generate a pseudo-random name. 
 The field is fixed in length, so remaining characters should be space characters.
 
 `ProcName` Up to 25 ascii characters for the test procedure name. The test procedure must exist in the 
-C:\\Maccor\\Procedur folder and the “.000” should not be part of the name. The field is fixed in length, 
+C:\\Maccor\\Procedure folder and the “.000” should not be part of the name. The field is fixed in length, 
 so remaining characters should be space characters.
 
 `Comment` Up to 80 characters for the test comment. The field is fixed in length, 
 so remaining characters should be space characters.
 
 `Crate` C-rate. If C-rate is not used, enter 1.
 
@@ -195,15 +195,15 @@
         'FNum': 7,
         'Chan': -1,
         'Result': 'OK'
     },
     'id': 1987
 }
 """
-Starts test with direct control response message
+Response message for starting test with direct control.
 """
 
 tx_set_direct_output_msg = {
     "jsonrpc": "2.0",
     "method": "MacNet",
     "params":
     {
@@ -397,7 +397,125 @@
         'Result': 'OK'
     },
     'id': 1987
 }
 """
 Response message for setting channel variables.
 """
+
+tx_system_info_msg = {
+    "jsonrpc": "2.0", 
+    "method": "MacNet", 
+    "params":
+    {
+    "FClass": 1,
+    "FNum": 1 
+    },
+    "id": 1987 
+}
+"""
+Requests the software system information from the Maccor cycler, message (1,1)
+"""
+
+rx_system_info_msg = {
+    "jsonrpc":"2.0", 
+    "result":
+    {
+        "FClass":1,
+        "FNum":1,
+        "APIVersion":1, 
+        "MacTest32EXEversionMajor":3, 
+        "MacTest32EXEversionMinor":2, 
+        "MacTest32EXEversionBuild":18, 
+        "MacTest32DLLversionMajor":3, 
+        "MacTest32DLLversionMsinor":2, 
+        "MacTest32DLLversionBuild":18, 
+        "MacTest32ExeDT":"2016-11-08T15:02:58", 
+        "MacTest32DLLDT":"2016-11-13T11:29:48"
+    },
+    "id":1987
+}
+"""
+Example response for system software version, message (1,1)
+"""
+
+tx_general_info_msg = {
+    "jsonrpc": "2.0", 
+    "method": "MacNet", 
+    "params":
+    {
+        "FClass": 1,
+        "FNum": 2 
+    },
+    "id": 1987 
+}
+"""
+Requests the general system information from the Maccor cycler, message (1,2)
+"""
+
+rx_general_info_msg = {
+    "jsonrpc":"2.0", 
+    "result":
+    {
+        "FClass":1, 
+        "FNum":2, 
+        "SystemID":"Win10", 
+        "SystemType":0, 
+        "ControllerBoards":3, 
+        "TestChannels":12, 
+        "AuxBoards":1, 
+        "AuxChannels":128, 
+        "SMB1Pos":0,
+        "SMB3Pos":1 
+    },
+    "id":1987
+}
+"""
+Example response for general system information from the Maccor cycler, message (1,2)
+"""
+
+tx_channel_status_multiple_channels = {
+    "jsonrpc": "2.0", 
+    "method": "MacNet", 
+    "params":
+    {
+        "FClass": 4, 
+        "FNum": 1, 
+        "Chan": 0, 
+        "Len": 2
+    },
+    "id": 1987
+}
+"""
+Requests the status of “Len” channels starting from “Chan” will be returned. 
+Four bytes per requested channel. Up to 128 channels can be requested in one message.
+
+MacNet message: (4, 1) Channel status of multiple channels
+"""
+
+rx_channel_status_multiple_channels = {
+    "jsonrpc":"2.0",
+    "result":
+    {
+        "FClass":4, 
+        "FNum":1, 
+        "Chan":0, 
+        "Len":2, 
+        "Status":
+        [
+            {
+                "RF1":0, 
+                "RF2":0, 
+                "Stat":0
+            }, 
+            {
+                "RF1":0,
+                "RF2":0, 
+                "Stat":0
+            } 
+        ]
+    }, 
+    "id":1987
+}
+"""
+Example response for MacNet message: (4, 1) Channel status of multiple channels)
+"""
```

