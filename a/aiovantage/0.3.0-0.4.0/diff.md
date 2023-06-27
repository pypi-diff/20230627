# Comparing `tmp/aiovantage-0.3.0.tar.gz` & `tmp/aiovantage-0.4.0.tar.gz`

## Comparing `aiovantage-0.3.0.tar` & `aiovantage-0.4.0.tar`

### file list

```diff
@@ -1,149 +1,153 @@
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 aiovantage-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/dump_system.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/monitor_all.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/anemo_sensors/dump_anemo_sensors.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/anemo_sensors/monitor_anemo_sensors.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/light_sensors/dump_light_sensors.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/light_sensors/monitor_light_sensors.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/control_load.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/stations/jingle_bells.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/tasks/run_task.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/temperature_sensors/dump_temperature_sensors.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/temperature_sensors/monitor_temperature_sensors.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/__init__.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/connection.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/errors.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/query.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/commands.py
--rw-r--r--   0        0        0    13502 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/light_sensor.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/sounder.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/temperature.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/helpers.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/xml_dataclass.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/__init__.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/login/login.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/anemo_sensors.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/light_sensors.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/temperature_sensors.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.3.0/LICENSE
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 aiovantage-0.3.0/README.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 aiovantage-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 aiovantage-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 aiovantage-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 aiovantage-0.4.0/testrgbw.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/dump_system.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/monitor_all.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/anemo_sensors/dump_anemo_sensors.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/anemo_sensors/monitor_anemo_sensors.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/light_sensors/dump_light_sensors.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/light_sensors/monitor_light_sensors.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/stations/jingle_bells.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/tasks/run_task.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/temperature_sensors/dump_temperature_sensors.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/temperature_sensors/monitor_temperature_sensors.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/connection.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/errors.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/commands.py
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/light_sensor.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/sounder.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/temperature.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/helpers.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/xml_dataclass.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/__init__.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/login/login.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/module.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/module_gen2.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/anemo_sensors.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/light_sensors.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/modules.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/temperature_sensors.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 aiovantage-0.4.0/README.md
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 aiovantage-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 aiovantage-0.4.0/PKG-INFO
```

### Comparing `aiovantage-0.3.0/.github/ISSUE_TEMPLATE/bug.yml` & `aiovantage-0.4.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `aiovantage-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/dump_system.py` & `aiovantage-0.4.0/examples/dump_system.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/monitor_all.py` & `aiovantage-0.4.0/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/anemo_sensors/dump_anemo_sensors.py` & `aiovantage-0.4.0/examples/anemo_sensors/dump_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/anemo_sensors/monitor_anemo_sensors.py` & `aiovantage-0.4.0/examples/anemo_sensors/monitor_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/areas/dump_areas.py` & `aiovantage-0.4.0/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.4.0/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/blinds/dump_blinds.py` & `aiovantage-0.4.0/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/blinds/monitor_blinds.py` & `aiovantage-0.4.0/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/buttons/dump_buttons.py` & `aiovantage-0.4.0/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/buttons/monitor_buttons.py` & `aiovantage-0.4.0/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/command_client/event_log.py` & `aiovantage-0.4.0/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/command_client/status_load.py` & `aiovantage-0.4.0/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/config_client/dump_objects.py` & `aiovantage-0.4.0/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/config_client/get_version.py` & `aiovantage-0.4.0/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.4.0/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.4.0/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/gmem/dump_gmem.py` & `aiovantage-0.4.0/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/gmem/monitor_gmem.py` & `aiovantage-0.4.0/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/gmem/set_gmem.py` & `aiovantage-0.4.0/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/light_sensors/dump_light_sensors.py` & `aiovantage-0.4.0/examples/light_sensors/dump_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/light_sensors/monitor_light_sensors.py` & `aiovantage-0.4.0/examples/light_sensors/monitor_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/load_groups/dump_load_groups.py` & `aiovantage-0.4.0/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/loads/control_load.py` & `aiovantage-0.4.0/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/loads/dump_loads.py` & `aiovantage-0.4.0/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/loads/monitor_loads.py` & `aiovantage-0.4.0/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/loads/poll_on_loads.py` & `aiovantage-0.4.0/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/loads/toggle_load.py` & `aiovantage-0.4.0/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.4.0/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.4.0/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.4.0/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.4.0/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/stations/dump_stations.py` & `aiovantage-0.4.0/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/stations/jingle_bells.py` & `aiovantage-0.4.0/examples/stations/jingle_bells.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/tasks/dump_tasks.py` & `aiovantage-0.4.0/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/tasks/run_task.py` & `aiovantage-0.4.0/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/temperature_sensors/dump_temperature_sensors.py` & `aiovantage-0.4.0/examples/temperature_sensors/dump_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/examples/temperature_sensors/monitor_temperature_sensors.py` & `aiovantage-0.4.0/examples/temperature_sensors/monitor_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/__init__.py` & `aiovantage-0.4.0/src/aiovantage/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from aiovantage.controllers.buttons import ButtonsController
 from aiovantage.controllers.dry_contacts import DryContactsController
 from aiovantage.controllers.gmem import GMemController
 from aiovantage.controllers.light_sensors import LightSensorsController
 from aiovantage.controllers.load_groups import LoadGroupsController
 from aiovantage.controllers.loads import LoadsController
 from aiovantage.controllers.masters import MastersController
+from aiovantage.controllers.modules import ModulesController
 from aiovantage.controllers.omni_sensors import OmniSensorsController
 from aiovantage.controllers.rgb_loads import RGBLoadsController
 from aiovantage.controllers.stations import StationsController
 from aiovantage.controllers.tasks import TasksController
 from aiovantage.controllers.temperature_sensors import TemperatureSensorsController
 
 from .events import VantageEvent
@@ -68,14 +69,15 @@
         self._buttons = ButtonsController(self)
         self._dry_contacts = DryContactsController(self)
         self._gmem = GMemController(self)
         self._light_sensors = LightSensorsController(self)
         self._loads = LoadsController(self)
         self._load_groups = LoadGroupsController(self)
         self._masters = MastersController(self)
+        self._modules = ModulesController(self)
         self._rgb_loads = RGBLoadsController(self)
         self._omni_sensors = OmniSensorsController(self)
         self._stations = StationsController(self)
         self._tasks = TasksController(self)
         self._temperature_sensors = TemperatureSensorsController(self)
 
     async def __aenter__(self) -> Self:
@@ -156,14 +158,19 @@
 
     @property
     def masters(self) -> MastersController:
         """Return the Masters controller for managing Vantage Controllers."""
         return self._masters
 
     @property
+    def modules(self) -> ModulesController:
+        """Return the Modules controller for managing modules."""
+        return self._modules
+
+    @property
     def gmem(self) -> GMemController:
         """Return the GMem controller for managing global memory."""
         return self._gmem
 
     @property
     def omni_sensors(self) -> OmniSensorsController:
         """Return the OmniSensors controller for managing generic sensors."""
@@ -206,14 +213,15 @@
             self._blind_groups.initialize(),
             self._buttons.initialize(),
             self._dry_contacts.initialize(),
             self._gmem.initialize(),
             self._light_sensors.initialize(),
             self._loads.initialize(),
             self._masters.initialize(),
+            self._modules.initialize(),
             self._rgb_loads.initialize(),
             self._omni_sensors.initialize(),
             self._stations.initialize(),
             self._tasks.initialize(),
             self._temperature_sensors.initialize(),
         )
 
@@ -231,14 +239,15 @@
             self.blind_groups.subscribe(callback),
             self.buttons.subscribe(callback),
             self.dry_contacts.subscribe(callback),
             self.gmem.subscribe(callback),
             self.light_sensors.subscribe(callback),
             self.loads.subscribe(callback),
             self.masters.subscribe(callback),
+            self.modules.subscribe(callback),
             self.rgb_loads.subscribe(callback),
             self.omni_sensors.subscribe(callback),
             self.stations.subscribe(callback),
             self.tasks.subscribe(callback),
             self.temperature_sensors.subscribe(callback),
         ]
```

### Comparing `aiovantage-0.3.0/src/aiovantage/connection.py` & `aiovantage-0.4.0/src/aiovantage/connection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/errors.py` & `aiovantage-0.4.0/src/aiovantage/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/query.py` & `aiovantage-0.4.0/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/README.md` & `aiovantage-0.4.0/src/aiovantage/command_client/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,9 +64,9 @@
 from aiovantage.command_client import Event, EventStream, EventType
 
 def callback(event: Event) -> None:
     assert event["type"] == EventType.STATUS
     print(f"Load {event['id']} changed state")
 
 events = EventStream("10.2.0.103")
-await events.subscribe_status(callback, "LOAD")
+events.subscribe_status(callback, "LOAD")
 ```
```

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/__init__.py` & `aiovantage-0.4.0/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/commands.py` & `aiovantage-0.4.0/src/aiovantage/command_client/commands.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/events.py` & `aiovantage-0.4.0/src/aiovantage/command_client/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,16 @@
         self._connection = CommandConnection(host, port, ssl, conn_timeout)
         self._username = username
         self._password = password
         self._tasks: List[asyncio.Task[None]] = []
         self._subscriptions: List[EventSubscription] = []
         self._status_subscribers: Dict[str, int] = defaultdict(int)
         self._enhanced_log_subscribers: Dict[str, int] = defaultdict(int)
+        self._start_lock = asyncio.Lock()
+        self._started = False
         self._connection_lock = asyncio.Lock()
         self._command_queue: asyncio.Queue[str] = asyncio.Queue()
         self._logger = logging.getLogger(__name__)
 
     async def __aenter__(self) -> Self:
         """Return context manager."""
         await self.start()
@@ -118,25 +120,33 @@
         """Exit context manager."""
         await self.stop()
         if exc_val:
             raise exc_val
 
     async def start(self) -> None:
         """Initialize the event stream."""
-        await self.get_connection()
-        self._tasks.append(asyncio.create_task(self._message_handler()))
-        self._tasks.append(asyncio.create_task(self._command_handler()))
-        self._tasks.append(asyncio.create_task(self._keepalive()))
+        async with self._start_lock:
+            if self._started:
+                return
+
+            await self.get_connection()
+            self._tasks.append(asyncio.create_task(self._message_handler()))
+            self._tasks.append(asyncio.create_task(self._command_handler()))
+            self._tasks.append(asyncio.create_task(self._keepalive()))
+
+            self._started = True
 
     async def stop(self) -> None:
         """Stop the event stream."""
-        for task in self._tasks:
-            task.cancel()
-        self._tasks.clear()
-        self._connection.close()
+        async with self._start_lock:
+            for task in self._tasks:
+                task.cancel()
+            self._tasks.clear()
+            self._connection.close()
+            self._started = False
 
     async def get_connection(self) -> CommandConnection:
         """Get a connection to the Host Command service."""
         async with self._connection_lock:
             if self._connection.closed:
                 # Open a new connection
                 await self._connection.open()
@@ -176,73 +186,85 @@
         # Return an unsubscribe callback to remove the subscription
         def unsubscribe() -> None:
             self._subscriptions.remove(subscription)
 
         return unsubscribe
 
     def subscribe_status(
-        self, callback: EventCallback, status_type: str
+        self, callback: EventCallback, status_types: Union[str, Iterable[str]]
     ) -> Callable[[], None]:
         """Subscribe to "Status" events from the Host Command service.
 
         Args:
             callback: The callback to invoke when an event is received.
-            status_type: The type of status to subscribe to.
+            status_types: The status types to subscribe to status events for.
 
         Returns:
             A coroutine that can be used to unsubscribe from status events.
         """
 
+        # Support both a single status type and a list of status types
+        if isinstance(status_types, str):
+            status_types = (status_types,)
+
         # Enable this status type if it's not already enabled
-        self._status_subscribers[status_type] += 1
-        if self._status_subscribers[status_type] == 1:
-            self._enable_status(status_type)
+        for status_type in status_types:
+            self._status_subscribers[status_type] += 1
+            if self._status_subscribers[status_type] == 1:
+                self._enable_status(status_type)
 
         # Subscribe, and return an unsubscribe callback
         remove_subscription = self.subscribe(
             callback,
             lambda event: (
                 event["type"] == EventType.STATUS
-                and event["status_type"] == status_type
+                and event["status_type"] in status_type
             ),
         )
 
         def unsubscribe() -> None:
-            self._status_subscribers[status_type] -= 1
-            if self._status_subscribers[status_type] == 0:
-                self._disable_status(status_type)
+            for status_type in status_types:
+                self._status_subscribers[status_type] -= 1
+                if self._status_subscribers[status_type] == 0:
+                    self._disable_status(status_type)
             remove_subscription()
 
         return unsubscribe
 
     def subscribe_enhanced_log(
-        self, callback: EventCallback, log_type: str
+        self, callback: EventCallback, log_types: Union[str, Iterable[str]]
     ) -> Callable[[], None]:
         """Subscribe to "Enhanced Log" events from the Host Command service.
 
         Args:
             callback: The callback to invoke when an event is received.
-            log_type: The type of log to subscribe to.
+            log_types: The event log types to subscribe to.
 
         Returns:
             A coroutine that can be used to unsubscribe from log events.
         """
 
+        # Support both a single log type and a list of log types
+        if isinstance(log_types, str):
+            log_types = (log_types,)
+
         # Enable this log type if it's not already enabled
-        self._enhanced_log_subscribers[log_type] += 1
-        if self._enhanced_log_subscribers[log_type] == 1:
-            self._enable_enhanced_log(log_type)
+        for log_type in log_types:
+            self._enhanced_log_subscribers[log_type] += 1
+            if self._enhanced_log_subscribers[log_type] == 1:
+                self._enable_enhanced_log(log_type)
 
         # Subscribe, and return an unsubscribe callback
         remove_subscription = self.subscribe(callback, EventType.ENHANCED_LOG)
 
         def unsubscribe() -> None:
-            self._enhanced_log_subscribers[log_type] -= 1
-            if self._enhanced_log_subscribers[log_type] == 0:
-                self._disable_enhanced_log(log_type)
+            for log_type in log_types:
+                self._enhanced_log_subscribers[log_type] -= 1
+                if self._enhanced_log_subscribers[log_type] == 0:
+                    self._disable_enhanced_log(log_type)
             remove_subscription()
 
         return unsubscribe
 
     def emit(self, event: Event) -> None:
         """Emit an event to subscribers.
```

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/utils.py` & `aiovantage-0.4.0/src/aiovantage/command_client/utils.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/anemo_sensor.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/anemo_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/light_sensor.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/light_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Interface for querying and controlling loads."""
 
-from enum import Enum
+from enum import IntEnum
 from typing import Sequence
 
 from .base import Interface
 
 
 class LoadInterface(Interface):
     """Interface for querying and controlling loads."""
 
-    class RampType(Enum):
+    class RampType(IntEnum):
         """The type of ramp to perform."""
 
         STOP = 2
         OPPOSITE = 3
         DOWN = 4
         UP = 5
         FIXED = 6
@@ -95,15 +95,15 @@
             level: The level to ramp the load to (0-100).
             seconds: The number of seconds to ramp the load over.
             ramp_type: The type of ramp to perform.
         """
 
         # INVOKE <id> Load.Ramp <type> <seconds> <level>
         # -> R:INVOKE <id> <rcode> Load.Ramp <type> <seconds> <level>
-        await self.invoke(vid, "Load.Ramp", ramp_type.value, seconds, level)
+        await self.invoke(vid, "Load.Ramp", ramp_type, seconds, level)
 
     @classmethod
     def parse_load_status(cls, args: Sequence[str]) -> float:
         """Parse a simple 'S:LOAD' event.
 
         Args:
             args: The arguments of the event.
```

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         Args:
             vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the RGBW color as a tuple of (red, green, blue, white).
         """
 
-        return tuple([await self.get_rgb_channel(vid, channel) for channel in range(4)])
+        return tuple(
+            [await self.get_rgbw_channel(vid, channel) for channel in range(4)]
+        )
 
     async def get_hsl(self, vid: int) -> Tuple[int, ...]:
         """Get the HSL color of a load from the controller.
 
         Args:
             vid: The Vantage ID of the RGB load.
 
@@ -115,15 +117,15 @@
         # INVOKE <id> RGBLoad.GetHSL <channel>
         # -> R:INVOKE <id> <value> RGBLoad.GetHSL <channel>
         response = await self.invoke(vid, "RGBLoad.GetHSL", attribute)
         color = int(response.args[1])
 
         return color
 
-    async def set_rgb(self, vid: int, red: int, green: int, blue: int) -> None:
+    async def set_rgb(self, vid: int, red: float, green: float, blue: float) -> None:
         """Set the color of an RGB load.
 
         Args:
             vid: The Vantage ID of the RGB load.
             red: The red value of the color, (0-255)
             green: The green value of the color, (0-255)
             blue: The blue value of the color, (0-255)
@@ -135,15 +137,15 @@
         blue = int(max(min(blue, 255), 0))
 
         # INVOKE <id> RGBLoad.SetRGB <red> <green> <blue>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetRGB <red> <green> <blue>
         await self.invoke(vid, "RGBLoad.SetRGB", red, green, blue)
 
     async def set_rgbw(
-        self, vid: int, red: int, green: int, blue: int, white: int
+        self, vid: int, red: float, green: float, blue: float, white: float
     ) -> None:
         """Set the color of an RGBW load.
 
         Args:
             vid: The Vantage ID of the RGB load.
             red: The red value of the color, (0-255)
             green: The green value of the color, (0-255)
@@ -158,15 +160,15 @@
         white = int(max(min(white, 255), 0))
 
         # INVOKE <id> RGBLoad.SetRGBW <red> <green> <blue> <white>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetRGBW <red> <green> <blue> <white>
         await self.invoke(vid, "RGBLoad.SetRGBW", red, green, blue, white)
 
     async def set_hsl(
-        self, vid: int, hue: int, saturation: int, lightness: int
+        self, vid: int, hue: float, saturation: float, lightness: float
     ) -> None:
         """Set the color of an HSL load.
 
         Args:
             vid: The Vantage ID of the RGB load.
             hue: The hue value of the color, in degrees (0-360).
             saturation: The saturation value of the color, in percent (0-100).
@@ -179,15 +181,15 @@
         lightness = int(max(min(lightness, 100), 0))
 
         # INVOKE <id> RGBLoad.SetHSL <hue> <saturation> <lightness>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetHSL <hue> <saturation> <lightness>
         await self.invoke(vid, "RGBLoad.SetHSL", hue, saturation, lightness)
 
     async def dissolve_rgb(
-        self, vid: int, red: int, green: int, blue: int, seconds: int
+        self, vid: int, red: float, green: float, blue: float, seconds: float
     ) -> None:
         """Transition the color of an RGB load over a number of seconds.
 
         Args:
             vid: The Vantage ID of the RGB load.
             red: The new red value of the color, (0-255)
             green: The new green value of the color, (0-255)
@@ -200,16 +202,33 @@
         green = int(max(min(green, 255), 0))
         blue = int(max(min(blue, 255), 0))
 
         # INVOKE <id> RGBLoad.DissolveRGB <red> <green> <blue>
         # -> R:INVOKE <id> <rcode> RGBLoad.DissolveRGB <red> <green> <blue>
         await self.invoke(vid, "RGBLoad.DissolveRGB", red, green, blue, seconds)
 
+    async def set_rgb_component(self, vid: int, channel: int, value: float) -> None:
+        """
+        Set a single RGB(W) color channel of a load.
+
+        Args:
+            vid: The Vantage ID of the RGB load.
+            channel: The channel to set the color of.
+            value: The value to set the channel to, 0-255.
+        """
+
+        # Clamp levels to 0-255, ensure they're integers
+        value = int(max(min(value, 255), 0))
+
+        # INVOKE <id> RGBLoad.SetRGBComponent <channel> <value>
+        # -> R:INVOKE <id> <rcode> RGBLoad.SetRGBComponent <channel> <value>
+        await self.invoke(vid, "RGBLoad.SetRGBComponent", channel, value)
+
     async def dissolve_hsl(
-        self, vid: int, hue: int, saturation: int, lightness: int, seconds: int
+        self, vid: int, hue: float, saturation: float, lightness: float, seconds: float
     ) -> None:
         """Transition the color of an HSL load over a number of seconds.
 
         Args:
             vid: The Vantage ID of the RGB load.
             hue: The new hue value of the color, in degrees (0-360).
             saturation: The new saturation value of the color, in percent (0-100).
```

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/sounder.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/sounder.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/temperature.py` & `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/README.md` & `aiovantage-0.4.0/src/aiovantage/config_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/__init__.py` & `aiovantage-0.4.0/src/aiovantage/config_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/helpers.py` & `aiovantage-0.4.0/src/aiovantage/config_client/helpers.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.4.0/src/aiovantage/config_client/xml_dataclass.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,11 +33,11 @@
 
     return field(metadata=metadata, **kwargs)
 
 
 def xml_tag_from_class(cls: Type[Any]) -> str:
     """Get the XML tag name for a class."""
 
-    meta = cls.Meta if "Meta" in cls.__dict__ else None
+    meta = getattr(cls, "Meta", None)
     name = getattr(meta, "name", cls.__qualname__)
 
     return name
```

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/methods/types.py` & `aiovantage-0.4.0/src/aiovantage/config_client/methods/types.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/open_filter.py` & `aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.4.0/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/methods/login/login.py` & `aiovantage-0.4.0/src/aiovantage/config_client/methods/login/login.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.4.0/src/aiovantage/config_client/objects/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from .gmem import GMem
 from .keypad import Keypad
 from .light_sensor import LightSensor
 from .load import Load
 from .load_group import LoadGroup
 from .location_object import LocationObject
 from .master import Master
+from .module import Module
+from .module_gen2 import ModuleGen2
 from .omni_sensor import OmniSensor
 from .power_profile import PowerProfile
 from .pwm_power_profile import PWMPowerProfile
 from .qis_blind import QISBlind
 from .qube_blind import QubeBlind
 from .relay_blind import RelayBlind
 from .rgb_load import RGBLoad
@@ -56,14 +58,16 @@
     "GMem",
     "Keypad",
     "LightSensor",
     "Load",
     "LoadGroup",
     "LocationObject",
     "Master",
+    "Module",
+    "ModuleGen2",
     "OmniSensor",
     "PowerProfile",
     "PWMPowerProfile",
     "QISBlind",
     "QubeBlind",
     "RelayBlind",
     "RGBLoad",
```

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.4.0/src/aiovantage/config_client/objects/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.4.0/src/aiovantage/config_client/objects/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.4.0/src/aiovantage/config_client/objects/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.4.0/src/aiovantage/config_client/objects/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.4.0/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.4.0/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 """RGB load object."""
 
 from dataclasses import dataclass
-from enum import Enum
+from enum import Enum, IntEnum
 from typing import Optional, Tuple
 
 from aiovantage.config_client.xml_dataclass import xml_element
 
 from .location_object import LocationObject
 
 # This isn't strictly a Vantage object type, but this helps us avoid
 # code duplication in RGBLoad-like objects.
 
 
 @dataclass
 class RGBLoad(LocationObject):
     """RGB load object."""
 
+    class RGBChannel(IntEnum):
+        """RGB channel."""
+
+        RED = 0
+        GREEN = 1
+        BLUE = 2
+        WHITE = 3
+
+    class HSLAttribute(IntEnum):
+        """HSL attribute."""
+
+        HUE = 0
+        SATURATION = 1
+        LEVEL = 2
+
     class ColorType(Enum):
         """Color type."""
 
         RGB = "RGB"
         RGBW = "RGBW"
         HSL = "HSL"
         HSIC = "HSIC"
```

### Comparing `aiovantage-0.3.0/src/aiovantage/config_client/objects/system_object.py` & `aiovantage-0.4.0/src/aiovantage/config_client/objects/system_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/anemo_sensors.py` & `aiovantage-0.4.0/src/aiovantage/controllers/anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/base.py` & `aiovantage-0.4.0/src/aiovantage/controllers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,44 +208,47 @@
         """
 
         if self._initialized:
             return
 
         await self.fetch_objects()
         await self.fetch_full_state()
-        self.subscribe_to_updates()
+        await self.subscribe_to_updates()
 
         self.event_stream.subscribe(self._handle_event, EventType.RECONNECTED)
 
         self._initialized = True
 
     async def fetch_full_state(self) -> None:
         """Fetch the full state of all objects managed by this controller."""
 
         await asyncio.gather(
             *[self.fetch_object_state(obj.id) for obj in self._items.values()]
         )
 
         self._logger.info("%s fetched full state", self.__class__.__name__)
 
-    def subscribe_to_updates(self) -> None:
+    async def subscribe_to_updates(self) -> None:
         """Subscribe to state updates for objects managed by this controller."""
 
         if not self._items:
             return
 
+        # Ensure that the event stream is running
+        await self.event_stream.start()
+
         # Subscribe to "STATUS {type}" updates, if this controller cares about them
         if self.status_types:
-            for status_type in self.status_types:
-                self.event_stream.subscribe_status(self._handle_event, status_type)
+            self.event_stream.subscribe_status(self._handle_event, self.status_types)
 
         # Subscribe to object status events from the "Enhanced Log"
         if self.enhanced_log_status:
-            self.event_stream.subscribe_enhanced_log(self._handle_event, "STATUS")
-            self.event_stream.subscribe_enhanced_log(self._handle_event, "STATUSEX")
+            self.event_stream.subscribe_enhanced_log(
+                self._handle_event, ("STATUS", "STATUSEX")
+            )
 
         self._logger.info("%s subscribed to updates", self.__class__.__name__)
 
     def update_state(self, vid: int, state: Dict[str, Any]) -> None:
         """Update the state of an object and notify subscribers if it changed.
 
         Args:
```

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.4.0/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/blinds.py` & `aiovantage-0.4.0/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/buttons.py` & `aiovantage-0.4.0/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.4.0/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/gmem.py` & `aiovantage-0.4.0/src/aiovantage/controllers/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/light_sensors.py` & `aiovantage-0.4.0/src/aiovantage/controllers/light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.4.0/src/aiovantage/controllers/load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/loads.py` & `aiovantage-0.4.0/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.4.0/src/aiovantage/controllers/omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.4.0/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/tasks.py` & `aiovantage-0.4.0/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/src/aiovantage/controllers/temperature_sensors.py` & `aiovantage-0.4.0/src/aiovantage/controllers/temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/LICENSE` & `aiovantage-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.3.0/README.md` & `aiovantage-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,36 +2,34 @@
 
 aiovantage is a Python library for interacting with and controlling Vantage InFusion home automation controllers.
 
 Uses a "controller" pattern inspired heavily by the [aiohue](https://github.com/home-assistant-libs/aiohue) library.
 
 This open-source, non-commercial library is not affiliated, associated, authorized, endorsed by, or in any way officially connected with Vantage, and is provided for interoperability purposes only.
 
-
 ## Example
 
 ```python
 from aiovantage import Vantage
 
 async with Vantage("192.168.1.2", "username", "password") as vantage:
     async for load in vantage.loads:
         print(f"{load.name} is at {load.level}%")
 ```
 
 See the [examples](examples) folder for more examples.
 
-
 ## Features
+
 - Uses Python asyncio for non-blocking I/O.
 - Exposes "controllers" to make fetching and controlling various objects easy.
 - Uses SSL connections by default, with automatic reconnection.
 - Fetch objects lazily (with `async for obj in controller`).
 - Alternatively, eager-fetch objects with `controller.initialize`.
 
-
 ## Supported objects types
 
 The following interfaces/controllers are currently supported.
 
 | Type          | Description           | Controller                    | Examples                                  |
 | ------------- | --------------------- | ----------------------------- | ----------------------------------------- |
 | AnemoSensor   | Wind speed sensors    | `vantage.anemo_sensors`       | [Examples](examples/anemo_sensors)        |
@@ -48,13 +46,12 @@
 | RGBLoad       | RGB lights            | `vantage.rgb_loads`           | [Examples](examples/rgb_loads)            |
 | Stations      | Keypads, etc          | `vantage.stations`            | [Examples](examples/stations)             |
 | Tasks         | Vantage tasks         | `vantage.tasks`               | [Examples](examples/tasks)                |
 | Temperature   | Temperature sensors   | `vantage.temperature_sensors` | [Examples](examples/temperature_sensors)  |
 
 If you have an object that you expect to show up in one of these controllers, but it is missing, please let me know in an issue.
 
-
 ## Installation
 
 ```shell
 pip3 install aiovantage
-```
+```
```

### Comparing `aiovantage-0.3.0/pyproject.toml` & `aiovantage-0.4.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -16,51 +16,53 @@
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "xsdata==23.5",
+    "xsdata==23.6",
     "typing_extensions>=4.6.3,<5.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/loopj/aiovantage#readme"
 Issues = "https://github.com/loopj/aiovantage/issues"
 Source = "https://github.com/loopj/aiovantage"
 
+[project.optional-dependencies]
+dev = [
+    "black==23.3.0",
+    "mypy==1.4.1",
+    "ruff==0.0.275",
+    "pre-commit==3.3.3",
+]
+
 [tool.hatch.version]
 path = "src/aiovantage/__about__.py"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 
+[tool.hatch.envs.dev]
+features = ["dev"]
+
 [tool.hatch.envs.lint]
-dependencies = [
-  "black==23.3.0",
-  "mypy==1.4.0",
-  "ruff==0.0.272",
-]
+features = ["dev"]
 
 [tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:.}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
 fmt = [
   "black {args:.}",
   "ruff --fix {args:.}",
-  "style",
-]
-all = [
-  "style",
-  "typing",
 ]
+typing = "mypy {args:.}"
 
 [tool.mypy]
 strict = true
 
 [tool.black]
 target-version = ["py38"]
 skip-string-normalization = true
```

### Comparing `aiovantage-0.3.0/PKG-INFO` & `aiovantage-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.3.0
+Version: 0.4.0
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions<5.0,>=4.6.3
-Requires-Dist: xsdata==23.5
+Requires-Dist: xsdata==23.6
+Provides-Extra: dev
+Requires-Dist: black==23.3.0; extra == 'dev'
+Requires-Dist: mypy==1.4.1; extra == 'dev'
+Requires-Dist: pre-commit==3.3.3; extra == 'dev'
+Requires-Dist: ruff==0.0.275; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # aiovantage
 
 aiovantage is a Python library for interacting with and controlling Vantage InFusion home automation controllers.
 
 Uses a "controller" pattern inspired heavily by the [aiohue](https://github.com/home-assistant-libs/aiohue) library.
 
 This open-source, non-commercial library is not affiliated, associated, authorized, endorsed by, or in any way officially connected with Vantage, and is provided for interoperability purposes only.
 
-
 ## Example
 
 ```python
 from aiovantage import Vantage
 
 async with Vantage("192.168.1.2", "username", "password") as vantage:
     async for load in vantage.loads:
         print(f"{load.name} is at {load.level}%")
 ```
 
 See the [examples](examples) folder for more examples.
 
-
 ## Features
+
 - Uses Python asyncio for non-blocking I/O.
 - Exposes "controllers" to make fetching and controlling various objects easy.
 - Uses SSL connections by default, with automatic reconnection.
 - Fetch objects lazily (with `async for obj in controller`).
 - Alternatively, eager-fetch objects with `controller.initialize`.
 
-
 ## Supported objects types
 
 The following interfaces/controllers are currently supported.
 
 | Type          | Description           | Controller                    | Examples                                  |
 | ------------- | --------------------- | ----------------------------- | ----------------------------------------- |
 | AnemoSensor   | Wind speed sensors    | `vantage.anemo_sensors`       | [Examples](examples/anemo_sensors)        |
@@ -68,13 +71,12 @@
 | RGBLoad       | RGB lights            | `vantage.rgb_loads`           | [Examples](examples/rgb_loads)            |
 | Stations      | Keypads, etc          | `vantage.stations`            | [Examples](examples/stations)             |
 | Tasks         | Vantage tasks         | `vantage.tasks`               | [Examples](examples/tasks)                |
 | Temperature   | Temperature sensors   | `vantage.temperature_sensors` | [Examples](examples/temperature_sensors)  |
 
 If you have an object that you expect to show up in one of these controllers, but it is missing, please let me know in an issue.
 
-
 ## Installation
 
 ```shell
 pip3 install aiovantage
-```
+```
```

