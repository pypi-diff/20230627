# Comparing `tmp/vivintpy-2023.3.3.tar.gz` & `tmp/vivintpy-2023.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivintpy-2023.3.3.tar", max compression
+gzip compressed data, was "vivintpy-2023.3.4.tar", max compression
```

## Comparing `vivintpy-2023.3.3.tar` & `vivintpy-2023.3.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1071 2021-08-09 16:33:03.000000 vivintpy-2023.3.3/LICENSE
--rw-r--r--   0        0        0     2658 2022-08-03 21:25:24.452558 vivintpy-2023.3.3/README.md
--rw-r--r--   0        0        0      955 2023-03-10 17:49:57.845686 vivintpy-2023.3.3/pyproject.toml
--rw-r--r--   0        0        0       63 2023-03-10 17:49:57.846064 vivintpy-2023.3.3/vivintpy/__init__.py
--rw-r--r--   0        0        0     7346 2022-12-09 18:06:57.665156 vivintpy-2023.3.3/vivintpy/account.py
--rw-r--r--   0        0        0     4333 2023-03-10 00:12:51.914896 vivintpy-2023.3.3/vivintpy/const.py
--rw-r--r--   0        0        0     7591 2022-08-03 21:25:24.458680 vivintpy-2023.3.3/vivintpy/devices/__init__.py
--rw-r--r--   0        0        0    11402 2023-03-10 00:12:51.915404 vivintpy-2023.3.3/vivintpy/devices/alarm_panel.py
--rw-r--r--   0        0        0     8597 2023-03-10 17:49:57.846277 vivintpy-2023.3.3/vivintpy/devices/camera.py
--rw-r--r--   0        0        0     1288 2023-03-10 00:12:51.916273 vivintpy-2023.3.3/vivintpy/devices/door_lock.py
--rw-r--r--   0        0        0     2077 2023-03-10 00:12:51.916437 vivintpy-2023.3.3/vivintpy/devices/garage_door.py
--rw-r--r--   0        0        0     1807 2023-03-10 00:12:51.916595 vivintpy-2023.3.3/vivintpy/devices/switch.py
--rw-r--r--   0        0        0     3334 2022-08-03 15:10:36.558284 vivintpy-2023.3.3/vivintpy/devices/thermostat.py
--rw-r--r--   0        0        0     3283 2022-12-09 18:06:57.666491 vivintpy-2023.3.3/vivintpy/devices/wireless_sensor.py
--rw-r--r--   0        0        0     1657 2022-08-03 15:30:59.833155 vivintpy-2023.3.3/vivintpy/entity.py
--rw-r--r--   0        0        0    11357 2022-12-12 19:49:44.780082 vivintpy-2023.3.3/vivintpy/enums.py
--rw-r--r--   0        0        0      705 2021-09-14 16:20:05.000000 vivintpy-2023.3.3/vivintpy/exceptions.py
--rw-r--r--   0        0        0    81878 2023-03-10 00:12:51.917163 vivintpy-2023.3.3/vivintpy/proto/beam_pb2.py
--rw-r--r--   0        0        0   102437 2023-03-10 00:12:51.917905 vivintpy-2023.3.3/vivintpy/proto/beam_pb2.pyi
--rw-r--r--   0        0        0   168580 2023-03-10 00:12:51.918506 vivintpy-2023.3.3/vivintpy/proto/beam_pb2_grpc.py
--rw-r--r--   0        0        0     4657 2023-03-10 17:49:38.569881 vivintpy-2023.3.3/vivintpy/pubnub.py
--rw-r--r--   0        0        0        0 2022-08-03 05:45:21.339885 vivintpy-2023.3.3/vivintpy/py.typed
--rw-r--r--   0        0        0     3273 2022-08-03 15:30:44.857990 vivintpy-2023.3.3/vivintpy/system.py
--rw-r--r--   0        0        0     1288 2022-08-03 15:30:15.276292 vivintpy-2023.3.3/vivintpy/utils.py
--rw-r--r--   0        0        0    18614 2023-03-10 17:49:57.846481 vivintpy-2023.3.3/vivintpy/vivintskyapi.py
--rw-r--r--   0        0        0   411296 2023-03-10 00:12:51.920481 vivintpy-2023.3.3/vivintpy/zjs_device_config_db.json
--rw-r--r--   0        0        0     1036 2022-11-22 00:31:34.499538 vivintpy-2023.3.3/vivintpy/zjs_device_config_db.py
--rw-r--r--   0        0        0     3571 1970-01-01 00:00:00.000000 vivintpy-2023.3.3/setup.py
--rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 vivintpy-2023.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-26 22:21:54.390737 vivintpy-2023.3.4/LICENSE
+-rw-r--r--   0        0        0     2658 2023-06-26 22:21:54.390737 vivintpy-2023.3.4/README.md
+-rw-r--r--   0        0        0     1108 2023-06-26 22:22:17.543220 vivintpy-2023.3.4/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-06-26 22:22:17.543220 vivintpy-2023.3.4/vivintpy/__init__.py
+-rw-r--r--   0        0        0     7673 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/account.py
+-rw-r--r--   0        0        0     4371 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/const.py
+-rw-r--r--   0        0        0     8165 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/__init__.py
+-rw-r--r--   0        0        0    12054 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/alarm_panel.py
+-rw-r--r--   0        0        0     9255 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/camera.py
+-rw-r--r--   0        0        0     1279 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/door_lock.py
+-rw-r--r--   0        0        0     2068 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/garage_door.py
+-rw-r--r--   0        0        0     1798 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/switch.py
+-rw-r--r--   0        0        0     3325 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/thermostat.py
+-rw-r--r--   0        0        0     3274 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/devices/wireless_sensor.py
+-rw-r--r--   0        0        0     1657 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/entity.py
+-rw-r--r--   0        0        0    11826 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/enums.py
+-rw-r--r--   0        0        0      705 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/exceptions.py
+-rw-r--r--   0        0        0    81878 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/proto/beam_pb2.py
+-rw-r--r--   0        0        0   102437 2023-06-26 22:21:54.394737 vivintpy-2023.3.4/vivintpy/proto/beam_pb2.pyi
+-rw-r--r--   0        0        0   168580 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/proto/beam_pb2_grpc.py
+-rw-r--r--   0        0        0     4657 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/pubnub.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/py.typed
+-rw-r--r--   0        0        0     3664 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/system.py
+-rw-r--r--   0        0        0     1288 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/utils.py
+-rw-r--r--   0        0        0    19437 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/vivintskyapi.py
+-rw-r--r--   0        0        0   411296 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/zjs_device_config_db.json
+-rw-r--r--   0        0        0     1036 2023-06-26 22:21:54.398738 vivintpy-2023.3.4/vivintpy/zjs_device_config_db.py
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 vivintpy-2023.3.4/PKG-INFO
```

### Comparing `vivintpy-2023.3.3/LICENSE` & `vivintpy-2023.3.4/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Nathan Spencer
+Copyright (c) 2021-2023 Nathan Spencer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `vivintpy-2023.3.3/README.md` & `vivintpy-2023.3.4/README.md`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/account.py` & `vivintpy-2023.3.4/vivintpy/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     PubNubMessageAttribute,
     SystemAttribute,
     UserAttribute,
 )
 from .exceptions import VivintSkyApiError
 from .pubnub import PN_CHANNEL, PN_SUBSCRIBE_KEY, VivintPubNubSubscribeListener
 from .system import System
-from .utils import first_or_none
+from .utils import first_or_none, send_deprecation_warning
 from .vivintskyapi import VivintSkyApi
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Account:
     """Class for interacting with VivintSky API using asyncio."""
@@ -36,37 +36,48 @@
         client_session: aiohttp.ClientSession | None = None,
     ):
         """Initialize an account."""
         self.__connected = False
         self.__load_devices = False
         self.__pubnub: PubNubAsyncio | None = None
         self.__pubnub_listener: VivintPubNubSubscribeListener | None = None
-        self.vivintskyapi = VivintSkyApi(
+        self._api = VivintSkyApi(
             username=username,
             password=password,
             persist_session=persist_session,
             client_session=client_session,
         )
         self.systems: list[System] = []
 
     @property
+    def api(self) -> VivintSkyApi:
+        """Return the API."""
+        return self._api
+
+    @property
+    def vivintskyapi(self) -> VivintSkyApi:
+        """Return the API."""
+        send_deprecation_warning("vivintskyapi", "api")
+        return self.api
+
+    @property
     def connected(self) -> bool:
         """Return True if connected."""
         return self.__connected
 
     async def connect(
         self, load_devices: bool = False, subscribe_for_realtime_updates: bool = False
     ) -> None:
         """Connect to the VivintSky API."""
         _LOGGER.debug("Connecting to VivintSky")
 
         self.__load_devices = load_devices
 
         # initialize the vivintsky cloud session
-        authuser_data = await self.vivintskyapi.connect()
+        authuser_data = await self.api.connect()
         self.__connected = True
 
         # subscribe to pubnub for realtime updates
         if subscribe_for_realtime_updates:
             _LOGGER.debug("Subscribing to PubNub for realtime updates")
             await self.subscribe_for_realtime_updates(authuser_data)
 
@@ -79,15 +90,15 @@
         """Disconnect from the API."""
         _LOGGER.debug("Disconnecting from VivintSky")
         if self.connected:
             if self.__pubnub:
                 self.__pubnub.remove_listener(self.__pubnub_listener)
                 await self.__pubnub_unsubscribe_all()
                 await self.__pubnub.stop()
-        await self.vivintskyapi.disconnect()
+        await self.api.disconnect()
         self.__connected = False
 
     async def __pubnub_unsubscribe_all(self) -> None:
         """
         Unsubscribe from all channels and wait for the response.
 
         The pubnub code doesn't properly wait for the unsubscribe event to finish or to
@@ -101,27 +112,27 @@
             if getattr(getattr(task.get_coro(), "cr_code", None), "co_name", None)
             == "_send_leave_helper"
         ]
         await asyncio.gather(*tasks)
 
     async def verify_mfa(self, code: str) -> None:
         """Verify multi-factor authentication with the VivintSky API."""
-        await self.vivintskyapi.verify_mfa(code)
+        await self.api.verify_mfa(code)
 
         # load all systems, panels and devices
         if self.__load_devices:
             _LOGGER.debug("Loading devices")
             await self.refresh()
 
     async def refresh(self, authuser_data: dict | None = None) -> None:
         """Refresh the account."""
         # make a call to vivint's authuser endpoint to get a list of all the system_accounts (locations) & panels if not supplied
         if not authuser_data:
             try:
-                authuser_data = await self.vivintskyapi.get_authuser_data()
+                authuser_data = await self.api.get_authuser_data()
             except (ClientConnectionError, VivintSkyApiError):
                 _LOGGER.error("Unable to refresh system(s)")
 
         if authuser_data:
             # for each system_account, make another call to load all the devices
             for system_data in authuser_data[AuthUserAttribute.USERS][
                 UserAttribute.SYSTEM
@@ -131,37 +142,38 @@
                     self.systems,
                     lambda system, system_data=system_data: system.id  # type: ignore
                     == system_data[SystemAttribute.PANEL_ID],
                 )
                 if system:
                     await system.refresh()
                 else:
-                    full_system_data = await self.vivintskyapi.get_system_data(
+                    full_system_data = await self.api.get_system_data(
                         system_data[SystemAttribute.PANEL_ID]
                     )
                     self.systems.append(
                         System(
-                            system_data.get(SystemAttribute.SYSTEM_NICKNAME),
-                            full_system_data,
-                            self.vivintskyapi,
+                            data=full_system_data,
+                            api=self.api,
+                            name=system_data.get(SystemAttribute.SYSTEM_NICKNAME),
+                            is_admin=system_data.get(SystemAttribute.ADMIN, False),
                         )
                     )
 
             _LOGGER.debug(
                 "Refreshed %s system(s)",
                 len(authuser_data[AuthUserAttribute.USERS][UserAttribute.SYSTEM]),
             )
 
     async def subscribe_for_realtime_updates(
         self, authuser_data: dict | None = None
     ) -> None:
         """Subscribe to PubNub for realtime updates."""
         # make a call to vivint's authuser endpoint to get message broadcast channel if not supplied
         if not authuser_data:
-            authuser_data = await self.vivintskyapi.get_authuser_data()
+            authuser_data = await self.api.get_authuser_data()
 
         user_data = authuser_data[AuthUserAttribute.USERS]
 
         pnconfig = PNConfiguration()
         pnconfig.subscribe_key = PN_SUBSCRIBE_KEY
         pnconfig.uuid = f"pn-{user_data[UserAttribute.ID].upper()}"
         pnconfig.ssl = True
```

### Comparing `vivintpy-2023.3.3/vivintpy/const.py` & `vivintpy-2023.3.4/vivintpy/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     CURRENT_VERSION = "csv"
     UPDATE_REASON = "rsn"
 
 
 class SystemAttribute:
     """System attributes."""
 
+    ADMIN = "ad"
     PANEL_ID = "panid"
     PARTITION = "par"
     PARTITION_ID = "parid"
     SYSTEM = "system"
     SYSTEM_NICKNAME = "sn"
 
 
@@ -95,14 +96,15 @@
     """Vivint device attributes."""
 
     BATTERY_LEVEL = "bl"
     BYPASSED = "b"
     CAPABILITY = "ca"
     CAPABILITY_CATEGORY = "caca"
     CURRENT_SOFTWARE_VERSION = "csv"
+    FEATURES = "fea"
     FIRMWARE_VERSION = "fwv"
     HIDDEN = "hidden"
     ID = "_id"
     LOW_BATTERY = "lb"
     NAME = "n"
     ONLINE = "ol"
     PANEL_ID = "panid"
```

### Comparing `vivintpy-2023.3.3/vivintpy/devices/__init__.py` & `vivintpy-2023.3.4/vivintpy/devices/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 """This package contains the various devices attached to a Vivint system."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Type
 
 from ..const import VivintDeviceAttribute as Attribute
 from ..entity import Entity
-from ..enums import CapabilityCategoryType, CapabilityType, DeviceType, ZoneBypass
+from ..enums import (
+    CapabilityCategoryType,
+    CapabilityType,
+    DeviceType,
+    FeatureType,
+    ZoneBypass,
+)
+from ..utils import send_deprecation_warning
 from ..vivintskyapi import VivintSkyApi
 from ..zjs_device_config_db import get_zwave_device_info
 
 if TYPE_CHECKING:
     from .alarm_panel import AlarmPanel
 
 DEVICE = "device"
@@ -55,21 +62,32 @@
                     for capability in capability_category.get(Attribute.CAPABILITY)
                 ]
                 for capability_category in caca
             }
             if (caca := data.get(Attribute.CAPABILITY_CATEGORY)) is not None
             else None
         )
+        self._features = (
+            [FeatureType(feature) for feature in feats if feats.get(feature) is True]
+            if (feats := data.get(Attribute.FEATURES)) is not None
+            else None
+        )
         self._parent: VivintDevice | None = None
 
     def __repr__(self) -> str:
         """Return custom __repr__ of device."""
         return f"<{self.__class__.__name__} {self.id}, {self.name}>"
 
     @property
+    def api(self) -> VivintSkyApi:
+        """Return the API."""
+        assert self.alarm_panel, """no alarm panel set for this device"""
+        return self.alarm_panel.system.api
+
+    @property
     def id(self) -> int:  # pylint: disable=invalid-name
         """Device's id."""
         return int(self.data[Attribute.ID])
 
     @property
     def is_valid(self) -> bool:
         """Return `True` if the device is valid."""
@@ -98,14 +116,19 @@
 
     @property
     def device_type(self) -> DeviceType:
         """Return the device type."""
         return DeviceType(self.data.get(Attribute.TYPE))
 
     @property
+    def features(self) -> list[FeatureType] | None:
+        """Device Features."""
+        return self._features
+
+    @property
     def has_battery(self) -> bool:
         """Return `True` if the device has battery details."""
         return (
             self.data.get(Attribute.BATTERY_LEVEL) is not None
             or self.data.get(Attribute.LOW_BATTERY) is not None
         )
 
@@ -163,16 +186,16 @@
             if (fwv := self.data.get(Attribute.FIRMWARE_VERSION)) is not None
             else None
         )
 
     @property
     def vivintskyapi(self) -> VivintSkyApi:
         """Instance of VivintSkyApi."""
-        assert self.alarm_panel, """no alarm panel set for this device"""
-        return self.alarm_panel.system.vivintskyapi
+        send_deprecation_warning("vivintskyapi", "api")
+        return self.api
 
     def get_zwave_details(self) -> None:
         """Get Z-Wave details."""
         if self.data.get("zpd") is None:
             return
 
         result = get_zwave_device_info(
```

### Comparing `vivintpy-2023.3.3/vivintpy/devices/alarm_panel.py` & `vivintpy-2023.3.4/vivintpy/devices/alarm_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,17 +48,23 @@
         )
 
     def __repr__(self) -> str:
         """Return custom __repr__ of device."""
         return f"<{self.__class__.__name__} {self.id}, {self.name}: {self.state.name}>"
 
     @property
+    def api(self) -> VivintSkyApi:
+        """Return the API."""
+        return self.system.api
+
+    @property
     def vivintskyapi(self) -> VivintSkyApi:
         """Instance of VivitSkyApi."""
-        return self.system.vivintskyapi
+        send_deprecation_warning("vivintskyapi", "api")
+        return self.api
 
     @property
     def id(self) -> int:
         """Panel's id."""
         return int(self.data[Attribute.PANEL_ID])
 
     @property
@@ -119,20 +125,20 @@
         """Return the panel's arm state."""
         send_deprecation_warning("method get_armed_state", "property state")
         return self.data[Attribute.STATE]
 
     async def set_armed_state(self, state: int) -> None:
         """Set the armed state for a panel."""
         _LOGGER.debug("Setting %s to %s", self.name, ArmedState(state).name)
-        await self.vivintskyapi.set_alarm_state(self.id, self.partition_id, state)
+        await self.api.set_alarm_state(self.id, self.partition_id, state)
 
     async def trigger_alarm(self) -> None:
         """Trigger an alarm."""
         _LOGGER.debug("Triggering an alarm on %s", self.name)
-        await self.vivintskyapi.trigger_alarm(self.id, self.partition_id)
+        await self.api.trigger_alarm(self.id, self.partition_id)
 
     async def disarm(self) -> None:
         """Disarm the alarm."""
         await self.set_armed_state(ArmedState.DISARMED)
 
     async def arm_stay(self) -> None:
         """Set the alarm to armed stay."""
@@ -141,43 +147,58 @@
     async def arm_away(self) -> None:
         """Set the alarm to armed away."""
         await self.set_armed_state(ArmedState.ARMED_AWAY)
 
     async def get_panel_credentials(self) -> dict:
         """Get the panel credentials."""
         if not self.__panel_credentials:
-            self.__panel_credentials = await self.vivintskyapi.get_panel_credentials(
-                self.id
-            )
+            self.__panel_credentials = await self.api.get_panel_credentials(self.id)
         return self.__panel_credentials
 
     async def get_software_update_details(self) -> dict[str, bool | str]:
         """Get the software update details."""
-        details = await self.vivintskyapi.get_system_update(self.id)
+        if not self.system.is_admin:
+            _LOGGER.warning(
+                "%s - Cannot get software update details as user is not an admin",
+                self.name,
+            )
+            details = {}
+        else:
+            details = await self.api.get_system_update(self.id)
         return {
             "available": details.get(PanelUpdateAttribute.AVAILABLE, False),
             "available_version": details.get(
                 PanelUpdateAttribute.AVAILABLE_VERSION, ""
             ),
             "current_version": details.get(PanelUpdateAttribute.CURRENT_VERSION, ""),
             "update_reason": details.get(PanelUpdateAttribute.UPDATE_REASON, ""),
         }
 
     async def update_software(self) -> bool:
         """Update the panel software version."""
+        if not self.system.is_admin:
+            _LOGGER.warning(
+                "%s - Cannot update software as user is not an admin", self.name
+            )
+            return False
         try:
-            await self.vivintskyapi.update_panel_software(self.id)
+            await self.api.update_panel_software(self.id)
         except VivintSkyApiError as err:
-            _LOGGER.error("%s for %s", err, self.name)
+            _LOGGER.error("%s - %s", self.name, err)
             return False
         return True
 
     async def reboot(self) -> None:
         """Reboot the panel."""
-        await self.vivintskyapi.reboot_panel(self.id)
+        if not self.system.is_admin:
+            _LOGGER.warning(
+                "%s - Cannot reboot panel as user is not an admin", self.name
+            )
+            return
+        await self.api.reboot_panel(self.id)
 
     def get_devices(
         self, device_types: set[Type[VivintDevice]] | None = None
     ) -> list[VivintDevice]:
         """Get a list of associated devices."""
         devices: list[VivintDevice] = []
 
@@ -268,15 +289,15 @@
         try:
             device = first_or_none(self.devices, lambda device: device.id == device_id)
             assert device
             while not device.is_valid:
                 await asyncio.sleep(1)
                 if device.id in self.unregistered_devices:
                     return
-            resp = await self.vivintskyapi.get_device_data(self.id, device_id)
+            resp = await self.api.get_device_data(self.id, device_id)
             data = resp[SystemAttribute.SYSTEM][SystemAttribute.PARTITION][0]
             self.refresh(data, new_device=True)
             self.emit(DEVICE_DISCOVERED, {"device": device})
         except VivintSkyApiError:
             _LOGGER.error("Error getting new device data for device %s", device_id)
 
     def __parse_data(self, data: dict, init: bool = False) -> None:
```

### Comparing `vivintpy-2023.3.3/vivintpy/devices/camera.py` & `vivintpy-2023.3.4/vivintpy/devices/camera.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,14 +94,19 @@
 
     @property
     def ip_address(self) -> str:
         """Camera's IP address."""
         return str(self.data[Attribute.CAMERA_IP_ADDRESS])
 
     @property
+    def is_in_deter_mode(self) -> bool:
+        """Return True if deter mode is active."""
+        return bool(self.data[Attribute.DETER_ON_DUTY])
+
+    @property
     def mac_address(self) -> str:
         """Camera's MAC Address."""
         return str(self.data[Attribute.CAMERA_MAC])
 
     @property
     def is_in_privacy_mode(self) -> bool:
         """Return True if privacy mode is active."""
@@ -115,29 +120,29 @@
     @property
     def wireless_signal_strength(self) -> int:
         """Camera's wireless signal strength."""
         return int(self.data[Attribute.WIRELESS_SIGNAL_STRENGTH])
 
     async def request_thumbnail(self) -> None:
         """Request a new thumbnail for the camera."""
-        await self.vivintskyapi.request_camera_thumbnail(
+        await self.api.request_camera_thumbnail(
             self.alarm_panel.id, self.alarm_panel.partition_id, self.id
         )
 
     async def get_thumbnail_url(self) -> str | None:
         """Return the latest camera thumbnail URL."""
         # Sometimes this date field comes back with a "Z" at the end
         # and sometimes it doesn't, so let's just safely remove it.
         camera_thumbnail_date = datetime.strptime(
             self.data[Attribute.CAMERA_THUMBNAIL_DATE].replace("Z", ""),
             "%Y-%m-%dT%H:%M:%S.%f",
         )
         thumbnail_timestamp = int(camera_thumbnail_date.timestamp() * 1000)
 
-        return await self.vivintskyapi.get_camera_thumbnail_url(
+        return await self.api.get_camera_thumbnail_url(
             self.alarm_panel.id,
             self.alarm_panel.partition_id,
             self.id,
             thumbnail_timestamp,
         )
 
     async def get_rtsp_url(
@@ -157,23 +162,35 @@
             if self.data[Attribute.CAMERA_DIRECT_AVAILABLE]
             and self.data.get(Attribute.ACTUAL_TYPE) not in SKIP_DIRECT
             else None
         )
 
     async def set_as_doorbell_chime_extender(self, state: bool) -> None:
         """Set use as doorbell chime extender."""
-        await self.vivintskyapi.set_camera_as_doorbell_chime_extender(
+        await self.api.set_camera_as_doorbell_chime_extender(
             self.alarm_panel.id, self.id, state
         )
 
     async def set_privacy_mode(self, state: bool) -> None:
         """Set privacy mode."""
-        await self.vivintskyapi.set_camera_privacy_mode(
-            self.alarm_panel.id, self.id, state
-        )
+        if not self.alarm_panel.system.is_admin:
+            _LOGGER.warning(
+                "%s - Cannot set privacy mode as user is not an admin", self.name
+            )
+            return
+        await self.api.set_camera_privacy_mode(self.alarm_panel.id, self.id, state)
+
+    async def set_deter_mode(self, state: bool) -> None:
+        """Set deter mode."""
+        if not self.alarm_panel.system.is_admin:
+            _LOGGER.warning(
+                "%s - Cannot set deter mode as user is not an admin", self.name
+            )
+            return
+        await self.api.set_camera_deter_mode(self.alarm_panel.id, self.id, state)
 
     def handle_pubnub_message(self, message: dict) -> None:
         """Handle a pubnub message addressed to this camera."""
         super().handle_pubnub_message(message)
 
         event = None
```

### Comparing `vivintpy-2023.3.3/vivintpy/devices/door_lock.py` & `vivintpy-2023.3.4/vivintpy/devices/door_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """Return True if the node is online."""
         send_deprecation_warning("node_online", "is_online")
         return self.is_online
 
     async def set_state(self, locked: bool) -> None:
         """Set door lock's state."""
         assert self.alarm_panel
-        await self.vivintskyapi.set_lock_state(
+        await self.api.set_lock_state(
             self.alarm_panel.id, self.alarm_panel.partition_id, self.id, locked
         )
 
     async def lock(self) -> None:
         """Lock the door lock."""
         await self.set_state(True)
```

### Comparing `vivintpy-2023.3.3/vivintpy/devices/garage_door.py` & `vivintpy-2023.3.4/vivintpy/devices/garage_door.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def get_state(self) -> Any:
         """Return the garage door's state."""
         return self.data[Attribute.STATE]
 
     async def set_state(self, state: int) -> None:
         """Set garage door's state."""
         assert self.alarm_panel
-        await self.vivintskyapi.set_garage_door_state(
+        await self.api.set_garage_door_state(
             self.alarm_panel.id, self.alarm_panel.partition_id, self.id, state
         )
 
     async def close(self) -> None:
         """Close the garage door."""
         await self.set_state(GarageDoorState.CLOSING)
```

### Comparing `vivintpy-2023.3.3/vivintpy/devices/switch.py` & `vivintpy-2023.3.4/vivintpy/devices/switch.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     async def set_state(
         self,
         on: bool | None = None,  # pylint: disable=invalid-name
         level: int | None = None,
     ) -> None:
         """Set switch's state."""
         assert self.alarm_panel
-        await self.vivintskyapi.set_switch_state(
+        await self.api.set_switch_state(
             self.alarm_panel.id, self.alarm_panel.partition_id, self.id, on, level
         )
 
     async def turn_on(self) -> None:
         """Turn on the switch."""
         await self.set_state(on=True)
```

### Comparing `vivintpy-2023.3.3/vivintpy/devices/thermostat.py` & `vivintpy-2023.3.4/vivintpy/devices/thermostat.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,10 +86,10 @@
     def celsius_to_fahrenheit(celsius: float) -> int:
         """Convert Celsius to Fahrenheit."""
         return round(celsius * 1.8 + 32)
 
     async def set_state(self, **kwargs: Any) -> None:
         """Set the state of the thermostat."""
         assert self.alarm_panel
-        await self.vivintskyapi.set_thermostat_state(
+        await self.api.set_thermostat_state(
             self.alarm_panel.id, self.alarm_panel.partition_id, self.id, **kwargs
         )
```

### Comparing `vivintpy-2023.3.3/vivintpy/devices/wireless_sensor.py` & `vivintpy-2023.3.4/vivintpy/devices/wireless_sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             self._parent = first_or_none(
                 self.alarm_panel.devices,
                 lambda parent: parent.serial_number == self.serial_number,
             )
 
     async def set_bypass(self, bypass: bool) -> None:
         """Bypass/unbypass the sensor."""
-        await self.vivintskyapi.set_sensor_state(
+        await self.api.set_sensor_state(
             self.alarm_panel.id, self.alarm_panel.partition_id, self.id, bypass
         )
 
     async def bypass(self) -> None:
         """Bypass the sensor."""
         await self.set_bypass(True)
```

### Comparing `vivintpy-2023.3.3/vivintpy/entity.py` & `vivintpy-2023.3.4/vivintpy/entity.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/enums.py` & `vivintpy-2023.3.4/vivintpy/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,14 +328,33 @@
 
     @classmethod
     def _missing_(cls, value: Any) -> FanMode:
         _LOGGER.debug("Unknown fan mode value: %s", value)
         return cls.UNKNOWN
 
 
+class FeatureType(Enum):
+    """Feature type."""
+
+    DETER = "deter"
+    DYNAMIC_CHIMES = "dynamic_chimes_available"
+    PACKAGE_WATCH = "package_watch"
+    REBOOT = "rb"
+    RESTORE_DEFAULTS = "rstdef"
+    SELECTABLE_NIGHTVISION = "nght"
+    VIDEO_THUMBNAILS = "video_thumbnails"
+
+    UKNOWN = "unknown"
+
+    @classmethod
+    def _missing_(cls, value: object) -> FeatureType:
+        _LOGGER.debug("Unknown feature type value: %s", value)
+        return cls.UKNOWN
+
+
 @unique
 class GarageDoorState(IntEnum):
     """Garage door state."""
 
     UNKNOWN = 0
     CLOSED = 1
     CLOSING = 2
```

### Comparing `vivintpy-2023.3.3/vivintpy/exceptions.py` & `vivintpy-2023.3.4/vivintpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/proto/beam_pb2.py` & `vivintpy-2023.3.4/vivintpy/proto/beam_pb2.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/proto/beam_pb2.pyi` & `vivintpy-2023.3.4/vivintpy/proto/beam_pb2.pyi`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/proto/beam_pb2_grpc.py` & `vivintpy-2023.3.4/vivintpy/proto/beam_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/pubnub.py` & `vivintpy-2023.3.4/vivintpy/pubnub.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/system.py` & `vivintpy-2023.3.4/vivintpy/system.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 """Module that implements the System class."""
 from __future__ import annotations
 
 import logging
 
-from .const import PubNubMessageAttribute, SystemAttribute
+from .const import PubNubMessageAttribute
+from .const import SystemAttribute as Attribute
 from .devices.alarm_panel import AlarmPanel
 from .entity import Entity
-from .utils import first_or_none
+from .utils import first_or_none, send_deprecation_warning
 from .vivintskyapi import VivintSkyApi
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class System(Entity):
     """Describe a vivint system."""
 
-    def __init__(self, name: str, data: dict, vivintskyapi: VivintSkyApi):
+    def __init__(self, data: dict, api: VivintSkyApi, *, name: str, is_admin: bool):
         """Initialize a system."""
         super().__init__(data)
-        self.__name = name
-        self.vivintskyapi = vivintskyapi
+        self._api = api
+        self._name = name
+        self._is_admin = is_admin
         self.alarm_panels: list[AlarmPanel] = [
             AlarmPanel(panel_data, self)
-            for panel_data in self.data[SystemAttribute.SYSTEM][
-                SystemAttribute.PARTITION
-            ]
+            for panel_data in self.data[Attribute.SYSTEM][Attribute.PARTITION]
         ]
 
     @property
+    def api(self) -> VivintSkyApi:
+        """Return the API."""
+        return self._api
+
+    @property
+    def vivintskyapi(self) -> VivintSkyApi:
+        """Return the API."""
+        send_deprecation_warning("vivintskyapi", "api")
+        return self.api
+
+    @property
     def id(self) -> int:  # pylint: disable=invalid-name
         """System's id."""
-        return int(self.data[SystemAttribute.SYSTEM][SystemAttribute.PANEL_ID])
+        return int(self.data[Attribute.SYSTEM][Attribute.PANEL_ID])
+
+    @property
+    def is_admin(self) -> bool:
+        """Return True if the user is an admin for this system."""
+        return self._is_admin
 
     @property
     def name(self) -> str:
         """System's name."""
-        return self.__name
+        return self._name
 
     async def refresh(self) -> None:
         """Reload a system's data from the VivintSky API."""
-        system_data = await self.vivintskyapi.get_system_data(self.id)
+        system_data = await self.api.get_system_data(self.id)
 
-        for panel_data in system_data[SystemAttribute.SYSTEM][
-            SystemAttribute.PARTITION
-        ]:
+        for panel_data in system_data[Attribute.SYSTEM][Attribute.PARTITION]:
             alarm_panel = first_or_none(
                 self.alarm_panels,
                 lambda panel, panel_data=panel_data: panel.id  # type: ignore
-                == panel_data[SystemAttribute.PANEL_ID]
-                and panel.partition_id == panel_data[SystemAttribute.PARTITION_ID],
+                == panel_data[Attribute.PANEL_ID]
+                and panel.partition_id == panel_data[Attribute.PARTITION_ID],
             )
             if alarm_panel:
                 alarm_panel.refresh(panel_data)
             else:
                 self.alarm_panels.append(AlarmPanel(panel_data, self))
 
     def handle_pubnub_message(self, message: dict) -> None:
```

### Comparing `vivintpy-2023.3.3/vivintpy/utils.py` & `vivintpy-2023.3.4/vivintpy/utils.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/vivintskyapi.py` & `vivintpy-2023.3.4/vivintpy/vivintskyapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,32 @@
                     ),
                     metadata=[("session", cookie.value)],
                 )
             )
 
         _LOGGER.debug("Response received: %s", str(response))
 
+    async def set_camera_deter_mode(
+        self, panel_id: int, device_id: int, state: bool
+    ) -> None:
+        """Set the camera deter mode."""
+        creds = grpc.ssl_channel_credentials()
+        assert (cookie := self._get_session_cookie())
+
+        async with grpc.aio.secure_channel(BEAM_ENDPOINT, credentials=creds) as channel:
+            stub: beam_pb2_grpc.BeamStub = beam_pb2_grpc.BeamStub(channel)  # type: ignore
+            response: beam_pb2.SetDeterOverrideResponse = await stub.SetDeterOverride(
+                beam_pb2.SetDeterOverrideRequest(  # pylint: disable=no-member
+                    panel_id=panel_id, device_id=device_id, enabled=state
+                ),
+                metadata=[("session", cookie.value)],
+            )
+
+        _LOGGER.debug("Response received: %s", str(response))
+
     async def set_garage_door_state(
         self, panel_id: int, partition_id: int, device_id: int, state: int
     ) -> None:
         """Open/Close garage door."""
         resp = await self.__put(
             f"{panel_id}/{partition_id}/door/{device_id}",
             headers={
```

### Comparing `vivintpy-2023.3.3/vivintpy/zjs_device_config_db.json` & `vivintpy-2023.3.4/vivintpy/zjs_device_config_db.json`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/vivintpy/zjs_device_config_db.py` & `vivintpy-2023.3.4/vivintpy/zjs_device_config_db.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.3/setup.py` & `vivintpy-2023.3.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,85 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: vivintpy
+Version: 2023.3.4
+Summary: Python library for interacting with a Vivint security and smart home system.
+Home-page: https://github.com/natekspencer/vivintpy
+License: MIT
+Keywords: Vivint,alarm system,security,smart home,home automation,asynchronous
+Author: Nathan Spencer
+Author-email: natekspencer@gmail.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: certifi (>=2022.9.24,<2023.0.0)
+Requires-Dist: grpcio (==1.56.0)
+Requires-Dist: protobuf (>=4.22.1,<5.0.0)
+Requires-Dist: pubnub (>=7.0,<8.0)
+Project-URL: Repository, https://github.com/natekspencer/vivintpy
+Description-Content-Type: text/markdown
+
+[![pypi](https://img.shields.io/pypi/v/vivintpy?style=for-the-badge)](https://pypi.org/project/vivintpy)
+[![downloads](https://img.shields.io/pypi/dm/vivintpy?style=for-the-badge)](https://pypi.org/project/vivintpy)
+[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)
+
+# vivintpy
+
+Python library for interacting with a Vivint security and smart home system.
+
+This was built to support the `Vivint` integration in [Home-Assistant](https://www.home-assistant.io/) but _should_ work outside of it too. Currently, it can be utilized via [HACS](https://hacs.xyz/) by adding the [hacs-vivint](https://github.com/natekspencer/hacs-vivint) custom repository.
+
+## Credit
+
+This was inspired by the great work done by [Mike Reibard](https://github.com/Riebart/vivint.py) to reverse engineer the Vivint Sky API and [Ovidiu Stateina](https://github.com/ovirs/pyvivint) for the repository from which this is forked and expanded on.
+
+## Features
+
+It currently has support for the following device types:
+
+- alarm panels
+- cameras
+- door locks
+- garage doors
+- switches
+  - binary
+  - multilevel
+- thermostats
+- wireless sensors
+  - carbon monoxide
+  - door/window
+  - flood
+  - glass break
+  - motion
+  - smoke/fire
+  - etc
+
+In addition, it integrates with PubNub to receive real-time updates for devices. This subscription stops receiving notifications around 15-20 minutes unless a call is made to the Vivint Sky API periodically. This **might** be related to the cookie expiration since it expires 20 minutes after the last API call was received. If another client connects, however, the notifications start to stream again for all currently connected clients.
+
+## Usage
+
+See demo.py for a demonstration on how to use this library.
+
+## TODO:
+
+- write a better readme
+- write some documentation
+- add advanced support for:
+  - thermostats
+- add tests
+
+---
+
+## Support Me
 
-packages = \
-['vivintpy', 'vivintpy.devices', 'vivintpy.proto']
+I'm not employed by Vivint, and provide this python package as-is.
 
-package_data = \
-{'': ['*']}
+If you don't already own a Vivint system, please consider using [my referal code (kaf164)](https://www.vivint.com/get?refCode=kaf164&exid=165211vivint.com/get?refCode=kaf164&exid=165211) to get $50 off your bill (as well as a tip to me in appreciation)!
 
-install_requires = \
-['aiohttp>=3.8.4,<4.0.0',
- 'certifi>=2022.9.24,<2023.0.0',
- 'grpcio==1.51.1',
- 'protobuf>=4.22.1,<5.0.0',
- 'pubnub>=7.0,<8.0']
-
-setup_kwargs = {
-    'name': 'vivintpy',
-    'version': '2023.3.3',
-    'description': 'Python library for interacting with a Vivint security and smart home system.',
-    'long_description': "[![pypi](https://img.shields.io/pypi/v/vivintpy?style=for-the-badge)](https://pypi.org/project/vivintpy)\n[![downloads](https://img.shields.io/pypi/dm/vivintpy?style=for-the-badge)](https://pypi.org/project/vivintpy)\n[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)\n\n# vivintpy\n\nPython library for interacting with a Vivint security and smart home system.\n\nThis was built to support the `Vivint` integration in [Home-Assistant](https://www.home-assistant.io/) but _should_ work outside of it too. Currently, it can be utilized via [HACS](https://hacs.xyz/) by adding the [hacs-vivint](https://github.com/natekspencer/hacs-vivint) custom repository.\n\n## Credit\n\nThis was inspired by the great work done by [Mike Reibard](https://github.com/Riebart/vivint.py) to reverse engineer the Vivint Sky API and [Ovidiu Stateina](https://github.com/ovirs/pyvivint) for the repository from which this is forked and expanded on.\n\n## Features\n\nIt currently has support for the following device types:\n\n- alarm panels\n- cameras\n- door locks\n- garage doors\n- switches\n  - binary\n  - multilevel\n- thermostats\n- wireless sensors\n  - carbon monoxide\n  - door/window\n  - flood\n  - glass break\n  - motion\n  - smoke/fire\n  - etc\n\nIn addition, it integrates with PubNub to receive real-time updates for devices. This subscription stops receiving notifications around 15-20 minutes unless a call is made to the Vivint Sky API periodically. This **might** be related to the cookie expiration since it expires 20 minutes after the last API call was received. If another client connects, however, the notifications start to stream again for all currently connected clients.\n\n## Usage\n\nSee demo.py for a demonstration on how to use this library.\n\n## TODO:\n\n- write a better readme\n- write some documentation\n- add advanced support for:\n  - thermostats\n- add tests\n\n---\n\n## Support Me\n\nI'm not employed by Vivint, and provide this python package as-is.\n\nIf you don't already own a Vivint system, please consider using [my referal code (kaf164)](https://www.vivint.com/get?refCode=kaf164&exid=165211vivint.com/get?refCode=kaf164&exid=165211) to get $50 off your bill (as well as a tip to me in appreciation)!\n\nIf you already own a Vivint system and still want to donate, consider buying me a coffee ☕ (or beer 🍺) instead by using the link below:\n\n<a href='https://ko-fi.com/natekspencer' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' />\n",
-    'author': 'Nathan Spencer',
-    'author_email': 'natekspencer@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/natekspencer/vivintpy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+If you already own a Vivint system and still want to donate, consider buying me a coffee ☕ (or beer 🍺) instead by using the link below:
 
+<a href='https://ko-fi.com/natekspencer' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' />
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,44 +1,45 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['vivintpy',
-'vivintpy.devices', 'vivintpy.proto'] package_data = \ {'': ['*']}
-install_requires = \ ['aiohttp>=3.8.4,<4.0.0', 'certifi>=2022.9.24,<2023.0.0',
-'grpcio==1.51.1', 'protobuf>=4.22.1,<5.0.0', 'pubnub>=7.0,<8.0'] setup_kwargs =
-{ 'name': 'vivintpy', 'version': '2023.3.3', 'description': 'Python library for
-interacting with a Vivint security and smart home system.', 'long_description':
-"[![pypi](https://img.shields.io/pypi/v/vivintpy?style=for-the-badge)](https://
-pypi.org/project/vivintpy)\n[![downloads](https://img.shields.io/pypi/dm/
-vivintpy?style=for-the-badge)](https://pypi.org/project/vivintpy)\n[![Buy Me A
-Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_â/ðº-F16061?style=for-
-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/
-natekspencer)\n\n# vivintpy\n\nPython library for interacting with a Vivint
-security and smart home system.\n\nThis was built to support the `Vivint`
+Metadata-Version: 2.1 Name: vivintpy Version: 2023.3.4 Summary: Python library
+for interacting with a Vivint security and smart home system. Home-page: https:
+//github.com/natekspencer/vivintpy License: MIT Keywords: Vivint,alarm
+system,security,smart home,home automation,asynchronous Author: Nathan Spencer
+Author-email: natekspencer@gmail.com Requires-Python: >=3.7.2,<4.0.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: certifi
+(>=2022.9.24,<2023.0.0) Requires-Dist: grpcio (==1.56.0) Requires-Dist:
+protobuf (>=4.22.1,<5.0.0) Requires-Dist: pubnub (>=7.0,<8.0) Project-URL:
+Repository, https://github.com/natekspencer/vivintpy Description-Content-Type:
+text/markdown [![pypi](https://img.shields.io/pypi/v/vivintpy?style=for-the-
+badge)](https://pypi.org/project/vivintpy) [![downloads](https://
+img.shields.io/pypi/dm/vivintpy?style=for-the-badge)](https://pypi.org/project/
+vivintpy) [![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_â/
+ðº-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)]
+(https://ko-fi.com/natekspencer) # vivintpy Python library for interacting with
+a Vivint security and smart home system. This was built to support the `Vivint`
 integration in [Home-Assistant](https://www.home-assistant.io/) but _should_
 work outside of it too. Currently, it can be utilized via [HACS](https://
 hacs.xyz/) by adding the [hacs-vivint](https://github.com/natekspencer/hacs-
-vivint) custom repository.\n\n## Credit\n\nThis was inspired by the great work
-done by [Mike Reibard](https://github.com/Riebart/vivint.py) to reverse
-engineer the Vivint Sky API and [Ovidiu Stateina](https://github.com/ovirs/
-pyvivint) for the repository from which this is forked and expanded on.\n\n##
-Features\n\nIt currently has support for the following device types:\n\n- alarm
-panels\n- cameras\n- door locks\n- garage doors\n- switches\n - binary\n -
-multilevel\n- thermostats\n- wireless sensors\n - carbon monoxide\n - door/
-window\n - flood\n - glass break\n - motion\n - smoke/fire\n - etc\n\nIn
-addition, it integrates with PubNub to receive real-time updates for devices.
-This subscription stops receiving notifications around 15-20 minutes unless a
-call is made to the Vivint Sky API periodically. This **might** be related to
-the cookie expiration since it expires 20 minutes after the last API call was
-received. If another client connects, however, the notifications start to
-stream again for all currently connected clients.\n\n## Usage\n\nSee demo.py
-for a demonstration on how to use this library.\n\n## TODO:\n\n- write a better
-readme\n- write some documentation\n- add advanced support for:\n -
-thermostats\n- add tests\n\n---\n\n## Support Me\n\nI'm not employed by Vivint,
-and provide this python package as-is.\n\nIf you don't already own a Vivint
-system, please consider using [my referal code (kaf164)](https://
-www.vivint.com/get?refCode=kaf164&exid=165211vivint.com/
-get?refCode=kaf164&exid=165211) to get $50 off your bill (as well as a tip to
-me in appreciation)!\n\nIf you already own a Vivint system and still want to
-donate, consider buying me a coffee â (or beer ðº) instead by using the
-link below:\n\n[Buy_Me_a_Coffee_at_ko-fi.com]\n",_'author':_'Nathan_Spencer',
-'author_email':_'natekspencer@gmail.com',_'maintainer':_'None',
-'maintainer_email':_'None',_'url':_'https://github.com/natekspencer/vivintpy',
-'packages':_packages,_'package_data':_package_data,_'install_requires':
-install_requires,_'python_requires':_'>=3.7.2,<4.0.0',_}_setup(**setup_kwargs)_
+vivint) custom repository. ## Credit This was inspired by the great work done
+by [Mike Reibard](https://github.com/Riebart/vivint.py) to reverse engineer the
+Vivint Sky API and [Ovidiu Stateina](https://github.com/ovirs/pyvivint) for the
+repository from which this is forked and expanded on. ## Features It currently
+has support for the following device types: - alarm panels - cameras - door
+locks - garage doors - switches - binary - multilevel - thermostats - wireless
+sensors - carbon monoxide - door/window - flood - glass break - motion - smoke/
+fire - etc In addition, it integrates with PubNub to receive real-time updates
+for devices. This subscription stops receiving notifications around 15-20
+minutes unless a call is made to the Vivint Sky API periodically. This
+**might** be related to the cookie expiration since it expires 20 minutes after
+the last API call was received. If another client connects, however, the
+notifications start to stream again for all currently connected clients. ##
+Usage See demo.py for a demonstration on how to use this library. ## TODO: -
+write a better readme - write some documentation - add advanced support for: -
+thermostats - add tests --- ## Support Me I'm not employed by Vivint, and
+provide this python package as-is. If you don't already own a Vivint system,
+please consider using [my referal code (kaf164)](https://www.vivint.com/
+get?refCode=kaf164&exid=165211vivint.com/get?refCode=kaf164&exid=165211) to get
+$50 off your bill (as well as a tip to me in appreciation)! If you already own
+a Vivint system and still want to donate, consider buying me a coffee â (or
+beer ðº) instead by using the link below: [Buy_Me_a_Coffee_at_ko-fi.com]_
```

