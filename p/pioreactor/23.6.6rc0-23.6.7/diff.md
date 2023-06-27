# Comparing `tmp/pioreactor-23.6.6rc0-py3-none-any.whl.zip` & `tmp/pioreactor-23.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,85 +1,85 @@
-Zip file size: 185146 bytes, number of entries: 83
--rw-r--r--  2.0 unx      117 b- defN 23-Jun-06 19:35 pioreactor/__init__.py
--rw-r--r--  2.0 unx     6834 b- defN 23-Jun-06 19:35 pioreactor/config.py
--rw-r--r--  2.0 unx      265 b- defN 23-Jun-06 19:35 pioreactor/error_codes.py
--rw-r--r--  2.0 unx      443 b- defN 23-Jun-06 19:35 pioreactor/exc.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Jun-06 19:35 pioreactor/hardware.py
--rw-r--r--  2.0 unx     6614 b- defN 23-Jun-06 19:35 pioreactor/logging.py
--rw-r--r--  2.0 unx    14871 b- defN 23-Jun-06 19:35 pioreactor/mureq.py
--rw-r--r--  2.0 unx    12957 b- defN 23-Jun-06 19:35 pioreactor/pubsub.py
--rw-r--r--  2.0 unx     6400 b- defN 23-Jun-06 19:35 pioreactor/structs.py
--rw-r--r--  2.0 unx     2724 b- defN 23-Jun-06 19:35 pioreactor/types.py
--rw-r--r--  2.0 unx     2155 b- defN 23-Jun-06 19:35 pioreactor/version.py
--rw-r--r--  2.0 unx     3654 b- defN 23-Jun-06 19:35 pioreactor/whoami.py
--rw-r--r--  2.0 unx      540 b- defN 23-Jun-06 19:35 pioreactor/actions/__init__.py
--rw-r--r--  2.0 unx     8743 b- defN 23-Jun-06 19:35 pioreactor/actions/led_intensity.py
--rw-r--r--  2.0 unx     7755 b- defN 23-Jun-06 19:35 pioreactor/actions/od_blank.py
--rw-r--r--  2.0 unx    20343 b- defN 23-Jun-06 19:35 pioreactor/actions/od_calibration.py
--rw-r--r--  2.0 unx    17612 b- defN 23-Jun-06 19:35 pioreactor/actions/pump.py
--rw-r--r--  2.0 unx    21362 b- defN 23-Jun-06 19:35 pioreactor/actions/pump_calibration.py
--rw-r--r--  2.0 unx    16662 b- defN 23-Jun-06 19:35 pioreactor/actions/self_test.py
--rw-r--r--  2.0 unx     5175 b- defN 23-Jun-06 19:35 pioreactor/actions/stirring_calibration.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 19:35 pioreactor/actions/leader/__init__.py
--rw-r--r--  2.0 unx     4744 b- defN 23-Jun-06 19:35 pioreactor/actions/leader/backup_database.py
--rw-r--r--  2.0 unx     7151 b- defN 23-Jun-06 19:35 pioreactor/actions/leader/experiment_profile.py
--rw-r--r--  2.0 unx     6426 b- defN 23-Jun-06 19:35 pioreactor/actions/leader/export_experiment_data.py
--rw-r--r--  2.0 unx      445 b- defN 23-Jun-06 19:35 pioreactor/automations/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/__init__.py
--rw-r--r--  2.0 unx    28416 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/base.py
--rw-r--r--  2.0 unx     1404 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/chemostat.py
--rw-r--r--  2.0 unx     1194 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/fed_batch.py
--rw-r--r--  2.0 unx     2724 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/morbidostat.py
--rw-r--r--  2.0 unx     4880 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/pid_morbidostat.py
--rw-r--r--  2.0 unx      468 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/silent.py
--rw-r--r--  2.0 unx     2252 b- defN 23-Jun-06 19:35 pioreactor/automations/dosing/turbidostat.py
--rw-r--r--  2.0 unx      510 b- defN 23-Jun-06 19:35 pioreactor/automations/events/__init__.py
--rw-r--r--  2.0 unx      473 b- defN 23-Jun-06 19:35 pioreactor/automations/led/__init__.py
--rw-r--r--  2.0 unx    11851 b- defN 23-Jun-06 19:35 pioreactor/automations/led/base.py
--rw-r--r--  2.0 unx     3136 b- defN 23-Jun-06 19:35 pioreactor/automations/led/light_dark_cycle.py
--rw-r--r--  2.0 unx      205 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/__init__.py
--rw-r--r--  2.0 unx     9722 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/base.py
--rw-r--r--  2.0 unx      674 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/constant_duty_cycle.py
--rw-r--r--  2.0 unx      517 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/only_record_temperature.py
--rw-r--r--  2.0 unx     4314 b- defN 23-Jun-06 19:35 pioreactor/automations/temperature/thermostat.py
--rw-r--r--  2.0 unx      715 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/__init__.py
--rw-r--r--  2.0 unx    42618 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/base.py
--rw-r--r--  2.0 unx     6854 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/dosing_control.py
--rw-r--r--  2.0 unx    20221 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/growth_rate_calculating.py
--rw-r--r--  2.0 unx     5488 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/led_control.py
--rw-r--r--  2.0 unx    24314 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/monitor.py
--rw-r--r--  2.0 unx    47033 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/od_reading.py
--rw-r--r--  2.0 unx    17549 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/stirring.py
--rw-r--r--  2.0 unx    25723 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/temperature_control.py
--rw-r--r--  2.0 unx      605 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/leader/__init__.py
--rw-r--r--  2.0 unx    16280 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
--rw-r--r--  2.0 unx     3829 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/leader/watchdog.py
--rw-r--r--  2.0 unx      609 b- defN 23-Jun-06 19:35 pioreactor/background_jobs/subjobs/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 19:35 pioreactor/cli/__init__.py
--rw-r--r--  2.0 unx    29643 b- defN 23-Jun-06 19:35 pioreactor/cli/pio.py
--rw-r--r--  2.0 unx    22314 b- defN 23-Jun-06 19:35 pioreactor/cli/pios.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 19:35 pioreactor/experiment_profiles/__init__.py
--rw-r--r--  2.0 unx      963 b- defN 23-Jun-06 19:35 pioreactor/experiment_profiles/profile_struct.py
--rw-r--r--  2.0 unx     3517 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/__init__.py
--rw-r--r--  2.0 unx     1316 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/install_plugin.py
--rw-r--r--  2.0 unx     1086 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/list_plugins.py
--rw-r--r--  2.0 unx     1605 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/uninstall_plugin.py
--rw-r--r--  2.0 unx      792 b- defN 23-Jun-06 19:35 pioreactor/plugin_management/utils.py
--rw-r--r--  2.0 unx    10951 b- defN 23-Jun-06 19:35 pioreactor/utils/__init__.py
--rw-r--r--  2.0 unx     4096 b- defN 23-Jun-06 19:35 pioreactor/utils/adcs.py
--rw-r--r--  2.0 unx     1930 b- defN 23-Jun-06 19:35 pioreactor/utils/dacs.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jun-06 19:35 pioreactor/utils/gpio_helpers.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jun-06 19:35 pioreactor/utils/math_helpers.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Jun-06 19:35 pioreactor/utils/mock.py
--rw-r--r--  2.0 unx     3951 b- defN 23-Jun-06 19:35 pioreactor/utils/networking.py
--rw-r--r--  2.0 unx     7559 b- defN 23-Jun-06 19:35 pioreactor/utils/pwm.py
--rw-r--r--  2.0 unx     3393 b- defN 23-Jun-06 19:35 pioreactor/utils/rpi_bad_power.py
--rw-r--r--  2.0 unx     7749 b- defN 23-Jun-06 19:35 pioreactor/utils/sqlite_worker.py
--rw-r--r--  2.0 unx    15186 b- defN 23-Jun-06 19:35 pioreactor/utils/streaming_calculations.py
--rw-r--r--  2.0 unx     5614 b- defN 23-Jun-06 19:35 pioreactor/utils/timing.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3896 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7674 b- defN 23-Jun-06 19:35 pioreactor-23.6.6rc0.dist-info/RECORD
-83 files, 604612 bytes uncompressed, 172794 bytes compressed:  71.4%
+Zip file size: 185139 bytes, number of entries: 83
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-07 16:33 pioreactor/__init__.py
+-rw-r--r--  2.0 unx     6834 b- defN 23-Jun-07 16:33 pioreactor/config.py
+-rw-r--r--  2.0 unx      265 b- defN 23-Jun-07 16:33 pioreactor/error_codes.py
+-rw-r--r--  2.0 unx      443 b- defN 23-Jun-07 16:33 pioreactor/exc.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jun-07 16:33 pioreactor/hardware.py
+-rw-r--r--  2.0 unx     6614 b- defN 23-Jun-07 16:33 pioreactor/logging.py
+-rw-r--r--  2.0 unx    14871 b- defN 23-Jun-07 16:33 pioreactor/mureq.py
+-rw-r--r--  2.0 unx    12957 b- defN 23-Jun-07 16:33 pioreactor/pubsub.py
+-rw-r--r--  2.0 unx     6400 b- defN 23-Jun-07 16:33 pioreactor/structs.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jun-07 16:33 pioreactor/types.py
+-rw-r--r--  2.0 unx     2152 b- defN 23-Jun-07 16:33 pioreactor/version.py
+-rw-r--r--  2.0 unx     3654 b- defN 23-Jun-07 16:33 pioreactor/whoami.py
+-rw-r--r--  2.0 unx      540 b- defN 23-Jun-07 16:33 pioreactor/actions/__init__.py
+-rw-r--r--  2.0 unx     8743 b- defN 23-Jun-07 16:33 pioreactor/actions/led_intensity.py
+-rw-r--r--  2.0 unx     7755 b- defN 23-Jun-07 16:33 pioreactor/actions/od_blank.py
+-rw-r--r--  2.0 unx    20343 b- defN 23-Jun-07 16:33 pioreactor/actions/od_calibration.py
+-rw-r--r--  2.0 unx    17612 b- defN 23-Jun-07 16:33 pioreactor/actions/pump.py
+-rw-r--r--  2.0 unx    21362 b- defN 23-Jun-07 16:33 pioreactor/actions/pump_calibration.py
+-rw-r--r--  2.0 unx    16662 b- defN 23-Jun-07 16:33 pioreactor/actions/self_test.py
+-rw-r--r--  2.0 unx     5175 b- defN 23-Jun-07 16:33 pioreactor/actions/stirring_calibration.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 16:33 pioreactor/actions/leader/__init__.py
+-rw-r--r--  2.0 unx     4744 b- defN 23-Jun-07 16:33 pioreactor/actions/leader/backup_database.py
+-rw-r--r--  2.0 unx     7151 b- defN 23-Jun-07 16:33 pioreactor/actions/leader/experiment_profile.py
+-rw-r--r--  2.0 unx     6426 b- defN 23-Jun-07 16:33 pioreactor/actions/leader/export_experiment_data.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Jun-07 16:33 pioreactor/automations/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/__init__.py
+-rw-r--r--  2.0 unx    28416 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/base.py
+-rw-r--r--  2.0 unx     1404 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/chemostat.py
+-rw-r--r--  2.0 unx     1194 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/fed_batch.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/morbidostat.py
+-rw-r--r--  2.0 unx     4880 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/pid_morbidostat.py
+-rw-r--r--  2.0 unx      468 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/silent.py
+-rw-r--r--  2.0 unx     2252 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/turbidostat.py
+-rw-r--r--  2.0 unx      510 b- defN 23-Jun-07 16:33 pioreactor/automations/events/__init__.py
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-07 16:33 pioreactor/automations/led/__init__.py
+-rw-r--r--  2.0 unx    11851 b- defN 23-Jun-07 16:33 pioreactor/automations/led/base.py
+-rw-r--r--  2.0 unx     3136 b- defN 23-Jun-07 16:33 pioreactor/automations/led/light_dark_cycle.py
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/__init__.py
+-rw-r--r--  2.0 unx     9722 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/base.py
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/constant_duty_cycle.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/only_record_temperature.py
+-rw-r--r--  2.0 unx     4314 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/thermostat.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/__init__.py
+-rw-r--r--  2.0 unx    42618 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/base.py
+-rw-r--r--  2.0 unx     6854 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/dosing_control.py
+-rw-r--r--  2.0 unx    20221 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/growth_rate_calculating.py
+-rw-r--r--  2.0 unx     5488 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/led_control.py
+-rw-r--r--  2.0 unx    24314 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/monitor.py
+-rw-r--r--  2.0 unx    47033 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/od_reading.py
+-rw-r--r--  2.0 unx    17577 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/stirring.py
+-rw-r--r--  2.0 unx    25723 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/temperature_control.py
+-rw-r--r--  2.0 unx      605 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/leader/__init__.py
+-rw-r--r--  2.0 unx    16280 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
+-rw-r--r--  2.0 unx     3829 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/leader/watchdog.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/subjobs/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 16:33 pioreactor/cli/__init__.py
+-rw-r--r--  2.0 unx    29779 b- defN 23-Jun-07 16:33 pioreactor/cli/pio.py
+-rw-r--r--  2.0 unx    22314 b- defN 23-Jun-07 16:33 pioreactor/cli/pios.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 16:33 pioreactor/experiment_profiles/__init__.py
+-rw-r--r--  2.0 unx      963 b- defN 23-Jun-07 16:33 pioreactor/experiment_profiles/profile_struct.py
+-rw-r--r--  2.0 unx     3517 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/__init__.py
+-rw-r--r--  2.0 unx     1316 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/install_plugin.py
+-rw-r--r--  2.0 unx     1086 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/list_plugins.py
+-rw-r--r--  2.0 unx     1605 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/uninstall_plugin.py
+-rw-r--r--  2.0 unx      792 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/utils.py
+-rw-r--r--  2.0 unx    10951 b- defN 23-Jun-07 16:33 pioreactor/utils/__init__.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Jun-07 16:33 pioreactor/utils/adcs.py
+-rw-r--r--  2.0 unx     1930 b- defN 23-Jun-07 16:33 pioreactor/utils/dacs.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-07 16:33 pioreactor/utils/gpio_helpers.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jun-07 16:33 pioreactor/utils/math_helpers.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Jun-07 16:33 pioreactor/utils/mock.py
+-rw-r--r--  2.0 unx     3951 b- defN 23-Jun-07 16:33 pioreactor/utils/networking.py
+-rw-r--r--  2.0 unx     7559 b- defN 23-Jun-07 16:33 pioreactor/utils/pwm.py
+-rw-r--r--  2.0 unx     3393 b- defN 23-Jun-07 16:33 pioreactor/utils/rpi_bad_power.py
+-rw-r--r--  2.0 unx     7749 b- defN 23-Jun-07 16:33 pioreactor/utils/sqlite_worker.py
+-rw-r--r--  2.0 unx    15186 b- defN 23-Jun-07 16:33 pioreactor/utils/streaming_calculations.py
+-rw-r--r--  2.0 unx     5614 b- defN 23-Jun-07 16:33 pioreactor/utils/timing.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3893 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7656 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/RECORD
+83 files, 604752 bytes uncompressed, 172823 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -225,26 +225,26 @@
 
 Filename: pioreactor/utils/streaming_calculations.py
 Comment: 
 
 Filename: pioreactor/utils/timing.py
 Comment: 
 
-Filename: pioreactor-23.6.6rc0.dist-info/LICENSE
+Filename: pioreactor-23.6.7.dist-info/LICENSE
 Comment: 
 
-Filename: pioreactor-23.6.6rc0.dist-info/METADATA
+Filename: pioreactor-23.6.7.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor-23.6.6rc0.dist-info/WHEEL
+Filename: pioreactor-23.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor-23.6.6rc0.dist-info/entry_points.txt
+Filename: pioreactor-23.6.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor-23.6.6rc0.dist-info/top_level.txt
+Filename: pioreactor-23.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor-23.6.6rc0.dist-info/RECORD
+Filename: pioreactor-23.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor/version.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import os
 
 # Append "dev" if a dev version
 # Append "rc0" if a rc version
-__version__ = "23.6.6rc0"
+__version__ = "23.6.7"
 
 
 def _get_hardware_version() -> tuple[int, int] | tuple[int, int, str]:
     if os.environ.get("HARDWARE") is not None:
         # ex: > HARDWARE=1.1 pio ...
         return int(os.environ["HARDWARE"].split(".")[0]), int(os.environ["HARDWARE"].split(".")[1])
```

## pioreactor/background_jobs/stirring.py

```diff
@@ -374,15 +374,15 @@
                 self.kick_stirring_but_avoid_od_reading()
 
         return self.measured_rpm
 
     def poll_and_update_dc(self, poll_for_seconds: float = 4) -> None:
         self.poll(poll_for_seconds)
 
-        if self._measured_rpm is None:
+        if self._measured_rpm is None or self.state != self.READY:
             return
 
         result = self.pid.update(self._measured_rpm)
         self.set_duty_cycle(self.duty_cycle + result)
 
     def on_ready_to_sleeping(self) -> None:
         self.rpm_check_repeated_thread.pause()
@@ -421,15 +421,15 @@
 
         Returns
         --------
         bool: True if successfully waited until RPM is correct.
 
         """
         running_wait_time = 0.0
-        sleep_time = 0.5
+        sleep_time = 0.2
 
         if (self.rpm_calculator is None) or is_testing_env():
             # can't block if we aren't recording the RPM
             return False
 
         assert isinstance(self.target_rpm, float)
         self.logger.debug(f"stirring is blocking until RPM is near {self.target_rpm}.")
```

## pioreactor/cli/pio.py

```diff
@@ -460,17 +460,20 @@
                 f"sudo pip3 install -U --force-reinstall https://github.com/pioreactor/pioreactor/archive/{branch}.zip",
                 1,
             )
         )
 
     else:
         tag = get_tag_to_install(version)
-        release_metadata = loads(
-            get(f"https://api.github.com/repos/pioreactor/pioreactor/releases/{tag}").body
-        )
+        response = get(f"https://api.github.com/repos/pioreactor/pioreactor/releases/{tag}")
+        if response.raise_for_status():
+            logger.error(f"Version {version} not found")
+            raise click.Abort()
+
+        release_metadata = loads(response.body)
         version_installed = release_metadata["tag_name"]
         for asset in release_metadata["assets"]:
             # add the following files to the release. They should ideally be idempotent!
 
             # pre_update.sh runs (if exists)
             # `pip install pioreactor...whl` runs
             # update.sh runs (if exists)
```

## Comparing `pioreactor-23.6.6rc0.dist-info/LICENSE` & `pioreactor-23.6.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pioreactor-23.6.6rc0.dist-info/METADATA` & `pioreactor-23.6.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioreactor
-Version: 23.6.6rc0
+Version: 23.6.7
 Summary: The core Python app of the Pioreactor. Control your bioreactor through Python.
 Home-page: https://github.com/pioreactor/pioreactor
 Author: Pioreactor
 Author-email: hello@pioreactor.com
 License: MIT
 Keywords: microbiology,bioreactor,turbidostat,raspberry pi,education,research
 Classifier: Topic :: Scientific/Engineering
```

## Comparing `pioreactor-23.6.6rc0.dist-info/RECORD` & `pioreactor-23.6.7.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pioreactor/exc.py,sha256=GvNp0vvgeAclxB2eIGZMnhYU3bFIYKz_AGOU9hKYstM,443
 pioreactor/hardware.py,sha256=c7IpkPCcsxtfvgUSpxv3TCltzCVSsIybDGzuWTn6N8g,3105
 pioreactor/logging.py,sha256=rVyqqxwv2voS-TMpTodnTHAI-QkhEp_I4bau9gHmMcU,6614
 pioreactor/mureq.py,sha256=XYpmNoMTqBIrtfZ_mKbfDEyLYRAeBBH29Zl5zy72iwA,14871
 pioreactor/pubsub.py,sha256=Twu4EJBTLwgObVog4ZGujbbgTGXx6TTG33EOSktFvnU,12957
 pioreactor/structs.py,sha256=eRLqrO6ldJftnXPzxzz8CoQHwnvK4W9RgniJfchUoeA,6400
 pioreactor/types.py,sha256=l5JwLlj9YFcq1RC-IrIPsBaGwwFuNs1GAputHLwl1aI,2724
-pioreactor/version.py,sha256=kQvKIPX228p_uZh_CbOXt8OHFj86ot0ntYH1Q1lcg94,2155
+pioreactor/version.py,sha256=R9kZBsa0Nk01JR_pNbg2E9V_WY7_enuLmZByXiV806k,2152
 pioreactor/whoami.py,sha256=LnY7lP6oj89eiiR1CC1jCS9z3Ahbil2Qf7az1HRARYA,3654
 pioreactor/actions/__init__.py,sha256=VuwIL8llFFqBspvBRgC9yNm-Blu9tsE2kwgIJEs786o,540
 pioreactor/actions/led_intensity.py,sha256=C705sRk7_rQsdlgmYC8YB_w3Iq30aSeJ_Bq2QHhGJAQ,8743
 pioreactor/actions/od_blank.py,sha256=-4k03BQC1i0T3rMQUicicKBufzYRC4QZD829P_XRu-Q,7755
 pioreactor/actions/od_calibration.py,sha256=YOXDPz-8gpxeq2dCv93TgF3i7UluhonRc-bCd5TPAUM,20343
 pioreactor/actions/pump.py,sha256=iVAVqzNSJKWfj1thiJMAV04SSSOV20k8bb7BA7dEOZo,17612
 pioreactor/actions/pump_calibration.py,sha256=SdnQ2AWbVNEdWtG00cxG_TtkYSNc_4RHDAxfH_cE0sM,21362
@@ -43,22 +43,22 @@
 pioreactor/background_jobs/__init__.py,sha256=pn23vImMyfiHjbdKObOWpAwzNUbE1xnHWUYk4j4KSJM,715
 pioreactor/background_jobs/base.py,sha256=bDgxdKwDuZxf3L6DoZ6EC0BLKaMEU27zW6FkcKa7yQk,42618
 pioreactor/background_jobs/dosing_control.py,sha256=UJL5ngBzrNXb_B3tLJ4kpxSBL1PWEb_fL0qWdYgqMXA,6854
 pioreactor/background_jobs/growth_rate_calculating.py,sha256=96rGFwc9x7VGdWYlhyNMseNwPQQgBGXXeBzHhrcJHC0,20221
 pioreactor/background_jobs/led_control.py,sha256=prQEPE1xZbwadbKZtoBUzFvlmUjqcUGZ_4_DgGl63Us,5488
 pioreactor/background_jobs/monitor.py,sha256=uRiiNOW37stQefbZK7QyWpJxpOu5FMMMTP6kiMRbx3c,24314
 pioreactor/background_jobs/od_reading.py,sha256=jCH83AtT6F5Mdr6l5HF_rmGHvSgmpYfq6PEFmpreoGc,47033
-pioreactor/background_jobs/stirring.py,sha256=85piGolJueIHvm6Zj3Yx94bzPwsRXz8xbgIPWi6h7Eg,17549
+pioreactor/background_jobs/stirring.py,sha256=FE-b7Yblk0_FFczNnSKXu71S4-7oU6ciZDH1ppTYkt4,17577
 pioreactor/background_jobs/temperature_control.py,sha256=iYSkpei3fJLviFkBEzeBf2qRiKaIADwGGkPQWfcSewk,25723
 pioreactor/background_jobs/leader/__init__.py,sha256=Uhl2Xksfkf06lmfmz2scTxmBWDBnwkA9rSil_V94aWQ,605
 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py,sha256=UM4_L-cesPGfj9wws-16GrmHEvTbBOhOmJAmxKGD7E0,16280
 pioreactor/background_jobs/leader/watchdog.py,sha256=ZJmDVqYFWrMis_riJcW6ui27s6EHZJIbdEMUoeAYXvQ,3829
 pioreactor/background_jobs/subjobs/__init__.py,sha256=pT1lJJp3c4rHSXCdBKc662uQR591Xhp16oeDpDMKEKc,609
 pioreactor/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pioreactor/cli/pio.py,sha256=-z9qLXSjJ640PdXqwXFZhxlROv1xNlS0-h9XjIELy2U,29643
+pioreactor/cli/pio.py,sha256=6qs1WohIGqS2gD46ddNC7EvaPsMvsT9nQ2xkw5ioNmc,29779
 pioreactor/cli/pios.py,sha256=JroU6VqB20Dw97-1S-Rgg2UhlxkAWi1i7kQ3qR0M6II,22314
 pioreactor/experiment_profiles/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pioreactor/experiment_profiles/profile_struct.py,sha256=D_S8vRHjt_Us40FcQpuJunWdVmxD-6Q20Kvh89yrWW4,963
 pioreactor/plugin_management/__init__.py,sha256=MSu2s9kI7osSxBwKK1MQTcyw9sdabPvH2xCKnkNk16c,3517
 pioreactor/plugin_management/install_plugin.py,sha256=i3KchEps5cafvuhADOLacaziL9UpuoDvMnvDVBaTCuw,1316
 pioreactor/plugin_management/list_plugins.py,sha256=blTAKhlsJJ4cwyR0_HWjC_fP0xcIUNFIJWY21moewaM,1086
 pioreactor/plugin_management/uninstall_plugin.py,sha256=iKWN51-5RoYrwTgmFLREVUT7kgs5pMFBt4Tfbt-HqPM,1605
@@ -71,13 +71,13 @@
 pioreactor/utils/mock.py,sha256=V1_RqiD6gNctW-HxpCI0aDXepULIGWzD0tJUcfelONA,4122
 pioreactor/utils/networking.py,sha256=ePepmhpvP3uiVLhearQBeBe-csNjSqCzz81ylzDZ11g,3951
 pioreactor/utils/pwm.py,sha256=7KAdMF0w9YQbnI7swhZE_gfBLIkCOEYnQIrbHuoLxqo,7559
 pioreactor/utils/rpi_bad_power.py,sha256=CbtzIi9x8pvtVAX6aID8MG5YXNzkeIRFYfhri4qI-Xo,3393
 pioreactor/utils/sqlite_worker.py,sha256=69vb6s9bFdku7W7Akvb7dI0qYFW1ByhC_RECBRDwKPc,7749
 pioreactor/utils/streaming_calculations.py,sha256=7QLdhPKvOad18Z2rDgU5X8Eo_S1I2Kt7zqhuF1H8x5s,15186
 pioreactor/utils/timing.py,sha256=Yc4pG9FB9Ix5fLT98LwuK6jQawzgMaM8AB09zPWKkTM,5614
-pioreactor-23.6.6rc0.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
-pioreactor-23.6.6rc0.dist-info/METADATA,sha256=IIiF3IgpltXHm1ZpAVXI4wqPNp7uuzEbFwj9_apGeVQ,3896
-pioreactor-23.6.6rc0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pioreactor-23.6.6rc0.dist-info/entry_points.txt,sha256=1vQa-58PTH44hOQBeYFJdO3Tdfzea7_pYDxv5KQWvZ4,79
-pioreactor-23.6.6rc0.dist-info/top_level.txt,sha256=xhd14Ee_KR74whX88OzvljqlGXmfpBUHOSIqDrbs9_0,11
-pioreactor-23.6.6rc0.dist-info/RECORD,,
+pioreactor-23.6.7.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
+pioreactor-23.6.7.dist-info/METADATA,sha256=AMEjzzsCiVkQPaNtwS4FGgGF3ORk9i9I48xSjwokSAQ,3893
+pioreactor-23.6.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioreactor-23.6.7.dist-info/entry_points.txt,sha256=1vQa-58PTH44hOQBeYFJdO3Tdfzea7_pYDxv5KQWvZ4,79
+pioreactor-23.6.7.dist-info/top_level.txt,sha256=xhd14Ee_KR74whX88OzvljqlGXmfpBUHOSIqDrbs9_0,11
+pioreactor-23.6.7.dist-info/RECORD,,
```

