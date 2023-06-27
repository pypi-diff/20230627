# Comparing `tmp/unitelabs_connector_framework-0.1.1.tar.gz` & `tmp/unitelabs_connector_framework-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitelabs_connector_framework-0.1.1.tar", max compression
+gzip compressed data, was "unitelabs_connector_framework-0.1.2.tar", max compression
```

## Comparing `unitelabs_connector_framework-0.1.1.tar` & `unitelabs_connector_framework-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,78 @@
--rw-r--r--   0        0        0     1069 2023-06-11 17:51:12.165815 unitelabs_connector_framework-0.1.1/LICENSE
--rw-r--r--   0        0        0     3026 2023-06-18 10:34:53.733054 unitelabs_connector_framework-0.1.1/README.md
--rw-r--r--   0        0        0     2061 2023-06-18 10:34:53.742212 unitelabs_connector_framework-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      168 2023-06-14 09:28:37.005175 unitelabs_connector_framework-0.1.1/src/unitelabs/__init__.py
--rw-r--r--   0        0        0     1235 2023-06-10 08:57:12.994027 unitelabs_connector_framework-0.1.1/src/unitelabs/cli.py
--rw-r--r--   0        0        0      454 2023-06-10 08:19:00.892129 unitelabs_connector_framework-0.1.1/src/unitelabs/config.py
--rw-r--r--   0        0        0     1751 2023-06-18 10:34:53.743165 unitelabs_connector_framework-0.1.1/src/unitelabs/connector.py
--rw-r--r--   0        0        0     4429 2023-06-08 12:21:47.568189 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto
--rw-r--r--   0        0        0     5518 2023-06-08 12:21:47.572050 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml
--rw-r--r--   0        0        0      321 2023-06-08 12:21:47.573953 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/__init__.py
--rw-r--r--   0        0        0     3755 2023-06-14 09:35:35.940054 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/lock_controller.py
--rw-r--r--   0        0        0     3375 2023-06-10 08:57:13.031414 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/lock_controller_base.py
--rw-r--r--   0        0        0     7109 2023-06-08 12:01:08.346706 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto
--rw-r--r--   0        0        0     7902 2023-06-08 11:43:41.586033 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml
--rw-r--r--   0        0        0      111 2023-06-08 12:01:41.537455 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/__init__.py
--rw-r--r--   0        0        0     5936 2023-06-18 10:26:38.076224 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/sila_service.py
--rw-r--r--   0        0        0       93 2023-06-18 10:34:53.743616 unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/greeting_provider/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-18 10:34:53.744341 unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py
--rw-r--r--   0        0        0       84 2023-06-18 10:34:53.744719 unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/timer_provider/__init__.py
--rw-r--r--   0        0        0     1838 2023-06-18 10:34:53.745303 unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/timer_provider/timer_provider_base.py
--rw-r--r--   0        0        0    14833 2023-06-09 11:02:35.803576 unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto
--rw-r--r--   0        0        0    15654 2023-06-08 18:31:02.343015 unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml
--rw-r--r--   0        0        0      407 2023-06-14 09:34:31.175200 unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/__init__.py
--rw-r--r--   0        0        0    11116 2023-06-14 09:34:39.277307 unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py
--rw-r--r--   0        0        0     8041 2023-06-08 15:58:40.585326 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto
--rw-r--r--   0        0        0     8279 2023-06-08 15:58:37.034762 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml
--rw-r--r--   0        0        0       88 2023-06-08 15:56:50.422431 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/__init__.py
--rw-r--r--   0        0        0     5190 2023-06-11 10:29:43.300577 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py
--rw-r--r--   0        0        0     2891 2023-06-03 08:08:38.591011 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto
--rw-r--r--   0        0        0     2846 2023-06-10 09:38:31.720888 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml
--rw-r--r--   0        0        0       96 2023-05-07 08:13:10.387701 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/__init__.py
--rw-r--r--   0        0        0     2383 2023-06-11 10:54:49.863161 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/observable_command_test.py
--rw-r--r--   0        0        0     2146 2023-06-10 08:52:51.902499 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto
--rw-r--r--   0        0        0     1820 2023-06-10 08:52:10.669356 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml
--rw-r--r--   0        0        0       99 2023-06-10 08:56:35.314045 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/__init__.py
--rw-r--r--   0        0        0     1625 2023-06-10 09:22:10.087811 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/observable_property_test.py
--rw-r--r--   0        0        0     3147 2023-06-08 15:10:15.841233 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto
--rw-r--r--   0        0        0     4090 2023-06-08 15:12:39.575863 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml
--rw-r--r--   0        0        0      102 2023-06-08 15:57:00.405056 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/__init__.py
--rw-r--r--   0        0        0     2006 2023-06-11 10:22:39.326761 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py
--rw-r--r--   0        0        0     1465 2023-06-08 14:12:11.083908 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto
--rw-r--r--   0        0        0     1250 2023-06-08 14:13:49.773291 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml
--rw-r--r--   0        0        0      105 2023-06-08 14:14:24.590503 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/__init__.py
--rw-r--r--   0        0        0      725 2023-06-10 08:57:12.994633 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py
--rw-r--r--   0        0        0     4157 2023-06-03 08:14:35.038359 unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto
--rw-r--r--   0        0        0     8446 2023-05-07 08:33:49.313366 unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml
--rw-r--r--   0        0        0       85 2023-06-03 08:14:35.038563 unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/__init__.py
--rw-r--r--   0        0        0     2839 2023-06-11 10:28:57.427186 unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/weighing_service.py
--rw-r--r--   0        0        0      541 2023-06-06 19:24:50.656991 unitelabs_connector_framework-0.1.1/src/unitelabs/logging.py
--rw-r--r--   0        0        0        0 2023-06-12 08:59:43.667279 unitelabs_connector_framework-0.1.1/src/unitelabs/py.typed
--rw-r--r--   0        0        0     1121 2023-06-11 10:27:23.555778 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 09:33:36.508770 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/__init__.py
--rw-r--r--   0        0        0      425 2023-06-11 09:59:16.304398 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/intermediate.py
--rw-r--r--   0        0        0     1188 2023-06-11 10:57:11.616229 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/intermediate_response.py
--rw-r--r--   0        0        0     1455 2023-06-11 10:57:13.280572 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/response.py
--rw-r--r--   0        0        0      698 2023-06-11 09:59:11.555574 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/status.py
--rw-r--r--   0        0        0      704 2023-06-09 10:50:39.626785 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/data_type_definition.py
--rw-r--r--   0        0        0      651 2023-06-07 12:03:48.878896 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/defined_execution_error.py
--rw-r--r--   0        0        0     1249 2023-06-09 08:43:40.105340 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/feature.py
--rw-r--r--   0        0        0      675 2023-06-08 14:06:19.120898 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/metadata.py
--rw-r--r--   0        0        0     5027 2023-06-14 09:35:17.579080 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/observable_command.py
--rw-r--r--   0        0        0     1516 2023-06-10 08:48:26.073694 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/observable_property.py
--rw-r--r--   0        0        0     3486 2023-06-09 08:24:50.416452 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/parser.py
--rw-r--r--   0        0        0     3940 2023-06-11 10:31:42.067642 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/unobservable_command.py
--rw-r--r--   0        0        0     1377 2023-06-07 12:04:17.401494 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/unobservable_property.py
--rw-r--r--   0        0        0     2314 2023-06-06 20:10:09.131560 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/utils.py
--rw-r--r--   0        0        0      307 2023-04-04 16:41:46.514608 unitelabs_connector_framework-0.1.1/src/unitelabs/utils.py
--rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 unitelabs_connector_framework-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-11 17:51:12.165815 unitelabs_connector_framework-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3026 2023-06-18 10:34:53.733054 unitelabs_connector_framework-0.1.2/README.md
+-rw-r--r--   0        0        0     2061 2023-06-27 06:23:35.106315 unitelabs_connector_framework-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-06-14 09:28:37.005175 unitelabs_connector_framework-0.1.2/src/unitelabs/__init__.py
+-rw-r--r--   0        0        0     1235 2023-06-10 08:57:12.994027 unitelabs_connector_framework-0.1.2/src/unitelabs/cli.py
+-rw-r--r--   0        0        0      454 2023-06-10 08:19:00.892129 unitelabs_connector_framework-0.1.2/src/unitelabs/config.py
+-rw-r--r--   0        0        0     1751 2023-06-18 10:34:53.743165 unitelabs_connector_framework-0.1.2/src/unitelabs/connector.py
+-rw-r--r--   0        0        0     4429 2023-06-08 12:21:47.568189 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto
+-rw-r--r--   0        0        0     5518 2023-06-08 12:21:47.572050 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml
+-rw-r--r--   0        0        0      321 2023-06-08 12:21:47.573953 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/__init__.py
+-rw-r--r--   0        0        0     3755 2023-06-25 20:18:33.251237 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/lock_controller.py
+-rw-r--r--   0        0        0     3421 2023-06-27 06:15:54.669793 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/lock_controller_base.py
+-rw-r--r--   0        0        0     7109 2023-06-08 12:01:08.346706 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto
+-rw-r--r--   0        0        0     7902 2023-06-08 11:43:41.586033 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml
+-rw-r--r--   0        0        0      111 2023-06-08 12:01:41.537455 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/__init__.py
+-rw-r--r--   0        0        0     5936 2023-06-18 10:26:38.076224 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/sila_service.py
+-rw-r--r--   0        0        0       93 2023-06-18 10:34:53.743616 unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/greeting_provider/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-18 10:34:53.744341 unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py
+-rw-r--r--   0        0        0       84 2023-06-18 10:34:53.744719 unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/timer_provider/__init__.py
+-rw-r--r--   0        0        0     1838 2023-06-18 10:34:53.745303 unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/timer_provider/timer_provider_base.py
+-rw-r--r--   0        0        0      750 2023-06-27 06:15:54.670076 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/GripController-v1_0.proto
+-rw-r--r--   0        0        0      954 2023-06-27 06:15:54.670865 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/GripController-v1_0.sila.xml
+-rw-r--r--   0        0        0       87 2023-06-27 06:15:54.671502 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/__init__.py
+-rw-r--r--   0        0        0      637 2023-06-27 06:15:54.671777 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/grip_controller_base.py
+-rw-r--r--   0        0        0    14833 2023-06-27 05:46:00.048776 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto
+-rw-r--r--   0        0        0    15654 2023-06-08 18:31:02.343015 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml
+-rw-r--r--   0        0        0      407 2023-06-14 09:34:31.175200 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/__init__.py
+-rw-r--r--   0        0        0    11465 2023-06-27 06:05:53.910295 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py
+-rw-r--r--   0        0        0     3371 2023-06-27 06:02:55.958059 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.proto
+-rw-r--r--   0        0        0     3602 2023-06-27 06:02:55.959024 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.sila.xml
+-rw-r--r--   0        0        0      165 2023-06-27 06:02:55.959301 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/__init__.py
+-rw-r--r--   0        0        0     2046 2023-06-27 06:02:55.960189 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/movement_controller_base.py
+-rw-r--r--   0        0        0     8041 2023-06-08 15:58:40.585326 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto
+-rw-r--r--   0        0        0     8279 2023-06-08 15:58:37.034762 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       88 2023-06-08 15:56:50.422431 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/__init__.py
+-rw-r--r--   0        0        0     5190 2023-06-11 10:29:43.300577 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py
+-rw-r--r--   0        0        0     2891 2023-06-03 08:08:38.591011 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto
+-rw-r--r--   0        0        0     2846 2023-06-10 09:38:31.720888 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       96 2023-05-07 08:13:10.387701 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/__init__.py
+-rw-r--r--   0        0        0     2383 2023-06-25 19:52:23.455657 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/observable_command_test.py
+-rw-r--r--   0        0        0     2146 2023-06-10 08:52:51.902499 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto
+-rw-r--r--   0        0        0     1820 2023-06-10 08:52:10.669356 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       99 2023-06-10 08:56:35.314045 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/__init__.py
+-rw-r--r--   0        0        0     1625 2023-06-10 09:22:10.087811 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/observable_property_test.py
+-rw-r--r--   0        0        0     3147 2023-06-08 15:10:15.841233 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto
+-rw-r--r--   0        0        0     4090 2023-06-08 15:12:39.575863 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml
+-rw-r--r--   0        0        0      102 2023-06-08 15:57:00.405056 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/__init__.py
+-rw-r--r--   0        0        0     2006 2023-06-11 10:22:39.326761 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py
+-rw-r--r--   0        0        0     1465 2023-06-08 14:12:11.083908 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto
+-rw-r--r--   0        0        0     1250 2023-06-08 14:13:49.773291 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml
+-rw-r--r--   0        0        0      105 2023-06-08 14:14:24.590503 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-10 08:57:12.994633 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py
+-rw-r--r--   0        0        0     4157 2023-06-03 08:14:35.038359 unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto
+-rw-r--r--   0        0        0     8446 2023-05-07 08:33:49.313366 unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml
+-rw-r--r--   0        0        0       85 2023-06-03 08:14:35.038563 unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/__init__.py
+-rw-r--r--   0        0        0     2839 2023-06-11 10:28:57.427186 unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/weighing_service.py
+-rw-r--r--   0        0        0      541 2023-06-06 19:24:50.656991 unitelabs_connector_framework-0.1.2/src/unitelabs/logging.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:59:43.667279 unitelabs_connector_framework-0.1.2/src/unitelabs/py.typed
+-rw-r--r--   0        0        0     1140 2023-06-27 06:02:55.961038 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 09:33:36.508770 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-11 09:59:16.304398 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/intermediate.py
+-rw-r--r--   0        0        0     1188 2023-06-11 10:57:11.616229 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/intermediate_response.py
+-rw-r--r--   0        0        0     1455 2023-06-11 10:57:13.280572 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/response.py
+-rw-r--r--   0        0        0      776 2023-06-27 06:15:54.672163 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/status.py
+-rw-r--r--   0        0        0      661 2023-06-27 06:02:55.962831 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/__init__.py
+-rw-r--r--   0        0        0      701 2023-06-19 12:58:38.071860 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/custom_data_type.py
+-rw-r--r--   0        0        0     1513 2023-06-19 12:58:38.072789 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/data_type_definition.py
+-rw-r--r--   0        0        0     3795 2023-06-19 12:58:38.073840 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/parser.py
+-rw-r--r--   0        0        0      651 2023-06-19 10:48:02.425135 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/defined_execution_error.py
+-rw-r--r--   0        0        0     1249 2023-06-19 10:47:59.222382 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/feature.py
+-rw-r--r--   0        0        0      675 2023-06-19 10:47:57.307171 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/metadata.py
+-rw-r--r--   0        0        0     4852 2023-06-19 12:58:38.074888 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/observable_command.py
+-rw-r--r--   0        0        0     1539 2023-06-19 12:58:38.075687 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/observable_property.py
+-rw-r--r--   0        0        0     3765 2023-06-19 12:58:38.076635 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/unobservable_command.py
+-rw-r--r--   0        0        0     1400 2023-06-19 12:58:38.077493 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/unobservable_property.py
+-rw-r--r--   0        0        0     2314 2023-06-06 20:10:09.131560 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/utils.py
+-rw-r--r--   0        0        0      307 2023-04-04 16:41:46.514608 unitelabs_connector_framework-0.1.2/src/unitelabs/utils.py
+-rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 unitelabs_connector_framework-0.1.2/PKG-INFO
```

### Comparing `unitelabs_connector_framework-0.1.1/LICENSE` & `unitelabs_connector_framework-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/README.md` & `unitelabs_connector_framework-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/pyproject.toml` & `unitelabs_connector_framework-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitelabs-connector-framework"
-version = "0.1.1"
+version = "0.1.2"
 description = "A framework to build connectors based on the SiLA 2 standard specification."
 license = "MIT"
 authors = ["UniteLabs AG <developers+connector@unitelabs.ch>"]
 readme = "README.md"
 homepage = "https://unitelabs.ch"
 repository = "https://gitlab.com/unitelabs/connector-framework"
 documentation = "https://gitlab.com/unitelabs/connector-framework/-/tree/main/docs/"
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/cli.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/cli.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/connector.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/connector.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/lock_controller.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/lock_controller.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/lock_controller_base.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/lock_controller_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,16 +62,18 @@
         ],
     ) -> None:
         """
         Locks a SiLA Server for exclusive use by setting a lock identifier that has to be sent along with
         any following (lock protected) request as long as the SiLA Server is locked.
         The lock can be reset by issuing the 'Unlock Server' command.
 
-        .. parameter:: The lock identifier that has to be sent along with every (lock protected) request to use the server's functionality.
-        .. parameter:: The time (in seconds) after a SiLA Server is automatically unlocked when no request with a valid lock identifier has been received meanwhile. A timeout of zero seconds specifies an infinite time (no timeout).
+        .. parameter:: The lock identifier that has to be sent along with every (lock protected) request to use the
+                       server's functionality.
+        .. parameter:: The time (in seconds) after a SiLA Server is automatically unlocked when no request with a valid
+                       lock identifier has been received meanwhile. A timeout of zero seconds specifies an infinite time (no timeout).
         """
 
     @abc.abstractmethod
     @sila.UnobservableCommand(errors=[ServerNotLocked, InvalidLockIdentifier])
     def unlock_server(self, lock_identifier: str) -> None:
         """
         Unlocks a locked SiLA Server. No lock identifier has to be sent for any following calls until
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/sila_service.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/sila_service.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/timer_provider/timer_provider_base.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/timer_provider/timer_provider_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
 
 class LabwareNotPlaced(sila.DefinedExecutionError):
     """Placing the labware item at the destination device failed."""
 
 
 @dataclasses.dataclass
-class PositionIndex(sila.DataTypeDefinition):
+class PositionIndex(sila.CustomDataType):
     """Specifies a position via an index number, starting at 1."""
 
     position_index: typing.Annotated[int, sila.constraints.MinimalInclusive(value=1)]
 
 
 @dataclasses.dataclass
-class HandoverPosition(sila.DataTypeDefinition):
+class HandoverPosition(sila.CustomDataType):
     """
     Specifies one of the possible positions of a device where labware items can be handed over. Can contain a
     sub-position, e.g. for specifying a position in a rack.
 
     .. parameter:: The name of the handover position (must be unique within the device).
     .. parameter:: The index of a sub-position within a handover position or the number of sub-positions respectively,
                    e.g. for a rack.
@@ -123,14 +123,16 @@
     @sila.ObservableCommand(errors=[InvalidCommandSequence])
     async def prepare_for_input(
         self,
         handover_position: HandoverPosition,
         internal_position: PositionIndex,
         labware_type: str,
         labware_unique_id: str,
+        *,
+        status: sila.Status,
     ) -> None:
         """
         Put the device into a state in which it is ready to accept new labware at the specified handover position.
 
         .. parameter:: Indicates the position where the labware will be handed over.
         .. parameter:: Indicates the position which the labware will be stored at within the device, e.g. internal
                        storage positions of an incubator.
@@ -139,47 +141,69 @@
         .. parameter:: Represents the unique identification of a labware in the controlling system. It is assigned by
                        the system and must remain unchanged during the whole process.
            :display_name: Labware Unique ID
         """
 
     @abc.abstractmethod
     @sila.ObservableCommand(errors=[InvalidCommandSequence])
-    async def prepare_for_output(self, handover_position: HandoverPosition, internal_position: PositionIndex) -> None:
+    async def prepare_for_output(
+        self,
+        handover_position: HandoverPosition,
+        internal_position: PositionIndex,
+        *,
+        status: sila.Status,
+    ) -> None:
         """
         Put the device into a state in which it is ready to release the labware at the specified handover position.
 
         .. parameter:: Indicates the position where the labware will be handed over.
         .. parameter:: Indicates the position which the labware will be retrieved from within the device, e.g. internal
                        storage positions of an incubator.
         """
 
     @abc.abstractmethod
     @sila.ObservableCommand(errors=[InvalidCommandSequence, LabwareNotPlaced])
-    async def put_labware(self, handover_position: HandoverPosition, intermediate_actions: list[str]) -> None:
+    async def put_labware(
+        self,
+        handover_position: HandoverPosition,
+        intermediate_actions: list[str],
+        *,
+        status: sila.Status,
+    ) -> None:
         """
         Place the currently processed labware item at the specified handover position (sent to the active source device
         after a "Prepare For Output" command).
 
         .. parameter:: Indicates the position the labware item will be moved to.
-        .. parameter:: Specifies one or more commands that have to be executed within the command sequence (e.g. removing a lid).
+        .. parameter:: Specifies one or more commands that have to be executed within the command sequence (e.g.
+                       removing a lid).
                        The order of execution is specified by order within the given list.
-                       Each entry must be one of the commands returned by the AvailableIntermediateCommandExecutions property.
+                       Each entry must be one of the commands returned by the AvailableIntermediateCommandExecutions
+                       property.
         """
 
     @abc.abstractmethod
     @sila.ObservableCommand(errors=[InvalidCommandSequence, LabwareNotPicked])
-    async def get_labware(self, handover_position: HandoverPosition, intermediate_actions: list[str]) -> None:
+    async def get_labware(
+        self,
+        handover_position: HandoverPosition,
+        intermediate_actions: list[str],
+        *,
+        status: sila.Status,
+    ) -> HandoverPosition:
         """
         Retrieve a labware item from the specified handover position (sent to the active destination device after a
         "Prepare For Input" command).
 
         .. parameter:: Indicates the position where the labware will be retrieved from.
-        .. parameter:: Specifies one or more commands that have to be executed within the command sequence (e.g. removing a lid).
+        .. parameter:: Specifies one or more commands that have to be executed within the command sequence (e.g.
+                       removing a lid).
                        The order of execution is specified by order within the given list.
-                       Each entry must be one of the commands returned by the AvailableIntermediateCommandExecutions property.
+                       Each entry must be one of the commands returned by the AvailableIntermediateCommandExecutions
+                       property.
         """
 
     @abc.abstractmethod
     @sila.UnobservableProperty()
     async def get_available_handover_positions(self) -> list[HandoverPosition]:
         """All handover positions of the device including the number of sub-positions."""
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/observable_command_test.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/observable_command_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/observable_property_test.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/observable_property_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/weighing_service.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/weighing_service.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/logging.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/logging.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/__init__.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from sila import constraints, data_types, datetime, errors, identifiers
+from sila import constraints, datetime, errors, identifiers
 from sila.server import Handler, Server
 
-from . import utils
+from . import data_types, utils
 from .commands.intermediate import Intermediate
 from .commands.intermediate_response import IntermediateResponse
 from .commands.response import Response
 from .commands.status import Status
-from .data_type_definition import DataTypeDefinition
+from .data_types.custom_data_type import CustomDataType
 from .defined_execution_error import DefinedExecutionError
 from .feature import Feature
 from .metadata import Metadata
 from .observable_command import ObservableCommand
 from .observable_property import ObservableProperty, Stream
 from .unobservable_command import UnobservableCommand
 from .unobservable_property import UnobservableProperty
 
 __all__ = [
     "Server",
     "Feature",
     "Handler",
     "ObservableCommand",
+    "Intermediate",
     "IntermediateResponse",
     "Response",
     "UnobservableCommand",
     "UnobservableProperty",
     "ObservableProperty",
     "Stream",
-    "DataTypeDefinition",
+    "CustomDataType",
     "DefinedExecutionError",
     "Metadata",
     "Status",
     "data_types",
     "constraints",
     "errors",
     "datetime",
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/intermediate_response.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/intermediate_response.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/response.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/response.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/status.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/status.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 
     def update(
         self,
         progress: float | None = None,
         remaining_time: datetime.timedelta | None = None,
         updated_lifetime: datetime.timedelta | None = None,
     ) -> None:
+        """Updates the execution status of an observable command execution"""
         self.command_execution.update_execution_info(
             progress_info=progress,
             estimated_remaining_time=remaining_time,
             updated_lifetime_of_execution=updated_lifetime,
         )
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/data_type_definition.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/custom_data_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import abc
 import dataclasses
 import inspect
 import typing
 
-from . import utils
+from .. import utils
 
 
 @dataclasses.dataclass
-class DataTypeDefinition(abc.ABC):
+class CustomDataType(abc.ABC):
     identifier: typing.ClassVar[str] = ""
     display_name: typing.ClassVar[str] = ""
     description: typing.ClassVar[str] = ""
 
     def __init_subclass__(cls, *args, identifier="", display_name="", description="", **kwargs) -> None:
         super().__init_subclass__(*args, **kwargs)
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/defined_execution_error.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/defined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/feature.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/feature.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/metadata.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/metadata.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/observable_command.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/observable_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import dataclasses
 import inspect
 import typing
 
 import sila.server as sila
 from sila.commands import CommandExecution
 
-from . import parser, utils
+from . import utils
 from .commands.intermediate import Intermediate
 from .commands.intermediate_response import IntermediateResponse
 from .commands.response import Response
 from .commands.status import Status
-from .data_type_definition import DataTypeDefinition
+from .data_types import parser
 from .defined_execution_error import DefinedExecutionError
 
 
 @dataclasses.dataclass
 class ObservableCommand:
     name: str = ""
     description: str = ""
@@ -73,17 +73,14 @@
             if inspect.isawaitable(response):
                 response = await response
 
             if isinstance(response, type(None)):
                 return {}
             values = {}
             for index, response in enumerate([response] if not isinstance(response, tuple) else response):
-                if isinstance(response, DataTypeDefinition):
-                    response = {response.identifier: dataclasses.asdict(response)}
-
                 key = responses[index]
                 values[key.identifier] = response
 
             return values
 
         observable_command = sila.ObservableCommand(
             identifier=identifier,
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/observable_property.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/unobservable_property.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from __future__ import annotations
 
 import dataclasses
 import inspect
 import typing
-from collections.abc import AsyncIterator
 
 import sila.server as sila
 
-from . import parser, utils
+from . import utils
+from .data_types import parser
 from .defined_execution_error import DefinedExecutionError
 
-T = typing.TypeVar("T")
-Stream = AsyncIterator[T]
-
 
 @dataclasses.dataclass
-class ObservableProperty:
+class UnobservableProperty:
     identifier: str = ""
     display_name: str = ""
     description: str = ""
     errors: list[type[DefinedExecutionError]] = dataclasses.field(default_factory=list)
 
     def __call__(self, function: typing.Callable):
         setattr(function, "__handler", self)
         return function
 
     def attach(self, feature: sila.Feature, function: typing.Callable):
-        name = function.__name__.lower().removeprefix("subscribe_")
+        name = function.__name__.lower().removeprefix("get_")
         display_name = self.display_name or utils.humanize(name)
         identifier = self.identifier or display_name.replace(" ", "")
         description = self.description or inspect.getdoc(function) or ""
 
         type_hint = inspect.signature(function).return_annotation
-        type_hint = typing.get_args(type_hint)[0]
 
-        observable_property = sila.ObservableProperty(
+        unobservable_property = sila.UnobservableProperty(
             identifier=identifier,
             display_name=display_name,
             description=description,
             function=function,
             errors=[Error(feature=feature) for Error in self.errors],
             data_type=parser.parse(type_hint, feature),
         )
-        feature.add_handler(observable_property)
+        feature.add_handler(unobservable_property)
 
-        return observable_property
+        return unobservable_property
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/parser.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 from __future__ import annotations
 
 import dataclasses
 import inspect
 import typing
 
 import sila.server as sila
+from sila import identifiers
 
-from . import utils
+from .. import utils
+from .custom_data_type import CustomDataType
 from .data_type_definition import DataTypeDefinition
 
 
 def parse(type_hint: typing.Type, feature: sila.Feature) -> sila.data_types.DataType:
     origin = typing.get_origin(type_hint) or type_hint
 
     if origin is None:
         return sila.data_types.Void()
-    if issubclass(origin, DataTypeDefinition):
-        if data_type := next(
-            iter(
-                [
-                    data_type_definition
-                    for data_type_definition in feature.data_type_definitions
-                    if data_type_definition.identifier == origin.identifier
-                ]
-            ),
-            None,
-        ):
-            return data_type
+    if issubclass(origin, CustomDataType):
+        feature_identifier = feature.fully_qualified_identifier
+        identifier = identifiers.FullyQualifiedCustomDataTypeIdentifier(
+            **dataclasses.asdict(feature_identifier), custom_data_type=origin.identifier
+        )
+
+        if identifier in feature.data_type_definitions:
+            return feature.data_type_definitions[identifier]
 
         docs = utils.parse_docs(inspect.getdoc(origin) or "")
         fields = dataclasses.fields(origin)
 
         if len(fields) == 1 and utils.humanize(fields[0].name).replace(" ", "") == origin.identifier:
-            data_type_definition = sila.data_types.DataTypeDefinition(
+            data_type_definition = DataTypeDefinition(
                 identifier=origin.identifier,
                 display_name=origin.display_name,
                 description=origin.description,
+                fields_by_identifier={origin.identifier: fields[0].name},
                 factory=type_hint,
                 data_type=parse(fields[0].type, feature),
             )
 
             feature.add_data_type_definition(data_type_definition)
             return data_type_definition
 
         elements: list[sila.data_types.Structure.Element] = []
+        fields_by_identifier: dict[str, str] = {}
         for index, field in enumerate(fields):
             field_display_name = utils.humanize(field.name)
+            field_identifier = field_display_name.replace(" ", "")
+            fields_by_identifier[field_identifier] = field.name
             elements.append(
                 sila.data_types.Structure.Element(
-                    identifier=field_display_name.replace(" ", ""),
+                    identifier=field_identifier,
                     display_name=field_display_name,
                     description=docs.get("parameter", [])[index].get("default", ""),
                     data_type=parse(field.type, feature),
                 )
             )
 
-        data_type_definition = sila.data_types.DataTypeDefinition(
+        data_type_definition = DataTypeDefinition(
             identifier=origin.identifier,
             display_name=origin.display_name,
             description=origin.description,
-            factory=lambda x: type_hint(*x.values()),
+            fields_by_identifier=fields_by_identifier,
+            factory=type_hint,
             data_type=sila.data_types.Structure(elements=elements),
         )
         feature.add_data_type_definition(data_type_definition)
         return data_type_definition
     if issubclass(origin, sila.data_types.DataType):
         return origin()
     if issubclass(origin, bool):
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/unobservable_command.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/unobservable_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import dataclasses
 import inspect
 import typing
 
 import sila.server as sila
 
-from . import parser, utils
+from . import utils
 from .commands.response import Response
-from .data_type_definition import DataTypeDefinition
+from .data_types import parser
 from .defined_execution_error import DefinedExecutionError
 
 
 @dataclasses.dataclass
 class UnobservableCommand:
     identifier: str = ""
     display_name: str = ""
@@ -50,17 +50,14 @@
             if inspect.isawaitable(response):
                 response = await response
 
             if isinstance(response, type(None)):
                 return {}
             values = {}
             for index, response in enumerate([response] if not isinstance(response, tuple) else response):
-                if isinstance(response, DataTypeDefinition):
-                    response = {response.identifier: dataclasses.asdict(response)}
-
                 key = responses[index]
                 values[key.identifier] = response
 
             return values
 
         unobservable_command = sila.UnobservableCommand(
             identifier=identifier,
```

### Comparing `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/utils.py` & `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/utils.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.1/PKG-INFO` & `unitelabs_connector_framework-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitelabs-connector-framework
-Version: 0.1.1
+Version: 0.1.2
 Summary: A framework to build connectors based on the SiLA 2 standard specification.
 Home-page: https://unitelabs.ch
 License: MIT
 Keywords: SiLA 2,laboratory,automation,connectivity
 Author: UniteLabs AG
 Author-email: developers+connector@unitelabs.ch
 Requires-Python: >=3.9,<4.0
```

