# Comparing `tmp/aiomagra-0.1.2.tar.gz` & `tmp/aiomagra-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomagra-0.1.2.tar", max compression
+gzip compressed data, was "aiomagra-0.2.0.tar", max compression
```

## Comparing `aiomagra-0.1.2.tar` & `aiomagra-0.2.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0       12 2023-06-25 13:29:06.484907 aiomagra-0.1.2/README.md
--rw-r--r--   0        0        0      281 2023-06-25 14:20:33.712395 aiomagra-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       39 2023-06-25 13:29:06.474907 aiomagra-0.1.2/src/aiomagra/__init__.py
--rw-r--r--   0        0        0      366 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/accelerometer.proto
--rw-r--r--   0        0        0     1622 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/accelerometer_pb2.py
--rw-r--r--   0        0        0      745 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/addon.proto
--rw-r--r--   0        0        0     2466 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/addon_pb2.py
--rw-r--r--   0        0        0      566 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/admin.proto
--rw-r--r--   0        0        0     1930 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/admin_pb2.py
--rw-r--r--   0        0        0      460 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/battery.proto
--rw-r--r--   0        0        0     1779 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/battery_pb2.py
--rw-r--r--   0        0        0      417 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/ble.proto
--rw-r--r--   0        0        0     1563 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/ble_pb2.py
--rw-r--r--   0        0        0      507 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/bsensor.proto
--rw-r--r--   0        0        0     1926 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/bsensor_pb2.py
--rw-r--r--   0        0        0      894 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/carbon_dioxide.proto
--rw-r--r--   0        0        0     2422 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/carbon_dioxide_pb2.py
--rw-r--r--   0        0        0     1326 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/carbon_monoxide.proto
--rw-r--r--   0        0        0     3571 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/carbon_monoxide_pb2.py
--rw-r--r--   0        0        0     5204 2023-06-25 13:29:06.474907 aiomagra-0.1.2/src/aiomagra/client.py
--rw-r--r--   0        0        0      778 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/color.proto
--rw-r--r--   0        0        0     2500 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/color_pb2.py
--rw-r--r--   0        0        0     2116 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/configuration.proto
--rw-r--r--   0        0        0     4919 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/configuration_pb2.py
--rw-r--r--   0        0        0       79 2023-06-25 13:29:06.474907 aiomagra-0.1.2/src/aiomagra/const.py
--rw-r--r--   0        0        0     3883 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/devices.proto
--rw-r--r--   0        0        0    10693 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/devices_pb2.py
--rw-r--r--   0        0        0      327 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/door.proto
--rw-r--r--   0        0        0     1389 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/door_pb2.py
--rw-r--r--   0        0        0      276 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/doorbell.proto
--rw-r--r--   0        0        0     1379 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/doorbell_pb2.py
--rw-r--r--   0        0        0      329 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/emergency.proto
--rw-r--r--   0        0        0     1425 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/emergency_pb2.py
--rw-r--r--   0        0        0     1349 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/firmware.proto
--rw-r--r--   0        0        0     3640 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/firmware_pb2.py
--rw-r--r--   0        0        0      272 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/flood.proto
--rw-r--r--   0        0        0     1347 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/flood_pb2.py
--rw-r--r--   0        0        0      622 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/gate.proto
--rw-r--r--   0        0        0     2079 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/gate_pb2.py
--rw-r--r--   0        0        0      617 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/gateway.proto
--rw-r--r--   0        0        0     2115 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/gateway_pb2.py
--rw-r--r--   0        0        0      300 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/heartbeat.proto
--rw-r--r--   0        0        0     1319 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/heartbeat_pb2.py
--rw-r--r--   0        0        0      424 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/info.proto
--rw-r--r--   0        0        0     1560 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/info_pb2.py
--rw-r--r--   0        0        0     1080 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/level.proto
--rw-r--r--   0        0        0     2991 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/level_pb2.py
--rw-r--r--   0        0        0      639 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/lock.proto
--rw-r--r--   0        0        0     2121 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/lock_pb2.py
--rw-r--r--   0        0        0      405 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/messaging.proto
--rw-r--r--   0        0        0     1525 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/messaging_pb2.py
--rw-r--r--   0        0        0      678 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/metadata.proto
--rw-r--r--   0        0        0     2316 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/metadata_pb2.py
--rw-r--r--   0        0        0      689 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/meter.proto
--rw-r--r--   0        0        0     2384 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/meter_pb2.py
--rw-r--r--   0        0        0      303 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/mqtt.proto
--rw-r--r--   0        0        0     1338 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/mqtt_pb2.py
--rw-r--r--   0        0        0      647 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/power_source.proto
--rw-r--r--   0        0        0     1974 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/power_source_pb2.py
--rw-r--r--   0        0        0    11060 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/pubsub.proto
--rw-r--r--   0        0        0    20652 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/pubsub_pb2.py
--rw-r--r--   0        0        0      622 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/remote.proto
--rw-r--r--   0        0        0     2160 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/remote_pb2.py
--rw-r--r--   0        0        0     3457 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/reports.proto
--rw-r--r--   0        0        0     8944 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/reports_pb2.py
--rw-r--r--   0        0        0      724 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/roller_shutter.proto
--rw-r--r--   0        0        0     2280 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/roller_shutter_pb2.py
--rw-r--r--   0        0        0      357 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/seismic.proto
--rw-r--r--   0        0        0     1558 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/seismic_pb2.py
--rw-r--r--   0        0        0      410 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/sensor.proto
--rw-r--r--   0        0        0     1719 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/sensor_pb2.py
--rw-r--r--   0        0        0     2040 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/siren.proto
--rw-r--r--   0        0        0     5557 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/siren_pb2.py
--rw-r--r--   0        0        0      827 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/smoke.proto
--rw-r--r--   0        0        0     2290 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/smoke_pb2.py
--rw-r--r--   0        0        0      510 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/status.proto
--rw-r--r--   0        0        0     1868 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/status_pb2.py
--rw-r--r--   0        0        0      574 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/structure.proto
--rw-r--r--   0        0        0     1975 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/structure_pb2.py
--rw-r--r--   0        0        0      562 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/switch.proto
--rw-r--r--   0        0        0     1985 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/switch_pb2.py
--rw-r--r--   0        0        0      327 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/tamper.proto
--rw-r--r--   0        0        0     1394 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/tamper_pb2.py
--rw-r--r--   0        0        0      222 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/taptap.proto
--rw-r--r--   0        0        0     1162 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/taptap_pb2.py
--rw-r--r--   0        0        0      575 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/temperature.proto
--rw-r--r--   0        0        0     2078 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/temperature_pb2.py
--rw-r--r--   0        0        0     2051 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/thermostat.proto
--rw-r--r--   0        0        0     5292 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/thermostat_pb2.py
--rw-r--r--   0        0        0      562 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/ultraviolet.proto
--rw-r--r--   0        0        0     2057 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/ultraviolet_pb2.py
--rw-r--r--   0        0        0     8927 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/units.proto
--rw-r--r--   0        0        0     1693 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/units_pb2.py
--rw-r--r--   0        0        0      390 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/websocket.proto
--rw-r--r--   0        0        0     1586 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/websocket_pb2.py
--rw-r--r--   0        0        0     1130 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/wifi.proto
--rw-r--r--   0        0        0     3178 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/wifi_pb2.py
--rw-r--r--   0        0        0      909 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/zigbee.proto
--rw-r--r--   0        0        0     2769 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/zigbee_pb2.py
--rw-r--r--   0        0        0     6499 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/zwave.proto
--rw-r--r--   0        0        0    16023 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/zwave_pb2.py
--rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 aiomagra-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-06-25 13:29:06.484907 aiomagra-0.2.0/README.md
+-rw-r--r--   0        0        0      281 2023-06-27 15:34:01.324446 aiomagra-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-06-25 13:29:06.474907 aiomagra-0.2.0/src/aiomagra/__init__.py
+-rw-r--r--   0        0        0      366 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/accelerometer.proto
+-rw-r--r--   0        0        0     1622 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/accelerometer_pb2.py
+-rw-r--r--   0        0        0      745 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/addon.proto
+-rw-r--r--   0        0        0     2466 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/addon_pb2.py
+-rw-r--r--   0        0        0      566 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/admin.proto
+-rw-r--r--   0        0        0     1930 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/admin_pb2.py
+-rw-r--r--   0        0        0      460 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/battery.proto
+-rw-r--r--   0        0        0     1779 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/battery_pb2.py
+-rw-r--r--   0        0        0      417 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/ble.proto
+-rw-r--r--   0        0        0     1563 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/ble_pb2.py
+-rw-r--r--   0        0        0      507 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/bsensor.proto
+-rw-r--r--   0        0        0     1926 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/bsensor_pb2.py
+-rw-r--r--   0        0        0      894 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/carbon_dioxide.proto
+-rw-r--r--   0        0        0     2422 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/carbon_dioxide_pb2.py
+-rw-r--r--   0        0        0     1326 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/carbon_monoxide.proto
+-rw-r--r--   0        0        0     3571 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/carbon_monoxide_pb2.py
+-rw-r--r--   0        0        0     5209 2023-06-27 15:33:08.840877 aiomagra-0.2.0/src/aiomagra/client.py
+-rw-r--r--   0        0        0      778 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/color.proto
+-rw-r--r--   0        0        0     2500 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/color_pb2.py
+-rw-r--r--   0        0        0     2116 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/configuration.proto
+-rw-r--r--   0        0        0     4919 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/configuration_pb2.py
+-rw-r--r--   0        0        0       79 2023-06-25 13:29:06.474907 aiomagra-0.2.0/src/aiomagra/const.py
+-rw-r--r--   0        0        0     3883 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/devices.proto
+-rw-r--r--   0        0        0    10693 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/devices_pb2.py
+-rw-r--r--   0        0        0      327 2023-06-25 14:21:13.962522 aiomagra-0.2.0/src/aiomagra/door.proto
+-rw-r--r--   0        0        0     1389 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/door_pb2.py
+-rw-r--r--   0        0        0      276 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/doorbell.proto
+-rw-r--r--   0        0        0     1379 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/doorbell_pb2.py
+-rw-r--r--   0        0        0      329 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/emergency.proto
+-rw-r--r--   0        0        0     1425 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/emergency_pb2.py
+-rw-r--r--   0        0        0     1349 2023-06-25 14:21:13.962522 aiomagra-0.2.0/src/aiomagra/firmware.proto
+-rw-r--r--   0        0        0     3640 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/firmware_pb2.py
+-rw-r--r--   0        0        0      272 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/flood.proto
+-rw-r--r--   0        0        0     1347 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/flood_pb2.py
+-rw-r--r--   0        0        0      622 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/gate.proto
+-rw-r--r--   0        0        0     2079 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/gate_pb2.py
+-rw-r--r--   0        0        0      617 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/gateway.proto
+-rw-r--r--   0        0        0     2115 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/gateway_pb2.py
+-rw-r--r--   0        0        0      300 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/heartbeat.proto
+-rw-r--r--   0        0        0     1319 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/heartbeat_pb2.py
+-rw-r--r--   0        0        0      424 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/info.proto
+-rw-r--r--   0        0        0     1560 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/info_pb2.py
+-rw-r--r--   0        0        0     1080 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/level.proto
+-rw-r--r--   0        0        0     2991 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/level_pb2.py
+-rw-r--r--   0        0        0      639 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/lock.proto
+-rw-r--r--   0        0        0     2121 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/lock_pb2.py
+-rw-r--r--   0        0        0      405 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/messaging.proto
+-rw-r--r--   0        0        0     1525 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/messaging_pb2.py
+-rw-r--r--   0        0        0      678 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/metadata.proto
+-rw-r--r--   0        0        0     2316 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/metadata_pb2.py
+-rw-r--r--   0        0        0      689 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/meter.proto
+-rw-r--r--   0        0        0     2384 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/meter_pb2.py
+-rw-r--r--   0        0        0      303 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/mqtt.proto
+-rw-r--r--   0        0        0     1338 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/mqtt_pb2.py
+-rw-r--r--   0        0        0      647 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/power_source.proto
+-rw-r--r--   0        0        0     1974 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/power_source_pb2.py
+-rw-r--r--   0        0        0    11060 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/pubsub.proto
+-rw-r--r--   0        0        0    20652 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/pubsub_pb2.py
+-rw-r--r--   0        0        0      622 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/remote.proto
+-rw-r--r--   0        0        0     2160 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/remote_pb2.py
+-rw-r--r--   0        0        0     3457 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/reports.proto
+-rw-r--r--   0        0        0     8944 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/reports_pb2.py
+-rw-r--r--   0        0        0      724 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/roller_shutter.proto
+-rw-r--r--   0        0        0     2280 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/roller_shutter_pb2.py
+-rw-r--r--   0        0        0      357 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/seismic.proto
+-rw-r--r--   0        0        0     1558 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/seismic_pb2.py
+-rw-r--r--   0        0        0      410 2023-06-25 14:21:13.962522 aiomagra-0.2.0/src/aiomagra/sensor.proto
+-rw-r--r--   0        0        0     1719 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/sensor_pb2.py
+-rw-r--r--   0        0        0     2040 2023-06-25 14:21:13.962522 aiomagra-0.2.0/src/aiomagra/siren.proto
+-rw-r--r--   0        0        0     5557 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/siren_pb2.py
+-rw-r--r--   0        0        0      827 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/smoke.proto
+-rw-r--r--   0        0        0     2290 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/smoke_pb2.py
+-rw-r--r--   0        0        0      510 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/status.proto
+-rw-r--r--   0        0        0     1868 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/status_pb2.py
+-rw-r--r--   0        0        0      574 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/structure.proto
+-rw-r--r--   0        0        0     1975 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/structure_pb2.py
+-rw-r--r--   0        0        0      562 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/switch.proto
+-rw-r--r--   0        0        0     1985 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/switch_pb2.py
+-rw-r--r--   0        0        0      327 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/tamper.proto
+-rw-r--r--   0        0        0     1394 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/tamper_pb2.py
+-rw-r--r--   0        0        0      222 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/taptap.proto
+-rw-r--r--   0        0        0     1162 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/taptap_pb2.py
+-rw-r--r--   0        0        0      575 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/temperature.proto
+-rw-r--r--   0        0        0     2078 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/temperature_pb2.py
+-rw-r--r--   0        0        0     2051 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/thermostat.proto
+-rw-r--r--   0        0        0     5292 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/thermostat_pb2.py
+-rw-r--r--   0        0        0      562 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/ultraviolet.proto
+-rw-r--r--   0        0        0     2057 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/ultraviolet_pb2.py
+-rw-r--r--   0        0        0     8927 2023-06-25 14:21:13.962522 aiomagra-0.2.0/src/aiomagra/units.proto
+-rw-r--r--   0        0        0     1693 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/units_pb2.py
+-rw-r--r--   0        0        0      390 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/websocket.proto
+-rw-r--r--   0        0        0     1586 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/websocket_pb2.py
+-rw-r--r--   0        0        0     1130 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/wifi.proto
+-rw-r--r--   0        0        0     3178 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/wifi_pb2.py
+-rw-r--r--   0        0        0      909 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/zigbee.proto
+-rw-r--r--   0        0        0     2769 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/zigbee_pb2.py
+-rw-r--r--   0        0        0     6499 2023-06-25 14:21:13.965855 aiomagra-0.2.0/src/aiomagra/zwave.proto
+-rw-r--r--   0        0        0    16023 2023-06-25 14:21:13.982522 aiomagra-0.2.0/src/aiomagra/zwave_pb2.py
+-rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 aiomagra-0.2.0/PKG-INFO
```

### Comparing `aiomagra-0.1.2/src/aiomagra/accelerometer_pb2.py` & `aiomagra-0.2.0/src/aiomagra/accelerometer_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/addon.proto` & `aiomagra-0.2.0/src/aiomagra/addon.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/addon_pb2.py` & `aiomagra-0.2.0/src/aiomagra/addon_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/admin.proto` & `aiomagra-0.2.0/src/aiomagra/admin.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/admin_pb2.py` & `aiomagra-0.2.0/src/aiomagra/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/battery_pb2.py` & `aiomagra-0.2.0/src/aiomagra/battery_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/ble_pb2.py` & `aiomagra-0.2.0/src/aiomagra/ble_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/bsensor_pb2.py` & `aiomagra-0.2.0/src/aiomagra/bsensor_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/carbon_dioxide.proto` & `aiomagra-0.2.0/src/aiomagra/carbon_dioxide.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/carbon_dioxide_pb2.py` & `aiomagra-0.2.0/src/aiomagra/carbon_dioxide_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/carbon_monoxide.proto` & `aiomagra-0.2.0/src/aiomagra/carbon_monoxide.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/carbon_monoxide_pb2.py` & `aiomagra-0.2.0/src/aiomagra/carbon_monoxide_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/client.py` & `aiomagra-0.2.0/src/aiomagra/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import pprint
+from typing import Callable
 
 import aiohttp
 from aiohttp import WSMsgType
 import async_timeout
 
 from .const import LOGGER
 from .metadata_pb2 import DeviceMetadata
@@ -19,20 +20,23 @@
     StructureRequest,
     StructureResponse,
 )
 from .websocket_pb2 import WebsocketMessage
 
 
 class Client:
-    def __init__(self, host: str, session: aiohttp.ClientSession) -> None:
+    def __init__(
+        self, host: str, session: aiohttp.ClientSession, on_close: Callable
+    ) -> None:
         self._host = host
         self.session = session
         self._calls: dict[int, Call] = {}
         self._call_id = 0
         self._consumers = []
+        self.on_close = on_close
 
     @property
     def _next_id(self) -> int:
         self._call_id += 1
         return self._call_id
 
     async def connect(self):
@@ -43,28 +47,27 @@
         self._rx_task = asyncio.create_task(self._rx_msgs())
         LOGGER.info("Connected to %s", self._host)
 
     async def _rx_msgs(self) -> None:
         while not self._client.closed:
             msg = await self._client.receive()
             LOGGER.info("Received msg (%s): %s", self._host, msg)
-            LOGGER.debug("MSG type %s : %s", msg.type, msg.type == WSMsgType.CLOSED)
-            if msg.type == WSMsgType.CLOSED:
-                LOGGER.debug("MSG TYPE CLOSED")
-                break
-            m = WebsocketMessage()
-            m.ParseFromString(msg.data)
-
-            pp = pprint.PrettyPrinter(indent=4)
-            LOGGER.info("MSG: %s", pp.pprint(m))
 
             if not self._client.closed:
+                m = WebsocketMessage()
+                m.ParseFromString(msg.data)
+
+                pp = pprint.PrettyPrinter(indent=4)
+                LOGGER.info("MSG: %s", pp.pprint(m))
+
                 if m.frame_id > 0:
                     if m.frame_id not in self._calls:
-                        LOGGER.warning("Response for an unknown request id: %s", m.frame_id)
+                        LOGGER.warning(
+                            "Response for an unknown request id: %s", m.frame_id
+                        )
                         return
                     call = self._calls.pop(m.frame_id)
                     if not call.resolve.cancelled():
                         call.resolve.set_result(m.reply)
                 else:
                     for consumer in self._consumers:
                         consumer(m.gateway_report)
@@ -76,14 +79,15 @@
                 call_item.resolve.set_exception(Exception())
         self._calls.clear()
 
         if not self._client.closed:
             await self._client.close()
 
         self._client = None
+        self.on_close()
 
     async def add_consumer(self, consumer):
         self._consumers.append(consumer)
 
     async def close(self):
         if self._rx_task:
             self._rx_task.cancel()
@@ -102,15 +106,17 @@
         await self._call("Switch/SwitchOn", data)
 
     async def switch_off(self, device_id: bytes) -> None:
         data = CommandRequestData()
         data.SwitchOff.metadata.CopyFrom(self._metadata(device_id))
         await self._call("Switch/SwitchOff", data)
 
-    async def _call(self, method: str, data: CommandRequestData, timeout: int = 10) -> CommandReplyData:
+    async def _call(
+        self, method: str, data: CommandRequestData, timeout: int = 10
+    ) -> CommandReplyData:
         call = Call(self._next_id, method, data)
         self._calls[call.frame_id] = call
         LOGGER.debug("%s: send request", call.frame_id)
         try:
             async with async_timeout.timeout(timeout):
                 await call.send_request(self._client)
                 reply: CommandReply = await call.resolve
@@ -130,14 +136,15 @@
         return reply.data
 
     def _metadata(self, device_id: bytes) -> DeviceMetadata:
         metadata = DeviceMetadata()
         metadata.mqtt.device_id = device_id
         return metadata
 
+
 class Call:
     def __init__(self, frame_id, method: str, data: CommandRequestData) -> None:
         self.frame_id = frame_id
         self.method = method
         self.data = data
         self.resolve: asyncio.Future = asyncio.Future()
```

### Comparing `aiomagra-0.1.2/src/aiomagra/color.proto` & `aiomagra-0.2.0/src/aiomagra/color.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/color_pb2.py` & `aiomagra-0.2.0/src/aiomagra/color_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/configuration.proto` & `aiomagra-0.2.0/src/aiomagra/configuration.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/configuration_pb2.py` & `aiomagra-0.2.0/src/aiomagra/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/devices.proto` & `aiomagra-0.2.0/src/aiomagra/devices.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/devices_pb2.py` & `aiomagra-0.2.0/src/aiomagra/devices_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/door_pb2.py` & `aiomagra-0.2.0/src/aiomagra/door_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/doorbell_pb2.py` & `aiomagra-0.2.0/src/aiomagra/doorbell_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/emergency_pb2.py` & `aiomagra-0.2.0/src/aiomagra/emergency_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/firmware.proto` & `aiomagra-0.2.0/src/aiomagra/firmware.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/firmware_pb2.py` & `aiomagra-0.2.0/src/aiomagra/firmware_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/flood_pb2.py` & `aiomagra-0.2.0/src/aiomagra/flood_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/gate.proto` & `aiomagra-0.2.0/src/aiomagra/gate.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/gate_pb2.py` & `aiomagra-0.2.0/src/aiomagra/gate_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/gateway.proto` & `aiomagra-0.2.0/src/aiomagra/gateway.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/gateway_pb2.py` & `aiomagra-0.2.0/src/aiomagra/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/heartbeat_pb2.py` & `aiomagra-0.2.0/src/aiomagra/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/info_pb2.py` & `aiomagra-0.2.0/src/aiomagra/info_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/level.proto` & `aiomagra-0.2.0/src/aiomagra/level.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/level_pb2.py` & `aiomagra-0.2.0/src/aiomagra/level_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/lock.proto` & `aiomagra-0.2.0/src/aiomagra/lock.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/lock_pb2.py` & `aiomagra-0.2.0/src/aiomagra/lock_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/messaging_pb2.py` & `aiomagra-0.2.0/src/aiomagra/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/metadata.proto` & `aiomagra-0.2.0/src/aiomagra/metadata.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/metadata_pb2.py` & `aiomagra-0.2.0/src/aiomagra/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/meter.proto` & `aiomagra-0.2.0/src/aiomagra/meter.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/meter_pb2.py` & `aiomagra-0.2.0/src/aiomagra/meter_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/mqtt_pb2.py` & `aiomagra-0.2.0/src/aiomagra/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/power_source.proto` & `aiomagra-0.2.0/src/aiomagra/power_source.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/power_source_pb2.py` & `aiomagra-0.2.0/src/aiomagra/power_source_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/pubsub.proto` & `aiomagra-0.2.0/src/aiomagra/pubsub.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/pubsub_pb2.py` & `aiomagra-0.2.0/src/aiomagra/pubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/remote.proto` & `aiomagra-0.2.0/src/aiomagra/remote.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/remote_pb2.py` & `aiomagra-0.2.0/src/aiomagra/remote_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/reports.proto` & `aiomagra-0.2.0/src/aiomagra/reports.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/reports_pb2.py` & `aiomagra-0.2.0/src/aiomagra/reports_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/roller_shutter.proto` & `aiomagra-0.2.0/src/aiomagra/roller_shutter.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/roller_shutter_pb2.py` & `aiomagra-0.2.0/src/aiomagra/roller_shutter_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/seismic_pb2.py` & `aiomagra-0.2.0/src/aiomagra/seismic_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/sensor_pb2.py` & `aiomagra-0.2.0/src/aiomagra/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/siren.proto` & `aiomagra-0.2.0/src/aiomagra/siren.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/siren_pb2.py` & `aiomagra-0.2.0/src/aiomagra/siren_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/smoke.proto` & `aiomagra-0.2.0/src/aiomagra/smoke.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/smoke_pb2.py` & `aiomagra-0.2.0/src/aiomagra/smoke_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/status_pb2.py` & `aiomagra-0.2.0/src/aiomagra/status_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/structure.proto` & `aiomagra-0.2.0/src/aiomagra/structure.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/structure_pb2.py` & `aiomagra-0.2.0/src/aiomagra/structure_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/switch.proto` & `aiomagra-0.2.0/src/aiomagra/switch.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/switch_pb2.py` & `aiomagra-0.2.0/src/aiomagra/switch_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/tamper_pb2.py` & `aiomagra-0.2.0/src/aiomagra/tamper_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/taptap_pb2.py` & `aiomagra-0.2.0/src/aiomagra/taptap_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/temperature.proto` & `aiomagra-0.2.0/src/aiomagra/temperature.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/temperature_pb2.py` & `aiomagra-0.2.0/src/aiomagra/temperature_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/thermostat.proto` & `aiomagra-0.2.0/src/aiomagra/thermostat.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/thermostat_pb2.py` & `aiomagra-0.2.0/src/aiomagra/thermostat_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/ultraviolet.proto` & `aiomagra-0.2.0/src/aiomagra/ultraviolet.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/ultraviolet_pb2.py` & `aiomagra-0.2.0/src/aiomagra/ultraviolet_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/units.proto` & `aiomagra-0.2.0/src/aiomagra/units.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/units_pb2.py` & `aiomagra-0.2.0/src/aiomagra/units_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/websocket_pb2.py` & `aiomagra-0.2.0/src/aiomagra/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/wifi.proto` & `aiomagra-0.2.0/src/aiomagra/wifi.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/wifi_pb2.py` & `aiomagra-0.2.0/src/aiomagra/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/zigbee.proto` & `aiomagra-0.2.0/src/aiomagra/zigbee.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/zigbee_pb2.py` & `aiomagra-0.2.0/src/aiomagra/zigbee_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/zwave.proto` & `aiomagra-0.2.0/src/aiomagra/zwave.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.2/src/aiomagra/zwave_pb2.py` & `aiomagra-0.2.0/src/aiomagra/zwave_pb2.py`

 * *Files identical despite different names*

