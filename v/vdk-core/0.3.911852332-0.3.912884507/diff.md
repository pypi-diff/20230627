# Comparing `tmp/vdk-core-0.3.911852332.tar.gz` & `tmp/vdk-core-0.3.912884507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-core-0.3.911852332.tar", last modified: Mon Jun 26 12:10:56 2023, max compression
+gzip compressed data, was "dist/vdk-core-0.3.912884507.tar", last modified: Tue Jun 27 08:54:29 2023, max compression
```

## Comparing `vdk-core-0.3.911852332.tar` & `vdk-core-0.3.912884507.tar`

### file list

```diff
@@ -1,109 +1,118 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1542 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/api/
--rw-rw-rw-   0 root         (0) root         (0)     2561 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/api/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)    19041 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/api/job_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/api/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     6715 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/api/plugin/connection_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     7784 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/api/plugin/core_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/api/plugin/hook_markers.py
--rw-rw-rw-   0 root         (0) root         (0)    27782 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/api/plugin/plugin_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4057 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/api/plugin/plugin_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/api/plugin/plugin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/
--rw-rw-rw-   0 root         (0) root         (0)     5894 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/
--rw-rw-rw-   0 root         (0) root         (0)     5112 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/config_help.py
--rw-rw-rw-   0 root         (0) root         (0)     9440 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/job_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11191 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4661 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/impl/
--rw-rw-rw-   0 root         (0) root         (0)     6464 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/impl/router.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
--rw-rw-rw-   0 root         (0) root         (0)    10048 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/pep249/
--rw-rw-rw-   0 root         (0) root         (0)     2958 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/debug/
--rw-rw-rw-   0 root         (0) root         (0)     6082 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/debug/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/
--rw-rw-rw-   0 root         (0) root         (0)    29371 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4069 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13247 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/internal_hookspecs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8208 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/notification/
--rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/notification/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    10656 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/notification/notification_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7985 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/
--rw-rw-rw-   0 root         (0) root         (0)     9148 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/cli_run.py
--rw-rw-rw-   0 root         (0) root         (0)    13573 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/execution_environment.py
--rw-rw-rw-   0 root         (0) root         (0)     5515 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/execution_results.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/execution_state.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/execution_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)     7130 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/file_based_step.py
--rw-rw-rw-   0 root         (0) root         (0)     3911 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/job_context.py
--rw-rw-rw-   0 root         (0) root         (0)     7082 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/job_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4856 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/run_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
--rw-rw-rw-   0 root         (0) root         (0)     7959 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/templates/template_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/termination_message/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/termination_message/file_util.py
--rw-rw-rw-   0 root         (0) root         (0)     3119 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/termination_message/writer.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/version/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/version/new_version_check.py
--rw-rw-rw-   0 root         (0) root         (0)     4973 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/version/version.py
--rw-rw-rw-   0 root         (0) root         (0)     6471 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/cli_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/core/
--rw-rw-rw-   0 root         (0) root         (0)     9586 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/core/context.py
--rw-rw-rw-   0 root         (0) root         (0)    21237 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/core/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5683 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/core/statestore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     5200 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/plugin/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/plugin/plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk/internal/util/
--rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/util/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2023-06-26 12:10:34.000000 vdk-core-0.3.911852332/src/vdk/internal/util/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-26 12:10:54.000000 vdk-core-0.3.911852332/src/vdk/internal/vdk_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-26 12:10:56.000000 vdk-core-0.3.911852332/src/vdk_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-26 12:10:54.000000 vdk-core-0.3.911852332/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/api/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)    19040 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/api/job_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/api/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     6715 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/api/plugin/connection_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/api/plugin/core_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/api/plugin/hook_markers.py
+-rw-rw-rw-   0 root         (0) root         (0)    27782 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/api/plugin/plugin_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/api/plugin/plugin_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/api/plugin/plugin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     6060 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/config_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     9440 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/job_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11191 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/impl/
+-rw-rw-rw-   0 root         (0) root         (0)     6464 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/impl/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10048 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/pep249/
+-rw-rw-rw-   0 root         (0) root         (0)     2958 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/debug/
+-rw-rw-rw-   0 root         (0) root         (0)     6082 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/debug/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/
+-rw-rw-rw-   0 root         (0) root         (0)    29371 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4069 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13247 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/internal_hookspecs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8208 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/base_secrets_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/cached_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/datajobs_service_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/inmemsecrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/secrets_api_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/secrets_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7835 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/secrets_router.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_secrets/secretsnotavailable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/notification/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    10656 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/notification/notification_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7985 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/
+-rw-rw-rw-   0 root         (0) root         (0)     9148 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/cli_run.py
+-rw-rw-rw-   0 root         (0) root         (0)    13573 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/execution_environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5515 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/execution_results.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/execution_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/execution_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)     7130 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/file_based_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4252 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/job_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/job_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4856 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/run_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7959 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/templates/template_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/termination_message/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/termination_message/file_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3119 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/termination_message/writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/version/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/version/new_version_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/version/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6471 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/cli_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/core/
+-rw-rw-rw-   0 root         (0) root         (0)     9586 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/core/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    21237 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/core/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5683 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/core/statestore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/plugin/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/plugin/plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk/internal/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/util/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-06-27 08:54:06.000000 vdk-core-0.3.912884507/src/vdk/internal/util/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-27 08:54:27.000000 vdk-core-0.3.912884507/src/vdk/internal/vdk_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4857 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-27 08:54:29.000000 vdk-core-0.3.912884507/src/vdk_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-27 08:54:27.000000 vdk-core-0.3.912884507/version.txt
```

### Comparing `vdk-core-0.3.911852332/PKG-INFO` & `vdk-core-0.3.912884507/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.911852332
+Version: 0.3.912884507
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.911852332/README.md` & `vdk-core-0.3.912884507/README.md`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/setup.cfg` & `vdk-core-0.3.912884507/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/api/data_job.py` & `vdk-core-0.3.912884507/src/vdk/api/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/api/job_input.py` & `vdk-core-0.3.912884507/src/vdk/api/job_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """
     Allows for Data Job to store and retrieve sensitive data.
     Secrets are solution for the following use cases
     * Keeping API keys and passwords necessary to connect to different systems
     """
 
     @abstractmethod
-    def get_secret(self, name: str, default_value: Any = None) -> str:
+    def get_secret(self, key: str, default_value: Any = None) -> str:
         pass
 
     @abstractmethod
     def get_all_secrets(self) -> dict:
         pass
 
     @abstractmethod
```

### Comparing `vdk-core-0.3.911852332/src/vdk/api/plugin/connection_hook_spec.py` & `vdk-core-0.3.912884507/src/vdk/api/plugin/connection_hook_spec.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/api/plugin/core_hook_spec.py` & `vdk-core-0.3.912884507/src/vdk/api/plugin/core_hook_spec.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/api/plugin/hook_markers.py` & `vdk-core-0.3.912884507/src/vdk/api/plugin/hook_markers.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/api/plugin/plugin_input.py` & `vdk-core-0.3.912884507/src/vdk/api/plugin/plugin_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/api/plugin/plugin_registry.py` & `vdk-core-0.3.912884507/src/vdk/api/plugin/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/api/plugin/plugin_utils.py` & `vdk-core-0.3.912884507/src/vdk/api/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/builtin_hook_impl.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/builtin_hook_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 from vdk.internal.builtin_plugins.debug.debug import DebugPlugins
 from vdk.internal.builtin_plugins.ingestion.ingester_configuration_plugin import (
     IngesterConfigurationPlugin,
 )
 from vdk.internal.builtin_plugins.job_properties.properties_api_plugin import (
     PropertiesApiPlugin,
 )
+from vdk.internal.builtin_plugins.job_secrets.secrets_api_plugin import (
+    SecretsApiPlugin,
+)
 from vdk.internal.builtin_plugins.notification.notification import NotificationPlugin
 from vdk.internal.builtin_plugins.termination_message.writer import (
     TerminationMessageWriterPlugin,
 )
 from vdk.internal.builtin_plugins.version.new_version_check_plugin import (
     NewVersionCheckPlugin,
 )
@@ -115,14 +118,15 @@
     plugin_registry.load_plugin_with_hooks_impl(CoreConfigDefinitionPlugin())
     plugin_registry.load_plugin_with_hooks_impl(EnvironmentVarsConfigPlugin())
     plugin_registry.load_plugin_with_hooks_impl(RuntimeStateInitializePlugin())
     plugin_registry.load_plugin_with_hooks_impl(NewVersionCheckPlugin())
     plugin_registry.load_plugin_with_hooks_impl(NotificationPlugin())
     plugin_registry.load_plugin_with_hooks_impl(IngesterConfigurationPlugin())
     plugin_registry.load_plugin_with_hooks_impl(PropertiesApiPlugin())
+    plugin_registry.load_plugin_with_hooks_impl(SecretsApiPlugin())
     # TODO: should be in run package only
     plugin_registry.add_hook_specs(JobRunHookSpecs)
     plugin_registry.load_plugin_with_hooks_impl(JobConfigIniPlugin())
     plugin_registry.load_plugin_with_hooks_impl(TerminationMessageWriterPlugin())
     # connection plugins
     plugin_registry.add_hook_specs(ConnectionHookSpec)
     plugin_registry.load_plugin_with_hooks_impl(QueryDecoratorPlugin())
```

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/config_help.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/config_help.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/job_config.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/log_config.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/config/vdk_config.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/config/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/connection_hooks.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/connection_hooks.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/connection_plugin.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/connection_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/execution_cursor.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/execution_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/impl/router.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/impl/router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/managed_cursor.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/managed_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/debug/debug.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/debug/debug.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/internal_hookspecs.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/internal_hookspecs.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
-from typing import List
-from typing import Type
 
 
-def check_valid_property(k: str, v: str, supported_types: List[Type] = []) -> None:
+def check_valid_property(k: str, v: str, supported_types=None) -> None:
     """
     Check if property key and value are valid
     """
+    if supported_types is None:
+        supported_types = []
+
     if str != type(k) or k.strip() != k or "".join(k.split()) != k:
         msg = (
             f"Property {k} is of unsupported type or has unsupported name. "
             f"Only string properties with no whitespaces in the name are supported."
         )
         raise ValueError(msg)
```

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/properties_config.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/properties_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/properties_router.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/properties_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 class PropertiesNotAvailable(IProperties):
     """
     Implementation of IProperties that will throw an error if user tries to access them.
     """
 
     def __init__(self, error_handler: Callable[[str], None]):
         self._error_handler = error_handler
-        pass
 
     def get_property(self, name, default_value=None):  # @UnusedVariable
         self.tell_user("get_property")
 
     def get_all_properties(self):  # @UnusedVariable
         self.tell_user("get_all_properties")
```

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/notification/notification.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/notification/notification.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/notification/notification_base.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/notification/notification_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/notification/notification_configuration.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/notification/notification_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/cli_run.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/cli_run.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/data_job.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/execution_environment.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/execution_environment.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/execution_results.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/execution_results.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/execution_state.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/execution_state.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/execution_tracking.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/execution_tracking.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/file_based_step.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/file_based_step.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/job_context.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/job_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 from vdk.api.job_input import ITemplate
 from vdk.api.plugin.connection_hook_spec import (
     ConnectionHookSpec,
 )
 from vdk.api.plugin.plugin_input import IIngesterRegistry
 from vdk.api.plugin.plugin_input import IManagedConnectionRegistry
 from vdk.api.plugin.plugin_input import IPropertiesRegistry
+from vdk.api.plugin.plugin_input import ISecretsRegistry
 from vdk.api.plugin.plugin_input import ITemplateRegistry
 from vdk.internal.builtin_plugins.connection.connection_hooks import (
     ConnectionHookSpecFactory,
 )
 from vdk.internal.builtin_plugins.connection.impl.router import ManagedConnectionRouter
 from vdk.internal.builtin_plugins.ingestion.ingester_router import IngesterRouter
 from vdk.internal.builtin_plugins.job_properties.properties_router import (
     PropertiesRouter,
 )
+from vdk.internal.builtin_plugins.job_secrets.secrets_router import (
+    SecretsRouter,
+)
 from vdk.internal.builtin_plugins.run.step import StepBuilder
 from vdk.internal.core.context import CoreContext
 
 
 # TODO: split into mutable and immutable job context (e.g JobContextBuilder and JobContext)
 # JobContext is mutable only until initializing phase. After init phase only state store should be mutable.
 
@@ -59,16 +63,18 @@
     templates: ITemplateRegistry
     # job arguments passed by user for current execution
     job_args: IJobArguments
     # initialized job input
     job_input: IJobInput
     # initialize ingestion
     ingester: IIngesterRegistry
-    # initialize ingestion
+    # initialize properties
     properties: IPropertiesRegistry
+    # initialize secrets
+    secrets: ISecretsRegistry
 
     def __init__(
         self,
         name: str,
         job_directory: pathlib.Path,
         core_context: CoreContext,
         job_args: IJobArguments,
@@ -87,19 +93,22 @@
         self.templates = cast(ITemplateRegistry, templates)
         self.ingester = IngesterRouter(core_context.configuration, core_context.state)
 
         self.properties = PropertiesRouter(
             job_name=self.name, cfg=core_context.configuration
         )
 
+        self.secrets = SecretsRouter(job_name=self.name, cfg=core_context.configuration)
+
         from vdk.internal.builtin_plugins.run.job_input import JobInput
 
         self.job_input = JobInput(
             self.name,
             self.job_directory,
             self.core_context,
             self.job_args,
             cast(ITemplate, self.templates),
             cast(ManagedConnectionRouter, self.connections),
             cast(IngesterRouter, self.ingester),
             cast(PropertiesRouter, self.properties),
+            cast(SecretsRouter, self.secrets),
         )
```

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/job_input.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/job_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from vdk.internal.builtin_plugins.connection.managed_connection_base import (
     ManagedConnectionBase,
 )
 from vdk.internal.builtin_plugins.ingestion.ingester_router import IngesterRouter
 from vdk.internal.builtin_plugins.job_properties.properties_router import (
     PropertiesRouter,
 )
+from vdk.internal.builtin_plugins.job_secrets.secrets_router import (
+    SecretsRouter,
+)
 from vdk.internal.builtin_plugins.run.execution_results import ExecutionResult
 from vdk.internal.builtin_plugins.run.sql_argument_substitutor import (
     SqlArgumentSubstitutor,
 )
 from vdk.internal.core.context import CoreContext
 from vdk.internal.core.errors import ErrorMessage
 from vdk.internal.core.errors import SkipRemainingStepsException
@@ -41,25 +44,27 @@
         job_directory: pathlib.Path,
         core_context: CoreContext,
         job_arguments: IJobArguments,
         templates: ITemplate,
         managed_connection_builder: ManagedConnectionRouter,
         ingester: IngesterRouter,
         properties_router: PropertiesRouter,
+        secrets_router: SecretsRouter,
     ):
         """Constructor."""
 
         self.__name = name
         self.__job_directory = job_directory
         self.__statestore = core_context.state
         self.__job_arguments = job_arguments
         self.__templates = templates
         self.__managed_connection_builder = managed_connection_builder
         self.__ingester = ingester
         self.__properties_router = properties_router
+        self.__secrets_router = secrets_router
         self.__vdk_internal_telemetry = None
 
     # Connections
 
     def get_managed_connection(self) -> ManagedConnectionBase:
         return self.__managed_connection_builder.open_default_connection()
 
@@ -73,14 +78,23 @@
 
     def get_all_properties(self):
         return self.__properties_router.get_all_properties()
 
     def set_all_properties(self, properties):
         return self.__properties_router.set_all_properties(properties)
 
+    def get_secret(self, name, default_value=None):
+        return self.__secrets_router.get_secret(name, default_value)
+
+    def get_all_secrets(self):
+        return self.__secrets_router.get_all_secrets()
+
+    def set_all_secrets(self, secrets):
+        return self.__secrets_router.set_all_secrets(secrets)
+
     def _substitute_query_params(self, sql: str):
         sql = textwrap.dedent(sql).strip("\n") + "\n"
         query = sql
         sql_susbstitute_args = {}
         if not self.__properties_router.has_properties_impl():
             logging.getLogger(__name__).info(
                 "Data Job Properties has not been initialized., "
```

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/standalone_data_job.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/standalone_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/run/step.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/run/step.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/templates/template_impl.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/templates/template_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/termination_message/file_util.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/termination_message/file_util.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/termination_message/writer.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/termination_message/writer.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/version/new_version_check.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/version/new_version_check.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/builtin_plugins/version/version.py` & `vdk-core-0.3.912884507/src/vdk/internal/builtin_plugins/version/version.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/cli_entry.py` & `vdk-core-0.3.912884507/src/vdk/internal/cli_entry.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/core/config.py` & `vdk-core-0.3.912884507/src/vdk/internal/core/config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/core/context.py` & `vdk-core-0.3.912884507/src/vdk/internal/core/context.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/core/errors.py` & `vdk-core-0.3.912884507/src/vdk/internal/core/errors.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/core/statestore.py` & `vdk-core-0.3.912884507/src/vdk/internal/core/statestore.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/plugin/plugin.py` & `vdk-core-0.3.912884507/src/vdk/internal/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/util/decorators.py` & `vdk-core-0.3.912884507/src/vdk/internal/util/decorators.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk/internal/util/utils.py` & `vdk-core-0.3.912884507/src/vdk/internal/util/utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.911852332/src/vdk_core.egg-info/PKG-INFO` & `vdk-core-0.3.912884507/src/vdk_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.911852332
+Version: 0.3.912884507
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.911852332/src/vdk_core.egg-info/SOURCES.txt` & `vdk-core-0.3.912884507/src/vdk_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,22 @@
 src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
 src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
 src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
 src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
 src/vdk/internal/builtin_plugins/job_properties/properties_config.py
 src/vdk/internal/builtin_plugins/job_properties/properties_router.py
 src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
+src/vdk/internal/builtin_plugins/job_secrets/base_secrets_impl.py
+src/vdk/internal/builtin_plugins/job_secrets/cached_secrets.py
+src/vdk/internal/builtin_plugins/job_secrets/datajobs_service_secrets.py
+src/vdk/internal/builtin_plugins/job_secrets/inmemsecrets.py
+src/vdk/internal/builtin_plugins/job_secrets/secrets_api_plugin.py
+src/vdk/internal/builtin_plugins/job_secrets/secrets_config.py
+src/vdk/internal/builtin_plugins/job_secrets/secrets_router.py
+src/vdk/internal/builtin_plugins/job_secrets/secretsnotavailable.py
 src/vdk/internal/builtin_plugins/notification/notification.py
 src/vdk/internal/builtin_plugins/notification/notification_base.py
 src/vdk/internal/builtin_plugins/notification/notification_configuration.py
 src/vdk/internal/builtin_plugins/run/cli_run.py
 src/vdk/internal/builtin_plugins/run/data_job.py
 src/vdk/internal/builtin_plugins/run/execution_environment.py
 src/vdk/internal/builtin_plugins/run/execution_results.py
```

