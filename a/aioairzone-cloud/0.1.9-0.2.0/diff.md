# Comparing `tmp/aioairzone-cloud-0.1.9.tar.gz` & `tmp/aioairzone-cloud-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.1.9.tar", last modified: Sat Jun 24 07:46:56 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.2.0.tar", last modified: Tue Jun 27 18:41:21 2023, max compression
```

## Comparing `aioairzone-cloud-0.1.9.tar` & `aioairzone-cloud-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-24 07:46:56.860138 aioairzone-cloud-0.1.9/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.9/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.9/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-06-24 07:46:56.860138 aioairzone-cloud-0.1.9/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.9/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-24 07:46:56.860138 aioairzone-cloud-0.1.9/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      532 2023-06-24 07:39:53.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/aidoo.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18516 2023-06-08 07:52:33.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6843 2023-05-31 17:41:58.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4355 2023-06-24 07:42:13.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    17493 2023-06-24 07:39:28.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/hvac.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      976 2023-06-24 07:35:03.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     5294 2023-06-24 07:41:32.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2431 2023-06-24 07:40:34.000000 aioairzone-cloud-0.1.9/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-24 07:46:56.860138 aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-06-24 07:46:56.000000 aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-06-24 07:46:56.000000 aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-24 07:46:56.000000 aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-24 07:46:56.000000 aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-06-24 07:46:56.000000 aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-06-24 07:46:56.000000 aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-06-24 07:46:25.000000 aioairzone-cloud-0.1.9/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.9/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-06-24 07:46:56.864138 aioairzone-cloud-0.1.9/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.0/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.0/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.0/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      936 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    21059 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1800 2023-06-26 18:43:43.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     7503 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4886 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    23649 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-06-25 08:46:58.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1605 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5294 2023-06-25 08:46:58.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3091 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.0/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/setup.cfg
```

### Comparing `aioairzone-cloud-0.1.9/LICENSE` & `aioairzone-cloud-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.9/PKG-INFO` & `aioairzone-cloud-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.9
+Version: 0.2.0
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.9/README.md` & `aioairzone-cloud-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/cloudapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,26 @@
     API_DEVICE_ID,
     API_DEVICE_TYPE,
     API_DEVICES,
     API_EMAIL,
     API_GROUPS,
     API_INSTALLATION_ID,
     API_INSTALLATIONS,
+    API_OPTS,
+    API_PARAM,
     API_PASSWORD,
     API_REFRESH_TOKEN,
     API_STATUS,
     API_TOKEN,
     API_TYPE,
     API_URL,
     API_USER,
     API_USER_LOGOUT,
     API_V1,
+    API_VALUE,
     API_WS,
     API_WS_ID,
     AZD_AIDOOS,
     AZD_INSTALLATIONS,
     AZD_SYSTEMS,
     AZD_WEBSERVERS,
     AZD_ZONES,
@@ -224,14 +227,91 @@
             "GET",
             f"{API_V1}/{API_DEVICES}/{API_WS}/{url_id}/{API_STATUS}?{ws_params}",
         )
         self._api_raw_data[RAW_WEBSERVERS][ws_id] = res
 
         return res
 
+    async def api_patch_device(
+        self, device: Device, json: dict[str, Any]
+    ) -> dict[str, Any]:
+        """Perform a PATCH request to update device parameters."""
+        dev_id = device.get_id()
+        url_id = urllib.parse.quote(dev_id)
+
+        return await self.api_request(
+            "PATCH",
+            f"{API_V1}/{API_DEVICES}/{url_id}",
+            json,
+        )
+
+    async def api_set_device_param(
+        self, device: Device, param: str, data: dict[str, Any]
+    ) -> None:
+        """Set device parameter."""
+        json = {
+            API_PARAM: param,
+            API_VALUE: data[API_VALUE],
+            API_INSTALLATION_ID: device.get_installation(),
+        }
+
+        if API_OPTS in data:
+            json[API_OPTS] = data[API_OPTS]
+
+        await self.api_patch_device(device, json)
+
+        device.set_param(param, data)
+
+    async def api_set_device_params(
+        self, device: Device, params: dict[str, Any]
+    ) -> None:
+        """Set device parameters."""
+        tasks = []
+
+        for param, data in params.items():
+            tasks += [self.api_set_device_param(device, param, data)]
+
+        await asyncio.gather(*tasks)
+
+    async def api_set_aidoo_id_params(
+        self, aidoo_id: str, params: dict[str, Any]
+    ) -> None:
+        """Set aidoo parameters."""
+        aidoo = self.get_aidoo_id(aidoo_id)
+        if aidoo is not None:
+            await self.api_set_device_params(aidoo, params)
+
+    async def api_set_device_id_params(
+        self, device_id: str, params: dict[str, Any]
+    ) -> None:
+        """Set device parameters."""
+        device = (
+            self.get_aidoo_id(device_id)
+            or self.get_system_id(device_id)
+            or self.get_zone_id(device_id)
+        )
+        if device is not None:
+            await self.api_set_device_params(device, params)
+
+    async def api_set_system_id_params(
+        self, system_id: str, params: dict[str, Any]
+    ) -> None:
+        """Set system parameters."""
+        system = self.get_system_id(system_id)
+        if system is not None:
+            await self.api_set_device_params(system, params)
+
+    async def api_set_zone_id_params(
+        self, zone_id: str, params: dict[str, Any]
+    ) -> None:
+        """Set zone parameters."""
+        zone = self.get_zone_id(zone_id)
+        if zone is not None:
+            await self.api_set_device_params(zone, params)
+
     async def login(self) -> None:
         """Perform Airzone Cloud API login."""
         if self.token is not None:
             await self.logout()
         resp = await self.api_request(
             "POST",
             f"{API_V1}/{API_AUTH_LOGIN}",
@@ -356,24 +436,26 @@
             if self.get_webserver_id(ws_id) is None:
                 self.webservers[ws_id] = WebServer(inst.get_id(), ws_id)
 
     def set_system_zones_data(self, system: System) -> None:
         """Set slave zones modes from master zone."""
         modes = system.get_modes()
         installation_id = system.get_installation()
-        system_id = system.get_id()
-        system_num = system.get_system()
+        system_num = system.get_system_num()
+        system_ws = system.get_webserver()
         for zone in self.zones.values():
             if (
                 zone.get_installation() != installation_id
-                or zone.get_system() != system_num
+                or zone.get_system_num() != system_num
+                or zone.get_webserver() != system_ws
             ):
                 continue
 
-            zone.set_system_id(system_id)
+            system.add_zone(zone)
+            zone.set_system(system)
             if zone.get_master() is False and modes:
                 zone.set_modes(modes)
 
     async def update_aidoo(self, aidoo: Aidoo) -> None:
         """Update Airzone Cloud Zone from API."""
         device_data = await self.api_get_device_status(aidoo)
         aidoo.update(device_data)
```

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/common.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,25 @@
 class ConnectionOptions:
     """Airzone Cloud options for connection."""
 
     username: str
     password: str
 
 
+class OperationAction(IntEnum):
+    """Airzone Cloud operation actions."""
+
+    COOLING = 1
+    DRYING = 2
+    FAN = 3
+    HEATING = 4
+    IDLE = 5
+    OFF = 6
+
+
 class OperationMode(IntEnum):
     """Airzone Cloud operation modes."""
 
     STOP = 0
     AUTO = 1
     COOLING = 2
     HEATING = 3
@@ -26,14 +37,18 @@
     HEAT_AIR = 7
     HEAT_RADIANT = 8
     HEAT_COMBINED = 9
     COOLING_AIR = 10
     COOLING_RADIANT = 11
     COOLING_COMBINED = 12
 
+    def is_auto(self) -> bool:
+        """Return if mode is Auto."""
+        return self.value in [self.AUTO]
+
     def is_cool(self) -> bool:
         """Return if mode is Cool."""
         return self.value in [
             self.COOLING,
             self.COOLING_AIR,
             self.COOLING_COMBINED,
             self.COOLING_RADIANT,
```

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/const.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Airzone Cloud API constants."""
 
 from datetime import timedelta
 from typing import Final
 
+API_ACTIVE: Final[str] = "active"
 API_AUTH_LOGIN: Final[str] = "auth/login"
 API_AUTH_REFRESH_TOKEN: Final[str] = "auth/refreshToken"
 API_CELSIUS: Final[str] = "celsius"
 API_CITY: Final[str] = "city"
 API_CONFIG: Final[str] = "config"
 API_CONNECTION_DATE: Final[str] = "connection_date"
 API_DEVICE_ID: Final[str] = "device_id"
@@ -27,33 +28,39 @@
 API_LOCATION_ID: Final[str] = "location_id"
 API_META: Final[str] = "meta"
 API_MODE: Final[str] = "mode"
 API_MODE_AVAIL: Final[str] = "mode_available"
 API_NAME: Final[str] = "name"
 API_OLD_ID: Final[str] = "_id"
 API_OPTS: Final[str] = "opts"
+API_PARAM: Final[str] = "param"
 API_PARAMS: Final[str] = "params"
 API_PASSWORD: Final[str] = "password"
 API_PIN: Final[str] = "pin"
 API_POWER: Final[str] = "power"
+API_RANGE_MAX_AIR: Final[str] = "range_air_max"
+API_RANGE_MIN_AIR: Final[str] = "range_air_min"
+API_RANGE_SP_MAX_AUTO_AIR: Final[str] = "range_sp_auto_air_max"
 API_RANGE_SP_MAX_COOL_AIR: Final[str] = "range_sp_cool_air_max"
 API_RANGE_SP_MAX_DRY_AIR: Final[str] = "range_sp_dry_air_max"
 API_RANGE_SP_MAX_EMERHEAT_AIR: Final[str] = "range_sp_emerheat_air_max"
 API_RANGE_SP_MAX_HOT_AIR: Final[str] = "range_sp_hot_air_max"
 API_RANGE_SP_MAX_STOP_AIR: Final[str] = "range_sp_stop_air_max"
 API_RANGE_SP_MAX_VENT_AIR: Final[str] = "range_sp_vent_air_max"
+API_RANGE_SP_MIN_AUTO_AIR: Final[str] = "range_sp_auto_air_min"
 API_RANGE_SP_MIN_COOL_AIR: Final[str] = "range_sp_cool_air_min"
 API_RANGE_SP_MIN_DRY_AIR: Final[str] = "range_sp_dry_air_min"
 API_RANGE_SP_MIN_EMERHEAT_AIR: Final[str] = "range_sp_emerheat_air_min"
 API_RANGE_SP_MIN_HOT_AIR: Final[str] = "range_sp_hot_air_min"
 API_RANGE_SP_MIN_STOP_AIR: Final[str] = "range_sp_stop_air_min"
 API_RANGE_SP_MIN_VENT_AIR: Final[str] = "range_sp_vent_air_min"
 API_REFRESH_TOKEN: Final[str] = "refreshToken"
 API_SETPOINT: Final[str] = "setpoint"
 API_SLEEP: Final[str] = "sleep"
+API_SP_AIR_AUTO: Final[str] = "setpoint_air_auto"
 API_SP_AIR_COOL: Final[str] = "setpoint_air_cool"
 API_SP_AIR_DRY: Final[str] = "setpoint_air_dry"
 API_SP_AIR_HEAT: Final[str] = "setpoint_air_heat"
 API_SP_AIR_STOP: Final[str] = "setpoint_air_stop"
 API_SP_AIR_VENT: Final[str] = "setpoint_air_vent"
 API_SPEED: Final[str] = "speed"
 API_STAT_AP_MAC: Final[str] = "stat_ap_mac"
@@ -70,14 +77,15 @@
 API_UNITS: Final[str] = "units"
 API_URL: Final[str] = "https://m.airzonecloud.com"
 API_USER: Final[str] = "user"
 API_USER_ID: Final[str] = "user_id"
 API_USER_LOGOUT: Final[str] = "user/logout"
 API_USER_MODE_CONF: Final[str] = "usermode_conf"
 API_V1: Final[str] = "api/v1"
+API_VALUE: Final[str] = "value"
 API_WARNINGS: Final[str] = "warnings"
 API_WS: Final[str] = "ws"
 API_WS_CONNECTED: Final[str] = "ws_connected"
 API_WS_FW: Final[str] = "ws_fw"
 API_WS_ID: Final[str] = "ws_id"
 API_WS_IDS: Final[str] = "ws_ids"
 API_WS_TYPE: Final[str] = "ws_type"
@@ -85,14 +93,16 @@
 
 API_AZ_AIDOO: Final[str] = "aidoo"
 API_AZ_SYSTEM: Final[str] = "az_system"
 API_AZ_ZONE: Final[str] = "az_zone"
 
 API_DEFAULT_TEMP_STEP: Final[float] = 0.5
 
+AZD_ACTION: Final[str] = "action"
+AZD_ACTIVE: Final[str] = "active"
 AZD_AIDOOS: Final[str] = "aidoos"
 AZD_AVAILABLE: Final[str] = "available"
 AZD_CONNECTION_DATE: Final[str] = "connection-date"
 AZD_DISCONNECTION_DATE: Final[str] = "disconnection-date"
 AZD_ERRORS: Final[str] = "errors"
 AZD_FIRMWARE: Final[str] = "firmware"
 AZD_HUMIDITY: Final[str] = "humidity"
@@ -108,26 +118,29 @@
 AZD_PROBLEMS: Final[str] = "problems"
 AZD_SYSTEM: Final[str] = "system"
 AZD_SYSTEM_ID: Final[str] = "system-id"
 AZD_SYSTEMS: Final[str] = "systems"
 AZD_TEMP: Final[str] = "temperature"
 AZD_TEMP_STEP: Final[str] = "temperature-step"
 AZD_TEMP_SET: Final[str] = "temperature-setpoint"
+AZD_TEMP_SET_AUTO_AIR: Final[str] = "temperature-setpoint-auto-air"
 AZD_TEMP_SET_COOL_AIR: Final[str] = "temperature-setpoint-cool-air"
 AZD_TEMP_SET_DRY_AIR: Final[str] = "temperature-setpoint-dry-air"
 AZD_TEMP_SET_HOT_AIR: Final[str] = "temperature-setpoint-hot-air"
 AZD_TEMP_SET_STOP_AIR: Final[str] = "temperature-setpoint-stop-air"
 AZD_TEMP_SET_VENT_AIR: Final[str] = "temperature-setpoint-vent-air"
 AZD_TEMP_SET_MAX: Final[str] = "temperature-setpoint-max"
+AZD_TEMP_SET_MAX_AUTO_AIR: Final[str] = "temperature-setpoint-max-auto-air"
 AZD_TEMP_SET_MAX_COOL_AIR: Final[str] = "temperature-setpoint-max-cool-air"
 AZD_TEMP_SET_MAX_DRY_AIR: Final[str] = "temperature-setpoint-max-dry-air"
 AZD_TEMP_SET_MAX_EMERHEAT_AIR: Final[str] = "temperature-setpoint-max-emerheat-air"
 AZD_TEMP_SET_MAX_HOT_AIR: Final[str] = "temperature-setpoint-max-hot-air"
 AZD_TEMP_SET_MAX_STOP_AIR: Final[str] = "temperature-setpoint-max-stop-air"
 AZD_TEMP_SET_MAX_VENT_AIR: Final[str] = "temperature-setpoint-max-vent-air"
+AZD_TEMP_SET_MIN_AUTO_AIR: Final[str] = "temperature-setpoint-min-auto-air"
 AZD_TEMP_SET_MIN_COOL_AIR: Final[str] = "temperature-setpoint-min-cool-air"
 AZD_TEMP_SET_MIN_DRY_AIR: Final[str] = "temperature-setpoint-min-dry-air"
 AZD_TEMP_SET_MIN_EMERHEAT_AIR: Final[str] = "temperature-setpoint-min-emerheat-air"
 AZD_TEMP_SET_MIN_HOT_AIR: Final[str] = "temperature-setpoint-min-hot-air"
 AZD_TEMP_SET_MIN_STOP_AIR: Final[str] = "temperature-setpoint-min-stop-air"
 AZD_TEMP_SET_MIN_VENT_AIR: Final[str] = "temperature-setpoint-min-vent-air"
 AZD_TEMP_SET_MIN: Final[str] = "temperature-setpoint-min"
```

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/device.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Airzone Cloud API Device."""
 from __future__ import annotations
 
+import logging
+from abc import ABC, abstractmethod
 from typing import Any
 
 from .common import OperationMode
 from .const import (
     API_DEVICE_ID,
     API_ERRORS,
     API_IS_CONNECTED,
@@ -22,16 +24,18 @@
     AZD_NAME,
     AZD_PROBLEMS,
     AZD_WARNINGS,
     AZD_WEBSERVER,
     AZD_WS_CONNECTED,
 )
 
+_LOGGER = logging.getLogger(__name__)
 
-class Device:
+
+class Device(ABC):
     """Airzone Cloud Device."""
 
     name: str
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
         """Airzone Cloud Device init."""
         self.errors: list[str] = []
@@ -123,14 +127,26 @@
         """Return WebServer ID."""
         return self.webserver_id
 
     def get_ws_connected(self) -> bool:
         """Return WebServer connection status."""
         return self.ws_connected
 
+    def set_mode(self, mode: int | OperationMode) -> None:
+        """Set device operation mode."""
+        _mode = OperationMode(mode)
+        if _mode in self.modes:
+            self.mode = _mode
+        else:
+            _LOGGER.error("%s: mode %s not in %s", self.id, _mode, self.modes)
+
+    @abstractmethod
+    def set_param(self, param: str, data: dict[str, Any]) -> None:
+        """Update device parameter from API request."""
+
     def update(self, data: dict[str, Any]) -> None:
         """Update Device data."""
         if API_IS_CONNECTED in data:
             self.is_connected = bool(data[API_IS_CONNECTED])
         if API_WS_CONNECTED in data:
             self.ws_connected = bool(data[API_WS_CONNECTED])
```

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/hvac.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/hvac.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 """Airzone Cloud API HVAC device."""
 from __future__ import annotations
 
 from typing import Any
 
+from .common import OperationAction, OperationMode
 from .const import (
+    API_ACTIVE,
     API_CELSIUS,
     API_DEFAULT_TEMP_STEP,
     API_HUMIDITY,
     API_LOCAL_TEMP,
     API_POWER,
+    API_RANGE_MAX_AIR,
+    API_RANGE_MIN_AIR,
+    API_RANGE_SP_MAX_AUTO_AIR,
     API_RANGE_SP_MAX_COOL_AIR,
     API_RANGE_SP_MAX_DRY_AIR,
     API_RANGE_SP_MAX_EMERHEAT_AIR,
     API_RANGE_SP_MAX_HOT_AIR,
     API_RANGE_SP_MAX_STOP_AIR,
     API_RANGE_SP_MAX_VENT_AIR,
+    API_RANGE_SP_MIN_AUTO_AIR,
     API_RANGE_SP_MIN_COOL_AIR,
     API_RANGE_SP_MIN_DRY_AIR,
     API_RANGE_SP_MIN_EMERHEAT_AIR,
     API_RANGE_SP_MIN_HOT_AIR,
     API_RANGE_SP_MIN_STOP_AIR,
     API_RANGE_SP_MIN_VENT_AIR,
     API_SP_AIR_COOL,
     API_SP_AIR_DRY,
     API_SP_AIR_HEAT,
     API_SP_AIR_STOP,
     API_SP_AIR_VENT,
     API_STEP,
+    AZD_ACTION,
+    AZD_ACTIVE,
     AZD_HUMIDITY,
     AZD_POWER,
     AZD_TEMP,
     AZD_TEMP_SET,
+    AZD_TEMP_SET_AUTO_AIR,
     AZD_TEMP_SET_COOL_AIR,
     AZD_TEMP_SET_DRY_AIR,
     AZD_TEMP_SET_HOT_AIR,
     AZD_TEMP_SET_MAX,
+    AZD_TEMP_SET_MAX_AUTO_AIR,
     AZD_TEMP_SET_MAX_COOL_AIR,
     AZD_TEMP_SET_MAX_DRY_AIR,
     AZD_TEMP_SET_MAX_EMERHEAT_AIR,
     AZD_TEMP_SET_MAX_HOT_AIR,
     AZD_TEMP_SET_MAX_STOP_AIR,
     AZD_TEMP_SET_MAX_VENT_AIR,
     AZD_TEMP_SET_MIN,
+    AZD_TEMP_SET_MIN_AUTO_AIR,
     AZD_TEMP_SET_MIN_COOL_AIR,
     AZD_TEMP_SET_MIN_DRY_AIR,
     AZD_TEMP_SET_MIN_EMERHEAT_AIR,
     AZD_TEMP_SET_MIN_HOT_AIR,
     AZD_TEMP_SET_MIN_STOP_AIR,
     AZD_TEMP_SET_MIN_VENT_AIR,
     AZD_TEMP_SET_STOP_AIR,
@@ -58,52 +69,63 @@
 class HVAC(Device):
     """Airzone Cloud HVAC device."""
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
         """Airzone Cloud HVAC device init."""
         super().__init__(inst_id, ws_id, device_data)
 
+        self.active: bool | None = None
         self.humidity: int | None = None
         self.name: str = "HVAC"
         self.power: bool | None = None
+        self.temp_set_max: float | None = None
+        self.temp_set_max_auto_air: float | None = None
         self.temp_set_max_cool_air: float | None = None
         self.temp_set_max_dry_air: float | None = None
         self.temp_set_max_emerheat_air: float | None = None
         self.temp_set_max_hot_air: float | None = None
         self.temp_set_max_stop_air: float | None = None
         self.temp_set_max_vent_air: float | None = None
+        self.temp_set_min: float | None = None
+        self.temp_set_min_auto_air: float | None = None
         self.temp_set_min_cool_air: float | None = None
         self.temp_set_min_dry_air: float | None = None
         self.temp_set_min_emerheat_air: float | None = None
         self.temp_set_min_hot_air: float | None = None
         self.temp_set_min_stop_air: float | None = None
         self.temp_set_min_vent_air: float | None = None
+        self.temp_set_auto_air: float | None = None
         self.temp_set_cool_air: float | None = None
         self.temp_set_dry_air: float | None = None
         self.temp_set_hot_air: float | None = None
         self.temp_set_stop_air: float | None = None
         self.temp_set_vent_air: float | None = None
         self.temp: float | None = None
         self.temp_step: float | None = None
 
     def data(self) -> dict[str, Any]:
         """Return HVAC device data."""
         data = super().data()
 
+        data[AZD_ACTION] = self.get_action()
+        data[AZD_ACTIVE] = self.get_active()
         data[AZD_POWER] = self.get_power()
         data[AZD_TEMP] = self.get_temperature()
         data[AZD_TEMP_STEP] = self.get_temp_step()
 
         humidity = self.get_humidity()
         if humidity is not None:
             data[AZD_HUMIDITY] = humidity
 
         temp_set_max = self.get_temp_set_max()
         if temp_set_max is not None:
             data[AZD_TEMP_SET_MAX] = temp_set_max
+        temp_set_max_auto_air = self.get_temp_set_max_auto_air()
+        if temp_set_max_auto_air is not None:
+            data[AZD_TEMP_SET_MAX_AUTO_AIR] = temp_set_max_auto_air
         temp_set_max_cool_air = self.get_temp_set_max_cool_air()
         if temp_set_max_cool_air is not None:
             data[AZD_TEMP_SET_MAX_COOL_AIR] = temp_set_max_cool_air
         temp_set_max_dry_air = self.get_temp_set_max_dry_air()
         if temp_set_max_dry_air is not None:
             data[AZD_TEMP_SET_MAX_DRY_AIR] = temp_set_max_dry_air
         temp_set_max_emerheat_air = self.get_temp_set_max_emerheat_air()
@@ -118,14 +140,17 @@
         temp_set_max_vent_air = self.get_temp_set_max_vent_air()
         if temp_set_max_vent_air is not None:
             data[AZD_TEMP_SET_MAX_VENT_AIR] = temp_set_max_vent_air
 
         temp_set_min = self.get_temp_set_min()
         if temp_set_min is not None:
             data[AZD_TEMP_SET_MIN] = temp_set_min
+        temp_set_min_auto_air = self.get_temp_set_min_auto_air()
+        if temp_set_min_auto_air is not None:
+            data[AZD_TEMP_SET_MIN_AUTO_AIR] = temp_set_min_auto_air
         temp_set_min_cool_air = self.get_temp_set_min_cool_air()
         if temp_set_min_cool_air is not None:
             data[AZD_TEMP_SET_MIN_COOL_AIR] = temp_set_min_cool_air
         temp_set_min_dry_air = self.get_temp_set_min_dry_air()
         if temp_set_min_dry_air is not None:
             data[AZD_TEMP_SET_MIN_DRY_AIR] = temp_set_min_dry_air
         temp_set_min_emerheat_air = self.get_temp_set_min_emerheat_air()
@@ -140,14 +165,17 @@
         temp_set_min_vent_air = self.get_temp_set_min_vent_air()
         if temp_set_min_vent_air is not None:
             data[AZD_TEMP_SET_MIN_VENT_AIR] = temp_set_min_vent_air
 
         temp_set = self.get_temp_set()
         if temp_set is not None:
             data[AZD_TEMP_SET] = temp_set
+        temp_set_auto_air = self.get_temp_set_auto_air()
+        if temp_set_auto_air is not None:
+            data[AZD_TEMP_SET_AUTO_AIR] = temp_set_auto_air
         temp_set_cool_air = self.get_temp_set_cool_air()
         if temp_set_cool_air is not None:
             data[AZD_TEMP_SET_COOL_AIR] = temp_set_cool_air
         temp_set_dry_air = self.get_temp_set_dry_air()
         if temp_set_dry_air is not None:
             data[AZD_TEMP_SET_DRY_AIR] = temp_set_dry_air
         temp_set_hot_air = self.get_temp_set_hot_air()
@@ -158,14 +186,80 @@
             data[AZD_TEMP_SET_STOP_AIR] = temp_set_stop_air
         temp_set_vent_air = self.get_temp_set_vent_air()
         if temp_set_vent_air is not None:
             data[AZD_TEMP_SET_VENT_AIR] = temp_set_vent_air
 
         return data
 
+    def get_action(self) -> OperationAction:
+        """Return HVAC action."""
+
+        if self.get_power():
+            if self.get_active():
+                mode = self.get_mode() or OperationMode.STOP
+                if mode.is_cool():
+                    action = OperationAction.COOLING
+                elif mode.is_heat():
+                    action = OperationAction.HEATING
+                elif mode.is_vent():
+                    action = OperationAction.FAN
+                elif mode.is_dry():
+                    action = OperationAction.DRYING
+                elif mode.is_auto():
+                    action = self.get_auto_mode()
+                else:
+                    action = OperationAction.OFF
+            else:
+                action = OperationAction.IDLE
+        else:
+            action = OperationAction.OFF
+
+        return action
+
+    def get_active(self) -> bool | None:
+        """Return HVAC device active status."""
+        return self.active
+
+    def get_auto_mode(self) -> OperationAction:
+        """Return action from auto mode."""
+        temp_sp = self.get_temp_set()
+        temp_min = self.temp_set_min
+        temp_max = self.temp_set_max
+        cool_sp = self.get_temp_set_cool_air()
+        cool_max = self.get_temp_set_max_cool_air()
+        cool_min = self.get_temp_set_min_cool_air()
+        heat_sp = self.get_temp_set_hot_air()
+        heat_max = self.get_temp_set_max_hot_air()
+        heat_min = self.get_temp_set_min_hot_air()
+
+        if (
+            cool_max is not None
+            and cool_min is not None
+            and heat_max is not None
+            and heat_min is not None
+        ):
+            cool_match = cool_max == temp_max and cool_min == temp_min
+            heat_match = heat_max == temp_max and heat_min == temp_min
+
+            if cool_match and not heat_match:
+                return OperationAction.COOLING
+            if heat_match and not cool_match:
+                return OperationAction.HEATING
+
+        if cool_sp is not None and heat_sp is not None:
+            cool_match = cool_sp == temp_sp
+            heat_match = heat_sp == temp_sp
+
+            if cool_match and not heat_match:
+                return OperationAction.COOLING
+            if heat_match and not cool_match:
+                return OperationAction.HEATING
+
+        return OperationAction.IDLE
+
     def get_humidity(self) -> int | None:
         """Return HVAC device humidity."""
         return self.humidity
 
     def get_power(self) -> bool | None:
         """Return HVAC device power."""
         return self.power
@@ -177,26 +271,34 @@
         return None
 
     def get_temp_set(self) -> float | None:
         """Return HVAC device temperature setpoint."""
         temp_set: float | None = None
         mode = self.get_mode()
         if mode is not None:
-            if mode.is_cool():
+            if mode.is_auto():
+                temp_set = self.get_temp_set_auto_air()
+            elif mode.is_cool():
                 temp_set = self.get_temp_set_cool_air()
             elif mode.is_dry():
                 temp_set = self.get_temp_set_dry_air()
             elif mode.is_heat():
                 temp_set = self.get_temp_set_hot_air()
             elif mode.is_stop():
                 temp_set = self.get_temp_set_stop_air()
             elif mode.is_vent():
                 temp_set = self.get_temp_set_vent_air()
         return temp_set
 
+    def get_temp_set_auto_air(self) -> float | None:
+        """Return HVAC device setpoint for Auto Air."""
+        if self.temp_set_auto_air is not None:
+            return round(self.temp_set_auto_air, 1)
+        return None
+
     def get_temp_set_cool_air(self) -> float | None:
         """Return HVAC device setpoint for Cool Air."""
         if self.temp_set_cool_air is not None:
             return round(self.temp_set_cool_air, 1)
         return None
 
     def get_temp_set_dry_air(self) -> float | None:
@@ -223,27 +325,35 @@
             return round(self.temp_set_vent_air, 1)
         return None
 
     def get_temp_set_max(self) -> float | None:
         """Return HVAC device max setpoint."""
         max_temp: float | None = None
         temps = [
+            self.temp_set_max,
+            self.get_temp_set_max_auto_air(),
             self.get_temp_set_max_cool_air(),
             self.get_temp_set_max_dry_air(),
             self.get_temp_set_max_emerheat_air(),
             self.get_temp_set_max_hot_air(),
             self.get_temp_set_max_stop_air(),
             self.get_temp_set_max_vent_air(),
         ]
         for temp in temps:
             if temp is not None:
                 if max_temp is None or temp > max_temp:
                     max_temp = temp
         return max_temp
 
+    def get_temp_set_max_auto_air(self) -> float | None:
+        """Return HVAC device max setpoint for Auto Air."""
+        if self.temp_set_max_auto_air is not None:
+            return round(self.temp_set_max_auto_air, 1)
+        return None
+
     def get_temp_set_max_cool_air(self) -> float | None:
         """Return HVAC device max setpoint for Cool Air."""
         if self.temp_set_max_cool_air is not None:
             return round(self.temp_set_max_cool_air, 1)
         return None
 
     def get_temp_set_max_dry_air(self) -> float | None:
@@ -276,27 +386,35 @@
             return round(self.temp_set_max_vent_air, 1)
         return None
 
     def get_temp_set_min(self) -> float | None:
         """Return HVAC device min setpoint."""
         min_temp: float | None = None
         temps = [
+            self.temp_set_min,
+            self.get_temp_set_min_auto_air(),
             self.get_temp_set_min_cool_air(),
             self.get_temp_set_min_dry_air(),
             self.get_temp_set_min_emerheat_air(),
             self.get_temp_set_min_hot_air(),
             self.get_temp_set_min_stop_air(),
             self.get_temp_set_min_vent_air(),
         ]
         for temp in temps:
             if temp is not None:
                 if min_temp is None or temp < min_temp:
                     min_temp = temp
         return min_temp
 
+    def get_temp_set_min_auto_air(self) -> float | None:
+        """Return HVAC device min setpoint for Auto Air."""
+        if self.temp_set_min_auto_air:
+            return round(self.temp_set_min_auto_air, 1)
+        return None
+
     def get_temp_set_min_cool_air(self) -> float | None:
         """Return HVAC device min setpoint for Cool Air."""
         if self.temp_set_min_cool_air:
             return round(self.temp_set_min_cool_air, 1)
         return None
 
     def get_temp_set_min_dry_air(self) -> float | None:
@@ -331,28 +449,58 @@
 
     def get_temp_step(self) -> float | None:
         """Return HVAC device temperature step."""
         if self.temp_step is not None:
             return round(self.temp_step, 1)
         return API_DEFAULT_TEMP_STEP
 
+    def set_power(self, power: bool) -> None:
+        """Set HVAC power."""
+        self.power = power
+
+    def set_setpoint(self, setpoint: float) -> None:
+        """Set HVAC setpoint."""
+        if self.temp_set_auto_air is not None:
+            self.temp_set_auto_air = setpoint
+        if self.temp_set_cool_air is not None:
+            self.temp_set_cool_air = setpoint
+        if self.temp_set_dry_air is not None:
+            self.temp_set_dry_air = setpoint
+        if self.temp_set_hot_air is not None:
+            self.temp_set_hot_air = setpoint
+        if self.temp_set_stop_air is not None:
+            self.temp_set_stop_air = setpoint
+        if self.temp_set_vent_air is not None:
+            self.temp_set_vent_air = setpoint
+
     def update(self, data: dict[str, Any]) -> None:
         """Update HVAC device data."""
         super().update(data)
 
+        if API_ACTIVE in data:
+            self.active = bool(data[API_ACTIVE])
+
         if API_HUMIDITY in data:
             self.humidity = int(data[API_HUMIDITY])
 
         if API_LOCAL_TEMP in data:
             if API_CELSIUS in data[API_LOCAL_TEMP]:
                 self.temp = float(data[API_LOCAL_TEMP][API_CELSIUS])
 
         if API_POWER in data:
             self.power = bool(data[API_POWER])
 
+        if API_RANGE_MAX_AIR in data:
+            if API_CELSIUS in data[API_RANGE_MAX_AIR]:
+                self.temp_set_max = float(data[API_RANGE_MAX_AIR][API_CELSIUS])
+        if API_RANGE_SP_MAX_AUTO_AIR in data:
+            if API_CELSIUS in data[API_RANGE_SP_MAX_AUTO_AIR]:
+                self.temp_set_max_auto_air = float(
+                    data[API_RANGE_SP_MAX_AUTO_AIR][API_CELSIUS]
+                )
         if API_RANGE_SP_MAX_COOL_AIR in data:
             if API_CELSIUS in data[API_RANGE_SP_MAX_COOL_AIR]:
                 self.temp_set_max_cool_air = float(
                     data[API_RANGE_SP_MAX_COOL_AIR][API_CELSIUS]
                 )
         if API_RANGE_SP_MAX_DRY_AIR in data:
             if API_CELSIUS in data[API_RANGE_SP_MAX_DRY_AIR]:
@@ -376,14 +524,22 @@
                 )
         if API_RANGE_SP_MAX_VENT_AIR in data:
             if API_CELSIUS in data[API_RANGE_SP_MAX_VENT_AIR]:
                 self.temp_set_max_vent_air = float(
                     data[API_RANGE_SP_MAX_VENT_AIR][API_CELSIUS]
                 )
 
+        if API_RANGE_MIN_AIR in data:
+            if API_CELSIUS in data[API_RANGE_MIN_AIR]:
+                self.temp_set_min = float(data[API_RANGE_MIN_AIR][API_CELSIUS])
+        if API_RANGE_SP_MIN_AUTO_AIR in data:
+            if API_CELSIUS in data[API_RANGE_SP_MIN_AUTO_AIR]:
+                self.temp_set_min_auto_air = float(
+                    data[API_RANGE_SP_MIN_AUTO_AIR][API_CELSIUS]
+                )
         if API_RANGE_SP_MIN_COOL_AIR in data:
             if API_CELSIUS in data[API_RANGE_SP_MIN_COOL_AIR]:
                 self.temp_set_min_cool_air = float(
                     data[API_RANGE_SP_MIN_COOL_AIR][API_CELSIUS]
                 )
         if API_RANGE_SP_MIN_DRY_AIR in data:
             if API_CELSIUS in data[API_RANGE_SP_MIN_DRY_AIR]:
```

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/system.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/aidoo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-"""Airzone Cloud API System."""
+"""Airzone Cloud API Aidoo device."""
 from __future__ import annotations
 
 from typing import Any
 
-from .const import API_CONFIG, API_META, API_SYSTEM_NUMBER, AZD_SYSTEM
-from .device import Device
+from .const import API_MODE, API_NAME, API_POWER, API_SETPOINT, API_VALUE
+from .hvac import HVAC
 
 
-class System(Device):
-    """Airzone Cloud System device."""
+class Aidoo(HVAC):
+    """Airzone Cloud Aidoo device."""
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
-        """Airzone Cloud System device init."""
+        """Airzone Cloud Aidoo device init."""
         super().__init__(inst_id, ws_id, device_data)
 
-        if API_CONFIG in device_data:
-            sub_data = device_data[API_CONFIG]
+        if API_NAME in device_data:
+            self.name = str(device_data[API_NAME])
         else:
-            sub_data = device_data[API_META]
+            self.name = f"Aidoo {ws_id}"
 
-        self.system_number = int(sub_data[API_SYSTEM_NUMBER])
+    def set_param(self, param: str, data: dict[str, Any]) -> None:
+        """Update device parameter from API request."""
 
-        self.name = f"System {self.system_number}"
-
-    def data(self) -> dict[str, Any]:
-        """Return System device data."""
-        data = super().data()
-
-        data[AZD_SYSTEM] = self.get_system()
-
-        return data
-
-    def get_system(self) -> int:
-        """Return System number."""
-        return self.system_number
+        if param == API_MODE:
+            self.set_mode(data[API_VALUE])
+        elif param == API_POWER:
+            self.set_power(data[API_VALUE])
+        elif param == API_SETPOINT:
+            self.set_setpoint(data[API_VALUE])
```

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.2.0/aioairzone_cloud/zone.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 """Airzone Cloud API Zone device."""
 from __future__ import annotations
 
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from aioairzone_cloud.common import OperationMode
 
 from .const import (
     API_CONFIG,
     API_META,
+    API_MODE,
     API_MODE_AVAIL,
     API_NAME,
+    API_POWER,
+    API_SETPOINT,
     API_SYSTEM_NUMBER,
+    API_VALUE,
     API_ZONE_NUMBER,
     AZD_MASTER,
     AZD_SYSTEM,
     AZD_SYSTEM_ID,
     AZD_ZONE,
 )
 from .hvac import HVAC
 
+if TYPE_CHECKING:
+    from .system import System
+
 
 class Zone(HVAC):
     """Airzone Cloud Zone device."""
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
         """Airzone Cloud Zone device init."""
         super().__init__(inst_id, ws_id, device_data)
 
         self.master: bool | None = None
-        self.system_id: str | None = None
+        self.system: System | None = None
 
         if API_CONFIG in device_data:
             sub_data = device_data[API_CONFIG]
         else:
             sub_data = device_data[API_META]
 
         self.system_number = int(sub_data[API_SYSTEM_NUMBER])
@@ -44,46 +51,61 @@
             self.name = f"Zone {self.system_number}:{self.zone_number}"
 
     def data(self) -> dict[str, Any]:
         """Return Zone data."""
         data = super().data()
 
         data[AZD_MASTER] = self.get_master()
-        data[AZD_SYSTEM] = self.get_system()
+        data[AZD_SYSTEM] = self.get_system_num()
         data[AZD_ZONE] = self.get_zone()
 
         system_id = self.get_system_id()
         if system_id is not None:
             data[AZD_SYSTEM_ID] = system_id
 
         return data
 
     def get_master(self) -> bool | None:
         """Return Zone device master/slave."""
         return self.master
 
-    def get_system(self) -> int:
-        """Return System number."""
-        return self.system_number
-
     def get_system_id(self) -> str | None:
         """Return Zone device System ID."""
-        return self.system_id
+        if self.system is not None:
+            return self.system.get_id()
+        return None
+
+    def get_system_num(self) -> int:
+        """Return System number."""
+        return self.system_number
 
     def get_zone(self) -> int:
         """Return Zone number."""
         return self.zone_number
 
     def set_modes(self, modes: list[OperationMode]) -> None:
         """Set slave zone modes."""
         self.modes = modes
 
-    def set_system_id(self, system_id: str) -> None:
-        """Set System ID."""
-        self.system_id = system_id
+    def set_param(self, param: str, data: dict[str, Any]) -> None:
+        """Update device parameter from API request."""
+
+        if param == API_MODE:
+            if self.system is not None:
+                self.system.set_param(param, data)
+            else:
+                self.set_mode(data[API_VALUE])
+        elif param == API_POWER:
+            self.set_power(data[API_VALUE])
+        elif param == API_SETPOINT:
+            self.set_setpoint(data[API_VALUE])
+
+    def set_system(self, system: System) -> None:
+        """Set System."""
+        self.system = system
 
     def update(self, data: dict[str, Any]) -> None:
         """Update Zone data."""
         super().update(data)
 
         if API_MODE_AVAIL in data:
             self.master = len(data[API_MODE_AVAIL]) > 0
```

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.9
+Version: 0.2.0
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.9/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.9/pyproject.toml` & `aioairzone-cloud-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.1.9"
+version = "0.2.0"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

