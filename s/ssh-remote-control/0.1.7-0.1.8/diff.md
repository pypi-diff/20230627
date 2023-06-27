# Comparing `tmp/ssh_remote_control-0.1.7.tar.gz` & `tmp/ssh_remote_control-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_remote_control-0.1.7.tar", last modified: Mon Jun 26 09:20:05 2023, max compression
+gzip compressed data, was "ssh_remote_control-0.1.8.tar", last modified: Tue Jun 27 09:53:23 2023, max compression
```

## Comparing `ssh_remote_control-0.1.7.tar` & `ssh_remote_control-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.127841 ssh_remote_control-0.1.7/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1569 2023-06-26 09:20:05.122837 ssh_remote_control-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.7/README.md
--rw-rw-rw-   0        0        0      846 2023-06-26 09:15:45.000000 ssh_remote_control-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 09:20:05.127841 ssh_remote_control-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.020843 ssh_remote_control-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.067837 ssh_remote_control-0.1.7/src/ssh_remote_control/
--rw-rw-rw-   0        0        0    10701 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/__init__.py
--rw-rw-rw-   0        0        0     6641 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/command.py
--rw-rw-rw-   0        0        0     3503 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/command_set.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.120834 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/
--rw-rw-rw-   0        0        0      161 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/const.py
--rw-rw-rw-   0        0        0     3969 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/linux.py
--rw-rw-rw-   0        0        0     3813 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/windows_cmd.py
--rw-rw-rw-   0        0        0     4078 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/windows_ps.py
--rw-rw-rw-   0        0        0      645 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/event.py
--rw-rw-rw-   0        0        0      222 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/helpers.py
--rw-rw-rw-   0        0        0     1313 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/locker.py
--rw-rw-rw-   0        0        0     3995 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/manager.py
--rw-rw-rw-   0        0        0     8323 2023-06-26 09:17:08.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/sensor.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.109834 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/
--rw-rw-rw-   0        0        0     1569 2023-06-26 09:20:04.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-06-26 09:20:05.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:20:04.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-26 09:20:04.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-26 09:20:04.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 09:53:23.957049 ssh_remote_control-0.1.8/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1569 2023-06-27 09:53:23.955046 ssh_remote_control-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.8/README.md
+-rw-rw-rw-   0        0        0      846 2023-06-27 09:51:07.000000 ssh_remote_control-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:53:23.957049 ssh_remote_control-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 09:53:23.852045 ssh_remote_control-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 09:53:23.895045 ssh_remote_control-0.1.8/src/ssh_remote_control/
+-rw-rw-rw-   0        0        0    10418 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/__init__.py
+-rw-rw-rw-   0        0        0     3503 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/collection.py
+-rw-rw-rw-   0        0        0     6533 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/command.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:53:23.952050 ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/
+-rw-rw-rw-   0        0        0      161 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/const.py
+-rw-rw-rw-   0        0        0     3968 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/linux.py
+-rw-rw-rw-   0        0        0     3812 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/windows_cmd.py
+-rw-rw-rw-   0        0        0     4077 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/windows_ps.py
+-rw-rw-rw-   0        0        0      637 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/errors.py
+-rw-rw-rw-   0        0        0      645 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/event.py
+-rw-rw-rw-   0        0        0      222 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/helpers.py
+-rw-rw-rw-   0        0        0     1313 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/locker.py
+-rw-rw-rw-   0        0        0     4340 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/manager.py
+-rw-rw-rw-   0        0        0     9624 2023-06-27 09:48:00.000000 ssh_remote_control-0.1.8/src/ssh_remote_control/sensor.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:53:23.940073 ssh_remote_control-0.1.8/src/ssh_remote_control.egg-info/
+-rw-rw-rw-   0        0        0     1569 2023-06-27 09:53:23.000000 ssh_remote_control-0.1.8/src/ssh_remote_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2023-06-27 09:53:23.000000 ssh_remote_control-0.1.8/src/ssh_remote_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:53:23.000000 ssh_remote_control-0.1.8/src/ssh_remote_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-27 09:53:23.000000 ssh_remote_control-0.1.8/src/ssh_remote_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 09:53:23.000000 ssh_remote_control-0.1.8/src/ssh_remote_control.egg-info/top_level.txt
```

### Comparing `ssh_remote_control-0.1.7/LICENSE` & `ssh_remote_control-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.7/PKG-INFO` & `ssh_remote_control-0.1.8/src/ssh_remote_control.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh_remote_control
-Version: 0.1.7
+Name: ssh-remote-control
+Version: 0.1.8
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.7/README.md` & `ssh_remote_control-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.7/pyproject.toml` & `ssh_remote_control-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_remote_control"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor remote devices through SSH"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/__init__.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 from time import time
 
 import async_timeout
 import icmplib
 import paramiko
 import wakeonlan
 
-from .command import (
-    ActionCommand,
-    Command,
+from .collection import Collection
+from .command import ActionCommand, Command, CommandOutput, SensorCommand
+from .default_collections import ActionKey, SensorKey
+from .errors import (
+    CommandExecuteError,
     CommandFormatError,
-    CommandOutput,
-    SensorCommand,
+    MACAdressUnavailableError,
+    OfflineError,
+    SSHAuthError,
+    SSHConnectError,
+    SSHHostKeyUnknownError,
 )
-from .command_set import CommandSet
-from .default_command_sets import ActionKey, SensorKey
 from .event import Event
 from .helpers import name_to_key
-from .manager import DEFAULT_COMMAND_TIMEOUT, CommandExecuteError, Manager
+from .manager import DEFAULT_COMMAND_TIMEOUT, Manager
 from .sensor import DynamicSensor, Sensor
 
 _LOGGER = logging.getLogger(__name__)
+_TEST_COMMAND = Command("")
 
 DEFAULT_SSH_PORT = 22
 DEFAULT_PING_TIMEOUT = 4
 DEFAULT_SSH_TIMEOUT = 4
 DEFAULT_ADD_HOST_KEYS = False
 DEFAULT_ALLOW_TURN_OFF = False
 
@@ -79,22 +83,22 @@
         ssh_user: str | None = None,
         ssh_password: str | None = None,
         ssh_key_file: str | None = None,
         ssh_host_keys_file: str | None = None,
         ssh_timeout: int = DEFAULT_SSH_TIMEOUT,
         ping_timeout: int = DEFAULT_PING_TIMEOUT,
         command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
-        command_set: CommandSet | None = None,
+        collection: Collection | None = None,
         allow_turn_off: bool = DEFAULT_ALLOW_TURN_OFF,
         logger: logging.Logger = _LOGGER,
     ) -> None:
         super().__init__(
             name=name or host,
             command_timeout=command_timeout,
-            command_set=command_set,
+            collection=collection,
             logger=logger,
         )
         self.host = host
         self._mac_address = mac_address
         self.ssh_port = ssh_port
         self.ssh_user = ssh_user
         self.ssh_password = ssh_password
@@ -252,26 +256,26 @@
 
         Set `state.is_connected` to `False` and the
         sensor values of all sensor commands to `None`.
         """
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, self._disconnect)
 
-    async def async_update_state(self, *, validate: bool = False) -> None:
+    async def async_update_state(self, *, raise_errors: bool = False) -> None:
         """Update state.
 
         Raises:
-            OfflineError (validate)
+            OfflineError (`raise_errors`)
             SSHHostKeyUnknownError
             SSHAuthError
-            SSHConnectError (validate)
+            SSHConnectError (`raise_errors`)
         """
         if self.state.is_connected:
             try:
-                await self.async_execute_command(Command(""))
+                await self.async_execute_command(_TEST_COMMAND)
                 return
             except CommandExecuteError:
                 pass
 
         try:
             host = await icmplib.async_ping(
                 self.host,
@@ -282,62 +286,42 @@
         except Exception as exc:  # pylint: disable=broad-except
             self.logger.info("%s: Ping request failed: %s", self.name, exc)
             self.state.update(IS_ONLINE, False)
         else:
             self.state.update(IS_ONLINE, host.is_alive)
 
         if not self.state.is_online:
-            if validate:
+            if raise_errors:
                 raise OfflineError("Host is offline")
             return
 
         try:
             await self.async_connect()
         except SSHConnectError:
-            if validate:
+            if raise_errors:
                 raise
 
-    async def turn_on(self) -> None:
+    async def async_turn_on(self) -> None:
         """Turn the host on.
 
         Raises:
             MACAddressUnavailableError
         """
         if self.state.is_online:
             return
 
         if self.mac_address is None:
             raise MACAdressUnavailableError("MAC address is unavailable")
 
         wakeonlan.send_magic_packet(self.mac_address)
 
-    async def turn_off(self) -> None:
+    async def async_turn_off(self) -> None:
         """Turn the host on.
 
         Raises:
             CommandFormatError
             CommandExecuteError
         """
         if self.allow_turn_off is False:
             return
 
         await self.async_run_action(ActionKey.TURN_OFF)
-
-
-class OfflineError(Exception):
-    """Error to indicate host is offline."""
-
-
-class SSHAuthError(Exception):
-    """Error to indicate SSH authentication failed."""
-
-
-class SSHConnectError(Exception):
-    """Error to indicate SSH connection failed."""
-
-
-class SSHHostKeyUnknownError(Exception):
-    """Error to indicate SSH host key is unknown."""
-
-
-class MACAdressUnavailableError(Exception):
-    """Error to indicate MAC address is unavailable."""
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/command.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 from collections.abc import Callable
 from dataclasses import dataclass
 from string import Formatter
 from time import time
 from typing import TYPE_CHECKING
 
+from .errors import CommandExecuteError, CommandFormatError
 from .helpers import name_to_key
 from .sensor import DynamicSensor, Sensor
 
 if TYPE_CHECKING:
     from .manager import Manager
 
-PLACEHOLDER_KEY = "_"
+SENSOR_PLACEHOLDER_KEY = "_"
 
 
 @dataclass(frozen=True)
 class CommandOutput:
     """The CommandOutput class."""
 
     timestamp: float
@@ -158,20 +159,21 @@
         self.interval = interval
 
     @property
     def sensors_by_key(self) -> dict[str, Sensor]:
         """Sensors by key."""
         result = {}
         for sensor in self.sensors:
-            if sensor.key != PLACEHOLDER_KEY:
-                result.update(
-                    {sensor.key: sensor, **sensor.children_by_key}
-                    if isinstance(sensor, DynamicSensor)
-                    else {sensor.key: sensor}
-                )
+            if sensor.key == SENSOR_PLACEHOLDER_KEY:
+                continue
+            result.update(
+                {sensor.key: sensor, **sensor.child_sensors_by_key}
+                if isinstance(sensor, DynamicSensor)
+                else {sensor.key: sensor}
+            )
         return result
 
     @property
     def dynamic_sensor(self) -> DynamicSensor | None:
         return next(
             (sensor for sensor in self.sensors if isinstance(sensor, DynamicSensor)),
             None,
@@ -183,49 +185,41 @@
         return self.last_update is None or (
             self.interval and time() - self.last_update >= self.interval
         )
 
     def remove_sensor(self, key: str) -> None:
         """Remove a sensor."""
         self.sensors = [
-            Sensor(key=PLACEHOLDER_KEY) if sensor.key == key else sensor
+            Sensor(key=SENSOR_PLACEHOLDER_KEY) if sensor.key == key else sensor
             for sensor in self.sensors
         ]
 
     def update_sensors(self, output: CommandOutput | None) -> None:
         """Update sensors."""
         if output and output.code == 0:
             self.last_update = output.timestamp
             data = output.stdout
         else:
             data = None
 
         if dynamic_sensor := self.dynamic_sensor:
             dynamic_sensor.update(data)
+            return
 
-        else:
-            if data is None:
-                data = []
+        if data is None:
+            data = []
 
-            for i, sensor in enumerate(self.sensors):
-                sensor.update(data[i] if len(data) > i else None)
+        for i, sensor in enumerate(self.sensors):
+            sensor.update(data[i] if len(data) > i else None)
 
     async def async_execute(
         self, manager: Manager, context: dict | None = None
     ) -> CommandOutput:
         try:
             output = await super().async_execute(manager, context)
         except (CommandFormatError, CommandExecuteError):
             self.update_sensors(None)
             raise
 
         self.update_sensors(output)
 
         return output
-
-
-class CommandFormatError(Exception):
-    """Error to indicate command formatting failed."""
-
-
-class CommandExecuteError(Exception):
-    """Error to indicate command execution failed."""
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/command_set.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from copy import deepcopy
 
 from .command import ActionCommand, SensorCommand
 from .sensor import Sensor
 
 
-class CommandSet:
-    """The CommandSet class."""
+class Collection:
+    """The Collection class."""
 
     action_commands: list[ActionCommand]
     sensor_commands: list[SensorCommand]
 
     def __init__(
         self,
         name: str,
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/const.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/linux.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from ..collection import Collection
 from ..command import ActionCommand, SensorCommand
-from ..command_set import CommandSet
 from ..sensor import DynamicSensor, Sensor
 from .const import ActionKey, ActionName, SensorKey, SensorName
 
-linux = CommandSet(
+linux = Collection(
     "Linux",
     [
         ActionCommand(
             "/sbin/shutdown -h now",
             ActionName.TURN_OFF,
             ActionKey.TURN_OFF,
         ),
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/windows_cmd.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/windows_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from ..collection import Collection
 from ..command import ActionCommand, SensorCommand
-from ..command_set import CommandSet
 from ..sensor import Sensor
 from .const import ActionKey, ActionName, SensorKey, SensorName
 
-windows_cmd = CommandSet(
+windows_cmd = Collection(
     "Windows",
     [
         ActionCommand(
             "shutdown -t 0",
             ActionName.TURN_OFF,
             ActionKey.TURN_OFF,
         ),
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/windows_ps.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/default_collections/windows_ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from ..collection import Collection
 from ..command import ActionCommand, SensorCommand
-from ..command_set import CommandSet
 from ..sensor import DynamicSensor, Sensor
 from .const import ActionKey, ActionName, SensorKey, SensorName
 
-windows_ps = CommandSet(
+windows_ps = Collection(
     "Windows (Power Shell)",
     [
         ActionCommand(
             "Stop-Computer -Force",
             ActionName.TURN_OFF,
             ActionKey.TURN_OFF,
         ),
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/event.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/event.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/locker.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/locker.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control/sensor.py` & `ssh_remote_control-0.1.8/src/ssh_remote_control/sensor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
-import logging
 from collections.abc import Callable
+import logging
+import re
 from typing import TYPE_CHECKING, Any
 
 from .event import Event
 from .helpers import name_to_key
 
 if TYPE_CHECKING:
     from .command import Command
@@ -13,18 +14,17 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 TRUE_STRINGS = ["true", "enabled", "on", "active", "1"]
 FALSE_STRINGS = ["false", "disabled", "off", "inactive", "0"]
 
 
-def string_to_bool(
+def _string_to_bool(
     payload_on: str | None, payload_off: str | None, string: str
 ) -> bool | None:
-    """String to bool."""
     if payload_on:
         if string == payload_on:
             return True
         if not payload_off:
             return False
 
     if payload_off:
@@ -37,15 +37,15 @@
         return True
 
     if string.lower() in FALSE_STRINGS:
         return False
 
 
 class DynamicData:
-    """The DynamicData class"""
+    """The DynamicData class."""
 
     def __init__(
         self,
         parent_name: str | None,
         parent_key: str,
         data_id: str,
         data_value_string: str,
@@ -70,14 +70,15 @@
         key: str | None = None,
         child_id: str | None = None,
         *,
         value_type: type | None = None,
         value_unit: str | None = None,
         value_min: int | float | None = None,
         value_max: int | float | None = None,
+        value_pattern: str | None = None,
         value_renderer: Callable[[str], str] | None = None,
         command_set: Command | None = None,
         command_on: Command | None = None,
         command_off: Command | None = None,
         payload_on: str | None = None,
         payload_off: str | None = None,
         options: dict | None = None,
@@ -85,77 +86,102 @@
         self.name = name
         self.key = key or name_to_key(name)
         self.child_id = child_id
         self.value_type = value_type or str
         self.value_unit = value_unit
         self.value_min = value_min
         self.value_max = value_max
+        self.value_pattern = value_pattern
         self.value_renderer = value_renderer
         self.command_set = command_set
         self.command_on = command_on
         self.command_off = command_off
         self.payload_on = payload_on
         self.payload_off = payload_off
         self.options = options or {}
         self.on_update = Event()
 
     @property
     def is_controllable(self) -> bool:
+        """Return `True` if `async_set` is available."""
         if self.value_type == bool and self.command_on and self.command_off:
             return True
+
         return self.command_set is not None
 
-    def _render(self, value_string: str | None) -> Any | None:
-        if value_string is None:
-            return None
+    def _render(self, value_string: str) -> Any:
         if self.value_renderer:
             value_string = self.value_renderer(value_string)
+
         if self.value_type is bool:
-            return string_to_bool(self.payload_on, self.payload_off, value_string)
+            return _string_to_bool(self.payload_on, self.payload_off, value_string)
+
         if self.value_type is int:
             return int(float(value_string))
+
         return self.value_type(value_string)
 
     def _validate(self, value: Any) -> bool:
         if not isinstance(value, self.value_type):
-            return False
-        if self.value_type == str and (
-            (self.value_min and len(value) < self.value_min)
-            or (self.value_max and len(value) > self.value_max)
-        ):
-            return False
-        if self.value_type in [int, float] and (
-            (self.value_min and value < self.value_min)
-            or (self.value_max and value > self.value_max)
-        ):
-            return False
-        return True
+            raise TypeError(f"Value is {type(value)} and not {self.value_type}")
+
+        if self.value_type == str:
+            if self.value_min and len(value) < self.value_min:
+                raise ValueError(f"Value is shorter then {self.value_min} characters")
+            if self.value_max and len(value) > self.value_max:
+                raise ValueError(f"Value is longer then {self.value_min} characters")
+            if self.value_pattern and not re.fullmatch(self.value_pattern, value):
+                raise ValueError(f"Value doesn't match {self.value_pattern}")
+
+        if self.value_type in [int, float]:
+            if self.value_min and value < self.value_min:
+                raise ValueError(f"Value is smaller then {self.value_min}")
+            if self.value_max and value > self.value_max:
+                raise ValueError(f"Value is bigger then {self.value_min}")
 
     def _update_value(self, data: str | None) -> None:
+        if data is None:
+            self.value = None
+            return
+
         try:
             value = self._render(data)
         except Exception as exc:  # pylint: disable=broad-except
             _LOGGER.warning("%s: Render error: %s (%s)", self.key, exc, data)
-            value = None
+            self.value = None
+            return
 
-        if self._validate(value):
-            self.value = self.last_known_value = value
-        else:
+        try:
+            self._validate(value)
+        except (TypeError, ValueError) as exc:
+            _LOGGER.warning("%s: Validate error: %s (%s)", self.key, exc, value)
             self.value = None
+            return
+
+        self.value = self.last_known_value = value
 
-    def update(self, data: str | None) -> None:
-        """Update."""
+    def update(self, data: Any | None) -> None:
+        """Update value and notify `on_update` subscribers."""
         self._update_value(data)
         self.on_update.notify(self)
 
     async def async_set(self, manager: Manager, value: Any) -> None:
-        """Set."""
-        if value == self.value or not self._validate(value):
+        """Set.
+
+        Raises:
+            TypeError
+            ValueError
+            CommandFormatError
+            CommandExecuteError
+        """
+        if not self.is_controllable or value == self.value:
             return
 
+        self._validate(value)
+
         if self.value_type == bool and self.command_on and self.command_off:
             command = self.command_on if value else self.command_off
         else:
             command = self.command_set
 
         await manager.async_execute_command(
             command, context={"id": self.child_id, "value": value}
@@ -173,14 +199,15 @@
         key: str | None = None,
         *,
         separator: str | None = None,
         value_type: type | None = None,
         value_unit: str | None = None,
         value_min: int | float | None = None,
         value_max: int | float | None = None,
+        value_pattern: str | None = None,
         value_renderer: Callable[[str], str] | None = None,
         command_set: Command | None = None,
         command_on: str | None = None,
         command_off: str | None = None,
         payload_on: str | None = None,
         payload_off: str | None = None,
         options: dict | None = None,
@@ -188,61 +215,35 @@
         super().__init__(
             name,
             key,
             value_type=value_type,
             value_unit=value_unit,
             value_min=value_min,
             value_max=value_max,
+            value_pattern=value_pattern,
             value_renderer=value_renderer,
             command_set=command_set,
             command_on=command_on,
             command_off=command_off,
             payload_on=payload_on,
             payload_off=payload_off,
             options=options,
         )
         self.separator = separator
         self.value = []
         self.on_child_added = Event()
         self.on_child_removed = Event()
 
     @property
-    def children_by_key(self) -> dict[str, Sensor]:
+    def child_sensors_by_key(self) -> dict[str, Sensor]:
+        """Child sensors by key."""
         return {child.key: child for child in self.value}
 
-    def _update_value(self, data: list[str] | None) -> None:
-        if data is None:
-            for child in self.value:
-                child.update(None)
-            return
-
-        dynamic_data_list = [
-            DynamicData(self.name, self.key, *data_items)
-            for data_items in [line.split(self.separator, 2) for line in data]
-            if len(data_items) >= 2
-        ]
-
-        dynamic_data_by_key = {
-            dynamic_data.key: dynamic_data for dynamic_data in dynamic_data_list
-        }
-
-        for key, dynamic_data in dynamic_data_by_key.items():
-            if key not in self.children_by_key:
-                self.add_child(dynamic_data)
-
-        for child in self.value:
-            if child.key in dynamic_data_by_key:
-                dynamic_data = dynamic_data_by_key[child.key]
-                child.update(dynamic_data.value_string)
-            else:
-                self.remove_child(child)
-
-    def add_child(self, dynamic_data: DynamicData) -> None:
-        """Add a child."""
-        child = Sensor(
+    def _create_child(self, dynamic_data: DynamicData) -> Sensor:
+        return Sensor(
             dynamic_data.name,
             dynamic_data.key,
             dynamic_data.id,
             value_type=self.value_type,
             value_unit=self.value_unit,
             value_min=self.value_min,
             value_max=self.value_max,
@@ -250,16 +251,49 @@
             command_set=self.command_set,
             command_on=self.command_on,
             command_off=self.command_off,
             payload_on=self.payload_on,
             payload_off=self.payload_off,
             options=self.options,
         )
+
+    def _add_child(self, child: Sensor) -> None:
         self.value.append(child)
         self.on_child_added.notify(self, child)
 
-    def remove_child(self, child: Sensor) -> None:
-        """Remove a child."""
+    def _remove_child(self, child: Sensor) -> None:
         if child.value is not None:
             child.update(None)
         self.value.remove(child)
         self.on_child_removed.notify(self, child)
+
+    def _update_value(self, data: list[str] | None) -> None:
+        if data is None:
+            for child in self.value:
+                child.update(None)
+            return
+
+        dynamic_data_list = [
+            DynamicData(self.name, self.key, *(field.strip() for field in row))
+            for row in (line.split(self.separator, 2) for line in data)
+            if len(row) >= 2
+        ]
+
+        dynamic_data_by_key = {
+            dynamic_data.key: dynamic_data for dynamic_data in dynamic_data_list
+        }
+
+        for key, dynamic_data in dynamic_data_by_key.items():
+            if key not in self.child_sensors_by_key:
+                new_child = self._create_child(dynamic_data)
+                self._add_child(new_child)
+
+        for child in self.value:
+            if child.key in dynamic_data_by_key:
+                dynamic_data = dynamic_data_by_key[child.key]
+                child.update(dynamic_data.value_string)
+            else:
+                self._remove_child(child)
+
+    async def async_set(self, manager: Manager, value: Any) -> None:
+        for child in self.value:
+            await child.async_set(manager, value)
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/PKG-INFO` & `ssh_remote_control-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh-remote-control
-Version: 0.1.7
+Name: ssh_remote_control
+Version: 0.1.8
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/SOURCES.txt` & `ssh_remote_control-0.1.8/src/ssh_remote_control.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 src/ssh_remote_control/__init__.py
+src/ssh_remote_control/collection.py
 src/ssh_remote_control/command.py
-src/ssh_remote_control/command_set.py
+src/ssh_remote_control/errors.py
 src/ssh_remote_control/event.py
 src/ssh_remote_control/helpers.py
 src/ssh_remote_control/locker.py
 src/ssh_remote_control/manager.py
 src/ssh_remote_control/sensor.py
 src/ssh_remote_control.egg-info/PKG-INFO
 src/ssh_remote_control.egg-info/SOURCES.txt
 src/ssh_remote_control.egg-info/dependency_links.txt
 src/ssh_remote_control.egg-info/requires.txt
 src/ssh_remote_control.egg-info/top_level.txt
-src/ssh_remote_control/default_command_sets/__init__.py
-src/ssh_remote_control/default_command_sets/const.py
-src/ssh_remote_control/default_command_sets/linux.py
-src/ssh_remote_control/default_command_sets/windows_cmd.py
-src/ssh_remote_control/default_command_sets/windows_ps.py
+src/ssh_remote_control/default_collections/__init__.py
+src/ssh_remote_control/default_collections/const.py
+src/ssh_remote_control/default_collections/linux.py
+src/ssh_remote_control/default_collections/windows_cmd.py
+src/ssh_remote_control/default_collections/windows_ps.py
```

