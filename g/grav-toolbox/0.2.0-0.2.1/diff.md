# Comparing `tmp/grav-toolbox-0.2.0.tar.gz` & `tmp/grav-toolbox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grav-toolbox-0.2.0.tar", last modified: Tue Jun 20 14:25:09 2023, max compression
+gzip compressed data, was "grav-toolbox-0.2.1.tar", last modified: Tue Jun 27 11:49:27 2023, max compression
```

## Comparing `grav-toolbox-0.2.0.tar` & `grav-toolbox-0.2.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/LICENSE
--rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.2.0/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.691353 grav-toolbox-0.2.0/bev_legacy/
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/__init__.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/adjust.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/adjust_reilly1970.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/command_line.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/const.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/drift_mlr.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/init.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/output.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/plots.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/schwaus.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.2.0/bev_legacy/settings.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/utils.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.695353 grav-toolbox-0.2.0/grav_toolbox.egg-info/
--rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2418 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)      320 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/zip-safe
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.695353 grav-toolbox-0.2.0/gravtools/
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.695353 grav-toolbox-0.2.0/gravtools/CG5_utils/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/CG5_utils/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32616 2023-03-22 14:22:41.000000 grav-toolbox-0.2.0/gravtools/CG5_utils/cg5_survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-06-20 14:24:54.000000 grav-toolbox-0.2.0/gravtools/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/const.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.703353 grav-toolbox-0.2.0/gravtools/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    65835 2023-06-20 14:23:44.000000 grav-toolbox-0.2.0/gravtools/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_autoselection_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    11546 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_estimation_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_export_results.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_gis_export_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_load_stations.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_load_tsf_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_new_campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_options.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_setup_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15540 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/gui/dlg_correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1784 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/gui/dlg_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/gui/dlg_load_tsf_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)   199744 2023-06-20 14:23:44.000000 grav-toolbox-0.2.0/gravtools/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_observation_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_correlation_matrix_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_drift_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_obs_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_stat_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_vg_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_setup_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_station_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_survey_table.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.707353 grav-toolbox-0.2.0/gravtools/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    49915 2023-06-13 16:10:17.000000 grav-toolbox-0.2.0/gravtools/models/campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/models/exceptions.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    38608 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/lsm.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    38803 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/lsm_diff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    35256 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/lsm_nondiff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/models/misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18698 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/mlr_bev_legacy.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.2.0/gravtools/models/station.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    99692 2023-06-13 16:10:17.000000 grav-toolbox-0.2.0/gravtools/models/survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32396 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/vg_lsm.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/gravtools/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/scripts/create_correction_time_seriens_from_tsf.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/scripts/load_tfs_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/scripts/run_gui.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    12110 2023-06-20 14:23:44.000000 grav-toolbox-0.2.0/gravtools/settings.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/gravtools/tides/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/tides/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16244 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/tides/correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/tides/longman1959.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/tides/tide_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18016 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/tides/tide_data_tfs.py
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)     1105 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.786410 grav-toolbox-0.2.1/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/LICENSE
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7522 2023-06-27 11:49:27.786410 grav-toolbox-0.2.1/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.2.1/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.766410 grav-toolbox-0.2.1/bev_legacy/
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/__init__.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/adjust.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/adjust_reilly1970.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/command_line.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/const.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/drift_mlr.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/init.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/output.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/plots.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/schwaus.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.2.1/bev_legacy/settings.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/utils.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.770410 grav-toolbox-0.2.1/grav_toolbox.egg-info/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7522 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2418 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       59 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/zip-safe
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.770410 grav-toolbox-0.2.1/gravtools/
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.770410 grav-toolbox-0.2.1/gravtools/CG5_utils/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/CG5_utils/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32664 2023-06-27 11:18:52.000000 grav-toolbox-0.2.1/gravtools/CG5_utils/cg5_survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-06-27 11:49:15.000000 grav-toolbox-0.2.1/gravtools/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/const.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.778410 grav-toolbox-0.2.1/gravtools/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    65835 2023-06-20 14:23:44.000000 grav-toolbox-0.2.1/gravtools/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_autoselection_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    11546 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_estimation_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_export_results.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_gis_export_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_load_stations.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_new_campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_options.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_setup_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15540 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/gui/dlg_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1784 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/gui/dlg_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/gui/dlg_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   199780 2023-06-27 11:34:07.000000 grav-toolbox-0.2.1/gravtools/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_observation_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_correlation_matrix_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_drift_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_obs_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_stat_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_vg_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_setup_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_station_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_survey_table.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.782410 grav-toolbox-0.2.1/gravtools/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    49963 2023-06-27 11:30:46.000000 grav-toolbox-0.2.1/gravtools/models/campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/models/exceptions.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    38608 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/lsm.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    38803 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/lsm_diff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35256 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/lsm_nondiff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/models/misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18698 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/mlr_bev_legacy.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.2.1/gravtools/models/station.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    99692 2023-06-13 16:10:17.000000 grav-toolbox-0.2.1/gravtools/models/survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32396 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/vg_lsm.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.782410 grav-toolbox-0.2.1/gravtools/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/scripts/create_correction_time_seriens_from_tsf.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/scripts/load_tfs_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/scripts/run_gui.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    12252 2023-06-27 11:24:11.000000 grav-toolbox-0.2.1/gravtools/settings.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.786410 grav-toolbox-0.2.1/gravtools/tides/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/tides/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16244 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/tides/correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/tides/longman1959.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/tides/tide_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18016 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/tides/tide_data_tfs.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)      917 2023-06-27 11:49:27.786410 grav-toolbox-0.2.1/setup.cfg
```

### Comparing `grav-toolbox-0.2.0/LICENSE` & `grav-toolbox-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/PKG-INFO` & `grav-toolbox-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: gis
 License-File: LICENSE
 
 # GravTools
 GravTools is an open source software toolbox for processing relative gravity surveys developed at the Austrian
 Federal Office of Metrology and Surveying (BEV).
```

### Comparing `grav-toolbox-0.2.0/README.md` & `grav-toolbox-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/adjust.py` & `grav-toolbox-0.2.1/bev_legacy/adjust.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/adjust_reilly1970.py` & `grav-toolbox-0.2.1/bev_legacy/adjust_reilly1970.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/command_line.py` & `grav-toolbox-0.2.1/bev_legacy/command_line.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/drift_mlr.py` & `grav-toolbox-0.2.1/bev_legacy/drift_mlr.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/init.py` & `grav-toolbox-0.2.1/bev_legacy/init.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/output.py` & `grav-toolbox-0.2.1/bev_legacy/output.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/plots.py` & `grav-toolbox-0.2.1/bev_legacy/plots.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/schwaus.py` & `grav-toolbox-0.2.1/bev_legacy/schwaus.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/settings.py` & `grav-toolbox-0.2.1/bev_legacy/settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/bev_legacy/utils.py` & `grav-toolbox-0.2.1/bev_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/grav_toolbox.egg-info/PKG-INFO` & `grav-toolbox-0.2.1/grav_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: gis
 License-File: LICENSE
 
 # GravTools
 GravTools is an open source software toolbox for processing relative gravity surveys developed at the Austrian
 Federal Office of Metrology and Surveying (BEV).
```

### Comparing `grav-toolbox-0.2.0/grav_toolbox.egg-info/SOURCES.txt` & `grav-toolbox-0.2.1/grav_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/CG5_utils/__init__.py` & `grav-toolbox-0.2.1/gravtools/CG5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/CG5_utils/cg5_survey.py` & `grav-toolbox-0.2.1/gravtools/CG5_utils/cg5_survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import pandas as pd
 import numpy as np
 import re
 import datetime as dt
-import matplotlib.pyplot as plt
-# from io import StringIO  # Python 3.x required
 
 from gravtools.models.exceptions import InvaliFileContentError
 from gravtools import settings
 
 
 class DataCursor:
     """Data cursor for matplotlib plot. X and Y coordinates are printed life to the plot canvas.
@@ -675,14 +673,18 @@
                 self.obs_df['date'] + ' ' + self.obs_df['time_str'], format='%Y/%m/%d %H:%M:%S')
 
         self.obs_df.drop(columns=['time_str', 'date'], inplace=True)  # Drop columns that are not required any more
 
     def plot_g_values(self, station_names=None):
         """Plot g-values of selected or all stations in the df.
 
+        Notes
+        -----
+        This method requires matplotlib as optional dependency!
+
         Parameters
         ----------
         station_names : list of str, optional
             List of names of stations for which the observations will be plotted.
             The default value is None which implied that the data of all stations
             is plotted.
 
@@ -707,14 +709,15 @@
             fig.canvas.mpl_connect('pick_event', DataCursor(plt.gca()))
 
             plt.show()
 
 
 # Run as standalone program:
 if __name__ == "__main__":
+    import matplotlib.pyplot as plt
     path = settings.PATH_OBS_FILE_CG5 + settings.NAME_OBS_FILE_CG5
     s1 = CG5Survey()
     s1.read_obs_file(path)
     # s1.plot_g_values(['1-164-04', '1-164-12', '1-164-11'])
     # s1.plot_g_values(['TEST'])
     s1.plot_g_values()
 else:
```

### Comparing `grav-toolbox-0.2.0/gravtools/__init__.py` & `grav-toolbox-0.2.1/gravtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (andreas.hellerschmied@bev.gv.at)
 """
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __author__ = 'Andreas Hellerschmied'
 __git_repo__ = 'https://github.com/ahellers/GravTools'
 __pypi_repo__ = 'https://pypi.org/project/grav-toolbox/'
 __email__ = 'andreas.hellerschmied@bev.gv.at'
 __copyright__ = '(c) 2022 Andreas Hellerschmied'
```

### Comparing `grav-toolbox-0.2.0/gravtools/const.py` & `grav-toolbox-0.2.1/gravtools/const.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/MainWindow.py` & `grav-toolbox-0.2.1/gravtools/gui/MainWindow.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/__init__.py` & `grav-toolbox-0.2.1/gravtools/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_about.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_about.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_autoselection_settings.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_autoselection_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_correction_time_series.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_corrections.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_corrections.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_estimation_settings.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_estimation_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_export_results.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_export_results.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_gis_export_settings.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_gis_export_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_load_stations.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_load_stations.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_load_tsf_file.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_load_tsf_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_new_campaign.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_new_campaign.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_options.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_options.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dialog_setup_data.py` & `grav-toolbox-0.2.1/gravtools/gui/dialog_setup_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dlg_correction_time_series.py` & `grav-toolbox-0.2.1/gravtools/gui/dlg_correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dlg_corrections.py` & `grav-toolbox-0.2.1/gravtools/gui/dlg_corrections.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/dlg_load_tsf_file.py` & `grav-toolbox-0.2.1/gravtools/gui/dlg_load_tsf_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_main.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     Notes
     -----
     The timestamps need to refer to UTC!"
     """
 
     def tickStrings(self, values, scale, spacing) -> str:
         """Handles the x-axes tags representing date and time."""
-        return [dt.datetime.fromtimestamp(value, tz=pytz.utc) for value in values]
+        return [dt.datetime.fromtimestamp(value, tz=pytz.utc).strftime(settings.Y_TICK_DATETIME_FORMAT) for value in values]
 
 
 class MainWindow(QMainWindow, Ui_MainWindow):
     """Main Window of the application."""
 
     # General options for the main window:
     BRUSH_ACTIVE_OBS = pg.mkBrush('g')
@@ -1434,15 +1434,15 @@
         self.plot_obs_results.clear()
         # Plot time series:
         if self.radioButton_results_obs_plot_timeseries.isChecked():
             self.init_observation_results_plots_timerseries()
             if results_obs_df is not None:  # Data available for plotting
                 # Get data:
                 data = results_obs_df[column_name].values
-                if isinstance(data, np.object):
+                if isinstance(data, object):
                     data = data.astype(float)
                 obs_epoch_timestamps = (results_obs_df['ref_epoch_dt'].values - np.datetime64(
                     '1970-01-01T00:00:00')) / np.timedelta64(1, 's')
                 plot_name = self.results_observation_model.get_short_column_description(column_name)
                 self.plot_xy_data(self.plot_obs_results, obs_epoch_timestamps, data, plot_name=plot_name, color='b',
                                   symbol='o', symbol_size=10)
                 self.plot_obs_results.showGrid(x=True, y=True)
@@ -1454,15 +1454,15 @@
         elif self.radioButton_results_obs_plot_histogram.isChecked():
             self.init_observation_results_plots_histogram()
             if results_obs_df is not None:  # Data available for plotting
                 # Get bin method:
                 bins = self.get_hist_bin_method()
                 # Get data:
                 data = results_obs_df[column_name].values
-                if isinstance(data, np.object):
+                if isinstance(data, object):
                     data = data.astype(float)
                 y, x = np.histogram(data, bins=bins)
                 self.plot_obs_results.plot(x, y, stepMode=True, fillLevel=0, brush=(0, 0, 255, 80))
                 self.plot_obs_results.showGrid(x=True, y=True)
 
                 # Add legend with statistics:
                 mean = np.mean(data)
```

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_misc.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_observation_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_observation_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_correlation_matrix_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_correlation_matrix_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_drift_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_drift_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_obs_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_obs_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_stat_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_stat_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_vg_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_vg_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_setup_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_setup_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_station_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_station_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/gui/gui_model_survey_table.py` & `grav-toolbox-0.2.1/gravtools/gui/gui_model_survey_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/__init__.py` & `grav-toolbox-0.2.1/gravtools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/campaign.py` & `grav-toolbox-0.2.1/gravtools/models/campaign.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,16 +821,17 @@
         verbose : bool, optional (default=False)
             If `True`, status messages are printed to the command line.
 
         Returns
         -------
         `Campaign` object
         """
-        with open(filename, 'rb') as handle:
-            campaign = pickle.load(handle)
+        campaign = pd.read_pickle(filename)
+        # with open(filename, 'rb') as handle:
+        #     campaign = pickle.load(handle)
         if verbose:
             print(
                 f'Loaded campaign "{campaign.campaign_name}" with {campaign.number_of_stations} station(s) and {campaign.number_of_surveys} survey(s).')
         return campaign
 
     def set_output_directory(self, output_directory):
         """Change the campaign's output directory.
```

### Comparing `grav-toolbox-0.2.0/gravtools/models/exceptions.py` & `grav-toolbox-0.2.1/gravtools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/lsm.py` & `grav-toolbox-0.2.1/gravtools/models/lsm.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/lsm_diff.py` & `grav-toolbox-0.2.1/gravtools/models/lsm_diff.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/lsm_nondiff.py` & `grav-toolbox-0.2.1/gravtools/models/lsm_nondiff.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/misc.py` & `grav-toolbox-0.2.1/gravtools/models/misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/mlr_bev_legacy.py` & `grav-toolbox-0.2.1/gravtools/models/mlr_bev_legacy.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/station.py` & `grav-toolbox-0.2.1/gravtools/models/station.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/survey.py` & `grav-toolbox-0.2.1/gravtools/models/survey.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/models/vg_lsm.py` & `grav-toolbox-0.2.1/gravtools/models/vg_lsm.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/scripts/__init__.py` & `grav-toolbox-0.2.1/gravtools/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/scripts/create_correction_time_seriens_from_tsf.py` & `grav-toolbox-0.2.1/gravtools/scripts/create_correction_time_seriens_from_tsf.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/scripts/load_tfs_file.py` & `grav-toolbox-0.2.1/gravtools/scripts/load_tfs_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/scripts/run_gui.py` & `grav-toolbox-0.2.1/gravtools/scripts/run_gui.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/settings.py` & `grav-toolbox-0.2.1/gravtools/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,18 @@
     'scott': 'Estimator based on leave-one-out cross-validation estimate of the integrated squared error. Can be regarded as a generalization of Scott’s rule.',
     'rice': 'Estimator does not take variability into account, only data size. Commonly overestimates number of bins required.',
     'sturges': 'R’s default method, only accounts for data size. Only optimal for gaussian data and underestimates number of bins for large non-gaussian datasets.',
     'sqrt': 'Square root (of data size) estimator, used by Excel and other programs for its speed and simplicity.',
     'Num. of bins': 'User defined number of bins (min. = 2, max. = 1000).'
 }
 
+# Time label format for y-ticks in time-series plots:
+# - Format string for datetime.strftime()
+Y_TICK_DATETIME_FORMAT = '%Y-%m-%d %H:%M:%S'
+
 # --- Gerneral color settings ---
 DATUM_STATION_COLOR = (255, 204, 204)
 
 # --- Drift plots in the results tab: ---
 # Number of plot items for plotting the drift function (polynomial):
 DRIFT_PLOT_NUM_ITEMS_IN_DRIFT_FUNCTION = 100
 # Options for the observation data points in the drift plot:
```

### Comparing `grav-toolbox-0.2.0/gravtools/tides/__init__.py` & `grav-toolbox-0.2.1/gravtools/tides/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/tides/correction_time_series.py` & `grav-toolbox-0.2.1/gravtools/tides/correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/tides/longman1959.py` & `grav-toolbox-0.2.1/gravtools/tides/longman1959.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/tides/tide_data.py` & `grav-toolbox-0.2.1/gravtools/tides/tide_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/gravtools/tides/tide_data_tfs.py` & `grav-toolbox-0.2.1/gravtools/tides/tide_data_tfs.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.0/setup.cfg` & `grav-toolbox-0.2.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -6,44 +6,33 @@
 url = https://github.com/ahellers/GravTools
 description = Gravity survey utility tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = gravity, gravimeter, least squares adjustment, geodesy, geophysics
 license = GNU GPLv3
 classifiers = 
-	License :: OSI Approved :: GNU General Public License (GPL)
-	Programming Language :: Python :: 3
+	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options]
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
-	cycler==0.11.0
-	joblib==1.1.0
-	kiwisolver==1.3.1
-	matplotlib==3.3.4
-	numpy==1.19.5
-	pandas==1.1.5
-	Pillow==8.4.0
-	pyparsing==3.0.6
-	PyQt5==5.15.6
-	PyQt5-Qt5==5.15.2
-	PyQt5-sip==12.9.0
-	pyqtgraph==0.11.1
-	python-dateutil==2.8.2
-	pytz==2021.3
-	scikit-learn==0.24.2
-	scipy==1.5.4
-	six==1.16.0
-	threadpoolctl==3.0.0
+	PyQt5
+	pandas
+	pyqtgraph
+	scipy
+	scikit-learn
 
 [options.extras_require]
 gis = 
-	geopandas==0.12.2
+	geopandas
 
 [options.entry_points]
 console_scripts = 
 	gt = gravtools.scripts.run_gui:run_gui
 
 [egg_info]
 tag_build =
```

