# Comparing `tmp/exasol_script_languages_container_tool-0.17.0.tar.gz` & `tmp/exasol_script_languages_container_tool-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_script_languages_container_tool-0.17.0.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_tool-0.18.0.tar", max compression
```

## Comparing `exasol_script_languages_container_tool-0.17.0.tar` & `exasol_script_languages_container_tool-0.18.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1063 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/LICENSE
--rw-r--r--   0        0        0     7271 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/README.md
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/__init__.py
--rw-r--r--   0        0        0      501 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/__init__.py
--rw-r--r--   0        0        0     3825 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/build.py
--rw-r--r--   0        0        0     2998 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/build_test_container.py
--rw-r--r--   0        0        0     2357 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/clean.py
--rw-r--r--   0        0        0     3781 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/export.py
--rw-r--r--   0        0        0     1066 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py
--rw-r--r--   0        0        0     1070 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py
--rw-r--r--   0        0        0     3057 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/push.py
--rw-r--r--   0        0        0     3017 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/push_test_container.py
--rw-r--r--   0        0        0    11821 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py
--rw-r--r--   0        0        0     3551 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/save.py
--rw-r--r--   0        0        0     3657 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/security_scan.py
--rw-r--r--   0        0        0     4519 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/upload.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/__init__.py
--rw-r--r--   0        0        0      820 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/flavor_options.py
--rw-r--r--   0        0        0      617 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/goal_options.py
--rw-r--r--   0        0        0      346 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/test_container_options.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/__init__.py
--rw-r--r--   0        0        0      501 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/__init__.py
--rw-r--r--   0        0        0       50 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/api_errors.py
--rw-r--r--   0        0        0     3049 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/build.py
--rw-r--r--   0        0        0     2725 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/build_test_container.py
--rw-r--r--   0        0        0     2588 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/clean.py
--rw-r--r--   0        0        0     3214 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/export.py
--rw-r--r--   0        0        0     1681 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py
--rw-r--r--   0        0        0      733 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py
--rw-r--r--   0        0        0     3186 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/push.py
--rw-r--r--   0        0        0     2738 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/push_test_container.py
--rw-r--r--   0        0        0     9072 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py
--rw-r--r--   0        0        0     3240 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/save.py
--rw-r--r--   0        0        0     3264 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/security_scan.py
--rw-r--r--   0        0        0     4081 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/upload.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/__init__.py
--rw-r--r--   0        0        0     1487 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py
--rw-r--r--   0        0        0     1311 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py
--rw-r--r--   0        0        0     4219 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/clean/__init__.py
--rw-r--r--   0        0        0     4470 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/__init__.py
--rw-r--r--   0        0        0      525 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py
--rw-r--r--   0        0        0     9855 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py
--rw-r--r--   0        0        0     1366 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py
--rw-r--r--   0        0        0     1736 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py
--rw-r--r--   0        0        0     3701 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py
--rw-r--r--   0        0        0      756 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py
--rw-r--r--   0        0        0     2958 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/push/__init__.py
--rw-r--r--   0        0        0     1702 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/save/__init__.py
--rw-r--r--   0        0        0     1600 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py
--rw-r--r--   0        0        0      231 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save_parameter.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/security_scan/__init__.py
--rw-r--r--   0        0        0     5728 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py
--rw-r--r--   0        0        0      223 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan_parameter.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/__init__.py
--rw-r--r--   0        0        0      553 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py
--rw-r--r--   0        0        0     1973 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py
--rw-r--r--   0        0        0     6871 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py
--rw-r--r--   0        0        0     2246 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py
--rw-r--r--   0        0        0     1961 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py
--rw-r--r--   0        0        0     2840 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py
--rw-r--r--   0        0        0     2235 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py
--rw-r--r--   0        0        0     3179 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py
--rw-r--r--   0        0        0     1450 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py
--rw-r--r--   0        0        0     8499 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py
--rw-r--r--   0        0        0     1420 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py
--rw-r--r--   0        0        0     9449 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py
--rw-r--r--   0        0        0     1010 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/__init__.py
--rw-r--r--   0        0        0     2663 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py
--rw-r--r--   0        0        0     4863 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py
--rw-r--r--   0        0        0      630 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py
--rw-r--r--   0        0        0     1312 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py
--rw-r--r--   0        0        0     1545 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py
--rw-r--r--   0        0        0     2995 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py
--rw-r--r--   0        0        0      248 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers_parameter.py
--rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/__init__.py
--rw-r--r--   0        0        0      922 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py
--rw-r--r--   0        0        0      915 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py
--rwxr-xr-x   0        0        0      278 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/main.py
--rwxr-xr-x   0        0        0      459 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/construct_docker_runner_image_name.sh
--rwxr-xr-x   0        0        0     1061 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh
--rwxr-xr-x   0        0        0     5629 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh
--rwxr-xr-x   0        0        0     2903 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh
--rwxr-xr-x   0        0        0     1502 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh
--rwxr-xr-x   0        0        0     4495 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh
--rw-r--r--   0        0        0     1055 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/pyproject.toml
--rw-r--r--   0        0        0     8262 1970-01-01 00:00:00.000000 exasol_script_languages_container_tool-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 12:56:39.378970 exasol_script_languages_container_tool-0.18.0/LICENSE
+-rw-r--r--   0        0        0     7271 2023-06-27 12:56:39.378970 exasol_script_languages_container_tool-0.18.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/__init__.py
+-rw-r--r--   0        0        0      501 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4511 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/build.py
+-rw-r--r--   0        0        0     3231 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/build_test_container.py
+-rw-r--r--   0        0        0     3145 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/clean.py
+-rw-r--r--   0        0        0     4539 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/export.py
+-rw-r--r--   0        0        0     1066 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py
+-rw-r--r--   0        0        0     1070 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py
+-rw-r--r--   0        0        0     3759 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/push.py
+-rw-r--r--   0        0        0     3571 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/push_test_container.py
+-rw-r--r--   0        0        0    13335 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py
+-rw-r--r--   0        0        0     4251 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/save.py
+-rw-r--r--   0        0        0     4413 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/security_scan.py
+-rw-r--r--   0        0        0     5364 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/upload.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/options/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/options/flavor_options.py
+-rw-r--r--   0        0        0      617 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/options/goal_options.py
+-rw-r--r--   0        0        0      346 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/options/test_container_options.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/__init__.py
+-rw-r--r--   0        0        0      501 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/api_errors.py
+-rw-r--r--   0        0        0     3363 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/build.py
+-rw-r--r--   0        0        0     2910 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/build_test_container.py
+-rw-r--r--   0        0        0     3120 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/clean.py
+-rw-r--r--   0        0        0     3519 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/export.py
+-rw-r--r--   0        0        0     1681 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py
+-rw-r--r--   0        0        0      733 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py
+-rw-r--r--   0        0        0     3497 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/push.py
+-rw-r--r--   0        0        0     3046 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/push_test_container.py
+-rw-r--r--   0        0        0     9455 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py
+-rw-r--r--   0        0        0     3552 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/save.py
+-rw-r--r--   0        0        0     3603 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/security_scan.py
+-rw-r--r--   0        0        0     4398 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/upload.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/build/__init__.py
+-rw-r--r--   0        0        0     1487 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py
+-rw-r--r--   0        0        0     1311 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py
+-rw-r--r--   0        0        0     4219 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/clean/__init__.py
+-rw-r--r--   0        0        0     4470 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/__init__.py
+-rw-r--r--   0        0        0      525 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py
+-rw-r--r--   0        0        0     9855 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py
+-rw-r--r--   0        0        0     1366 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py
+-rw-r--r--   0        0        0     1736 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py
+-rw-r--r--   0        0        0     3701 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py
+-rw-r--r--   0        0        0      756 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py
+-rw-r--r--   0        0        0     2958 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/push/__init__.py
+-rw-r--r--   0        0        0     1702 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/save/__init__.py
+-rw-r--r--   0        0        0     1600 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py
+-rw-r--r--   0        0        0      231 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save_parameter.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/security_scan/__init__.py
+-rw-r--r--   0        0        0     5728 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py
+-rw-r--r--   0        0        0      223 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan_parameter.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/__init__.py
+-rw-r--r--   0        0        0      553 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py
+-rw-r--r--   0        0        0     1973 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py
+-rw-r--r--   0        0        0     6871 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py
+-rw-r--r--   0        0        0     2246 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py
+-rw-r--r--   0        0        0     1961 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py
+-rw-r--r--   0        0        0     2840 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py
+-rw-r--r--   0        0        0     2235 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py
+-rw-r--r--   0        0        0     3179 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py
+-rw-r--r--   0        0        0     1450 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py
+-rw-r--r--   0        0        0     8499 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py
+-rw-r--r--   0        0        0     1420 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py
+-rw-r--r--   0        0        0     9225 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py
+-rw-r--r--   0        0        0     1010 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/__init__.py
+-rw-r--r--   0        0        0     2663 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py
+-rw-r--r--   0        0        0     4863 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py
+-rw-r--r--   0        0        0      630 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py
+-rw-r--r--   0        0        0     1312 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py
+-rw-r--r--   0        0        0     1545 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py
+-rw-r--r--   0        0        0     2995 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py
+-rw-r--r--   0        0        0      248 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers_parameter.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/utils/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py
+-rw-r--r--   0        0        0      915 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py
+-rwxr-xr-x   0        0        0      278 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/main.py
+-rwxr-xr-x   0        0        0      459 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/construct_docker_runner_image_name.sh
+-rwxr-xr-x   0        0        0     1061 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh
+-rwxr-xr-x   0        0        0     5629 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh
+-rwxr-xr-x   0        0        0     2903 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh
+-rwxr-xr-x   0        0        0     1502 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh
+-rwxr-xr-x   0        0        0     4495 2023-06-27 12:56:39.382970 exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh
+-rw-r--r--   0        0        0     1077 2023-06-27 12:56:39.386970 exasol_script_languages_container_tool-0.18.0/pyproject.toml
+-rw-r--r--   0        0        0     8304 1970-01-01 00:00:00.000000 exasol_script_languages_container_tool-0.18.0/PKG-INFO
```

### Comparing `exasol_script_languages_container_tool-0.17.0/LICENSE` & `exasol_script_languages_container_tool-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/README.md` & `exasol_script_languages_container_tool-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/build.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/build.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple, Optional
 
 import click
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
+from exasol_integration_test_docker_environment.cli.options.system_options import system_options, luigi_logging_options
 from exasol_integration_test_docker_environment.cli.termination_handler import TerminationHandler
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
 from exasol_script_languages_container_tool.cli.options.flavor_options import flavor_options
 from exasol_script_languages_container_tool.cli.options.goal_options import goal_options
 from exasol_script_languages_container_tool.lib import api
 
@@ -26,14 +26,15 @@
                    "they will get loaded or pulled. The only case, in which them get builded is "
                    "when they are not otherwise available. "
                    "This includes the case where a higher stage which transitivily "
                    "depends on a images is somewhere available, "
                    "but the images as self is not available.")
 @add_options(docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def build(flavor_path: Tuple[str, ...],
           goal: Tuple[str, ...],
           force_rebuild: bool,
           force_rebuild_from: Tuple[str, ...],
           force_pull: bool,
           output_directory: str,
           temporary_base_directory: str,
@@ -46,35 +47,41 @@
           source_docker_username: Optional[str],
           source_docker_password: Optional[str],
           target_docker_repository_name: str,
           target_docker_tag_prefix: str,
           target_docker_username: Optional[str],
           target_docker_password: Optional[str],
           workers: int,
-          task_dependencies_dot_file: Optional[str]):
+          task_dependencies_dot_file: Optional[str],
+          log_level: Optional[str],
+          use_job_specific_log_file: bool
+          ):
     """
     This command builds all stages of the script-language-container flavor.
     If stages are cached in a docker registry, this command is going to pull them,
     instead of building them.
     """
     with TerminationHandler():
-        api.build(flavor_path,
-                  goal,
-                  force_rebuild,
-                  force_rebuild_from,
-                  force_pull,
-                  output_directory,
-                  temporary_base_directory,
-                  log_build_context_content,
-                  cache_directory,
-                  build_name,
-                  shortcut_build,
-                  source_docker_repository_name,
-                  source_docker_tag_prefix,
-                  source_docker_username,
-                  source_docker_password,
-                  target_docker_repository_name,
-                  target_docker_tag_prefix,
-                  target_docker_username,
-                  target_docker_password,
-                  workers,
-                  task_dependencies_dot_file)
+        api.build(flavor_path=flavor_path,
+                  goal=goal,
+                  force_rebuild=force_rebuild,
+                  force_rebuild_from=force_rebuild_from,
+                  force_pull=force_pull,
+                  output_directory=output_directory,
+                  temporary_base_directory=temporary_base_directory,
+                  log_build_context_content=log_build_context_content,
+                  cache_directory=cache_directory,
+                  build_name=build_name,
+                  shortcut_build=shortcut_build,
+                  source_docker_repository_name=source_docker_repository_name,
+                  source_docker_tag_prefix=source_docker_tag_prefix,
+                  source_docker_username=source_docker_username,
+                  source_docker_password=source_docker_password,
+                  target_docker_repository_name=target_docker_repository_name,
+                  target_docker_tag_prefix=target_docker_tag_prefix,
+                  target_docker_username=target_docker_username,
+                  target_docker_password=target_docker_password,
+                  workers=workers,
+                  task_dependencies_dot_file=task_dependencies_dot_file,
+                  log_level=log_level,
+                  use_job_specific_log_file=use_job_specific_log_file
+                  )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/build_test_container.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/build_test_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Tuple, Optional
 
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
+from exasol_integration_test_docker_environment.cli.options.system_options import system_options, luigi_logging_options
 from exasol_integration_test_docker_environment.cli.termination_handler import TerminationHandler
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
 from exasol_script_languages_container_tool.cli.options.test_container_options import test_container_options
 from exasol_script_languages_container_tool.lib import api
 
 
 @cli.command(short_help="Builds the test container docker image.")
 @add_options(test_container_options)
 @add_options(build_options)
 @add_options(docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def build_test_container(
         test_container_folder: str,
         force_rebuild: bool,
         force_rebuild_from: Tuple[str, ...],
         force_pull: bool,
         output_directory: str,
         temporary_base_directory: str,
@@ -31,15 +32,18 @@
         source_docker_username: Optional[str],
         source_docker_password: Optional[str],
         target_docker_repository_name: str,
         target_docker_tag_prefix: str,
         target_docker_username: Optional[str],
         target_docker_password: Optional[str],
         workers: int,
-        task_dependencies_dot_file: Optional[str]):
+        task_dependencies_dot_file: Optional[str],
+        log_level: Optional[str],
+        use_job_specific_log_file: bool
+):
     """
     Builds the test container docker image.
 
     The test container is used during tests of the Script-Language-Container.
     """
     with TerminationHandler():
         api.build_test_container(
@@ -57,9 +61,11 @@
             source_docker_username=source_docker_username,
             source_docker_password=source_docker_password,
             target_docker_repository_name=target_docker_repository_name,
             target_docker_tag_prefix=target_docker_tag_prefix,
             target_docker_username=target_docker_username,
             target_docker_password=target_docker_password,
             workers=workers,
-            task_dependencies_dot_file=task_dependencies_dot_file
+            task_dependencies_dot_file=task_dependencies_dot_file,
+            log_level=log_level,
+            use_job_specific_log_file=use_job_specific_log_file
         )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/clean.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/clean.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,74 @@
 from typing import Tuple, Optional
 
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import \
     simple_docker_repository_options
 from exasol_integration_test_docker_environment.cli.options.system_options import output_directory_option, \
-    system_options
+    system_options, luigi_logging_options
 from exasol_integration_test_docker_environment.cli.termination_handler import TerminationHandler
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
 from exasol_script_languages_container_tool.cli.options.flavor_options import flavor_options
 from exasol_script_languages_container_tool.lib import api
 
 
 @cli.command(short_help="Cleans script-languages-container docker images for the given flavor.")
 @add_options(flavor_options)
 @add_options([output_directory_option])
 @add_options(simple_docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def clean_flavor_images(flavor_path: Tuple[str, ...],
                         output_directory: str,
                         docker_repository_name: str,
                         docker_tag_prefix: str,
                         workers: int,
-                        task_dependencies_dot_file: Optional[str]):
+                        task_dependencies_dot_file: Optional[str],
+                        log_level: Optional[str],
+                        use_job_specific_log_file: bool
+                        ):
     """
     This command removes the docker images of all stages of the script languages container for the given flavor.
     """
     with TerminationHandler():
-        api.clean_flavor_images(flavor_path, output_directory, docker_repository_name,
-                                docker_tag_prefix, workers, task_dependencies_dot_file)
+        api.clean_flavor_images(
+            flavor_path=flavor_path,
+            output_directory=output_directory,
+            docker_repository_name=docker_repository_name,
+            docker_tag_prefix=docker_tag_prefix,
+            workers=workers,
+            task_dependencies_dot_file=task_dependencies_dot_file,
+            log_level=log_level,
+            use_job_specific_log_file=use_job_specific_log_file
+        )
 
 
 @cli.command(short_help="Cleans all script-languages-container docker images for all flavors.")
 @add_options([output_directory_option])
 @add_options(simple_docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def clean_all_images(
         output_directory: str,
         docker_repository_name: str,
         docker_tag_prefix: str,
         workers: int,
-        task_dependencies_dot_file: Optional[str]):
+        task_dependencies_dot_file: Optional[str],
+        log_level: Optional[str],
+        use_job_specific_log_file: bool
+):
     """
     This command removes the docker images of all stages of the script languages container for all flavors.
     """
     with TerminationHandler():
-        api.clean_all_images(output_directory, docker_repository_name, docker_tag_prefix,
-                             workers, task_dependencies_dot_file)
+        api.clean_all_images(
+            output_directory=output_directory,
+            docker_repository_name=docker_repository_name,
+            docker_tag_prefix=docker_tag_prefix,
+            workers=workers,
+            task_dependencies_dot_file=task_dependencies_dot_file,
+            log_level=log_level,
+            use_job_specific_log_file=use_job_specific_log_file
+        )
 
 # TODO add commands clean containers, networks, all
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/export.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/push_test_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 from typing import Tuple, Optional
 
 import click
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
+from exasol_integration_test_docker_environment.cli.options.system_options import system_options, luigi_logging_options
 from exasol_integration_test_docker_environment.cli.termination_handler import TerminationHandler
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
-from exasol_script_languages_container_tool.cli.options.flavor_options import flavor_options
-from exasol_script_languages_container_tool.cli.options.goal_options import release_options
+from exasol_script_languages_container_tool.cli.options.test_container_options import test_container_options
 from exasol_script_languages_container_tool.lib import api
 
 
-@cli.command(short_help="Exports the script-language-container.")
-@add_options(flavor_options)
-@add_options(release_options)
-@click.option('--export-path', type=click.Path(exists=False, file_okay=False, dir_okay=True), default=None)
-@click.option('--release-name', type=str, default=None)
+@cli.command(short_help="Pushes the test container docker image to the registry.")
+@add_options(test_container_options)
+@click.option("--force-push", type=bool, default=False, help="Push images also if they already exist.")
+@click.option("--push-all", type=bool, default=False, help="Push all images.")
 @add_options(build_options)
 @add_options(docker_repository_options)
 @add_options(system_options)
-def export(flavor_path: Tuple[str, ...],
-           release_goal: Tuple[str, ...],
-           export_path: Optional[str],
-           release_name: Optional[str],
-           force_rebuild: bool,
-           force_rebuild_from: Tuple[str, ...],
-           force_pull: bool,
-           output_directory: str,
-           temporary_base_directory: str,
-           log_build_context_content: bool,
-           cache_directory: Optional[str],
-           build_name: Optional[str],
-           source_docker_repository_name: str,
-           source_docker_tag_prefix: str,
-           source_docker_username: Optional[str],
-           source_docker_password: Optional[str],
-           target_docker_repository_name: str,
-           target_docker_tag_prefix: str,
-           target_docker_username: Optional[str],
-           target_docker_password: Optional[str],
-           workers: int,
-           task_dependencies_dot_file: Optional[str]):
+@add_options(luigi_logging_options)
+def push_test_container(
+        test_container_folder: str,
+        force_push: bool,
+        push_all: bool,
+        force_rebuild: bool,
+        force_rebuild_from: Tuple[str, ...],
+        force_pull: bool,
+        output_directory: str,
+        temporary_base_directory: str,
+        log_build_context_content: bool,
+        cache_directory: Optional[str],
+        build_name: Optional[str],
+        source_docker_repository_name: str,
+        source_docker_tag_prefix: str,
+        source_docker_username: Optional[str],
+        source_docker_password: Optional[str],
+        target_docker_repository_name: str,
+        target_docker_tag_prefix: str,
+        target_docker_username: Optional[str],
+        target_docker_password: Optional[str],
+        workers: int,
+        task_dependencies_dot_file: Optional[str],
+        log_level: Optional[str],
+        use_job_specific_log_file: bool
+):
     """
-    This command exports the whole script-language-container package of the flavor,
-    ready for the upload into the bucketfs. If the stages do not exists locally,
-    the system will build or pull them before the exporting the packaged container.
+    Push the test container docker image to the registry.
+
+    The test container is used during tests of the Script-Language-Container.
     """
     with TerminationHandler():
-        export_result = api.export(flavor_path,
-                                   release_goal,
-                                   export_path,
-                                   release_name,
-                                   force_rebuild,
-                                   force_rebuild_from,
-                                   force_pull,
-                                   output_directory,
-                                   temporary_base_directory,
-                                   log_build_context_content,
-                                   cache_directory,
-                                   build_name,
-                                   source_docker_repository_name,
-                                   source_docker_tag_prefix,
-                                   source_docker_username,
-                                   source_docker_password,
-                                   target_docker_repository_name,
-                                   target_docker_tag_prefix,
-                                   target_docker_username,
-                                   target_docker_password,
-                                   workers,
-                                   task_dependencies_dot_file)
-        with open(export_result.command_line_output_path, "r") as f:
-            print(f.read())
+        api.push_test_container(
+            test_container_folder=test_container_folder,
+            force_push=force_push,
+            push_all=push_all,
+            force_rebuild=force_rebuild,
+            force_rebuild_from=force_rebuild_from,
+            force_pull=force_pull,
+            output_directory=output_directory,
+            temporary_base_directory=temporary_base_directory,
+            log_build_context_content=log_build_context_content,
+            cache_directory=cache_directory,
+            build_name=build_name,
+            source_docker_repository_name=source_docker_repository_name,
+            source_docker_tag_prefix=source_docker_tag_prefix,
+            source_docker_username=source_docker_username,
+            source_docker_password=source_docker_password,
+            target_docker_repository_name=target_docker_repository_name,
+            target_docker_tag_prefix=target_docker_tag_prefix,
+            target_docker_username=target_docker_username,
+            target_docker_password=target_docker_password,
+            workers=workers,
+            task_dependencies_dot_file=task_dependencies_dot_file,
+            log_level=log_level,
+            use_job_specific_log_file=use_job_specific_log_file
+        )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/push.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/push.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple, Optional
 
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
 from exasol_integration_test_docker_environment.cli.options.push_options import push_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
+from exasol_integration_test_docker_environment.cli.options.system_options import system_options, luigi_logging_options
 from exasol_integration_test_docker_environment.cli.termination_handler import TerminationHandler
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
 from exasol_script_languages_container_tool.cli.options.flavor_options import flavor_options
 from exasol_script_languages_container_tool.cli.options.goal_options import goal_options
 from exasol_script_languages_container_tool.lib import api
 
@@ -16,14 +16,15 @@
 @cli.command(short_help="Pushes script languages container to docker repository.")
 @add_options(flavor_options)
 @add_options(goal_options)
 @add_options(push_options)
 @add_options(build_options)
 @add_options(docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def push(flavor_path: Tuple[str, ...],
          goal: Tuple[str, ...],
          force_push: bool,
          push_all: bool,
          force_rebuild: bool,
          force_rebuild_from: Tuple[str, ...],
          force_pull: bool,
@@ -37,34 +38,41 @@
          source_docker_username: Optional[str],
          source_docker_password: Optional[str],
          target_docker_repository_name: str,
          target_docker_tag_prefix: str,
          target_docker_username: Optional[str],
          target_docker_password: Optional[str],
          workers: int,
-         task_dependencies_dot_file: Optional[str]):
+         task_dependencies_dot_file: Optional[str],
+         log_level: Optional[str],
+         use_job_specific_log_file: bool
+         ):
     """
     This command pushes all stages of the script-language-container flavor.
     If the stages do not exists locally, the system will build or pull them before the push.
     """
     with TerminationHandler():
-        api.push(flavor_path, goal,
-                 force_push,
-                 push_all,
-                 force_rebuild,
-                 force_rebuild_from,
-                 force_pull,
-                 output_directory,
-                 temporary_base_directory,
-                 log_build_context_content,
-                 cache_directory,
-                 build_name,
-                 source_docker_repository_name,
-                 source_docker_tag_prefix,
-                 source_docker_username,
-                 source_docker_password,
-                 target_docker_repository_name,
-                 target_docker_tag_prefix,
-                 target_docker_username,
-                 target_docker_password,
-                 workers,
-                 task_dependencies_dot_file)
+        api.push(flavor_path=flavor_path,
+                 goal=goal,
+                 force_push=force_push,
+                 push_all=push_all,
+                 force_rebuild=force_rebuild,
+                 force_rebuild_from=force_rebuild_from,
+                 force_pull=force_pull,
+                 output_directory=output_directory,
+                 temporary_base_directory=temporary_base_directory,
+                 log_build_context_content=log_build_context_content,
+                 cache_directory=cache_directory,
+                 build_name=build_name,
+                 source_docker_repository_name=source_docker_repository_name,
+                 source_docker_tag_prefix=source_docker_tag_prefix,
+                 source_docker_username=source_docker_username,
+                 source_docker_password=source_docker_password,
+                 target_docker_repository_name=target_docker_repository_name,
+                 target_docker_tag_prefix=target_docker_tag_prefix,
+                 target_docker_username=target_docker_username,
+                 target_docker_password=target_docker_password,
+                 workers=workers,
+                 task_dependencies_dot_file=task_dependencies_dot_file,
+                 log_level=log_level,
+                 use_job_specific_log_file=use_job_specific_log_file
+                 )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/push_test_container.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/build_test_container.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 from typing import Tuple, Optional
 
-from exasol_integration_test_docker_environment.cli.cli import cli
-from exasol_integration_test_docker_environment.cli.options.build_options import build_options
-from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
-from exasol_integration_test_docker_environment.cli.termination_handler import TerminationHandler
-from exasol_integration_test_docker_environment.lib.api.common import add_options
+from exasol_integration_test_docker_environment.lib import api
+from exasol_integration_test_docker_environment.lib.api.common import cli_function
+from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageInfo
 
-from exasol_script_languages_container_tool.cli.options.test_container_options import test_container_options
-from exasol_script_languages_container_tool.lib import api
+from exasol_script_languages_container_tool.cli.options.test_container_options import TEST_CONTAINER_DEFAULT_DIRECTORY
+from exasol_script_languages_container_tool.lib.tasks.test.test_container_content import build_test_container_content
 
 
-@cli.command(short_help="Pushes the test container docker image to the registry.")
-@add_options(test_container_options)
-@add_options(build_options)
-@add_options(docker_repository_options)
-@add_options(system_options)
-def push_test_container(
-        test_container_folder: str,
-        force_rebuild: bool,
-        force_rebuild_from: Tuple[str, ...],
-        force_pull: bool,
-        output_directory: str,
-        temporary_base_directory: str,
-        log_build_context_content: bool,
-        cache_directory: Optional[str],
-        build_name: Optional[str],
-        source_docker_repository_name: str,
-        source_docker_tag_prefix: str,
-        source_docker_username: Optional[str],
-        source_docker_password: Optional[str],
-        target_docker_repository_name: str,
-        target_docker_tag_prefix: str,
-        target_docker_username: Optional[str],
-        target_docker_password: Optional[str],
-        workers: int,
-        task_dependencies_dot_file: Optional[str]):
+@cli_function
+def build_test_container(
+        test_container_folder: str = TEST_CONTAINER_DEFAULT_DIRECTORY,
+        force_rebuild: bool = False,
+        force_rebuild_from: Tuple[str, ...] = tuple(),
+        force_pull: bool = False,
+        output_directory: str = ".build_output",
+        temporary_base_directory: str = "/tmp",
+        log_build_context_content: bool = False,
+        cache_directory: Optional[str] = None,
+        build_name: Optional[str] = None,
+        source_docker_repository_name: str = 'exasol/script-language-container',
+        source_docker_tag_prefix: str = '',
+        source_docker_username: Optional[str] = None,
+        source_docker_password: Optional[str] = None,
+        target_docker_repository_name: str = 'exasol/script-language-container',
+        target_docker_tag_prefix: str = '',
+        target_docker_username: Optional[str] = None,
+        target_docker_password: Optional[str] = None,
+        workers: int = 5,
+        task_dependencies_dot_file: Optional[str] = None,
+        log_level: Optional[str] = None,
+        use_job_specific_log_file: bool = True
+) -> ImageInfo:
     """
-    Push the test container docker image to the registry.
+    Build the test container docker image.
 
     The test container is used during tests of the Script-Language-Container.
     """
-    with TerminationHandler():
-        api.push_test_container(
-            test_container_folder=test_container_folder,
-            force_rebuild=force_rebuild,
-            force_rebuild_from=force_rebuild_from,
-            force_pull=force_pull,
-            output_directory=output_directory,
-            temporary_base_directory=temporary_base_directory,
-            log_build_context_content=log_build_context_content,
-            cache_directory=cache_directory,
-            build_name=build_name,
-            source_docker_repository_name=source_docker_repository_name,
-            source_docker_tag_prefix=source_docker_tag_prefix,
-            source_docker_username=source_docker_username,
-            source_docker_password=source_docker_password,
-            target_docker_repository_name=target_docker_repository_name,
-            target_docker_tag_prefix=target_docker_tag_prefix,
-            target_docker_username=target_docker_username,
-            target_docker_password=target_docker_password,
-            workers=workers,
-            task_dependencies_dot_file=task_dependencies_dot_file)
+    return api.build_test_container(
+        test_container_content=build_test_container_content(test_container_folder),
+        force_rebuild=force_rebuild,
+        force_rebuild_from=force_rebuild_from,
+        force_pull=force_pull,
+        output_directory=output_directory,
+        temporary_base_directory=temporary_base_directory,
+        log_build_context_content=log_build_context_content,
+        cache_directory=cache_directory,
+        build_name=build_name,
+        source_docker_repository_name=source_docker_repository_name,
+        source_docker_tag_prefix=source_docker_tag_prefix,
+        source_docker_username=source_docker_username,
+        source_docker_password=source_docker_password,
+        target_docker_repository_name=target_docker_repository_name,
+        target_docker_tag_prefix=target_docker_tag_prefix,
+        target_docker_username=target_docker_username,
+        target_docker_password=target_docker_password,
+        workers=workers,
+        task_dependencies_dot_file=task_dependencies_dot_file,
+        log_level=log_level,
+        use_job_specific_log_file=use_job_specific_log_file
+    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
 from exasol_script_languages_container_tool.cli.options.flavor_options import flavor_options
 from exasol_script_languages_container_tool.cli.options.goal_options import release_options
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
+from exasol_integration_test_docker_environment.cli.options.system_options import system_options, luigi_logging_options
 from exasol_integration_test_docker_environment.cli.options.test_environment_options import test_environment_options, \
     docker_db_options, external_db_options
 
 from exasol_script_languages_container_tool.cli.options.test_container_options import test_container_options
 from exasol_script_languages_container_tool.lib import api
 from exasol_script_languages_container_tool.lib.api import api_errors
 
@@ -72,25 +72,27 @@
 @click.option('--reuse-test-environment/--no-reuse-test-environment', default=False,
               help="Reuse the whole test environment with docker network, test container, "
                    "database, database setup and uploaded container")
 @add_options(test_container_options)
 @add_options(build_options)
 @add_options(docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def run_db_test(flavor_path: Tuple[str, ...],
                 release_goal: Tuple[str, ...],
                 generic_language_test: Tuple[str, ...],
                 test_folder: Tuple[str, ...],
                 test_file: Tuple[str, ...],
                 test_language: Tuple[str, ...],
                 test: Tuple[str, ...],
                 environment_type: str,
                 max_start_attempts: int,
                 docker_db_image_version: str,
                 docker_db_image_name: str,
+                db_os_access: str,
                 create_certificates: bool,
                 additional_db_parameter: Tuple[str, ...],
                 external_exasol_db_host: Optional[str],
                 external_exasol_db_port: int,
                 external_exasol_bucketfs_port: int,
                 external_exasol_db_user: Optional[str],
                 external_exasol_db_password: Optional[str],
@@ -123,76 +125,82 @@
                 source_docker_username: Optional[str],
                 source_docker_password: Optional[str],
                 target_docker_repository_name: str,
                 target_docker_tag_prefix: str,
                 target_docker_username: Optional[str],
                 target_docker_password: Optional[str],
                 workers: int,
-                task_dependencies_dot_file: Optional[str]):
+                task_dependencies_dot_file: Optional[str],
+                log_level: Optional[str],
+                use_job_specific_log_file: bool
+                ):
     """
     This command runs the integration tests in local docker-db.
     The system spawns a test environment in which the test are executed.
     After finishing the tests, the test environment gets cleaned up.
     If the stages or the packaged container do not exists locally,
     the system will build, pull or export them before running the tests.
     """
     with TerminationHandler():
         try:
-            result = api.run_db_test(flavor_path,
-                                     release_goal,
-                                     generic_language_test,
-                                     test_folder,
-                                     test_file,
-                                     test_language,
-                                     test,
-                                     environment_type,
-                                     max_start_attempts,
-                                     docker_db_image_version,
-                                     docker_db_image_name,
-                                     create_certificates,
-                                     additional_db_parameter,
-                                     external_exasol_db_host,
-                                     external_exasol_db_port,
-                                     external_exasol_bucketfs_port,
-                                     external_exasol_db_user,
-                                     external_exasol_db_password,
-                                     external_exasol_bucketfs_write_password,
-                                     external_exasol_xmlrpc_host,
-                                     external_exasol_xmlrpc_port,
-                                     external_exasol_xmlrpc_user,
-                                     external_exasol_xmlrpc_password,
-                                     external_exasol_xmlrpc_cluster_name,
-                                     db_mem_size,
-                                     db_disk_size,
-                                     test_environment_vars,
-                                     test_log_level,
-                                     reuse_database,
-                                     reuse_database_setup,
-                                     reuse_uploaded_container,
-                                     reuse_test_container,
-                                     reuse_test_environment,
-                                     test_container_folder,
-                                     force_rebuild,
-                                     force_rebuild_from,
-                                     force_pull,
-                                     output_directory,
-                                     temporary_base_directory,
-                                     log_build_context_content,
-                                     cache_directory,
-                                     build_name,
-                                     source_docker_repository_name,
-                                     source_docker_tag_prefix,
-                                     source_docker_username,
-                                     source_docker_password,
-                                     target_docker_repository_name,
-                                     target_docker_tag_prefix,
-                                     target_docker_username,
-                                     target_docker_password,
-                                     workers,
-                                     task_dependencies_dot_file)
+            result = api.run_db_test(flavor_path=flavor_path,
+                                     release_goal=release_goal,
+                                     generic_language_test=generic_language_test,
+                                     test_folder=test_folder,
+                                     test_file=test_file,
+                                     test_language=test_language,
+                                     test=test,
+                                     environment_type=environment_type,
+                                     max_start_attempts=max_start_attempts,
+                                     docker_db_image_version=docker_db_image_version,
+                                     docker_db_image_name=docker_db_image_name,
+                                     db_os_access=db_os_access,
+                                     create_certificates=create_certificates,
+                                     additional_db_parameter=additional_db_parameter,
+                                     external_exasol_db_host=external_exasol_db_host,
+                                     external_exasol_db_port=external_exasol_db_port,
+                                     external_exasol_bucketfs_port=external_exasol_bucketfs_port,
+                                     external_exasol_db_user=external_exasol_db_user,
+                                     external_exasol_db_password=external_exasol_db_password,
+                                     external_exasol_bucketfs_write_password=external_exasol_bucketfs_write_password,
+                                     external_exasol_xmlrpc_host=external_exasol_xmlrpc_host,
+                                     external_exasol_xmlrpc_port=external_exasol_xmlrpc_port,
+                                     external_exasol_xmlrpc_user=external_exasol_xmlrpc_user,
+                                     external_exasol_xmlrpc_password=external_exasol_xmlrpc_password,
+                                     external_exasol_xmlrpc_cluster_name=external_exasol_xmlrpc_cluster_name,
+                                     db_mem_size=db_mem_size,
+                                     db_disk_size=db_disk_size,
+                                     test_environment_vars=test_environment_vars,
+                                     test_log_level=test_log_level,
+                                     reuse_database=reuse_database,
+                                     reuse_database_setup=reuse_database_setup,
+                                     reuse_uploaded_container=reuse_uploaded_container,
+                                     reuse_test_container=reuse_test_container,
+                                     reuse_test_environment=reuse_test_environment,
+                                     test_container_folder=test_container_folder,
+                                     force_rebuild=force_rebuild,
+                                     force_rebuild_from=force_rebuild_from,
+                                     force_pull=force_pull,
+                                     output_directory=output_directory,
+                                     temporary_base_directory=temporary_base_directory,
+                                     log_build_context_content=log_build_context_content,
+                                     cache_directory=cache_directory,
+                                     build_name=build_name,
+                                     source_docker_repository_name=source_docker_repository_name,
+                                     source_docker_tag_prefix=source_docker_tag_prefix,
+                                     source_docker_username=source_docker_username,
+                                     source_docker_password=source_docker_password,
+                                     target_docker_repository_name=target_docker_repository_name,
+                                     target_docker_tag_prefix=target_docker_tag_prefix,
+                                     target_docker_username=target_docker_username,
+                                     target_docker_password=target_docker_password,
+                                     workers=workers,
+                                     task_dependencies_dot_file=task_dependencies_dot_file,
+                                     log_level=log_level,
+                                     use_job_specific_log_file=use_job_specific_log_file)
             if result.command_line_output_path.exists():
                 with result.command_line_output_path.open("r") as f:
                     print(f.read())
             if not result.tests_are_ok:
                 raise RuntimeError("Some tests failed")
         except api_errors.MissingArgumentError as e:
             handle_missing_argument_error(e.args)
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/save.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/save.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple, Optional
 
 import click
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
+from exasol_integration_test_docker_environment.cli.options.system_options import system_options, luigi_logging_options
 from exasol_integration_test_docker_environment.cli.termination_handler import TerminationHandler
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
 from exasol_script_languages_container_tool.cli.options.flavor_options import flavor_options
 from exasol_script_languages_container_tool.cli.options.goal_options import goal_options
 from exasol_script_languages_container_tool.lib import api
 
@@ -22,14 +22,15 @@
               help="Forces the system to overwrite existing save for build steps that run")
 @click.option('--save-all/--no-save-all', default=False,
               help="Forces the system to save all images of build-steps that are specified by the goals")
 @add_options(goal_options)
 @add_options(build_options)
 @add_options(docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def save(flavor_path: Tuple[str, ...],
          save_directory: Optional[str],
          force_save: bool,
          save_all: bool,
          goal: Tuple[str, ...],
          force_rebuild: bool,
          force_rebuild_from: Tuple[str, ...],
@@ -44,36 +45,42 @@
          source_docker_username: Optional[str],
          source_docker_password: Optional[str],
          target_docker_repository_name: str,
          target_docker_tag_prefix: str,
          target_docker_username: Optional[str],
          target_docker_password: Optional[str],
          workers: int,
-         task_dependencies_dot_file: Optional[str]):
+         task_dependencies_dot_file: Optional[str],
+         log_level: Optional[str],
+         use_job_specific_log_file: bool
+         ):
     """
     This command saves all stages of the script-language-container flavor to a local directory.
     If the stages do not exists locally, the system will build or pull them before the execution of save.
     """
     with TerminationHandler():
-        api.save(flavor_path,
-                 save_directory,
-                 force_save,
-                 save_all,
-                 goal,
-                 force_rebuild,
-                 force_rebuild_from,
-                 force_pull,
-                 output_directory,
-                 temporary_base_directory,
-                 log_build_context_content,
-                 cache_directory,
-                 build_name,
-                 source_docker_repository_name,
-                 source_docker_tag_prefix,
-                 source_docker_username,
-                 source_docker_password,
-                 target_docker_repository_name,
-                 target_docker_tag_prefix,
-                 target_docker_username,
-                 target_docker_password,
-                 workers,
-                 task_dependencies_dot_file)
+        api.save(flavor_path=flavor_path,
+                 save_directory=save_directory,
+                 force_save=force_save,
+                 save_all=save_all,
+                 goal=goal,
+                 force_rebuild=force_rebuild,
+                 force_rebuild_from=force_rebuild_from,
+                 force_pull=force_pull,
+                 output_directory=output_directory,
+                 temporary_base_directory=temporary_base_directory,
+                 log_build_context_content=log_build_context_content,
+                 cache_directory=cache_directory,
+                 build_name=build_name,
+                 source_docker_repository_name=source_docker_repository_name,
+                 source_docker_tag_prefix=source_docker_tag_prefix,
+                 source_docker_username=source_docker_username,
+                 source_docker_password=source_docker_password,
+                 target_docker_repository_name=target_docker_repository_name,
+                 target_docker_tag_prefix=target_docker_tag_prefix,
+                 target_docker_username=target_docker_username,
+                 target_docker_password=target_docker_password,
+                 workers=workers,
+                 task_dependencies_dot_file=task_dependencies_dot_file,
+                 log_level=log_level,
+                 use_job_specific_log_file=use_job_specific_log_file
+                 )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/security_scan.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/security_scan.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Tuple, Optional
 
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
+from exasol_integration_test_docker_environment.cli.options.system_options import system_options, luigi_logging_options
 from exasol_integration_test_docker_environment.cli.termination_handler import TerminationHandler
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
 from exasol_script_languages_container_tool.cli.options.flavor_options import flavor_options
 from exasol_script_languages_container_tool.lib import api
 
 
 @cli.command(short_help="Performs a security scan.")
 @add_options(flavor_options)
 @add_options(build_options)
 @add_options(docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def security_scan(flavor_path: Tuple[str, ...],
                   force_rebuild: bool,
                   force_rebuild_from: Tuple[str, ...],
                   force_pull: bool,
                   output_directory: str,
                   temporary_base_directory: str,
                   log_build_context_content: bool,
@@ -30,38 +31,44 @@
                   source_docker_username: Optional[str],
                   source_docker_password: Optional[str],
                   target_docker_repository_name: str,
                   target_docker_tag_prefix: str,
                   target_docker_username: Optional[str],
                   target_docker_password: Optional[str],
                   workers: int,
-                  task_dependencies_dot_file: Optional[str]):
+                  task_dependencies_dot_file: Optional[str],
+                  log_level: Optional[str],
+                  use_job_specific_log_file: bool
+                  ):
     """
     This command executes the security scan, which must be defined as separate step in the build steps declaration.
     The scan runs the docker container of the respective step, passing a folder of the output-dir as argument.
     If the stages do not exists locally, the system will build or pull them before running the scan.
     """
     with TerminationHandler():
-        scan_result = api.security_scan(flavor_path,
-                                        force_rebuild,
-                                        force_rebuild_from,
-                                        force_pull,
-                                        output_directory,
-                                        temporary_base_directory,
-                                        log_build_context_content,
-                                        cache_directory,
-                                        build_name,
-                                        source_docker_repository_name,
-                                        source_docker_tag_prefix,
-                                        source_docker_username,
-                                        source_docker_password,
-                                        target_docker_repository_name,
-                                        target_docker_tag_prefix,
-                                        target_docker_username,
-                                        target_docker_password,
-                                        workers,
-                                        task_dependencies_dot_file)
+        scan_result = api.security_scan(flavor_path=flavor_path,
+                                        force_rebuild=force_rebuild,
+                                        force_rebuild_from=force_rebuild_from,
+                                        force_pull=force_pull,
+                                        output_directory=output_directory,
+                                        temporary_base_directory=temporary_base_directory,
+                                        log_build_context_content=log_build_context_content,
+                                        cache_directory=cache_directory,
+                                        build_name=build_name,
+                                        source_docker_repository_name=source_docker_repository_name,
+                                        source_docker_tag_prefix=source_docker_tag_prefix,
+                                        source_docker_username=source_docker_username,
+                                        source_docker_password=source_docker_password,
+                                        target_docker_repository_name=target_docker_repository_name,
+                                        target_docker_tag_prefix=target_docker_tag_prefix,
+                                        target_docker_username=target_docker_username,
+                                        target_docker_password=target_docker_password,
+                                        workers=workers,
+                                        task_dependencies_dot_file=task_dependencies_dot_file,
+                                        log_level=log_level,
+                                        use_job_specific_log_file=use_job_specific_log_file
+                                        )
         if scan_result.report_path.exists():
             with scan_result.report_path.open("r") as f:
                 print(f.read())
         if not scan_result.scans_are_ok:
             raise RuntimeError("Some security scans not successful.")
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/upload.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/commands/upload.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from exasol_integration_test_docker_environment.lib.api.common import add_options
 
 from exasol_script_languages_container_tool.cli.options.flavor_options import flavor_options
 from exasol_script_languages_container_tool.cli.options.goal_options import release_options
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
-from exasol_integration_test_docker_environment.cli.options.system_options import system_options
+from exasol_integration_test_docker_environment.cli.options.system_options import system_options, luigi_logging_options
 from exasol_script_languages_container_tool.lib import api
 
 
 @cli.command(short_help="Uploads the script-language-container to the database.")
 @add_options(flavor_options)
 @click.option('--database-host', type=str,
               required=True)
@@ -25,14 +25,15 @@
 @click.option('--bucketfs-https/--no-bucketfs-https', default=False)
 @click.option('--path-in-bucket', type=str, required=False, default='')
 @add_options(release_options)
 @click.option('--release-name', type=str, default=None)
 @add_options(build_options)
 @add_options(docker_repository_options)
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def upload(flavor_path: Tuple[str, ...],
            database_host: str,
            bucketfs_port: int,
            bucketfs_username: str,
            bucketfs_name: str,
            bucket_name: str,
            bucketfs_password: Optional[str],
@@ -53,45 +54,51 @@
            source_docker_username: Optional[str],
            source_docker_password: Optional[str],
            target_docker_repository_name: str,
            target_docker_tag_prefix: str,
            target_docker_username: Optional[str],
            target_docker_password: Optional[str],
            workers: int,
-           task_dependencies_dot_file: Optional[str]):
+           task_dependencies_dot_file: Optional[str],
+           log_level: Optional[str],
+           use_job_specific_log_file: bool
+           ):
     """
     This command uploads the whole script-language-container package of the flavor to the database.
     If the stages or the packaged container do not exists locally, the system will build, pull or
     export them before the upload.
     """
     with TerminationHandler():
-        result = api.upload(flavor_path,
-                            database_host,
-                            bucketfs_port,
-                            bucketfs_username,
-                            bucketfs_name,
-                            bucket_name,
-                            bucketfs_password,
-                            bucketfs_https,
-                            path_in_bucket,
-                            release_goal,
-                            release_name,
-                            force_rebuild,
-                            force_rebuild_from,
-                            force_pull,
-                            output_directory,
-                            temporary_base_directory,
-                            log_build_context_content,
-                            cache_directory,
-                            build_name,
-                            source_docker_repository_name,
-                            source_docker_tag_prefix,
-                            source_docker_username,
-                            source_docker_password,
-                            target_docker_repository_name,
-                            target_docker_tag_prefix,
-                            target_docker_username,
-                            target_docker_password,
-                            workers,
-                            task_dependencies_dot_file)
+        result = api.upload(flavor_path=flavor_path,
+                            database_host=database_host,
+                            bucketfs_port=bucketfs_port,
+                            bucketfs_username=bucketfs_username,
+                            bucketfs_name=bucketfs_name,
+                            bucket_name=bucket_name,
+                            bucketfs_password=bucketfs_password,
+                            bucketfs_https=bucketfs_https,
+                            path_in_bucket=path_in_bucket,
+                            release_goal=release_goal,
+                            release_name=release_name,
+                            force_rebuild=force_rebuild,
+                            force_rebuild_from=force_rebuild_from,
+                            force_pull=force_pull,
+                            output_directory=output_directory,
+                            temporary_base_directory=temporary_base_directory,
+                            log_build_context_content=log_build_context_content,
+                            cache_directory=cache_directory,
+                            build_name=build_name,
+                            source_docker_repository_name=source_docker_repository_name,
+                            source_docker_tag_prefix=source_docker_tag_prefix,
+                            source_docker_username=source_docker_username,
+                            source_docker_password=source_docker_password,
+                            target_docker_repository_name=target_docker_repository_name,
+                            target_docker_tag_prefix=target_docker_tag_prefix,
+                            target_docker_username=target_docker_username,
+                            target_docker_password=target_docker_password,
+                            workers=workers,
+                            task_dependencies_dot_file=task_dependencies_dot_file,
+                            log_level=log_level,
+                            use_job_specific_log_file=use_job_specific_log_file
+                            )
         with result.open("r") as f:
             print(f.read())
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/flavor_options.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/options/flavor_options.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/goal_options.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/cli/options/goal_options.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/build.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,18 @@
           source_docker_username: Optional[str] = None,
           source_docker_password: Optional[str] = None,
           target_docker_repository_name: str = 'exasol/script-language-container',
           target_docker_tag_prefix: str = '',
           target_docker_username: Optional[str] = None,
           target_docker_password: Optional[str] = None,
           workers: int = 5,
-          task_dependencies_dot_file: Optional[str] = None) -> Dict[str, ImageInfo]:
+          task_dependencies_dot_file: Optional[str] = None,
+          log_level: Optional[str] = None,
+          use_job_specific_log_file: bool = True
+          ) -> Dict[str, ImageInfo]:
     """
     This command builds all stages of the script-language-container flavor.
     If stages are cached in a docker registry, they command is going to pull them,
     instead of building them.
     :raises api_errors.TaskFailureError: if operation is not successful.
     :return: Image info per goal.
     """
@@ -54,8 +57,13 @@
 
     def root_task_generator() -> DependencyLoggerBaseTask:
         return generate_root_task(task_class=DockerBuild,
                                   flavor_paths=list(flavor_path),
                                   goals=list(goal),
                                   shortcut_build=shortcut_build)
 
-    return run_task(root_task_generator, workers, task_dependencies_dot_file)
+    return run_task(root_task_generator,
+                    workers=workers,
+                    task_dependencies_dot_file=task_dependencies_dot_file,
+                    log_level=log_level,
+                    use_job_specific_log_file=use_job_specific_log_file
+                    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/build_test_container.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/push_test_container.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageInfo
 
 from exasol_script_languages_container_tool.cli.options.test_container_options import TEST_CONTAINER_DEFAULT_DIRECTORY
 from exasol_script_languages_container_tool.lib.tasks.test.test_container_content import build_test_container_content
 
 
 @cli_function
-def build_test_container(
+def push_test_container(
         test_container_folder: str = TEST_CONTAINER_DEFAULT_DIRECTORY,
+        force_push: bool = False,
+        push_all: bool = False,
         force_rebuild: bool = False,
         force_rebuild_from: Tuple[str, ...] = tuple(),
         force_pull: bool = False,
         output_directory: str = ".build_output",
         temporary_base_directory: str = "/tmp",
         log_build_context_content: bool = False,
         cache_directory: Optional[str] = None,
@@ -24,22 +26,26 @@
         source_docker_username: Optional[str] = None,
         source_docker_password: Optional[str] = None,
         target_docker_repository_name: str = 'exasol/script-language-container',
         target_docker_tag_prefix: str = '',
         target_docker_username: Optional[str] = None,
         target_docker_password: Optional[str] = None,
         workers: int = 5,
-        task_dependencies_dot_file: Optional[str] = None) -> ImageInfo:
+        task_dependencies_dot_file: Optional[str] = None,
+        log_level: Optional[str] = None,
+        use_job_specific_log_file: bool = True) -> ImageInfo:
     """
-    Build the test container docker image.
+    Push the test container docker image to the registry.
 
     The test container is used during tests of the Script-Language-Container.
     """
-    return api.build_test_container(
+    return api.push_test_container(
         test_container_content=build_test_container_content(test_container_folder),
+        force_push=force_push,
+        push_all=push_all,
         force_rebuild=force_rebuild,
         force_rebuild_from=force_rebuild_from,
         force_pull=force_pull,
         output_directory=output_directory,
         temporary_base_directory=temporary_base_directory,
         log_build_context_content=log_build_context_content,
         cache_directory=cache_directory,
@@ -49,8 +55,11 @@
         source_docker_username=source_docker_username,
         source_docker_password=source_docker_password,
         target_docker_repository_name=target_docker_repository_name,
         target_docker_tag_prefix=target_docker_tag_prefix,
         target_docker_username=target_docker_username,
         target_docker_password=target_docker_password,
         workers=workers,
-        task_dependencies_dot_file=task_dependencies_dot_file)
+        task_dependencies_dot_file=task_dependencies_dot_file,
+        log_level=log_level,
+        use_job_specific_log_file=use_job_specific_log_file
+    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/clean.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/clean.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,46 +10,58 @@
 
 @cli_function
 def clean_flavor_images(flavor_path: Tuple[str, ...],
                         output_directory: str = ".build_output",
                         docker_repository_name: str = 'exasol/script-language-container',
                         docker_tag_prefix: str = '',
                         workers: int = 5,
-                        task_dependencies_dot_file: Optional[str] = None) -> None:
+                        task_dependencies_dot_file: Optional[str] = None,
+                        log_level: Optional[str] = None,
+                        use_job_specific_log_file: bool = True) -> None:
     """
     This command removes the docker images of all stages of the script languages container for the given flavor.
     raises:
         api_errors.TaskFailureError: if operation is not successful.
     """
     import_build_steps(flavor_path)
     set_output_directory(output_directory)
     set_docker_repository_config(None, docker_repository_name, None, docker_tag_prefix, "source")
     set_docker_repository_config(None, docker_repository_name, None, docker_tag_prefix, "target")
 
     def root_task_generator() -> DependencyLoggerBaseTask:
         return generate_root_task(task_class=CleanExaslcFlavorsImages, flavor_paths=list(flavor_path))
 
-    run_task(root_task_generator, workers, task_dependencies_dot_file)
+    run_task(root_task_generator,
+             workers=workers,
+             task_dependencies_dot_file=task_dependencies_dot_file,
+             log_level=log_level,
+             use_job_specific_log_file=use_job_specific_log_file)
 
 
 @cli_function
 def clean_all_images(
         output_directory: str = '.build_output',
         docker_repository_name: str = 'exasol/script-language-container',
         docker_tag_prefix: str = '',
         workers: int = 5,
-        task_dependencies_dot_file: Optional[str] = None) -> None:
+        task_dependencies_dot_file: Optional[str] = None,
+        log_level: Optional[str] = None,
+        use_job_specific_log_file: bool = True) -> None:
     """
     This command removes the docker images of all stages of the script languages container for all flavors.
     raises:
         api_errors.TaskFailureError: if operation is not successful.
     """
     set_output_directory(output_directory)
     set_docker_repository_config(None, docker_repository_name, None, docker_tag_prefix, "source")
     set_docker_repository_config(None, docker_repository_name, None, docker_tag_prefix, "target")
 
     def root_task_generator() -> DependencyLoggerBaseTask:
         return generate_root_task(task_class=CleanExaslcAllImages)
 
-    run_task(root_task_generator, workers, task_dependencies_dot_file)
+    run_task(root_task_generator,
+             workers=workers,
+             task_dependencies_dot_file=task_dependencies_dot_file,
+             log_level=log_level,
+             use_job_specific_log_file=use_job_specific_log_file)
 
 # TODO add commands clean containers, networks, all
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/export.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,17 @@
            source_docker_username: Optional[str] = None,
            source_docker_password: Optional[str] = None,
            target_docker_repository_name: str = 'exasol/script-language-container',
            target_docker_tag_prefix: str = '',
            target_docker_username: Optional[str] = None,
            target_docker_password: Optional[str] = None,
            workers: int = 5,
-           task_dependencies_dot_file: Optional[str] = None) -> ExportContainerResult:
+           task_dependencies_dot_file: Optional[str] = None,
+           log_level: Optional[str] = None,
+           use_job_specific_log_file: bool = True) -> ExportContainerResult:
     """
     This command exports the whole script-language-container package of the flavor,
     ready for the upload into the bucketfs. If the stages do not exists locally,
     the system will build or pull them before the exporting the packaged container.
     :raises api_errors.TaskFailureError: if operation is not successful.
     :returns: ExportContainerResult
     """
@@ -55,8 +57,13 @@
     def root_task_generator() -> DependencyLoggerBaseTask:
         return generate_root_task(task_class=ExportContainers,
                                   flavor_paths=list(flavor_path),
                                   release_goals=list(release_goal),
                                   export_path=export_path,
                                   release_name=release_name)
 
-    return run_task(root_task_generator, workers, task_dependencies_dot_file)
+    return run_task(root_task_generator,
+                    workers=workers,
+                    task_dependencies_dot_file=task_dependencies_dot_file,
+                    log_level=log_level,
+                    use_job_specific_log_file=use_job_specific_log_file
+                    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/push.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/security_scan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,69 @@
-from typing import Tuple, Optional, Dict, List
+from pathlib import Path
+from typing import Tuple, Optional
 
-from exasol_integration_test_docker_environment.lib.api.common import set_docker_repository_config, generate_root_task, \
-    run_task, import_build_steps, set_build_config, cli_function
+import luigi
+from exasol_integration_test_docker_environment.lib.api.common import import_build_steps, set_build_config, \
+    set_docker_repository_config, generate_root_task, run_task, cli_function
 from exasol_integration_test_docker_environment.lib.base.dependency_logger_base_task import DependencyLoggerBaseTask
-from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageInfo
 
-from exasol_script_languages_container_tool.lib.api import api_errors
-from exasol_script_languages_container_tool.lib.tasks.push.docker_push import DockerFlavorsPush
+from exasol_script_languages_container_tool.lib.tasks.security_scan.security_scan import SecurityScan, AllScanResult
 
 
 @cli_function
-def push(flavor_path: Tuple[str, ...],
-         goal: Tuple[str, ...] = tuple(),
-         force_push: bool = False,
-         push_all: bool = False,
-         force_rebuild: bool = False,
-         force_rebuild_from: Tuple[str, ...] = tuple(),
-         force_pull: bool = False,
-         output_directory: str = '.build_output',
-         temporary_base_directory: str = "/tmp",
-         log_build_context_content: bool = False,
-         cache_directory: Optional[str] = None,
-         build_name: Optional[str] = None,
-         source_docker_repository_name: str = 'exasol/script-language-container',
-         source_docker_tag_prefix: str = '',
-         source_docker_username: Optional[str] = None,
-         source_docker_password: Optional[str] = None,
-         target_docker_repository_name: str = 'exasol/script-language-container',
-         target_docker_tag_prefix: str = '',
-         target_docker_username: Optional[str] = None,
-         target_docker_password: Optional[str] = None,
-         workers: int = 5,
-         task_dependencies_dot_file: Optional[str] = None) -> Dict[str, List[ImageInfo]]:
+def security_scan(flavor_path: Tuple[str, ...],
+                  force_rebuild: bool = False,
+                  force_rebuild_from: Tuple[str, ...] = tuple(),
+                  force_pull: bool = False,
+                  output_directory: str = ".build_output",
+                  temporary_base_directory: str = "/tmp",
+                  log_build_context_content: bool = False,
+                  cache_directory: Optional[str] = None,
+                  build_name: Optional[str] = None,
+                  source_docker_repository_name: str = 'exasol/script-language-container',
+                  source_docker_tag_prefix: str = '',
+                  source_docker_username: Optional[str] = None,
+                  source_docker_password: Optional[str] = None,
+                  target_docker_repository_name: str = 'exasol/script-language-container',
+                  target_docker_tag_prefix: str = '',
+                  target_docker_username: Optional[str] = None,
+                  target_docker_password: Optional[str] = None,
+                  workers: int = 5,
+                  task_dependencies_dot_file: Optional[str] = None,
+                  log_level: Optional[str] = None,
+                  use_job_specific_log_file: bool = True
+                  ) -> AllScanResult:
     """
-    This command pushes all stages of the script-language-container flavor.
-    If the stages do not exists locally, the system will build or pull them before the push.
+    This command executes the security scan, which must be defined as separate step in the build steps declaration.
+    The scan runs the docker container of the respective step, passing a folder of the output-dir as argument.
+    If the stages do not exists locally, the system will build or pull them before running the scan.
     :raises api_errors.TaskFailureError: if operation is not successful.
-    :return: list of image infos per flavor.
+    :return: Results of all scans.
     """
-
     import_build_steps(flavor_path)
     set_build_config(force_rebuild,
                      force_rebuild_from,
                      force_pull,
                      log_build_context_content,
                      output_directory,
                      temporary_base_directory,
                      cache_directory,
                      build_name)
     set_docker_repository_config(source_docker_password, source_docker_repository_name, source_docker_username,
                                  source_docker_tag_prefix, "source")
     set_docker_repository_config(target_docker_password, target_docker_repository_name, target_docker_username,
                                  target_docker_tag_prefix, "target")
 
-    def root_task_generator() -> DependencyLoggerBaseTask:
-        return generate_root_task(task_class=DockerFlavorsPush,
-                                  force_push=force_push,
-                                  push_all=push_all,
-                                  goals=list(goal),
-                                  flavor_paths=list(flavor_path))
+    report_path = Path(output_directory).joinpath("security_scan")
 
-    return run_task(root_task_generator, workers, task_dependencies_dot_file)
+    def root_task_generator() -> DependencyLoggerBaseTask:
+        return generate_root_task(task_class=SecurityScan,
+                                  flavor_paths=list(flavor_path),
+                                  report_path=str(report_path)
+                                  )
+
+    return run_task(root_task_generator,
+                    workers=workers,
+                    task_dependencies_dot_file=task_dependencies_dot_file,
+                    log_level=log_level,
+                    use_job_specific_log_file=use_job_specific_log_file
+                    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
                 test_file: Tuple[str, ...] = tuple(),
                 test_language: Tuple[str, ...] = (None,),
                 test: Tuple[str, ...] = tuple(),
                 environment_type: str = 'docker_db',
                 max_start_attempts: int = 2,
                 docker_db_image_version: str = LATEST_DB_VERSION,
                 docker_db_image_name: str = "exasol/docker-db",
+                db_os_access: str = "DOCKER_EXEC",
                 create_certificates: bool = False,
                 additional_db_parameter: Tuple[str, ...] = tuple(),
                 external_exasol_db_host: Optional[str] = None,
                 external_exasol_db_port: int = 8563,
                 external_exasol_bucketfs_port: int = 6583,
                 external_exasol_db_user: Optional[str] = None,
                 external_exasol_db_password: Optional[str] = None,
@@ -61,15 +62,18 @@
                 source_docker_username: Optional[str] = None,
                 source_docker_password: Optional[str] = None,
                 target_docker_repository_name: str = 'exasol/script-language-container',
                 target_docker_tag_prefix: str = '',
                 target_docker_username: Optional[str] = None,
                 target_docker_password: Optional[str] = None,
                 workers: int = 5,
-                task_dependencies_dot_file: Optional[str] = None) -> AllTestsResult:
+                task_dependencies_dot_file: Optional[str] = None,
+                log_level: Optional[str] = None,
+                use_job_specific_log_file: bool = True
+                ) -> AllTestsResult:
     """
     This command runs the integration tests in local docker-db.
     The system spawns a test environment in which the test are executed.
     After finishing the tests, the test environment gets cleaned up.
     If the stages or the packaged container do not exists locally,
     the system will build, pull or export them before running the tests.
     :raises api.errors.MissingArgumentError: if one or more arguments are not set.
@@ -140,8 +144,13 @@
                                   external_exasol_xmlrpc_password=external_exasol_xmlrpc_password,
                                   external_exasol_xmlrpc_cluster_name=external_exasol_xmlrpc_cluster_name,
                                   create_certificates=create_certificates,
                                   additional_db_parameter=additional_db_parameter,
                                   test_container_content=build_test_container_content(test_container_folder)
                                   )
 
-    return run_task(root_task_generator, workers, task_dependencies_dot_file)
+    return run_task(root_task_generator,
+                    workers=workers,
+                    task_dependencies_dot_file=task_dependencies_dot_file,
+                    log_level=log_level,
+                    use_job_specific_log_file=use_job_specific_log_file
+                    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/save.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/save.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,18 @@
          source_docker_username: Optional[str] = None,
          source_docker_password: Optional[str] = None,
          target_docker_repository_name: str = 'exasol/script-language-container',
          target_docker_tag_prefix: str = '',
          target_docker_username: Optional[str] = None,
          target_docker_password: Optional[str] = None,
          workers: int = 5,
-         task_dependencies_dot_file: Optional[str] = None) -> Dict[str, List[ImageInfo]]:
+         task_dependencies_dot_file: Optional[str] = None,
+         log_level: Optional[str] = None,
+         use_job_specific_log_file: bool = True
+         ) -> Dict[str, List[ImageInfo]]:
     """
     This command saves all stages of the script-language-container flavor to a local directory.
     If the stages do not exists locally, the system will build or pull them before the execution of save.
     :raises api_errors.TaskFailureError: if operation is not successful.
     :return: List of image infos per flavor.
     """
     import_build_steps(flavor_path)
@@ -55,8 +58,14 @@
     def root_task_generator() -> DependencyLoggerBaseTask:
         return generate_root_task(task_class=DockerSave,
                                   save_path=save_directory,
                                   force_save=force_save,
                                   save_all=save_all,
                                   flavor_paths=list(flavor_path),
                                   goals=list(goal))
-    return run_task(root_task_generator, workers, task_dependencies_dot_file)
+
+    return run_task(root_task_generator,
+                    workers=workers,
+                    task_dependencies_dot_file=task_dependencies_dot_file,
+                    log_level=log_level,
+                    use_job_specific_log_file=use_job_specific_log_file
+                    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/security_scan.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/push.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,71 @@
-from pathlib import Path
-from typing import Tuple, Optional
+from typing import Tuple, Optional, Dict, List
 
-import luigi
-from exasol_integration_test_docker_environment.lib.api.common import import_build_steps, set_build_config, \
-    set_docker_repository_config, generate_root_task, run_task, cli_function
+from exasol_integration_test_docker_environment.lib.api.common import set_docker_repository_config, generate_root_task, \
+    run_task, import_build_steps, set_build_config, cli_function
 from exasol_integration_test_docker_environment.lib.base.dependency_logger_base_task import DependencyLoggerBaseTask
+from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageInfo
 
-from exasol_script_languages_container_tool.lib.tasks.security_scan.security_scan import SecurityScan, AllScanResult
+from exasol_script_languages_container_tool.lib.api import api_errors
+from exasol_script_languages_container_tool.lib.tasks.push.docker_push import DockerFlavorsPush
 
 
 @cli_function
-def security_scan(flavor_path: Tuple[str, ...],
-                  force_rebuild: bool = False,
-                  force_rebuild_from: Tuple[str, ...] = tuple(),
-                  force_pull: bool = False,
-                  output_directory: str = ".build_output",
-                  temporary_base_directory: str = "/tmp",
-                  log_build_context_content: bool = False,
-                  cache_directory: Optional[str] = None,
-                  build_name: Optional[str] = None,
-                  source_docker_repository_name: str = 'exasol/script-language-container',
-                  source_docker_tag_prefix: str = '',
-                  source_docker_username: Optional[str] = None,
-                  source_docker_password: Optional[str] = None,
-                  target_docker_repository_name: str = 'exasol/script-language-container',
-                  target_docker_tag_prefix: str = '',
-                  target_docker_username: Optional[str] = None,
-                  target_docker_password: Optional[str] = None,
-                  workers: int = 5,
-                  task_dependencies_dot_file: Optional[str] = None) -> AllScanResult:
+def push(flavor_path: Tuple[str, ...],
+         goal: Tuple[str, ...] = tuple(),
+         force_push: bool = False,
+         push_all: bool = False,
+         force_rebuild: bool = False,
+         force_rebuild_from: Tuple[str, ...] = tuple(),
+         force_pull: bool = False,
+         output_directory: str = '.build_output',
+         temporary_base_directory: str = "/tmp",
+         log_build_context_content: bool = False,
+         cache_directory: Optional[str] = None,
+         build_name: Optional[str] = None,
+         source_docker_repository_name: str = 'exasol/script-language-container',
+         source_docker_tag_prefix: str = '',
+         source_docker_username: Optional[str] = None,
+         source_docker_password: Optional[str] = None,
+         target_docker_repository_name: str = 'exasol/script-language-container',
+         target_docker_tag_prefix: str = '',
+         target_docker_username: Optional[str] = None,
+         target_docker_password: Optional[str] = None,
+         workers: int = 5,
+         task_dependencies_dot_file: Optional[str] = None,
+         log_level: Optional[str] = None,
+         use_job_specific_log_file: bool = True
+         ) -> Dict[str, List[ImageInfo]]:
     """
-    This command executes the security scan, which must be defined as separate step in the build steps declaration.
-    The scan runs the docker container of the respective step, passing a folder of the output-dir as argument.
-    If the stages do not exists locally, the system will build or pull them before running the scan.
+    This command pushes all stages of the script-language-container flavor.
+    If the stages do not exists locally, the system will build or pull them before the push.
     :raises api_errors.TaskFailureError: if operation is not successful.
-    :return: Results of all scans.
+    :return: list of image infos per flavor.
     """
+
     import_build_steps(flavor_path)
     set_build_config(force_rebuild,
                      force_rebuild_from,
                      force_pull,
                      log_build_context_content,
                      output_directory,
                      temporary_base_directory,
                      cache_directory,
                      build_name)
     set_docker_repository_config(source_docker_password, source_docker_repository_name, source_docker_username,
                                  source_docker_tag_prefix, "source")
     set_docker_repository_config(target_docker_password, target_docker_repository_name, target_docker_username,
                                  target_docker_tag_prefix, "target")
 
-    report_path = Path(output_directory).joinpath("security_scan")
-
     def root_task_generator() -> DependencyLoggerBaseTask:
-        return generate_root_task(task_class=SecurityScan,
-                                  flavor_paths=list(flavor_path),
-                                  report_path=str(report_path)
-                                  )
-    return run_task(root_task_generator, workers, task_dependencies_dot_file)
+        return generate_root_task(task_class=DockerFlavorsPush,
+                                  force_push=force_push,
+                                  push_all=push_all,
+                                  goals=list(goal),
+                                  flavor_paths=list(flavor_path))
+
+    return run_task(root_task_generator,
+                    workers=workers,
+                    task_dependencies_dot_file=task_dependencies_dot_file,
+                    log_level=log_level,
+                    use_job_specific_log_file=use_job_specific_log_file
+                    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/upload.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/api/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,18 @@
            source_docker_username: Optional[str] = None,
            source_docker_password: Optional[str] = None,
            target_docker_repository_name: str = 'exasol/script-language-container',
            target_docker_tag_prefix: str = '',
            target_docker_username: Optional[str] = None,
            target_docker_password: Optional[str] = None,
            workers: int = 5,
-           task_dependencies_dot_file: Optional[str] = None) -> luigi.LocalTarget:
+           task_dependencies_dot_file: Optional[str] = None,
+           log_level: Optional[str] = None,
+           use_job_specific_log_file: bool = True
+           ) -> luigi.LocalTarget:
     """
     This command uploads the whole script-language-container package of the flavor to the database.
     If the stages or the packaged container do not exists locally, the system will build, pull or
     export them before the upload.
     :raises api_errors.TaskFailureError: if operation is not successful.
     :return: Path to resulting report file.
     """
@@ -73,8 +76,13 @@
                                   bucketfs_password=bucketfs_password,
                                   bucket_name=bucket_name,
                                   path_in_bucket=path_in_bucket,
                                   bucketfs_https=bucketfs_https,
                                   release_name=release_name,
                                   bucketfs_name=bucketfs_name)
 
-    return run_task(root_task_generator, workers, task_dependencies_dot_file)
+    return run_task(root_task_generator,
+                    workers=workers,
+                    task_dependencies_dot_file=task_dependencies_dot_file,
+                    log_level=log_level,
+                    use_job_specific_log_file=use_job_specific_log_file
+                    )
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,14 @@
     SpawnTestEnvironmentParameter
 from exasol_integration_test_docker_environment.lib.test_environment.spawn_test_environment import SpawnTestEnvironment
 
 
 class TestRunnerDBTestTask(FlavorBaseTask,
                            SpawnTestEnvironmentParameter,
                            RunDBTestsInTestConfigParameter):
-    # TODO execute tests only if the exported container is new build
-    #       - a pulled one is ok,
-    #       - needs change in image-info and export-info)
-    #       - add options force tests
-    #       - only possible if the hash of exaslc also goes into the image hashes
-
     reuse_uploaded_container = luigi.BoolParameter(False, significant=False)
     release_goal = luigi.Parameter()
 
     def __init__(self, *args, **kwargs):
         self.test_environment_info = None
         super().__init__(*args, **kwargs)
 
@@ -58,49 +52,50 @@
 
     def run_task(self):
         export_infos = self.get_values_from_future(
             self._export_infos_future)  # type: Dict[str,ExportInfo]
         export_info = export_infos[self.release_goal]
         self.test_environment_info = self.get_values_from_future(
             self._test_environment_info_future)  # type: EnvironmentInfo
-        reuse_release_container = \
-            self.reuse_database and \
-            self.reuse_uploaded_container and \
-            not export_info.is_new
         database_credentials = self.get_database_credentials()
         yield from self.upload_container(database_credentials,
-                                         export_info,
-                                         reuse_release_container)
+                                         export_info)
         yield from self.populate_test_engine_data(self.test_environment_info, database_credentials)
         test_results = yield from self.run_test(self.test_environment_info, export_info)
         self.return_object(test_results)
 
-    def upload_container(self, database_credentials, export_info, reuse_release_container):
+    def upload_container(self, database_credentials: DatabaseCredentials, export_info: ExportInfo):
+        reuse = \
+            self.reuse_database and \
+            self.reuse_uploaded_container and \
+            not export_info.is_new
         upload_task = self.create_child_task_with_common_params(
             UploadExportedContainer,
             export_info=export_info,
             environment_name=self.test_environment_info.name,
             test_environment_info=self.test_environment_info,
             release_name=export_info.name,
-            reuse_uploaded=reuse_release_container,
+            reuse_uploaded=reuse,
             bucketfs_write_password=database_credentials.bucketfs_write_password
         )
         yield from self.run_dependencies(upload_task)
 
     def populate_test_engine_data(self, test_environment_info: EnvironmentInfo,
                                   database_credentials: DatabaseCredentials) -> None:
-        task = self.create_child_task(
-            PopulateTestEngine,
-            test_environment_info=test_environment_info,
-            environment_name=self.test_environment_info.name,
-            db_user=database_credentials.db_user,
-            db_password=database_credentials.db_password,
-            bucketfs_write_password=database_credentials.bucketfs_write_password
-        )
-        yield from self.run_dependencies(task)
+        reuse = self.reuse_database_setup and self.test_environment_info.database_info.reused
+        if not reuse:
+            task = self.create_child_task(
+                PopulateTestEngine,
+                test_environment_info=test_environment_info,
+                environment_name=self.test_environment_info.name,
+                db_user=database_credentials.db_user,
+                db_password=database_credentials.db_password,
+                bucketfs_write_password=database_credentials.bucketfs_write_password
+            )
+            yield from self.run_dependencies(task)
 
     def get_database_credentials(self) -> DatabaseCredentials:
         if self.environment_type == EnvironmentType.external_db:
             return \
                 DatabaseCredentials(db_user=self.external_exasol_db_user,
                                     db_password=self.external_exasol_db_password,
                                     bucketfs_write_password=self.external_exasol_bucketfs_write_password)
```

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh` & `exasol_script_languages_container_tool-0.18.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.17.0/pyproject.toml` & `exasol_script_languages_container_tool-0.18.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exasol-script-languages-container-tool"
-version = "0.17.0"
+version = "0.18.0"
 description = "Script Languages Container Tool"
 
 license = "MIT"
 
 authors = [
     "Torsten Kilias <torsten.kilias@exasol.com>"
 ]
@@ -17,16 +17,18 @@
 keywords = ['exasol', 'udf', 'script-languages']
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 importlib_metadata = ">=4.6.0"
 importlib-resources = ">=5.4.0"
 networkx = "2.8.2" # We pinned networkx to this version, because in newer versions it throws an exception, see https://github.com/exasol/integration-test-docker-environment/issues/228
-exasol-integration-test-docker-environment = "^1.6.0"
+exasol-integration-test-docker-environment = "^1.7.1"
 typeguard = "<3.0.0"
+configobj = "^5.0.8"
+
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
 toml = ">=0.10.2"
```

### Comparing `exasol_script_languages_container_tool-0.17.0/PKG-INFO` & `exasol_script_languages_container_tool-0.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: exasol-script-languages-container-tool
-Version: 0.17.0
+Version: 0.18.0
 Summary: Script Languages Container Tool
 Home-page: https://github.com/exasol/script-languages-container-tool
 License: MIT
 Keywords: exasol,udf,script-languages
 Author: Torsten Kilias
 Author-email: torsten.kilias@exasol.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: exasol-integration-test-docker-environment (>=1.6.0,<2.0.0)
+Requires-Dist: configobj (>=5.0.8,<6.0.0)
+Requires-Dist: exasol-integration-test-docker-environment (>=1.7.1,<2.0.0)
 Requires-Dist: importlib-resources (>=5.4.0)
 Requires-Dist: importlib_metadata (>=4.6.0)
 Requires-Dist: networkx (==2.8.2)
 Requires-Dist: typeguard (<3.0.0)
 Project-URL: Repository, https://github.com/exasol/script-languages-container-tool
 Description-Content-Type: text/markdown
```

